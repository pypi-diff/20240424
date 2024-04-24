# Comparing `tmp/emiapi-0.1.1.tar.gz` & `tmp/emiapi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emiapi-0.1.1.tar", max compression
+gzip compressed data, was "emiapi-0.2.0.tar", max compression
```

## Comparing `emiapi-0.1.1.tar` & `emiapi-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       85 2023-05-05 16:23:20.107588 emiapi-0.1.1/emiapi/__init__.py
--rw-r--r--   0        0        0     7598 2023-05-05 16:23:20.107588 emiapi-0.1.1/emiapi/emiapi.py
--rw-r--r--   0        0        0     1263 2023-05-05 16:23:20.107588 emiapi-0.1.1/emiapi/plotting.py
--rw-r--r--   0        0        0      654 2023-08-24 10:05:18.568462 emiapi-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 emiapi-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       85 2023-05-05 16:23:20.107588 emiapi-0.2.0/emiapi/__init__.py
+-rw-r--r--   0        0        0     7598 2023-05-05 16:23:20.107588 emiapi-0.2.0/emiapi/emiapi.py
+-rw-r--r--   0        0        0     1263 2023-05-05 16:23:20.107588 emiapi-0.2.0/emiapi/plotting.py
+-rw-r--r--   0        0        0     1085 2023-08-24 13:39:14.462156 emiapi-0.2.0/LICENSE
+-rw-r--r--   0        0        0      543 2024-04-24 07:24:17.647998 emiapi-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 emiapi-0.2.0/PKG-INFO
```

### Comparing `emiapi-0.1.1/emiapi/emiapi.py` & `emiapi-0.2.0/emiapi/emiapi.py`

 * *Files identical despite different names*

### Comparing `emiapi-0.1.1/emiapi/plotting.py` & `emiapi-0.2.0/emiapi/plotting.py`

 * *Files identical despite different names*

### Comparing `emiapi-0.1.1/pyproject.toml` & `emiapi-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "emiapi"
-version = "0.1.1"
+version = "0.2.0"
 description = "A python API client to interact with EMI API"
 authors = ["Jean Luchier <jean.luchier@imageau.eu>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pandas = "^1.3.2"
 requests = "^2.26.0"
@@ -18,12 +18,8 @@
 jupyterlab = "^3.6.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [virtualenvs]
-in-project = true
-[repositories]
-
-[repositories.my-gitlab]
-url = "https://gitlab.com/api/v4/projects/29154471/packages/pypi"
+in-project = true
```

### Comparing `emiapi-0.1.1/PKG-INFO` & `emiapi-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emiapi
-Version: 0.1.1
+Version: 0.2.0
 Summary: A python API client to interact with EMI API
 Author: Jean Luchier
 Author-email: jean.luchier@imageau.eu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

