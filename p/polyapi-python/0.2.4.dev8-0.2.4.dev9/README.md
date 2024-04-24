# Comparing `tmp/polyapi_python-0.2.4.dev8.tar.gz` & `tmp/polyapi_python-0.2.4.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyapi_python-0.2.4.dev8.tar", last modified: Tue Apr 23 16:41:14 2024, max compression
+gzip compressed data, was "polyapi_python-0.2.4.dev9.tar", last modified: Tue Apr 23 19:40:46 2024, max compression
```

## Comparing `polyapi_python-0.2.4.dev8.tar` & `polyapi_python-0.2.4.dev9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:14.677046 polyapi_python-0.2.4.dev8/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-23 16:41:14.677046 polyapi_python-0.2.4.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:14.677046 polyapi_python-0.2.4.dev8/polyapi/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     9129 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/poly_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/polyapi/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:14.677046 polyapi_python-0.2.4.dev8/polyapi_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-23 16:41:14.000000 polyapi_python-0.2.4.dev8/polyapi_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-23 16:41:14.000000 polyapi_python-0.2.4.dev8/polyapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:41:14.000000 polyapi_python-0.2.4.dev8/polyapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-23 16:41:14.000000 polyapi_python-0.2.4.dev8/polyapi_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 16:41:14.000000 polyapi_python-0.2.4.dev8/polyapi_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:41:14.677046 polyapi_python-0.2.4.dev8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:41:14.677046 polyapi_python-0.2.4.dev8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/tests/test_function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-23 16:41:10.000000 polyapi_python-0.2.4.dev8/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:40:46.489624 polyapi_python-0.2.4.dev9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-23 19:40:46.489624 polyapi_python-0.2.4.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:40:46.485624 polyapi_python-0.2.4.dev9/polyapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9129 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/poly_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/polyapi/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:40:46.489624 polyapi_python-0.2.4.dev9/polyapi_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-23 19:40:46.000000 polyapi_python-0.2.4.dev9/polyapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-23 19:40:46.000000 polyapi_python-0.2.4.dev9/polyapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:40:46.000000 polyapi_python-0.2.4.dev9/polyapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-23 19:40:46.000000 polyapi_python-0.2.4.dev9/polyapi_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 19:40:46.000000 polyapi_python-0.2.4.dev9/polyapi_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:40:46.489624 polyapi_python-0.2.4.dev9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:40:46.489624 polyapi_python-0.2.4.dev9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/tests/test_function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-23 19:40:42.000000 polyapi_python-0.2.4.dev9/tests/test_variables.py
```

### Comparing `polyapi_python-0.2.4.dev8/LICENSE` & `polyapi_python-0.2.4.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev8/PKG-INFO` & `polyapi_python-0.2.4.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.4.dev8
+Version: 0.2.4.dev9
 Summary: The Python Client for PolyAPI, the IPaaS by Developers for Developers
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polyapi_python-0.2.4.dev8/README.md` & `polyapi_python-0.2.4.dev9/README.md`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev8/polyapi/api.py` & `polyapi_python-0.2.4.dev9/polyapi/api.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev8/polyapi/auth.py` & `polyapi_python-0.2.4.dev9/polyapi/auth.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev8/polyapi/cli.py` & `polyapi_python-0.2.4.dev9/polyapi/cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev8/polyapi/client.py` & `polyapi_python-0.2.4.dev9/polyapi/client.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev8/polyapi/config.py` & `polyapi_python-0.2.4.dev9/polyapi/config.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev8/polyapi/error_handler.py` & `polyapi_python-0.2.4.dev9/polyapi/error_handler.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev8/polyapi/execute.py` & `polyapi_python-0.2.4.dev9/polyapi/execute.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev8/polyapi/function_cli.py` & `polyapi_python-0.2.4.dev9/polyapi/function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev8/polyapi/generate.py` & `polyapi_python-0.2.4.dev9/polyapi/generate.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev8/polyapi/schema.py` & `polyapi_python-0.2.4.dev9/polyapi/schema.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev8/polyapi/server.py` & `polyapi_python-0.2.4.dev9/polyapi/server.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev8/polyapi/typedefs.py` & `polyapi_python-0.2.4.dev9/polyapi/typedefs.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev8/polyapi/utils.py` & `polyapi_python-0.2.4.dev9/polyapi/utils.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev8/polyapi/variables.py` & `polyapi_python-0.2.4.dev9/polyapi/variables.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev8/polyapi/webhook.py` & `polyapi_python-0.2.4.dev9/polyapi/webhook.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import socketio  # type: ignore
+from socketio.exceptions import ConnectionError  # type: ignore
 import uuid
 from typing import Any, Dict, List, Tuple
 
 from polyapi.config import get_api_key_and_url
 from polyapi.typedefs import PropertySpecification
 
 # all active webhook handlers, used by unregister_all to cleanup
@@ -88,16 +89,20 @@
         },
         "/events",
     )
 
 
 async def unregister_all():
     _, base_url = get_api_key_and_url()
-    # need to reconnect because maybe socketio client disconnected after Ctrl+C?
-    await client.connect(base_url, transports=["websocket"], namespaces=["/events"])
+    # maybe need to reconnect because maybe socketio client disconnected after Ctrl+C?
+    # feels like Linux disconnects but Windows stays connected
+    try:
+        await client.connect(base_url, transports=["websocket"], namespaces=["/events"])
+    except ConnectionError:
+        pass
     await asyncio.gather(*[unregister(handler) for handler in active_handlers])
 
 
 def render_webhook_handle(
     function_type: str,
     function_name: str,
     function_id: str,
```

### Comparing `polyapi_python-0.2.4.dev8/polyapi_python.egg-info/PKG-INFO` & `polyapi_python-0.2.4.dev9/polyapi_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.4.dev8
+Version: 0.2.4.dev9
 Summary: The Python Client for PolyAPI, the IPaaS by Developers for Developers
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polyapi_python-0.2.4.dev8/polyapi_python.egg-info/SOURCES.txt` & `polyapi_python-0.2.4.dev9/polyapi_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev8/pyproject.toml` & `polyapi_python-0.2.4.dev9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.2", "wheel"]
 
 [project]
 name = "polyapi-python"
-version = "0.2.4.dev8"
+version = "0.2.4.dev9"
 description = "The Python Client for PolyAPI, the IPaaS by Developers for Developers"
 authors = [{ name = "Dan Fellin", email = "dan@polyapi.io" }]
 dependencies = [
     "requests==2.31.0",
     "typing_extensions==4.10.0",
     "jsonschema-gentypes==2.4.0",
     "pydantic==2.6.4",
```

### Comparing `polyapi_python-0.2.4.dev8/tests/test_api.py` & `polyapi_python-0.2.4.dev9/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev8/tests/test_auth.py` & `polyapi_python-0.2.4.dev9/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev8/tests/test_function_cli.py` & `polyapi_python-0.2.4.dev9/tests/test_function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev8/tests/test_server.py` & `polyapi_python-0.2.4.dev9/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev8/tests/test_utils.py` & `polyapi_python-0.2.4.dev9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.4.dev8/tests/test_variables.py` & `polyapi_python-0.2.4.dev9/tests/test_variables.py`

 * *Files identical despite different names*

