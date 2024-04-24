# Comparing `tmp/lunary-1.0.4.tar.gz` & `tmp/lunary-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lunary-1.0.4.tar", max compression
+gzip compressed data, was "lunary-1.0.5.tar", max compression
```

## Comparing `lunary-1.0.4.tar` & `lunary-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      604 2024-02-28 21:10:30.380738 lunary-1.0.4/README.md
--rw-r--r--   0        0        0    61225 2024-04-24 01:16:27.567909 lunary-1.0.4/lunary/__init__.py
--rw-r--r--   0        0        0     2221 2024-04-01 02:07:49.605602 lunary-1.0.4/lunary/consumer.py
--rw-r--r--   0        0        0      607 2024-03-13 20:53:32.460623 lunary-1.0.4/lunary/event_queue.py
--rw-r--r--   0        0        0     2384 2024-03-04 00:09:26.744750 lunary-1.0.4/lunary/openai_utils.py
--rw-r--r--   0        0        0      670 2024-04-01 15:34:21.542269 lunary-1.0.4/lunary/parent.py
--rw-r--r--   0        0        0     1071 2024-04-02 01:49:22.083662 lunary-1.0.4/lunary/parsers.py
--rw-r--r--   0        0        0      425 2024-04-01 02:07:35.888287 lunary-1.0.4/lunary/project.py
--rw-r--r--   0        0        0      378 2024-03-04 00:09:26.744921 lunary-1.0.4/lunary/tags.py
--rw-r--r--   0        0        0     1164 2024-04-17 19:52:13.801396 lunary-1.0.4/lunary/thread.py
--rw-r--r--   0        0        0      573 2024-03-04 00:09:26.745039 lunary-1.0.4/lunary/users.py
--rw-r--r--   0        0        0      762 2024-04-24 01:16:47.829767 lunary-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1723 1970-01-01 00:00:00.000000 lunary-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      604 2024-02-28 21:10:30.380738 lunary-1.0.5/README.md
+-rw-r--r--   0        0        0    61221 2024-04-24 21:44:12.387421 lunary-1.0.5/lunary/__init__.py
+-rw-r--r--   0        0        0     2221 2024-04-01 02:07:49.605602 lunary-1.0.5/lunary/consumer.py
+-rw-r--r--   0        0        0      607 2024-03-13 20:53:32.460623 lunary-1.0.5/lunary/event_queue.py
+-rw-r--r--   0        0        0     2384 2024-03-04 00:09:26.744750 lunary-1.0.5/lunary/openai_utils.py
+-rw-r--r--   0        0        0      670 2024-04-01 15:34:21.542269 lunary-1.0.5/lunary/parent.py
+-rw-r--r--   0        0        0     1071 2024-04-02 01:49:22.083662 lunary-1.0.5/lunary/parsers.py
+-rw-r--r--   0        0        0      425 2024-04-01 02:07:35.888287 lunary-1.0.5/lunary/project.py
+-rw-r--r--   0        0        0      378 2024-03-04 00:09:26.744921 lunary-1.0.5/lunary/tags.py
+-rw-r--r--   0        0        0     1164 2024-04-17 19:52:13.801396 lunary-1.0.5/lunary/thread.py
+-rw-r--r--   0        0        0      573 2024-03-04 00:09:26.745039 lunary-1.0.5/lunary/users.py
+-rw-r--r--   0        0        0      762 2024-04-24 21:49:32.402144 lunary-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1723 1970-01-01 00:00:00.000000 lunary-1.0.5/PKG-INFO
```

### Comparing `lunary-1.0.4/README.md` & `lunary-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `lunary-1.0.4/lunary/__init__.py` & `lunary-1.0.5/lunary/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,16 +128,15 @@
     )
     VERBOSE = os.environ.get(
         "LUNARY_VERBOSE") or os.environ.get("LLMONITOR_VERBOSE")
 
     if not APP_ID:
         return warnings.warn("LUNARY_PUBLIC_KEY is not set, not sending events")
 
-    parent_run_id = get_parent_run_id(parent_run_id, run_type, app_id=app_id, run_id=run_id, is_openai=is_openai)
-    
+    parent_run_id = get_parent_run_id(parent_run_id, run_type, app_id=APP_ID, run_id=run_id, is_openai=is_openai) 
     event = {
         "event": event_name,
         "type": run_type,
         "name": name,
         "userId": user_id or user_ctx.get(),
         "userProps": user_props or user_props_ctx.get(),
         "tags": tags or tags_ctx.get(),
```

### Comparing `lunary-1.0.4/lunary/consumer.py` & `lunary-1.0.5/lunary/consumer.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.4/lunary/event_queue.py` & `lunary-1.0.5/lunary/event_queue.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.4/lunary/openai_utils.py` & `lunary-1.0.5/lunary/openai_utils.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.4/lunary/parent.py` & `lunary-1.0.5/lunary/parent.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.4/lunary/parsers.py` & `lunary-1.0.5/lunary/parsers.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.4/lunary/thread.py` & `lunary-1.0.5/lunary/thread.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.4/lunary/users.py` & `lunary-1.0.5/lunary/users.py`

 * *Files identical despite different names*

### Comparing `lunary-1.0.4/pyproject.toml` & `lunary-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lunary"
-version = "1.0.4"
+version = "1.0.5"
 description = "Observability, analytics and evaluations for AI agents and chatbots."
 authors = ["lunary <hello@lunary.ai>"]
 readme = "README.md"
 repository = "https://github.com/lunary-ai/lunary-py"
 documentation = "https://lunary.ai/docs/py"
 keywords = ["Lunary", "lunary.ai", "Langchain", "AI", "Analytics", "Monitoring"]
```

### Comparing `lunary-1.0.4/PKG-INFO` & `lunary-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lunary
-Version: 1.0.4
+Version: 1.0.5
 Summary: Observability, analytics and evaluations for AI agents and chatbots.
 Home-page: https://github.com/lunary-ai/lunary-py
 Keywords: Lunary,lunary.ai,Langchain,AI,Analytics,Monitoring
 Author: lunary
 Author-email: hello@lunary.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
```

