# Comparing `tmp/apipe-0.1.7.tar.gz` & `tmp/apipe-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apipe-0.1.7.tar", max compression
+gzip compressed data, was "apipe-0.1.8.tar", max compression
```

## Comparing `apipe-0.1.7.tar` & `apipe-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-04-24 09:50:28.884274 apipe-0.1.7/LICENSE
--rw-r--r--   0        0        0     2369 2024-04-24 09:50:28.884274 apipe-0.1.7/README.md
--rw-r--r--   0        0        0      273 2024-04-24 09:50:28.884274 apipe-0.1.7/apipe/__init__.py
--rw-r--r--   0        0        0    15864 2024-04-24 09:50:28.884274 apipe-0.1.7/apipe/_cached.py
--rw-r--r--   0        0        0     5203 2024-04-24 09:50:28.884274 apipe-0.1.7/apipe/_dask.py
--rw-r--r--   0        0        0     2389 2024-04-24 09:50:45.580366 apipe-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3355 1970-01-01 00:00:00.000000 apipe-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-24 10:28:19.017484 apipe-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2369 2024-04-24 10:28:19.017484 apipe-0.1.8/README.md
+-rw-r--r--   0        0        0      273 2024-04-24 10:28:19.017484 apipe-0.1.8/apipe/__init__.py
+-rw-r--r--   0        0        0    15864 2024-04-24 10:28:19.021484 apipe-0.1.8/apipe/_cached.py
+-rw-r--r--   0        0        0     5203 2024-04-24 10:28:19.021484 apipe-0.1.8/apipe/_dask.py
+-rw-r--r--   0        0        0     2403 2024-04-24 10:28:38.413587 apipe-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3322 1970-01-01 00:00:00.000000 apipe-0.1.8/PKG-INFO
```

### Comparing `apipe-0.1.7/LICENSE` & `apipe-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `apipe-0.1.7/README.md` & `apipe-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `apipe-0.1.7/apipe/_cached.py` & `apipe-0.1.8/apipe/_cached.py`

 * *Files identical despite different names*

### Comparing `apipe-0.1.7/apipe/_dask.py` & `apipe-0.1.8/apipe/_dask.py`

 * *Files identical despite different names*

### Comparing `apipe-0.1.7/pyproject.toml` & `apipe-0.1.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [tool.poetry]
 name = "apipe"
-version = "0.1.7"
+version = "0.1.8"
 description = "Data pipelines with lazy computation and caching"
 authors = ["Mysterious Ben <datascience@tuta.io>"]
 keywords = ["python", "pipeline", "dask", "pandas"]
 readme = "README.md"
 license = "Apache License, Version 2.0"
 homepage = "https://github.com/mysterious-ben/apipe"
 repository = "https://github.com/mysterious-ben/apipe"
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-numpy = "^1.26"
-pandas = "^2.2"
-pyarrow = "^16.0"
-dask = {extras = ["delayed"], version = "^2024.4"}
+numpy = "^1.25"
+pandas = {extras = ["pyarrow"], version = "^2.1"}
+dask = {extras = ["delayed"], version = "^2022"}
 xxhash = "^3.4"
 cloudpickle = "^2.0"
 loguru = ">=0.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^8"
 ruff = ">=0.4"
```

### Comparing `apipe-0.1.7/PKG-INFO` & `apipe-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: apipe
-Version: 0.1.7
+Version: 0.1.8
 Summary: Data pipelines with lazy computation and caching
 Home-page: https://github.com/mysterious-ben/apipe
 License: Apache License, Version 2.0
 Keywords: python,pipeline,dask,pandas
 Author: Mysterious Ben
 Author-email: datascience@tuta.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cloudpickle (>=2.0,<3.0)
-Requires-Dist: dask[delayed] (>=2024.4,<2025.0)
+Requires-Dist: dask[delayed] (>=2022,<2023)
 Requires-Dist: loguru (>=0.5)
-Requires-Dist: numpy (>=1.26,<2.0)
-Requires-Dist: pandas (>=2.2,<3.0)
-Requires-Dist: pyarrow (>=16.0,<17.0)
+Requires-Dist: numpy (>=1.25,<2.0)
+Requires-Dist: pandas[pyarrow] (>=2.1,<3.0)
 Requires-Dist: xxhash (>=3.4,<4.0)
 Project-URL: Repository, https://github.com/mysterious-ben/apipe
 Description-Content-Type: text/markdown
 
 # A-Pipe
 
 **A-Pipe** allows to create data pipelines with lazy computation and caching.
```

