# Comparing `tmp/stac-fastapi.opensearch-2.2.0.tar.gz` & `tmp/stac_fastapi_opensearch-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-fastapi.opensearch-2.2.0.tar", last modified: Wed Apr 10 17:06:38 2024, max compression
+gzip compressed data, was "stac_fastapi_opensearch-2.3.0.tar", last modified: Wed Apr 24 05:36:00 2024, max compression
```

## Comparing `stac-fastapi.opensearch-2.2.0.tar` & `stac_fastapi_opensearch-2.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-10 17:06:38.317047 stac-fastapi.opensearch-2.2.0/
--rw-r--r--   0 primeradiant   (501) staff       (20)     1462 2024-04-10 17:06:38.316791 stac-fastapi.opensearch-2.2.0/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)       92 2024-03-19 04:19:17.000000 stac-fastapi.opensearch-2.2.0/README.md
--rw-r--r--   0 primeradiant   (501) staff       (20)      110 2024-04-10 17:06:38.318054 stac-fastapi.opensearch-2.2.0/setup.cfg
--rw-r--r--   0 primeradiant   (501) staff       (20)     1541 2024-04-10 15:59:05.000000 stac-fastapi.opensearch-2.2.0/setup.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-10 17:06:37.964237 stac-fastapi.opensearch-2.2.0/stac_fastapi/
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-10 17:06:38.233767 stac-fastapi.opensearch-2.2.0/stac_fastapi/opensearch/
--rw-r--r--   0 primeradiant   (501) staff       (20)       28 2024-02-08 06:37:21.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi/opensearch/__init__.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     3191 2024-04-09 15:38:36.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi/opensearch/app.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     2366 2024-04-09 14:42:19.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi/opensearch/config.py
--rw-r--r--   0 primeradiant   (501) staff       (20)    34073 2024-03-19 04:19:17.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi/opensearch/database_logic.py
--rw-r--r--   0 primeradiant   (501) staff       (20)       45 2024-04-10 15:56:39.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi/opensearch/version.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-10 17:06:38.234910 stac-fastapi.opensearch-2.2.0/stac_fastapi.opensearch.egg-info/
--rw-r--r--   0 primeradiant   (501) staff       (20)     1462 2024-04-10 17:06:37.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi.opensearch.egg-info/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)      536 2024-04-10 17:06:37.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi.opensearch.egg-info/SOURCES.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-04-10 17:06:37.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi.opensearch.egg-info/dependency_links.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       76 2024-04-10 17:06:37.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi.opensearch.egg-info/entry_points.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-02-04 04:08:14.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi.opensearch.egg-info/not-zip-safe
--rw-r--r--   0 primeradiant   (501) staff       (20)      240 2024-04-10 17:06:37.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi.opensearch.egg-info/requires.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-04-10 17:06:37.000000 stac-fastapi.opensearch-2.2.0/stac_fastapi.opensearch.egg-info/top_level.txt
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-24 05:36:00.778804 stac_fastapi_opensearch-2.3.0/
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1462 2024-04-24 05:36:00.778538 stac_fastapi_opensearch-2.3.0/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)       92 2024-03-19 04:19:17.000000 stac_fastapi_opensearch-2.3.0/README.md
+-rw-r--r--   0 primeradiant   (501) staff       (20)      110 2024-04-24 05:36:00.779850 stac_fastapi_opensearch-2.3.0/setup.cfg
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1541 2024-04-24 05:29:38.000000 stac_fastapi_opensearch-2.3.0/setup.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-24 05:36:00.731127 stac_fastapi_opensearch-2.3.0/stac_fastapi/
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-24 05:36:00.767167 stac_fastapi_opensearch-2.3.0/stac_fastapi/opensearch/
+-rw-r--r--   0 primeradiant   (501) staff       (20)       28 2024-02-08 06:37:21.000000 stac_fastapi_opensearch-2.3.0/stac_fastapi/opensearch/__init__.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     3191 2024-04-09 15:38:36.000000 stac_fastapi_opensearch-2.3.0/stac_fastapi/opensearch/app.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     2366 2024-04-09 14:42:19.000000 stac_fastapi_opensearch-2.3.0/stac_fastapi/opensearch/config.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)    34073 2024-03-19 04:19:17.000000 stac_fastapi_opensearch-2.3.0/stac_fastapi/opensearch/database_logic.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)       45 2024-04-24 05:29:38.000000 stac_fastapi_opensearch-2.3.0/stac_fastapi/opensearch/version.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-24 05:36:00.770058 stac_fastapi_opensearch-2.3.0/stac_fastapi.opensearch.egg-info/
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1462 2024-04-24 05:36:00.000000 stac_fastapi_opensearch-2.3.0/stac_fastapi.opensearch.egg-info/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)      536 2024-04-24 05:36:00.000000 stac_fastapi_opensearch-2.3.0/stac_fastapi.opensearch.egg-info/SOURCES.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-04-24 05:36:00.000000 stac_fastapi_opensearch-2.3.0/stac_fastapi.opensearch.egg-info/dependency_links.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       76 2024-04-24 05:36:00.000000 stac_fastapi_opensearch-2.3.0/stac_fastapi.opensearch.egg-info/entry_points.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-02-04 04:08:14.000000 stac_fastapi_opensearch-2.3.0/stac_fastapi.opensearch.egg-info/not-zip-safe
+-rw-r--r--   0 primeradiant   (501) staff       (20)      240 2024-04-24 05:36:00.000000 stac_fastapi_opensearch-2.3.0/stac_fastapi.opensearch.egg-info/requires.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-04-24 05:36:00.000000 stac_fastapi_opensearch-2.3.0/stac_fastapi.opensearch.egg-info/top_level.txt
```

### Comparing `stac-fastapi.opensearch-2.2.0/PKG-INFO` & `stac_fastapi_opensearch-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.opensearch
-Version: 2.2.0
+Version: 2.3.0
 Summary: Opensearch stac-fastapi backend.
 Home-page: https://github.com/stac-utils/stac-fastapi-elasticsearch-opensearch
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: stac-fastapi.core==2.2.0
+Requires-Dist: stac-fastapi.core==2.3.0
 Requires-Dist: opensearch-py==2.4.2
 Requires-Dist: opensearch-py[async]==2.4.2
 Requires-Dist: uvicorn
 Requires-Dist: starlette
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
```

### Comparing `stac-fastapi.opensearch-2.2.0/setup.py` & `stac_fastapi_opensearch-2.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import find_namespace_packages, setup
 
 with open("README.md") as f:
     desc = f.read()
 
 install_requires = [
-    "stac-fastapi.core==2.2.0",
+    "stac-fastapi.core==2.3.0",
     "opensearch-py==2.4.2",
     "opensearch-py[async]==2.4.2",
     "uvicorn",
     "starlette",
 ]
 
 extra_reqs = {
```

### Comparing `stac-fastapi.opensearch-2.2.0/stac_fastapi/opensearch/app.py` & `stac_fastapi_opensearch-2.3.0/stac_fastapi/opensearch/app.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.opensearch-2.2.0/stac_fastapi/opensearch/config.py` & `stac_fastapi_opensearch-2.3.0/stac_fastapi/opensearch/config.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.opensearch-2.2.0/stac_fastapi/opensearch/database_logic.py` & `stac_fastapi_opensearch-2.3.0/stac_fastapi/opensearch/database_logic.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.opensearch-2.2.0/stac_fastapi.opensearch.egg-info/PKG-INFO` & `stac_fastapi_opensearch-2.3.0/stac_fastapi.opensearch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.opensearch
-Version: 2.2.0
+Version: 2.3.0
 Summary: Opensearch stac-fastapi backend.
 Home-page: https://github.com/stac-utils/stac-fastapi-elasticsearch-opensearch
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: stac-fastapi.core==2.2.0
+Requires-Dist: stac-fastapi.core==2.3.0
 Requires-Dist: opensearch-py==2.4.2
 Requires-Dist: opensearch-py[async]==2.4.2
 Requires-Dist: uvicorn
 Requires-Dist: starlette
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
```

### Comparing `stac-fastapi.opensearch-2.2.0/stac_fastapi.opensearch.egg-info/SOURCES.txt` & `stac_fastapi_opensearch-2.3.0/stac_fastapi.opensearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

