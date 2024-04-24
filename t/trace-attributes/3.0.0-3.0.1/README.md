# Comparing `tmp/trace-attributes-3.0.0.tar.gz` & `tmp/trace_attributes-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trace-attributes-3.0.0.tar", last modified: Thu Apr 18 01:44:00 2024, max compression
+gzip compressed data, was "trace_attributes-3.0.1.tar", last modified: Wed Apr 24 00:02:00 2024, max compression
```

## Comparing `trace-attributes-3.0.0.tar` & `trace_attributes-3.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 rohitkadhe   (501) staff       (20)        0 2024-04-18 01:44:00.746785 trace-attributes-3.0.0/
--rw-r--r--   0 rohitkadhe   (501) staff       (20)    11357 2024-04-04 15:20:34.000000 trace-attributes-3.0.0/LICENSE
--rw-r--r--   0 rohitkadhe   (501) staff       (20)      545 2024-04-18 01:44:00.746521 trace-attributes-3.0.0/PKG-INFO
--rw-r--r--   0 rohitkadhe   (501) staff       (20)     2825 2024-04-12 19:12:01.000000 trace-attributes-3.0.0/README.md
--rw-r--r--   0 rohitkadhe   (501) staff       (20)       38 2024-04-18 01:44:00.746824 trace-attributes-3.0.0/setup.cfg
--rw-r--r--   0 rohitkadhe   (501) staff       (20)      960 2024-04-18 01:07:18.000000 trace-attributes-3.0.0/setup.py
-drwxr-xr-x   0 rohitkadhe   (501) staff       (20)        0 2024-04-18 01:44:00.742502 trace-attributes-3.0.0/src/
-drwxr-xr-x   0 rohitkadhe   (501) staff       (20)        0 2024-04-18 01:44:00.742778 trace-attributes-3.0.0/src/python/
-drwxr-xr-x   0 rohitkadhe   (501) staff       (20)        0 2024-04-18 01:44:00.743661 trace-attributes-3.0.0/src/python/langtrace/
--rw-r--r--   0 rohitkadhe   (501) staff       (20)       13 2024-03-04 16:20:38.000000 trace-attributes-3.0.0/src/python/langtrace/__init__.py
-drwxr-xr-x   0 rohitkadhe   (501) staff       (20)        0 2024-04-18 01:44:00.743991 trace-attributes-3.0.0/src/python/langtrace/trace_attributes/
--rw-r--r--   0 rohitkadhe   (501) staff       (20)     1311 2024-04-04 15:20:34.000000 trace-attributes-3.0.0/src/python/langtrace/trace_attributes/__init__.py
-drwxr-xr-x   0 rohitkadhe   (501) staff       (20)        0 2024-04-18 01:44:00.745017 trace-attributes-3.0.0/src/python/langtrace/trace_attributes/models/
--rw-r--r--   0 rohitkadhe   (501) staff       (20)       13 2024-03-04 16:20:38.000000 trace-attributes-3.0.0/src/python/langtrace/trace_attributes/models/__init__.py
--rw-r--r--   0 rohitkadhe   (501) staff       (20)     1529 2024-04-12 19:12:01.000000 trace-attributes-3.0.0/src/python/langtrace/trace_attributes/models/database_span_attributes.py
--rw-r--r--   0 rohitkadhe   (501) staff       (20)     1418 2024-04-12 19:12:01.000000 trace-attributes-3.0.0/src/python/langtrace/trace_attributes/models/framework_span_attributes.py
--rw-r--r--   0 rohitkadhe   (501) staff       (20)     3599 2024-04-18 01:41:37.000000 trace-attributes-3.0.0/src/python/langtrace/trace_attributes/models/llm_span_attributes.py
-drwxr-xr-x   0 rohitkadhe   (501) staff       (20)        0 2024-04-18 01:44:00.746230 trace-attributes-3.0.0/src/python/trace_attributes.egg-info/
--rw-r--r--   0 rohitkadhe   (501) staff       (20)      545 2024-04-18 01:44:00.000000 trace-attributes-3.0.0/src/python/trace_attributes.egg-info/PKG-INFO
--rw-r--r--   0 rohitkadhe   (501) staff       (20)      635 2024-04-18 01:44:00.000000 trace-attributes-3.0.0/src/python/trace_attributes.egg-info/SOURCES.txt
--rw-r--r--   0 rohitkadhe   (501) staff       (20)        1 2024-04-18 01:44:00.000000 trace-attributes-3.0.0/src/python/trace_attributes.egg-info/dependency_links.txt
--rw-r--r--   0 rohitkadhe   (501) staff       (20)       21 2024-04-18 01:44:00.000000 trace-attributes-3.0.0/src/python/trace_attributes.egg-info/requires.txt
--rw-r--r--   0 rohitkadhe   (501) staff       (20)       10 2024-04-18 01:44:00.000000 trace-attributes-3.0.0/src/python/trace_attributes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:00.401780 trace_attributes-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 00:01:45.000000 trace_attributes-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-24 00:02:00.401780 trace_attributes-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-24 00:01:45.000000 trace_attributes-3.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 00:02:00.401780 trace_attributes-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-24 00:01:45.000000 trace_attributes-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:00.397780 trace_attributes-3.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:00.397780 trace_attributes-3.0.1/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:00.401780 trace_attributes-3.0.1/src/python/langtrace/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 00:01:45.000000 trace_attributes-3.0.1/src/python/langtrace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:00.401780 trace_attributes-3.0.1/src/python/langtrace/trace_attributes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-24 00:01:45.000000 trace_attributes-3.0.1/src/python/langtrace/trace_attributes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:00.401780 trace_attributes-3.0.1/src/python/langtrace/trace_attributes/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 00:01:45.000000 trace_attributes-3.0.1/src/python/langtrace/trace_attributes/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-24 00:01:45.000000 trace_attributes-3.0.1/src/python/langtrace/trace_attributes/models/database_span_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-24 00:01:45.000000 trace_attributes-3.0.1/src/python/langtrace/trace_attributes/models/framework_span_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-24 00:01:45.000000 trace_attributes-3.0.1/src/python/langtrace/trace_attributes/models/llm_span_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:00.401780 trace_attributes-3.0.1/src/python/trace_attributes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-24 00:02:00.000000 trace_attributes-3.0.1/src/python/trace_attributes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-24 00:02:00.000000 trace_attributes-3.0.1/src/python/trace_attributes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 00:02:00.000000 trace_attributes-3.0.1/src/python/trace_attributes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 00:02:00.000000 trace_attributes-3.0.1/src/python/trace_attributes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 00:02:00.000000 trace_attributes-3.0.1/src/python/trace_attributes.egg-info/top_level.txt
```

### Comparing `trace-attributes-3.0.0/LICENSE` & `trace_attributes-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trace-attributes-3.0.0/PKG-INFO` & `trace_attributes-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trace-attributes
-Version: 3.0.0
+Version: 3.0.1
 Summary: LangTrace - Trace Attributes
 Home-page: https://github.com/Scale3-Labs/langtrace-trace-attributes
 Author: Karthik Kalyanaraman
 Author-email: karthik@scale3labs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trace-attributes-3.0.0/README.md` & `trace_attributes-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `trace-attributes-3.0.0/setup.py` & `trace_attributes-3.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='trace-attributes',  # Choose a unique name for PyPI
-    version='3.0.0',
+    version='3.0.1',
     author='Karthik Kalyanaraman',
     author_email='karthik@scale3labs.com',
     description='LangTrace - Trace Attributes',
     long_description="LangTrace - Trace Attributes",
     long_description_content_type='text/markdown',
     url='https://github.com/Scale3-Labs/langtrace-trace-attributes',  # Project home page
     package_dir={'': 'src/python'},
```

### Comparing `trace-attributes-3.0.0/src/python/langtrace/trace_attributes/__init__.py` & `trace_attributes-3.0.1/src/python/langtrace/trace_attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `trace-attributes-3.0.0/src/python/langtrace/trace_attributes/models/database_span_attributes.py` & `trace_attributes-3.0.1/src/python/langtrace/trace_attributes/models/database_span_attributes.py`

 * *Files identical despite different names*

### Comparing `trace-attributes-3.0.0/src/python/langtrace/trace_attributes/models/framework_span_attributes.py` & `trace_attributes-3.0.1/src/python/langtrace/trace_attributes/models/framework_span_attributes.py`

 * *Files identical despite different names*

### Comparing `trace-attributes-3.0.0/src/python/langtrace/trace_attributes/models/llm_span_attributes.py` & `trace_attributes-3.0.1/src/python/langtrace/trace_attributes/models/llm_span_attributes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  llm_span_attributes.json
-#   timestamp: 2024-04-18T01:41:37+00:00
+#   timestamp: 2024-04-23T23:31:38+00:00
 
 from __future__ import annotations
 
 from typing import Optional
 
 from pydantic import BaseModel, Extra, Field
 
@@ -23,43 +23,59 @@
     url_full: str = Field(..., alias='url.full')
     llm_api: str = Field(..., alias='llm.api')
     llm_model: Optional[str] = Field(None, alias='llm.model')
     llm_temperature: Optional[float] = Field(None, alias='llm.temperature')
     llm_top_p: Optional[float] = Field(None, alias='llm.top_p')
     llm_top_k: Optional[float] = Field(None, alias='llm.top_k')
     llm_user: Optional[str] = Field(None, alias='llm.user')
-    llm_system_fingerprint: Optional[str] = Field(None, alias='llm.system.fingerprint')
-    llm_prompts: str = Field(..., alias='llm.prompts')
+    llm_system_fingerprint: Optional[str] = Field(
+        None, alias='llm.system.fingerprint')
+    llm_prompts: Optional[str] = Field(None, alias='llm.prompts')
+    llm_function_prompts: Optional[str] = Field(
+        None, alias='llm.function.prompts')
     llm_responses: Optional[str] = Field(None, alias='llm.responses')
     llm_token_counts: Optional[str] = Field(None, alias='llm.token.counts')
     llm_stream: Optional[bool] = Field(None, alias='llm.stream')
-    llm_encoding_formats: Optional[str] = Field(None, alias='llm.encoding.formats')
+    llm_encoding_formats: Optional[str] = Field(
+        None, alias='llm.encoding.formats')
     llm_dimensions: Optional[str] = Field(None, alias='llm.dimensions')
     llm_generation_id: Optional[str] = Field(None, alias='llm.generation_id')
     llm_response_id: Optional[str] = Field(None, alias='llm.response_id')
     llm_citations: Optional[str] = Field(None, alias='llm.citations')
     llm_documents: Optional[str] = Field(None, alias='llm.documents')
-    llm_is_search_required: Optional[bool] = Field(None, alias='llm.is_search_required')
+    llm_is_search_required: Optional[bool] = Field(
+        None, alias='llm.is_search_required')
     llm_search_results: Optional[str] = Field(None, alias='llm.search_results')
     llm_tool_calls: Optional[str] = Field(None, alias='llm.tool_calls')
     llm_max_tokens: Optional[str] = Field(None, alias='llm.max_tokens')
-    llm_max_input_tokens: Optional[str] = Field(None, alias='llm.max_input_tokens')
-    llm_conversation_id: Optional[str] = Field(None, alias='llm.conversation_id')
+    llm_max_input_tokens: Optional[str] = Field(
+        None, alias='llm.max_input_tokens')
+    llm_conversation_id: Optional[str] = Field(
+        None, alias='llm.conversation_id')
     llm_seed: Optional[str] = Field(None, alias='llm.seed')
-    llm_frequency_penalty: Optional[str] = Field(None, alias='llm.frequency_penalty')
-    llm_presence_penalty: Optional[str] = Field(None, alias='llm.presence_penalty')
+    llm_frequency_penalty: Optional[str] = Field(
+        None, alias='llm.frequency_penalty')
+    llm_presence_penalty: Optional[str] = Field(
+        None, alias='llm.presence_penalty')
     llm_connectors: Optional[str] = Field(None, alias='llm.connectors')
     llm_tools: Optional[str] = Field(None, alias='llm.tools')
     llm_tool_results: Optional[str] = Field(None, alias='llm.tool_results')
-    llm_embedding_inputs: Optional[str] = Field(None, alias='llm.embedding_inputs')
+    llm_embedding_inputs: Optional[str] = Field(
+        None, alias='llm.embedding_inputs')
     llm_embedding_dataset_id: Optional[str] = Field(
         None, alias='llm.embedding_dataset_id'
     )
     llm_embedding_input_type: Optional[str] = Field(
         None, alias='llm.embedding_input_type'
     )
-    llm_embedding_job_name: Optional[str] = Field(None, alias='llm.embedding_job_name')
+    llm_embedding_job_name: Optional[str] = Field(
+        None, alias='llm.embedding_job_name')
+    llm_retrieval_query: Optional[str] = Field(
+        None, alias='llm.retrieval.query')
+    llm_retrieval_results: Optional[str] = Field(
+        None, alias='llm.retrieval.results')
     user_id: Optional[str] = Field(None, alias='user.id')
-    user_feedback_rating: Optional[int] = Field(None, alias='user.feedback.rating')
+    user_feedback_rating: Optional[int] = Field(
+        None, alias='user.feedback.rating')
     http_max_retries: Optional[int] = Field(None, alias='http.max.retries')
     http_timeout: Optional[int] = Field(None, alias='http.timeout')
     langtrace_testId: Optional[str] = Field(None, alias='langtrace.testId')
```

### Comparing `trace-attributes-3.0.0/src/python/trace_attributes.egg-info/PKG-INFO` & `trace_attributes-3.0.1/src/python/trace_attributes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trace-attributes
-Version: 3.0.0
+Version: 3.0.1
 Summary: LangTrace - Trace Attributes
 Home-page: https://github.com/Scale3-Labs/langtrace-trace-attributes
 Author: Karthik Kalyanaraman
 Author-email: karthik@scale3labs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trace-attributes-3.0.0/src/python/trace_attributes.egg-info/SOURCES.txt` & `trace_attributes-3.0.1/src/python/trace_attributes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

