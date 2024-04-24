# Comparing `tmp/apipe-0.1.5.tar.gz` & `tmp/apipe-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apipe-0.1.5.tar", max compression
+gzip compressed data, was "apipe-0.1.6.tar", max compression
```

## Comparing `apipe-0.1.5.tar` & `apipe-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-04-23 16:25:03.522440 apipe-0.1.5/LICENSE
--rw-r--r--   0        0        0     2369 2024-04-23 16:25:03.522440 apipe-0.1.5/README.md
--rw-r--r--   0        0        0      273 2024-04-23 16:25:03.522440 apipe-0.1.5/apipe/__init__.py
--rw-r--r--   0        0        0    15864 2024-04-23 16:25:03.522440 apipe-0.1.5/apipe/_cached.py
--rw-r--r--   0        0        0     5203 2024-04-23 16:25:03.522440 apipe-0.1.5/apipe/_dask.py
--rw-r--r--   0        0        0     2412 2024-04-23 16:25:20.722422 apipe-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 apipe-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-24 09:09:28.040928 apipe-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2369 2024-04-24 09:09:28.040928 apipe-0.1.6/README.md
+-rw-r--r--   0        0        0      273 2024-04-24 09:09:28.040928 apipe-0.1.6/apipe/__init__.py
+-rw-r--r--   0        0        0    15864 2024-04-24 09:09:28.040928 apipe-0.1.6/apipe/_cached.py
+-rw-r--r--   0        0        0     5203 2024-04-24 09:09:28.040928 apipe-0.1.6/apipe/_dask.py
+-rw-r--r--   0        0        0     2388 2024-04-24 09:09:48.581003 apipe-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3360 1970-01-01 00:00:00.000000 apipe-0.1.6/PKG-INFO
```

### Comparing `apipe-0.1.5/LICENSE` & `apipe-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `apipe-0.1.5/README.md` & `apipe-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `apipe-0.1.5/apipe/_cached.py` & `apipe-0.1.6/apipe/_cached.py`

 * *Files identical despite different names*

### Comparing `apipe-0.1.5/apipe/_dask.py` & `apipe-0.1.6/apipe/_dask.py`

 * *Files identical despite different names*

### Comparing `apipe-0.1.5/pyproject.toml` & `apipe-0.1.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [tool.poetry]
 name = "apipe"
-version = "0.1.5"
+version = "0.1.6"
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
-numpy = "^1.26.4"
-pandas = "^2.2.2"
-pyarrow = "^16.0.0"
-dask = {extras = ["delayed"], version = "^2024.4.2"}
-xxhash = "^3.4.1"
-cloudpickle = "^2.0.0"
-loguru = "^0.6.0"
+numpy = "^1.26"
+pandas = "^2.2"
+pyarrow = "^16.0"
+dask = {extras = ["delayed"], version = "^2024.4"}
+xxhash = "^3.4"
+cloudpickle = "^2.0"
+loguru = "^0.6"
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
-ruff = "^0.4.1"
-black = "^24.4.0"
-pylint = "^3.1.0"
+pytest = "^6.2"
+ruff = "^0.4"
+black = "^24.4"
+pylint = "^3.1"
 mypy = "^0.910"
-pre-commit = "^3.7.0"
+pre-commit = "^3.7"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.black]
```

### Comparing `apipe-0.1.5/PKG-INFO` & `apipe-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: apipe
-Version: 0.1.5
+Version: 0.1.6
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
-Requires-Dist: cloudpickle (>=2.0.0,<3.0.0)
-Requires-Dist: dask[delayed] (>=2024.4.2,<2025.0.0)
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Requires-Dist: pandas (>=2.2.2,<3.0.0)
-Requires-Dist: pyarrow (>=16.0.0,<17.0.0)
-Requires-Dist: xxhash (>=3.4.1,<4.0.0)
+Requires-Dist: cloudpickle (>=2.0,<3.0)
+Requires-Dist: dask[delayed] (>=2024.4,<2025.0)
+Requires-Dist: loguru (>=0.6,<0.7)
+Requires-Dist: numpy (>=1.26,<2.0)
+Requires-Dist: pandas (>=2.2,<3.0)
+Requires-Dist: pyarrow (>=16.0,<17.0)
+Requires-Dist: xxhash (>=3.4,<4.0)
 Project-URL: Repository, https://github.com/mysterious-ben/apipe
 Description-Content-Type: text/markdown
 
 # A-Pipe
 
 **A-Pipe** allows to create data pipelines with lazy computation and caching.
```

