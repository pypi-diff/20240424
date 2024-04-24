# Comparing `tmp/lunary-1.0.3.tar.gz` & `tmp/lunary-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lunary-1.0.3.tar", max compression
+gzip compressed data, was "lunary-1.0.4.tar", max compression
```

## Comparing `lunary-1.0.3.tar` & `lunary-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      604 2024-02-28 21:10:30.380738 lunary-1.0.3/README.md
--rw-r--r--   0        0        0    57524 2024-04-16 01:14:07.135553 lunary-1.0.3/lunary/__init__.py
--rw-r--r--   0        0        0     2221 2024-04-01 02:07:49.605602 lunary-1.0.3/lunary/consumer.py
--rw-r--r--   0        0        0      607 2024-03-13 20:53:32.460623 lunary-1.0.3/lunary/event_queue.py
--rw-r--r--   0        0        0     2384 2024-03-04 00:09:26.744750 lunary-1.0.3/lunary/openai_utils.py
--rw-r--r--   0        0        0      670 2024-04-01 15:34:21.542269 lunary-1.0.3/lunary/parent.py
--rw-r--r--   0        0        0     1071 2024-04-02 01:49:22.083662 lunary-1.0.3/lunary/parsers.py
--rw-r--r--   0        0        0      425 2024-04-01 02:07:35.888287 lunary-1.0.3/lunary/project.py
--rw-r--r--   0        0        0      378 2024-03-04 00:09:26.744921 lunary-1.0.3/lunary/tags.py
--rw-r--r--   0        0        0     1164 2024-04-17 19:52:13.801396 lunary-1.0.3/lunary/thread.py
--rw-r--r--   0        0        0      573 2024-03-04 00:09:26.745039 lunary-1.0.3/lunary/users.py
--rw-r--r--   0        0        0      743 2024-04-17 19:52:36.218263 lunary-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1683 1970-01-01 00:00:00.000000 lunary-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      604 2024-02-28 21:10:30.380738 lunary-1.0.4/README.md
+-rw-r--r--   0        0        0    61225 2024-04-24 01:16:27.567909 lunary-1.0.4/lunary/__init__.py
+-rw-r--r--   0        0        0     2221 2024-04-01 02:07:49.605602 lunary-1.0.4/lunary/consumer.py
+-rw-r--r--   0        0        0      607 2024-03-13 20:53:32.460623 lunary-1.0.4/lunary/event_queue.py
+-rw-r--r--   0        0        0     2384 2024-03-04 00:09:26.744750 lunary-1.0.4/lunary/openai_utils.py
+-rw-r--r--   0        0        0      670 2024-04-01 15:34:21.542269 lunary-1.0.4/lunary/parent.py
+-rw-r--r--   0        0        0     1071 2024-04-02 01:49:22.083662 lunary-1.0.4/lunary/parsers.py
+-rw-r--r--   0        0        0      425 2024-04-01 02:07:35.888287 lunary-1.0.4/lunary/project.py
+-rw-r--r--   0        0        0      378 2024-03-04 00:09:26.744921 lunary-1.0.4/lunary/tags.py
+-rw-r--r--   0        0        0     1164 2024-04-17 19:52:13.801396 lunary-1.0.4/lunary/thread.py
+-rw-r--r--   0        0        0      573 2024-03-04 00:09:26.745039 lunary-1.0.4/lunary/users.py
+-rw-r--r--   0        0        0      762 2024-04-24 01:16:47.829767 lunary-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1723 1970-01-01 00:00:00.000000 lunary-1.0.4/PKG-INFO
```

### Comparing `lunary-1.0.3/README.md` & `lunary-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lunary-1.0.3/lunary/__init__.py` & `lunary-1.0.4/lunary/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import traceback
 import logging
 import copy
 import json
 import time
 import chevron
 import hashlib
+import aiohttp
 from pkg_resources import parse_version
 from importlib.metadata import version, PackageNotFoundError
 from contextvars import ContextVar
 from datetime import datetime, timezone
 from typing import Optional
 
 
@@ -1522,17 +1523,46 @@
     if not response.ok:
         raise Exception(f"Lunary: Error fetching template: {response.status_code} - {response.text}")
 
     data = response.json()
     templateCache[slug] = {'timestamp': now, 'data': data}
     return data
 
+async def get_raw_template_async(slug):
+    token = (
+        os.environ.get("LUNARY_PUBLIC_KEY") or os.environ.get(
+            "LUNARY_APP_ID") or os.environ.get("LLMONITOR_APP_ID")
+    )
+    api_url = os.environ.get("LUNARY_API_URL") or DEFAULT_API_URL
 
-def render_template(slug, data = {}):
+    global templateCache
+    now = time.time() * 1000
+    cache_entry = templateCache.get(slug)
+
+    if cache_entry and now - cache_entry['timestamp'] < 60000:
+        return cache_entry['data']
+
+    headers = {
+        'Authorization': f'Bearer {token}',
+        'Content-Type': 'application/json'
+    }
 
+    async with aiohttp.ClientSession() as session:
+        async with session.get(f"{api_url}/v1/template_versions/latest?slug={slug}", headers=headers) as response:
+            if not response.ok:
+                raise Exception(f"Lunary: Error fetching template: {response.status} - {await response.text()}")
+
+            data = await response.json()
+
+    templateCache[slug] = {'timestamp': now, 'data': data}
+    return data
+
+
+
+def render_template(slug, data = {}):
     raw_template = get_raw_template(slug)
 
     if(raw_template.get('message') == 'Template not found, is the project ID correct?'):
         raise Exception("Template not found, are the project ID and slug correct?")
 
     template_id = copy.deepcopy(raw_template['id'])
     content = copy.deepcopy(raw_template['content'])
@@ -1561,16 +1591,54 @@
             "messages": messages, 
             "extra_headers": extra_headers,
             **extra
         }
 
         return result
 
-def get_langchain_template(slug):
+async def render_template_async(slug, data={}):
+    raw_template = await get_raw_template_async(slug)
+
+    if raw_template.get('message') == 'Template not found, is the project ID correct?':
+        raise Exception("Template not found, are the project ID and slug correct?")
+
+    template_id = copy.deepcopy(raw_template['id'])
+    content = copy.deepcopy(raw_template['content'])
+    extra = copy.deepcopy(raw_template['extra'])
+
+    text_mode = isinstance(content, str)
+
+    # extra_headers is safe with OpenAI to be used to pass value
+    extra_headers = {
+        "Template-Id": str(template_id)
+    }
+
+    result = None
+    if text_mode:
+        rendered = chevron.render(content, data)
+        result = {
+            "text": rendered,
+            "extra_headers": extra_headers,
+            **extra
+        }
+        return result
+    else:
+        messages = []
+        for message in content:
+            message["content"] = chevron.render(message["content"], data)
+            messages.append(message)
+        result = {
+            "messages": messages,
+            "extra_headers": extra_headers,
+            **extra
+        }
 
+        return result
+
+def get_langchain_template(slug):
     try:
         from langchain_core.prompts import ChatPromptTemplate, PromptTemplate
 
         raw_template = get_raw_template(slug)
 
         if(raw_template.get('message') == 'Template not found, is the project ID correct?'):
             raise Exception("Template not found, are the project ID and slug correct?")
@@ -1608,14 +1676,59 @@
             template = ChatPromptTemplate.from_messages(messages)
 
             return template
         
     except Exception as e:
         print(f"Lunary: Error fetching template: {e}")
 
+async def get_langchain_template_async(slug):
+    try:
+        from langchain_core.prompts import ChatPromptTemplate, PromptTemplate
+
+        raw_template = await get_raw_template_async(slug)
+
+        if raw_template.get('message') == 'Template not found, is the project ID correct?':
+            raise Exception("Template not found, are the project ID and slug correct?")
+
+        content = copy.deepcopy(raw_template['content'])
+
+        def replace_double_braces(text):
+            return text.replace("{{", "{").replace("}}", "}")
+
+        text_mode = isinstance(content, str)
+
+        if text_mode:
+            # replace {{ variables }} with { variables }
+            rendered = replace_double_braces(content)
+
+            template = PromptTemplate.from_template(rendered)
+
+            return template
+
+        else:
+            messages = []
+
+            # Return array of messages like that:
+            #  [
+            #     ("system", "You are a helpful AI bot. Your name is {name}."),
+            #     ("human", "Hello, how are you doing?"),
+            #     ("ai", "I'm doing well, thanks!"),
+            #     ("human", "{user_input}"),
+            # ]
+
+            for message in content:
+                messages.append((message["role"].replace("assistant", "ai").replace('user', 'human'), replace_double_braces(message["content"])))
+
+            template = ChatPromptTemplate.from_messages(messages)
+
+            return template
+
+    except Exception as e:
+        print(f"Lunary: Error fetching template: {e}")
+
 import humps
 
 class DatasetItem:
     def __init__(self, d=None):
         if d is not None:
             for key, value in d.items():
                 setattr(self, key, value)
```

### Comparing `lunary-1.0.3/lunary/consumer.py` & `lunary-1.0.4/lunary/consumer.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.3/lunary/event_queue.py` & `lunary-1.0.4/lunary/event_queue.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.3/lunary/openai_utils.py` & `lunary-1.0.4/lunary/openai_utils.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.3/lunary/parent.py` & `lunary-1.0.4/lunary/parent.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.3/lunary/parsers.py` & `lunary-1.0.4/lunary/parsers.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.3/lunary/thread.py` & `lunary-1.0.4/lunary/thread.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.3/lunary/users.py` & `lunary-1.0.4/lunary/users.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.3/pyproject.toml` & `lunary-1.0.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lunary"
-version = "1.0.3"
+version = "1.0.4"
 description = "Observability, analytics and evaluations for AI agents and chatbots."
 authors = ["lunary <hello@lunary.ai>"]
 readme = "README.md"
 repository = "https://github.com/lunary-ai/lunary-py"
 documentation = "https://lunary.ai/docs/py"
 keywords = ["Lunary", "lunary.ai", "Langchain", "AI", "Analytics", "Monitoring"]
 
@@ -14,14 +14,15 @@
 setuptools = "^67.6.2"
 tenacity = "^8.2.3"
 opentelemetry-api = "^1.21.0"
 opentelemetry-sdk = "^1.21.0"
 packaging = "^23.2"
 chevron = "^0.14.0"
 pyhumps = "^3.8.0"
+aiohttp = "^3.9.5"
 
 [tool.poetry.group.dev.dependencies]
 openai = "^1.12.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lunary-1.0.3/PKG-INFO` & `lunary-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: lunary
-Version: 1.0.3
+Version: 1.0.4
 Summary: Observability, analytics and evaluations for AI agents and chatbots.
 Home-page: https://github.com/lunary-ai/lunary-py
 Keywords: Lunary,lunary.ai,Langchain,AI,Analytics,Monitoring
 Author: lunary
 Author-email: hello@lunary.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiohttp (>=3.9.5,<4.0.0)
 Requires-Dist: chevron (>=0.14.0,<0.15.0)
 Requires-Dist: opentelemetry-api (>=1.21.0,<2.0.0)
 Requires-Dist: opentelemetry-sdk (>=1.21.0,<2.0.0)
 Requires-Dist: packaging (>=23.2,<24.0)
 Requires-Dist: pyhumps (>=3.8.0,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: setuptools (>=67.6.2,<68.0.0)
```

