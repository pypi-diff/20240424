# Comparing `tmp/stac-fastapi.elasticsearch-2.2.0.tar.gz` & `tmp/stac_fastapi_elasticsearch-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-fastapi.elasticsearch-2.2.0.tar", last modified: Wed Apr 10 17:05:00 2024, max compression
+gzip compressed data, was "stac_fastapi_elasticsearch-2.3.0.tar", last modified: Wed Apr 24 05:30:36 2024, max compression
```

## Comparing `stac-fastapi.elasticsearch-2.2.0.tar` & `stac_fastapi_elasticsearch-2.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-10 17:05:00.447975 stac-fastapi.elasticsearch-2.2.0/
--rw-r--r--   0 primeradiant   (501) staff       (20)     1547 2024-04-10 17:05:00.447598 stac-fastapi.elasticsearch-2.2.0/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)      101 2024-03-19 04:19:17.000000 stac-fastapi.elasticsearch-2.2.0/README.md
--rw-r--r--   0 primeradiant   (501) staff       (20)      113 2024-04-10 17:05:00.449683 stac-fastapi.elasticsearch-2.2.0/setup.cfg
--rw-r--r--   0 primeradiant   (501) staff       (20)     1725 2024-04-10 15:59:17.000000 stac-fastapi.elasticsearch-2.2.0/setup.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-10 17:05:00.380576 stac-fastapi.elasticsearch-2.2.0/stac_fastapi/
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-10 17:05:00.442039 stac-fastapi.elasticsearch-2.2.0/stac_fastapi/elasticsearch/
--rw-r--r--   0 primeradiant   (501) staff       (20)       31 2024-01-31 03:57:09.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi/elasticsearch/__init__.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     3212 2024-04-09 14:42:19.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi/elasticsearch/app.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     2405 2024-04-09 14:42:19.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi/elasticsearch/config.py
--rw-r--r--   0 primeradiant   (501) staff       (20)    33316 2024-03-19 04:19:17.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi/elasticsearch/database_logic.py
--rw-r--r--   0 primeradiant   (501) staff       (20)       45 2024-04-10 15:56:09.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi/elasticsearch/version.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-10 17:05:00.444141 stac-fastapi.elasticsearch-2.2.0/stac_fastapi.elasticsearch.egg-info/
--rw-r--r--   0 primeradiant   (501) staff       (20)     1547 2024-04-10 17:05:00.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi.elasticsearch.egg-info/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)      572 2024-04-10 17:05:00.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi.elasticsearch.egg-info/SOURCES.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-04-10 17:05:00.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi.elasticsearch.egg-info/dependency_links.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       82 2024-04-10 17:05:00.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi.elasticsearch.egg-info/entry_points.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-02-03 03:16:23.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi.elasticsearch.egg-info/not-zip-safe
--rw-r--r--   0 primeradiant   (501) staff       (20)      246 2024-04-10 17:05:00.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi.elasticsearch.egg-info/requires.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-04-10 17:05:00.000000 stac-fastapi.elasticsearch-2.2.0/stac_fastapi.elasticsearch.egg-info/top_level.txt
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-24 05:30:36.961286 stac_fastapi_elasticsearch-2.3.0/
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1547 2024-04-24 05:30:36.960911 stac_fastapi_elasticsearch-2.3.0/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)      101 2024-03-19 04:19:17.000000 stac_fastapi_elasticsearch-2.3.0/README.md
+-rw-r--r--   0 primeradiant   (501) staff       (20)      113 2024-04-24 05:30:36.962207 stac_fastapi_elasticsearch-2.3.0/setup.cfg
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1725 2024-04-24 05:29:38.000000 stac_fastapi_elasticsearch-2.3.0/setup.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-24 05:30:36.910776 stac_fastapi_elasticsearch-2.3.0/stac_fastapi/
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-24 05:30:36.945595 stac_fastapi_elasticsearch-2.3.0/stac_fastapi/elasticsearch/
+-rw-r--r--   0 primeradiant   (501) staff       (20)       31 2024-01-31 03:57:09.000000 stac_fastapi_elasticsearch-2.3.0/stac_fastapi/elasticsearch/__init__.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     3212 2024-04-09 14:42:19.000000 stac_fastapi_elasticsearch-2.3.0/stac_fastapi/elasticsearch/app.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     2405 2024-04-09 14:42:19.000000 stac_fastapi_elasticsearch-2.3.0/stac_fastapi/elasticsearch/config.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)    33316 2024-03-19 04:19:17.000000 stac_fastapi_elasticsearch-2.3.0/stac_fastapi/elasticsearch/database_logic.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)       45 2024-04-24 05:29:38.000000 stac_fastapi_elasticsearch-2.3.0/stac_fastapi/elasticsearch/version.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-24 05:30:36.946995 stac_fastapi_elasticsearch-2.3.0/stac_fastapi.elasticsearch.egg-info/
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1547 2024-04-24 05:30:36.000000 stac_fastapi_elasticsearch-2.3.0/stac_fastapi.elasticsearch.egg-info/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)      572 2024-04-24 05:30:36.000000 stac_fastapi_elasticsearch-2.3.0/stac_fastapi.elasticsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-04-24 05:30:36.000000 stac_fastapi_elasticsearch-2.3.0/stac_fastapi.elasticsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       82 2024-04-24 05:30:36.000000 stac_fastapi_elasticsearch-2.3.0/stac_fastapi.elasticsearch.egg-info/entry_points.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-02-03 03:16:23.000000 stac_fastapi_elasticsearch-2.3.0/stac_fastapi.elasticsearch.egg-info/not-zip-safe
+-rw-r--r--   0 primeradiant   (501) staff       (20)      246 2024-04-24 05:30:36.000000 stac_fastapi_elasticsearch-2.3.0/stac_fastapi.elasticsearch.egg-info/requires.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-04-24 05:30:36.000000 stac_fastapi_elasticsearch-2.3.0/stac_fastapi.elasticsearch.egg-info/top_level.txt
```

### Comparing `stac-fastapi.elasticsearch-2.2.0/PKG-INFO` & `stac_fastapi_elasticsearch-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.elasticsearch
-Version: 2.2.0
+Version: 2.3.0
 Summary: An implementation of STAC API based on the FastAPI framework with both Elasticsearch and Opensearch.
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
 Requires-Dist: elasticsearch[async]==8.11.0
 Requires-Dist: elasticsearch-dsl==8.11.0
 Requires-Dist: uvicorn
 Requires-Dist: starlette
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
```

### Comparing `stac-fastapi.elasticsearch-2.2.0/setup.py` & `stac_fastapi_elasticsearch-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import find_namespace_packages, setup
 
 with open("README.md") as f:
     desc = f.read()
 
 install_requires = [
-    "stac-fastapi.core==2.2.0",
+    "stac-fastapi.core==2.3.0",
     "elasticsearch[async]==8.11.0",
     "elasticsearch-dsl==8.11.0",
     "uvicorn",
     "starlette",
 ]
 
 extra_reqs = {
```

### Comparing `stac-fastapi.elasticsearch-2.2.0/stac_fastapi/elasticsearch/app.py` & `stac_fastapi_elasticsearch-2.3.0/stac_fastapi/elasticsearch/app.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.elasticsearch-2.2.0/stac_fastapi/elasticsearch/config.py` & `stac_fastapi_elasticsearch-2.3.0/stac_fastapi/elasticsearch/config.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.elasticsearch-2.2.0/stac_fastapi/elasticsearch/database_logic.py` & `stac_fastapi_elasticsearch-2.3.0/stac_fastapi/elasticsearch/database_logic.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.elasticsearch-2.2.0/stac_fastapi.elasticsearch.egg-info/PKG-INFO` & `stac_fastapi_elasticsearch-2.3.0/stac_fastapi.elasticsearch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.elasticsearch
-Version: 2.2.0
+Version: 2.3.0
 Summary: An implementation of STAC API based on the FastAPI framework with both Elasticsearch and Opensearch.
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
 Requires-Dist: elasticsearch[async]==8.11.0
 Requires-Dist: elasticsearch-dsl==8.11.0
 Requires-Dist: uvicorn
 Requires-Dist: starlette
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
```

### Comparing `stac-fastapi.elasticsearch-2.2.0/stac_fastapi.elasticsearch.egg-info/SOURCES.txt` & `stac_fastapi_elasticsearch-2.3.0/stac_fastapi.elasticsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

