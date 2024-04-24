# Comparing `tmp/stac_fastapi_api-2.5.3.tar.gz` & `tmp/stac_fastapi_api-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_api-2.5.3.tar", last modified: Mon Apr 22 17:12:25 2024, max compression
+gzip compressed data, was "stac_fastapi_api-2.5.4.tar", last modified: Wed Apr 24 16:03:58 2024, max compression
```

## Comparing `stac_fastapi_api-2.5.3.tar` & `stac_fastapi_api-2.5.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:12:25.519811 stac_fastapi_api-2.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-22 17:12:25.519811 stac_fastapi_api-2.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 17:12:04.000000 stac_fastapi_api-2.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-22 17:12:25.519811 stac_fastapi_api-2.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-22 17:12:04.000000 stac_fastapi_api-2.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:12:25.515811 stac_fastapi_api-2.5.3/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:12:25.515811 stac_fastapi_api-2.5.3/stac_fastapi/api/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 17:12:04.000000 stac_fastapi_api-2.5.3/stac_fastapi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14595 2024-04-22 17:12:04.000000 stac_fastapi_api-2.5.3/stac_fastapi/api/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-22 17:12:04.000000 stac_fastapi_api-2.5.3/stac_fastapi/api/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-22 17:12:04.000000 stac_fastapi_api-2.5.3/stac_fastapi/api/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-22 17:12:04.000000 stac_fastapi_api-2.5.3/stac_fastapi/api/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-22 17:12:04.000000 stac_fastapi_api-2.5.3/stac_fastapi/api/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-22 17:12:04.000000 stac_fastapi_api-2.5.3/stac_fastapi/api/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-22 17:12:04.000000 stac_fastapi_api-2.5.3/stac_fastapi/api/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-22 17:12:04.000000 stac_fastapi_api-2.5.3/stac_fastapi/api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:12:25.519811 stac_fastapi_api-2.5.3/stac_fastapi.api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-22 17:12:25.000000 stac_fastapi_api-2.5.3/stac_fastapi.api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-22 17:12:25.000000 stac_fastapi_api-2.5.3/stac_fastapi.api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 17:12:25.000000 stac_fastapi_api-2.5.3/stac_fastapi.api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 17:12:25.000000 stac_fastapi_api-2.5.3/stac_fastapi.api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-22 17:12:25.000000 stac_fastapi_api-2.5.3/stac_fastapi.api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-22 17:12:25.000000 stac_fastapi_api-2.5.3/stac_fastapi.api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:12:25.519811 stac_fastapi_api-2.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-22 17:12:04.000000 stac_fastapi_api-2.5.3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-22 17:12:04.000000 stac_fastapi_api-2.5.3/tests/test_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:03:58.600550 stac_fastapi_api-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-24 16:03:58.600550 stac_fastapi_api-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:03:38.000000 stac_fastapi_api-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 16:03:58.600550 stac_fastapi_api-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-24 16:03:38.000000 stac_fastapi_api-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:03:58.592550 stac_fastapi_api-2.5.4/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:03:58.596550 stac_fastapi_api-2.5.4/stac_fastapi/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 16:03:38.000000 stac_fastapi_api-2.5.4/stac_fastapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14595 2024-04-24 16:03:38.000000 stac_fastapi_api-2.5.4/stac_fastapi/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-24 16:03:38.000000 stac_fastapi_api-2.5.4/stac_fastapi/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-24 16:03:38.000000 stac_fastapi_api-2.5.4/stac_fastapi/api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-24 16:03:38.000000 stac_fastapi_api-2.5.4/stac_fastapi/api/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-24 16:03:38.000000 stac_fastapi_api-2.5.4/stac_fastapi/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-24 16:03:38.000000 stac_fastapi_api-2.5.4/stac_fastapi/api/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-24 16:03:38.000000 stac_fastapi_api-2.5.4/stac_fastapi/api/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-24 16:03:38.000000 stac_fastapi_api-2.5.4/stac_fastapi/api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:03:58.596550 stac_fastapi_api-2.5.4/stac_fastapi.api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-24 16:03:58.000000 stac_fastapi_api-2.5.4/stac_fastapi.api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-24 16:03:58.000000 stac_fastapi_api-2.5.4/stac_fastapi.api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:03:58.000000 stac_fastapi_api-2.5.4/stac_fastapi.api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:03:58.000000 stac_fastapi_api-2.5.4/stac_fastapi.api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-24 16:03:58.000000 stac_fastapi_api-2.5.4/stac_fastapi.api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 16:03:58.000000 stac_fastapi_api-2.5.4/stac_fastapi.api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:03:58.596550 stac_fastapi_api-2.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-24 16:03:38.000000 stac_fastapi_api-2.5.4/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-24 16:03:38.000000 stac_fastapi_api-2.5.4/tests/test_middleware.py
```

### Comparing `stac_fastapi_api-2.5.3/PKG-INFO` & `stac_fastapi_api-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.api
-Version: 2.5.3
+Version: 2.5.4
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac_fastapi_api-2.5.3/setup.py` & `stac_fastapi_api-2.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-2.5.3/stac_fastapi/api/app.py` & `stac_fastapi_api-2.5.4/stac_fastapi/api/app.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-2.5.3/stac_fastapi/api/config.py` & `stac_fastapi_api-2.5.4/stac_fastapi/api/config.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-2.5.3/stac_fastapi/api/errors.py` & `stac_fastapi_api-2.5.4/stac_fastapi/api/errors.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-2.5.3/stac_fastapi/api/middleware.py` & `stac_fastapi_api-2.5.4/stac_fastapi/api/middleware.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-2.5.3/stac_fastapi/api/models.py` & `stac_fastapi_api-2.5.4/stac_fastapi/api/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,22 +99,22 @@
         extensions=extensions,
         request_type="POST",
     )
 
 
 @attr.s  # type:ignore
 class CollectionUri(APIRequest):
-    """Delete collection."""
+    """Get or delete collection."""
 
     collection_id: str = attr.ib(default=Path(..., description="Collection ID"))
 
 
 @attr.s
 class ItemUri(CollectionUri):
-    """Delete item."""
+    """Get or delete item."""
 
     item_id: str = attr.ib(default=Path(..., description="Item ID"))
 
 
 @attr.s
 class EmptyRequest(APIRequest):
     """Empty request."""
```

### Comparing `stac_fastapi_api-2.5.3/stac_fastapi/api/openapi.py` & `stac_fastapi_api-2.5.4/stac_fastapi/api/openapi.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-2.5.3/stac_fastapi/api/routes.py` & `stac_fastapi_api-2.5.4/stac_fastapi/api/routes.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-2.5.3/stac_fastapi.api.egg-info/PKG-INFO` & `stac_fastapi_api-2.5.4/stac_fastapi.api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.api
-Version: 2.5.3
+Version: 2.5.4
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac_fastapi_api-2.5.3/stac_fastapi.api.egg-info/SOURCES.txt` & `stac_fastapi_api-2.5.4/stac_fastapi.api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-2.5.3/tests/test_api.py` & `stac_fastapi_api-2.5.4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-2.5.3/tests/test_middleware.py` & `stac_fastapi_api-2.5.4/tests/test_middleware.py`

 * *Files identical despite different names*

