# Comparing `tmp/fiftyone_pipeline_cloudrequestengine-4.4.8.0.tar.gz` & `tmp/fiftyone_pipeline_cloudrequestengine-4.4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiftyone_pipeline_cloudrequestengine-4.4.8.0.tar", last modified: Sun Jul  2 01:56:21 2023, max compression
+gzip compressed data, was "fiftyone_pipeline_cloudrequestengine-4.4.9.0.tar", last modified: Fri Jul 14 01:53:28 2023, max compression
```

## Comparing `fiftyone_pipeline_cloudrequestengine-4.4.8.0.tar` & `fiftyone_pipeline_cloudrequestengine-4.4.9.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.962814 fiftyone_pipeline_cloudrequestengine-4.4.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-02 01:56:21.962814 fiftyone_pipeline_cloudrequestengine-4.4.8.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.958814 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:16.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-02 01:56:16.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/clouddata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-07-02 01:56:16.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/cloudengine.py
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-07-02 01:56:16.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/cloudrequestengine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-02 01:56:16.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/cloudrequestexception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-02 01:56:16.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-02 01:56:16.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/requestclient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.962814 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-02 01:56:21.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-02 01:56:21.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 01:56:21.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-02 01:56:21.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-02 01:56:21.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 01:56:21.962814 fiftyone_pipeline_cloudrequestengine-4.4.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-02 01:56:16.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:53:28.602667 fiftyone_pipeline_cloudrequestengine-4.4.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 01:53:20.000000 fiftyone_pipeline_cloudrequestengine-4.4.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-14 01:53:28.602667 fiftyone_pipeline_cloudrequestengine-4.4.9.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:53:28.602667 fiftyone_pipeline_cloudrequestengine-4.4.9.0/fiftyone_pipeline_cloudrequestengine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 01:53:20.000000 fiftyone_pipeline_cloudrequestengine-4.4.9.0/fiftyone_pipeline_cloudrequestengine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-14 01:53:20.000000 fiftyone_pipeline_cloudrequestengine-4.4.9.0/fiftyone_pipeline_cloudrequestengine/clouddata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-07-14 01:53:20.000000 fiftyone_pipeline_cloudrequestengine-4.4.9.0/fiftyone_pipeline_cloudrequestengine/cloudengine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-07-14 01:53:20.000000 fiftyone_pipeline_cloudrequestengine-4.4.9.0/fiftyone_pipeline_cloudrequestengine/cloudrequestengine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-14 01:53:20.000000 fiftyone_pipeline_cloudrequestengine-4.4.9.0/fiftyone_pipeline_cloudrequestengine/cloudrequestexception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-14 01:53:20.000000 fiftyone_pipeline_cloudrequestengine-4.4.9.0/fiftyone_pipeline_cloudrequestengine/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-14 01:53:20.000000 fiftyone_pipeline_cloudrequestengine-4.4.9.0/fiftyone_pipeline_cloudrequestengine/requestclient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:53:28.602667 fiftyone_pipeline_cloudrequestengine-4.4.9.0/fiftyone_pipeline_cloudrequestengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-14 01:53:28.000000 fiftyone_pipeline_cloudrequestengine-4.4.9.0/fiftyone_pipeline_cloudrequestengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-14 01:53:28.000000 fiftyone_pipeline_cloudrequestengine-4.4.9.0/fiftyone_pipeline_cloudrequestengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 01:53:28.000000 fiftyone_pipeline_cloudrequestengine-4.4.9.0/fiftyone_pipeline_cloudrequestengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-14 01:53:28.000000 fiftyone_pipeline_cloudrequestengine-4.4.9.0/fiftyone_pipeline_cloudrequestengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-14 01:53:28.000000 fiftyone_pipeline_cloudrequestengine-4.4.9.0/fiftyone_pipeline_cloudrequestengine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 01:53:28.602667 fiftyone_pipeline_cloudrequestengine-4.4.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-14 01:53:20.000000 fiftyone_pipeline_cloudrequestengine-4.4.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 01:53:28.000000 fiftyone_pipeline_cloudrequestengine-4.4.9.0/version.txt
```

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.8.0/PKG-INFO` & `fiftyone_pipeline_cloudrequestengine-4.4.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone_pipeline_cloudrequestengine
-Version: 4.4.8.0
+Version: 4.4.9.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). This package extends the flow element class created by the fiftyone-pipeline-core package into a specialized type of flow element called an engine.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/clouddata.py` & `fiftyone_pipeline_cloudrequestengine-4.4.9.0/fiftyone_pipeline_cloudrequestengine/clouddata.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/cloudengine.py` & `fiftyone_pipeline_cloudrequestengine-4.4.9.0/fiftyone_pipeline_cloudrequestengine/cloudengine.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/cloudrequestengine.py` & `fiftyone_pipeline_cloudrequestengine-4.4.9.0/fiftyone_pipeline_cloudrequestengine/cloudrequestengine.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/cloudrequestexception.py` & `fiftyone_pipeline_cloudrequestengine-4.4.9.0/fiftyone_pipeline_cloudrequestengine/cloudrequestexception.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/constants.py` & `fiftyone_pipeline_cloudrequestengine-4.4.9.0/fiftyone_pipeline_cloudrequestengine/constants.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/requestclient.py` & `fiftyone_pipeline_cloudrequestengine-4.4.9.0/fiftyone_pipeline_cloudrequestengine/requestclient.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine.egg-info/PKG-INFO` & `fiftyone_pipeline_cloudrequestengine-4.4.9.0/fiftyone_pipeline_cloudrequestengine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone-pipeline-cloudrequestengine
-Version: 4.4.8.0
+Version: 4.4.9.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). This package extends the flow element class created by the fiftyone-pipeline-core package into a specialized type of flow element called an engine.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine.egg-info/SOURCES.txt` & `fiftyone_pipeline_cloudrequestengine-4.4.9.0/fiftyone_pipeline_cloudrequestengine.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+MANIFEST.in
 setup.py
+version.txt
 fiftyone_pipeline_cloudrequestengine/__init__.py
 fiftyone_pipeline_cloudrequestengine/clouddata.py
 fiftyone_pipeline_cloudrequestengine/cloudengine.py
 fiftyone_pipeline_cloudrequestengine/cloudrequestengine.py
 fiftyone_pipeline_cloudrequestengine/cloudrequestexception.py
 fiftyone_pipeline_cloudrequestengine/constants.py
 fiftyone_pipeline_cloudrequestengine/requestclient.py
```

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.8.0/setup.py` & `fiftyone_pipeline_cloudrequestengine-4.4.9.0/setup.py`

 * *Files identical despite different names*

