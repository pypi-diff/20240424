# Comparing `tmp/literalai-0.0.507.tar.gz` & `tmp/literalai-0.0.508.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "literalai-0.0.507.tar", last modified: Tue Apr 23 12:04:29 2024, max compression
+gzip compressed data, was "literalai-0.0.508.tar", last modified: Wed Apr 24 16:17:07 2024, max compression
```

## Comparing `literalai-0.0.507.tar` & `literalai-0.0.508.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:04:29.755336 literalai-0.0.507/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 12:04:23.000000 literalai-0.0.507/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-23 12:04:29.755336 literalai-0.0.507/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-23 12:04:23.000000 literalai-0.0.507/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:04:29.751336 literalai-0.0.507/literalai/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:04:29.751336 literalai-0.0.507/literalai/api/
--rw-r--r--   0 runner    (1001) docker     (127)    81103 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/api/attachment_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/api/dataset_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/api/generation_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20172 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/api/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/api/prompt_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/api/score_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/api/step_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/api/thread_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/api/user_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:04:29.751336 literalai-0.0.507/literalai/callback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17193 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/callback/langchain_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/callback/llama_index_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/dataset_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/event_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:04:29.755336 literalai-0.0.507/literalai/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18352 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/instrumentation/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/my_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-23 12:04:23.000000 literalai-0.0.507/literalai/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:04:29.751336 literalai-0.0.507/literalai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-23 12:04:29.000000 literalai-0.0.507/literalai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-23 12:04:29.000000 literalai-0.0.507/literalai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:04:29.000000 literalai-0.0.507/literalai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-23 12:04:29.000000 literalai-0.0.507/literalai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 12:04:29.000000 literalai-0.0.507/literalai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 12:04:29.755336 literalai-0.0.507/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-23 12:04:23.000000 literalai-0.0.507/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:04:29.755336 literalai-0.0.507/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 12:04:23.000000 literalai-0.0.507/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:17:07.807956 literalai-0.0.508/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 16:16:58.000000 literalai-0.0.508/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-24 16:17:07.807956 literalai-0.0.508/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-24 16:16:58.000000 literalai-0.0.508/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:17:07.803956 literalai-0.0.508/literalai/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:17:07.807956 literalai-0.0.508/literalai/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    81103 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/api/attachment_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/api/dataset_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/api/generation_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20172 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/api/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/api/prompt_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/api/score_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/api/step_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/api/thread_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/api/user_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:17:07.807956 literalai-0.0.508/literalai/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17193 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/callback/langchain_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/callback/llama_index_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/dataset_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/event_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:17:07.807956 literalai-0.0.508/literalai/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18352 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/instrumentation/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12197 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/my_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-24 16:16:58.000000 literalai-0.0.508/literalai/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:17:07.803956 literalai-0.0.508/literalai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-24 16:17:07.000000 literalai-0.0.508/literalai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-24 16:17:07.000000 literalai-0.0.508/literalai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:17:07.000000 literalai-0.0.508/literalai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-24 16:17:07.000000 literalai-0.0.508/literalai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 16:17:07.000000 literalai-0.0.508/literalai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 16:17:07.807956 literalai-0.0.508/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-24 16:16:58.000000 literalai-0.0.508/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:17:07.807956 literalai-0.0.508/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:16:58.000000 literalai-0.0.508/tests/__init__.py
```

### Comparing `literalai-0.0.507/LICENSE` & `literalai-0.0.508/LICENSE`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/README.md` & `literalai-0.0.508/README.md`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/literalai/api/__init__.py` & `literalai-0.0.508/literalai/api/__init__.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/literalai/api/attachment_helpers.py` & `literalai-0.0.508/literalai/api/attachment_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/literalai/api/dataset_helpers.py` & `literalai-0.0.508/literalai/api/dataset_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/literalai/api/generation_helpers.py` & `literalai-0.0.508/literalai/api/generation_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,14 @@
         variables["orderBy"] = order_by
 
     def process_response(response):
         processed_response = response["data"]["generations"]
         processed_response["data"] = list(
             map(lambda x: x["node"], processed_response["edges"])
         )
-        del processed_response["edges"]
         return PaginatedResponse[BaseGeneration].from_dict(
             processed_response, BaseGeneration
         )
 
     description = "get generations"
 
     return gql.GET_GENERATIONS, description, variables, process_response
```

### Comparing `literalai-0.0.507/literalai/api/gql.py` & `literalai-0.0.508/literalai/api/gql.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/literalai/api/prompt_helpers.py` & `literalai-0.0.508/literalai/api/prompt_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/literalai/api/score_helpers.py` & `literalai-0.0.508/literalai/api/score_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         variables["filters"] = filters
     if order_by:
         variables["orderBy"] = order_by
 
     def process_response(response):
         response_data = response["data"]["scores"]
         response_data["data"] = list(map(lambda x: x["node"], response_data["edges"]))
-        del response_data["edges"]
         return PaginatedResponse[Score].from_dict(response_data, Score)  # type: ignore
 
     description = "get scores"
 
     return gql.GET_SCORES, description, variables, process_response
```

### Comparing `literalai-0.0.507/literalai/api/step_helpers.py` & `literalai-0.0.508/literalai/api/step_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/literalai/api/thread_helpers.py` & `literalai-0.0.508/literalai/api/thread_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
         variables["stepTypesToKeep"] = step_types_to_keep
 
     def process_response(response):
         processed_response = response["data"]["threads"]
         processed_response["data"] = [
             edge["node"] for edge in processed_response["edges"]
         ]
-        del processed_response["edges"]
         return PaginatedResponse[Thread].from_dict(processed_response, Thread)
 
     description = "get threads"
 
     return gql.GET_THREADS, description, variables, process_response
 
 
@@ -63,15 +62,14 @@
         variables["filters"] = filters
     if order_by:
         variables["orderBy"] = order_by
 
     def process_response(response):
         response_data = response["data"]["threads"]
         response_data["data"] = list(map(lambda x: x["node"], response_data["edges"]))
-        del response_data["edges"]
         return PaginatedResponse[Thread].from_dict(response_data, Thread)
 
     description = "get threads"
 
     return gql.LIST_THREADS, description, variables, process_response
```

### Comparing `literalai-0.0.507/literalai/api/user_helpers.py` & `literalai-0.0.508/literalai/api/user_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         variables["after"] = after
     if before:
         variables["before"] = before
     if filters:
         variables["filters"] = filters
 
     def process_response(response):
-        paginated_response = response["data"]["participants"]
-        response["data"] = list(map(lambda x: x["node"], paginated_response["edges"]))
+        response = response["data"]["participants"]
+        response["data"] = list(map(lambda x: x["node"], response["edges"]))
         return PaginatedResponse[User].from_dict(response, User)
 
     description = "get users"
 
     return gql.GET_PARTICIPANTS, description, variables, process_response
```

### Comparing `literalai-0.0.507/literalai/callback/langchain_callback.py` & `literalai-0.0.508/literalai/callback/langchain_callback.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/literalai/callback/llama_index_callback.py` & `literalai-0.0.508/literalai/callback/llama_index_callback.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/literalai/client.py` & `literalai-0.0.508/literalai/client.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/literalai/dataset.py` & `literalai-0.0.508/literalai/dataset.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/literalai/dataset_experiment.py` & `literalai-0.0.508/literalai/dataset_experiment.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/literalai/dataset_item.py` & `literalai-0.0.508/literalai/dataset_item.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/literalai/event_processor.py` & `literalai-0.0.508/literalai/event_processor.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/literalai/filter.py` & `literalai-0.0.508/literalai/filter.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/literalai/helper.py` & `literalai-0.0.508/literalai/helper.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/literalai/instrumentation/openai.py` & `literalai-0.0.508/literalai/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/literalai/message.py` & `literalai-0.0.508/literalai/message.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/literalai/my_types.py` & `literalai-0.0.508/literalai/my_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,33 +46,34 @@
         raise NotImplementedError()
 
 
 @dataclass
 class PaginatedResponse(Generic[T]):
     pageInfo: PageInfo
     data: List[T]
+    totalCount: Optional[int] = None
 
     def to_dict(self):
         return {
             "pageInfo": self.pageInfo.to_dict(),
+            "totalCount": self.totalCount,
             "data": [
                 (d.to_dict() if hasattr(d, "to_dict") and callable(d.to_dict) else d)
                 for d in self.data
             ],
         }
 
     @classmethod
     def from_dict(
         cls, paginated_response_dict: Dict, the_class: HasFromDict[T]
     ) -> "PaginatedResponse[T]":
         pageInfo = PageInfo.from_dict(paginated_response_dict.get("pageInfo", {}))
-
         data = [the_class.from_dict(d) for d in paginated_response_dict.get("data", [])]
-
-        return cls(pageInfo=pageInfo, data=data)
+        totalCount = paginated_response_dict.get("totalCount", None)
+        return cls(pageInfo=pageInfo, data=data, totalCount=totalCount)
 
 
 @unique
 class GenerationType(Enum):
     CHAT = "CHAT"
     COMPLETION = "COMPLETION"
```

### Comparing `literalai-0.0.507/literalai/prompt.py` & `literalai-0.0.508/literalai/prompt.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/literalai/requirements.py` & `literalai-0.0.508/literalai/requirements.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/literalai/step.py` & `literalai-0.0.508/literalai/step.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/literalai/thread.py` & `literalai-0.0.508/literalai/thread.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/literalai/wrappers.py` & `literalai-0.0.508/literalai/wrappers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.507/literalai.egg-info/SOURCES.txt` & `literalai-0.0.508/literalai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

