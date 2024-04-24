# Comparing `tmp/fiftyone_pipeline_engines-4.4.8.0.tar.gz` & `tmp/fiftyone_pipeline_engines-4.4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiftyone_pipeline_engines-4.4.8.0.tar", last modified: Sun Jul  2 01:56:21 2023, max compression
+gzip compressed data, was "fiftyone_pipeline_engines-4.4.9.0.tar", last modified: Fri Jul 14 01:53:28 2023, max compression
```

## Comparing `fiftyone_pipeline_engines-4.4.8.0.tar` & `fiftyone_pipeline_engines-4.4.9.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.574805 fiftyone_pipeline_engines-4.4.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-02 01:56:21.574805 fiftyone_pipeline_engines-4.4.8.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.574805 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/aspectdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/aspectdata_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/basic_dictionary_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/datafile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9991 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/datafile_update_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/datakeyed_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/missingproperty_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.574805 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-02 01:56:21.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-02 01:56:21.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 01:56:21.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-02 01:56:21.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-02 01:56:21.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 01:56:21.574805 fiftyone_pipeline_engines-4.4.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:53:28.006664 fiftyone_pipeline_engines-4.4.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 01:53:20.000000 fiftyone_pipeline_engines-4.4.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-14 01:53:28.006664 fiftyone_pipeline_engines-4.4.9.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:53:28.006664 fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 01:53:20.000000 fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-14 01:53:20.000000 fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines/aspectdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-14 01:53:20.000000 fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines/aspectdata_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-14 01:53:20.000000 fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines/basic_dictionary_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-07-14 01:53:20.000000 fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines/datafile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9991 2023-07-14 01:53:20.000000 fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines/datafile_update_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-14 01:53:20.000000 fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines/datakeyed_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-07-14 01:53:20.000000 fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-14 01:53:20.000000 fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines/lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-14 01:53:20.000000 fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines/missingproperty_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-14 01:53:20.000000 fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:53:28.006664 fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-14 01:53:27.000000 fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-14 01:53:28.000000 fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 01:53:27.000000 fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-14 01:53:27.000000 fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-14 01:53:27.000000 fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 01:53:28.006664 fiftyone_pipeline_engines-4.4.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-14 01:53:20.000000 fiftyone_pipeline_engines-4.4.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 01:53:27.000000 fiftyone_pipeline_engines-4.4.9.0/version.txt
```

### Comparing `fiftyone_pipeline_engines-4.4.8.0/PKG-INFO` & `fiftyone_pipeline_engines-4.4.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone_pipeline_engines
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

### Comparing `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/aspectdata.py` & `fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines/aspectdata.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/aspectdata_dictionary.py` & `fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines/aspectdata_dictionary.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/basic_dictionary_cache.py` & `fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines/basic_dictionary_cache.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/datafile.py` & `fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines/datafile.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/datafile_update_service.py` & `fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines/datafile_update_service.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/datakeyed_cache.py` & `fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines/datakeyed_cache.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/engine.py` & `fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines/engine.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/lru_cache.py` & `fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines/lru_cache.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/missingproperty_service.py` & `fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines/missingproperty_service.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/tracker.py` & `fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines/tracker.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines.egg-info/PKG-INFO` & `fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone-pipeline-engines
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

### Comparing `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines.egg-info/SOURCES.txt` & `fiftyone_pipeline_engines-4.4.9.0/fiftyone_pipeline_engines.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+MANIFEST.in
 setup.py
+version.txt
 fiftyone_pipeline_engines/__init__.py
 fiftyone_pipeline_engines/aspectdata.py
 fiftyone_pipeline_engines/aspectdata_dictionary.py
 fiftyone_pipeline_engines/basic_dictionary_cache.py
 fiftyone_pipeline_engines/datafile.py
 fiftyone_pipeline_engines/datafile_update_service.py
 fiftyone_pipeline_engines/datakeyed_cache.py
```

### Comparing `fiftyone_pipeline_engines-4.4.8.0/setup.py` & `fiftyone_pipeline_engines-4.4.9.0/setup.py`

 * *Files identical despite different names*

