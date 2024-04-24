# Comparing `tmp/gcp_pal-1.0.0.tar.gz` & `tmp/gcp_pal-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp_pal-1.0.0.tar", max compression
+gzip compressed data, was "gcp_pal-1.0.1.tar", max compression
```

## Comparing `gcp_pal-1.0.0.tar` & `gcp_pal-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    23163 2024-04-21 20:42:43.978491 gcp_pal-1.0.0/README.md
--rw-r--r--   0        0        0      760 2024-04-21 20:42:43.982492 gcp_pal-1.0.0/gcp_pal/__init__.py
--rw-r--r--   0        0        0    31402 2024-04-21 20:42:43.982492 gcp_pal-1.0.0/gcp_pal/bigquery.py
--rw-r--r--   0        0        0    13156 2024-04-21 20:42:43.982492 gcp_pal-1.0.0/gcp_pal/cloudfunctions.py
--rw-r--r--   0        0        0    13855 2024-04-21 20:42:43.982492 gcp_pal-1.0.0/gcp_pal/cloudrun.py
--rw-r--r--   0        0        0     7754 2024-04-21 20:42:43.982492 gcp_pal-1.0.0/gcp_pal/cloudscheduler.py
--rw-r--r--   0        0        0       42 2024-04-21 20:42:43.982492 gcp_pal-1.0.0/gcp_pal/config/__init__.py
--rw-r--r--   0        0        0      895 2024-04-21 20:42:43.982492 gcp_pal-1.0.0/gcp_pal/config/vars.py
--rw-r--r--   0        0        0    12490 2024-04-21 20:42:43.982492 gcp_pal-1.0.0/gcp_pal/firestore.py
--rw-r--r--   0        0        0     1674 2024-04-21 20:42:43.982492 gcp_pal-1.0.0/gcp_pal/pubsub.py
--rw-r--r--   0        0        0     3873 2024-04-21 20:42:43.982492 gcp_pal-1.0.0/gcp_pal/pydocker.py
--rw-r--r--   0        0        0     6860 2024-04-21 20:42:43.982492 gcp_pal-1.0.0/gcp_pal/pylogging.py
--rw-r--r--   0        0        0     4737 2024-04-21 20:42:43.982492 gcp_pal-1.0.0/gcp_pal/request.py
--rw-r--r--   0        0        0    23631 2024-04-21 20:42:43.982492 gcp_pal-1.0.0/gcp_pal/schema.py
--rw-r--r--   0        0        0     6332 2024-04-21 20:42:43.982492 gcp_pal-1.0.0/gcp_pal/secretmanager.py
--rw-r--r--   0        0        0       88 2024-04-21 20:42:43.982492 gcp_pal-1.0.0/gcp_pal/storage/__init__.py
--rw-r--r--   0        0        0     8735 2024-04-21 20:42:43.982492 gcp_pal-1.0.0/gcp_pal/storage/parquet.py
--rw-r--r--   0        0        0    17133 2024-04-21 20:42:43.982492 gcp_pal-1.0.0/gcp_pal/storage/storage.py
--rw-r--r--   0        0        0       82 2024-04-21 20:42:43.982492 gcp_pal-1.0.0/gcp_pal/utils/__init__.py
--rw-r--r--   0        0        0      935 2024-04-21 20:42:43.982492 gcp_pal-1.0.0/gcp_pal/utils/lazy_loader.py
--rw-r--r--   0        0        0    10898 2024-04-21 20:42:43.982492 gcp_pal-1.0.0/gcp_pal/utils/utils.py
--rw-r--r--   0        0        0      916 2024-04-21 20:42:43.982492 gcp_pal-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    23553 1970-01-01 00:00:00.000000 gcp_pal-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    23782 2024-04-24 08:47:13.070910 gcp_pal-1.0.1/README.md
+-rw-r--r--   0        0        0      760 2024-04-24 08:47:13.070910 gcp_pal-1.0.1/gcp_pal/__init__.py
+-rw-r--r--   0        0        0    31402 2024-04-24 08:47:13.070910 gcp_pal-1.0.1/gcp_pal/bigquery.py
+-rw-r--r--   0        0        0    13156 2024-04-24 08:47:13.070910 gcp_pal-1.0.1/gcp_pal/cloudfunctions.py
+-rw-r--r--   0        0        0    13855 2024-04-24 08:47:13.070910 gcp_pal-1.0.1/gcp_pal/cloudrun.py
+-rw-r--r--   0        0        0     7754 2024-04-24 08:47:13.070910 gcp_pal-1.0.1/gcp_pal/cloudscheduler.py
+-rw-r--r--   0        0        0       42 2024-04-24 08:47:13.070910 gcp_pal-1.0.1/gcp_pal/config/__init__.py
+-rw-r--r--   0        0        0      895 2024-04-24 08:47:13.070910 gcp_pal-1.0.1/gcp_pal/config/vars.py
+-rw-r--r--   0        0        0    12490 2024-04-24 08:47:13.070910 gcp_pal-1.0.1/gcp_pal/firestore.py
+-rw-r--r--   0        0        0     1674 2024-04-24 08:47:13.070910 gcp_pal-1.0.1/gcp_pal/pubsub.py
+-rw-r--r--   0        0        0     3873 2024-04-24 08:47:13.070910 gcp_pal-1.0.1/gcp_pal/pydocker.py
+-rw-r--r--   0        0        0     6860 2024-04-24 08:47:13.074910 gcp_pal-1.0.1/gcp_pal/pylogging.py
+-rw-r--r--   0        0        0     4737 2024-04-24 08:47:13.074910 gcp_pal-1.0.1/gcp_pal/request.py
+-rw-r--r--   0        0        0    23631 2024-04-24 08:47:13.074910 gcp_pal-1.0.1/gcp_pal/schema.py
+-rw-r--r--   0        0        0     6332 2024-04-24 08:47:13.074910 gcp_pal-1.0.1/gcp_pal/secretmanager.py
+-rw-r--r--   0        0        0       88 2024-04-24 08:47:13.074910 gcp_pal-1.0.1/gcp_pal/storage/__init__.py
+-rw-r--r--   0        0        0     8735 2024-04-24 08:47:13.074910 gcp_pal-1.0.1/gcp_pal/storage/parquet.py
+-rw-r--r--   0        0        0    17133 2024-04-24 08:47:13.074910 gcp_pal-1.0.1/gcp_pal/storage/storage.py
+-rw-r--r--   0        0        0       82 2024-04-24 08:47:13.074910 gcp_pal-1.0.1/gcp_pal/utils/__init__.py
+-rw-r--r--   0        0        0      935 2024-04-24 08:47:13.074910 gcp_pal-1.0.1/gcp_pal/utils/lazy_loader.py
+-rw-r--r--   0        0        0    10898 2024-04-24 08:47:13.074910 gcp_pal-1.0.1/gcp_pal/utils/utils.py
+-rw-r--r--   0        0        0      916 2024-04-24 08:47:13.074910 gcp_pal-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    24172 1970-01-01 00:00:00.000000 gcp_pal-1.0.1/PKG-INFO
```

### Comparing `gcp_pal-1.0.0/README.md` & `gcp_pal-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,34 @@
 
 The `gcp-pal` library provides a set of utilities for interacting with Google Cloud Platform (GCP) services, streamlining the process of implementing GCP functionalities within your Python applications.
 
 The utilities are designed to work with the `google-cloud` Python libraries, providing a more user-friendly and intuitive interface for common tasks.
 
 ---
 
+## Installation
+
+The package is available on PyPI as `gcp-pal`. To install with `pip`:
+
+```bash
+pip install gcp-pal
+```
+
+The library has no dependencies other than Python 3.10 or newer. The modules are set up to notify the user if any required libraries are missing. For example, when attempting to use the `Firestore` module:
+
+```python
+from gcp_pal import Firestore
+Firestore()
+# ImportError: Module 'Firestore' requires 'google.cloud.firestore' (PyPI: 'google-cloud-firestore') to be installed.
+```
+
+Which lets the user know that the `google-cloud-firestore` package is required to use the `Firestore` module.
+
+---
+
 ## Configuration
 
 Before you can start using the `gcp-pal` library with Firestore or any other GCP services, make sure you either have set up your GCP credentials properly or have the necessary permissions to access the services you want to use:
 
 ```bash
 gcloud auth application-default login
 ```
```

### Comparing `gcp_pal-1.0.0/gcp_pal/__init__.py` & `gcp_pal-1.0.1/gcp_pal/__init__.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.0/gcp_pal/bigquery.py` & `gcp_pal-1.0.1/gcp_pal/bigquery.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.0/gcp_pal/cloudfunctions.py` & `gcp_pal-1.0.1/gcp_pal/cloudfunctions.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.0/gcp_pal/cloudrun.py` & `gcp_pal-1.0.1/gcp_pal/cloudrun.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.0/gcp_pal/cloudscheduler.py` & `gcp_pal-1.0.1/gcp_pal/cloudscheduler.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.0/gcp_pal/config/vars.py` & `gcp_pal-1.0.1/gcp_pal/config/vars.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.0/gcp_pal/firestore.py` & `gcp_pal-1.0.1/gcp_pal/firestore.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.0/gcp_pal/pubsub.py` & `gcp_pal-1.0.1/gcp_pal/pubsub.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.0/gcp_pal/pydocker.py` & `gcp_pal-1.0.1/gcp_pal/pydocker.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.0/gcp_pal/pylogging.py` & `gcp_pal-1.0.1/gcp_pal/pylogging.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.0/gcp_pal/request.py` & `gcp_pal-1.0.1/gcp_pal/request.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.0/gcp_pal/schema.py` & `gcp_pal-1.0.1/gcp_pal/schema.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.0/gcp_pal/secretmanager.py` & `gcp_pal-1.0.1/gcp_pal/secretmanager.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.0/gcp_pal/storage/parquet.py` & `gcp_pal-1.0.1/gcp_pal/storage/parquet.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.0/gcp_pal/storage/storage.py` & `gcp_pal-1.0.1/gcp_pal/storage/storage.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.0/gcp_pal/utils/lazy_loader.py` & `gcp_pal-1.0.1/gcp_pal/utils/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.0/gcp_pal/utils/utils.py` & `gcp_pal-1.0.1/gcp_pal/utils/utils.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.0/pyproject.toml` & `gcp_pal-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gcp-pal"
-version = "1.0.0"
+version = "1.0.1"
 description = ""
 authors = ["VitaminB16 <artemiy.nosov@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gcp_pal-1.0.0/PKG-INFO` & `gcp_pal-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-pal
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 Author: VitaminB16
 Author-email: artemiy.nosov@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -36,14 +36,34 @@
 
 The `gcp-pal` library provides a set of utilities for interacting with Google Cloud Platform (GCP) services, streamlining the process of implementing GCP functionalities within your Python applications.
 
 The utilities are designed to work with the `google-cloud` Python libraries, providing a more user-friendly and intuitive interface for common tasks.
 
 ---
 
+## Installation
+
+The package is available on PyPI as `gcp-pal`. To install with `pip`:
+
+```bash
+pip install gcp-pal
+```
+
+The library has no dependencies other than Python 3.10 or newer. The modules are set up to notify the user if any required libraries are missing. For example, when attempting to use the `Firestore` module:
+
+```python
+from gcp_pal import Firestore
+Firestore()
+# ImportError: Module 'Firestore' requires 'google.cloud.firestore' (PyPI: 'google-cloud-firestore') to be installed.
+```
+
+Which lets the user know that the `google-cloud-firestore` package is required to use the `Firestore` module.
+
+---
+
 ## Configuration
 
 Before you can start using the `gcp-pal` library with Firestore or any other GCP services, make sure you either have set up your GCP credentials properly or have the necessary permissions to access the services you want to use:
 
 ```bash
 gcloud auth application-default login
 ```
```

