# Comparing `tmp/fiftyone_pipeline_engines_fiftyone-4.4.8.0.tar.gz` & `tmp/fiftyone_pipeline_engines_fiftyone-4.4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiftyone_pipeline_engines_fiftyone-4.4.8.0.tar", last modified: Sun Jul  2 01:56:21 2023, max compression
+gzip compressed data, was "fiftyone_pipeline_engines_fiftyone-4.4.9.0.tar", last modified: Fri Jul 14 01:53:28 2023, max compression
```

## Comparing `fiftyone_pipeline_engines_fiftyone-4.4.8.0.tar` & `fiftyone_pipeline_engines_fiftyone-4.4.9.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.770810 fiftyone_pipeline_engines_fiftyone-4.4.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-02 01:56:21.770810 fiftyone_pipeline_engines_fiftyone-4.4.8.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.766810 fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone/share_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone/share_usage_evidencekeyfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone/share_usage_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.770810 fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-02 01:56:21.000000 fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-02 01:56:21.000000 fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 01:56:21.000000 fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-02 01:56:21.000000 fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-02 01:56:21.000000 fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 01:56:21.770810 fiftyone_pipeline_engines_fiftyone-4.4.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines_fiftyone-4.4.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:53:28.310665 fiftyone_pipeline_engines_fiftyone-4.4.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 01:53:20.000000 fiftyone_pipeline_engines_fiftyone-4.4.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-14 01:53:28.310665 fiftyone_pipeline_engines_fiftyone-4.4.9.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:53:28.310665 fiftyone_pipeline_engines_fiftyone-4.4.9.0/fiftyone_pipeline_engines_fiftyone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 01:53:20.000000 fiftyone_pipeline_engines_fiftyone-4.4.9.0/fiftyone_pipeline_engines_fiftyone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-07-14 01:53:20.000000 fiftyone_pipeline_engines_fiftyone-4.4.9.0/fiftyone_pipeline_engines_fiftyone/share_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-14 01:53:20.000000 fiftyone_pipeline_engines_fiftyone-4.4.9.0/fiftyone_pipeline_engines_fiftyone/share_usage_evidencekeyfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-14 01:53:20.000000 fiftyone_pipeline_engines_fiftyone-4.4.9.0/fiftyone_pipeline_engines_fiftyone/share_usage_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:53:28.310665 fiftyone_pipeline_engines_fiftyone-4.4.9.0/fiftyone_pipeline_engines_fiftyone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-14 01:53:28.000000 fiftyone_pipeline_engines_fiftyone-4.4.9.0/fiftyone_pipeline_engines_fiftyone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-14 01:53:28.000000 fiftyone_pipeline_engines_fiftyone-4.4.9.0/fiftyone_pipeline_engines_fiftyone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 01:53:28.000000 fiftyone_pipeline_engines_fiftyone-4.4.9.0/fiftyone_pipeline_engines_fiftyone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-14 01:53:28.000000 fiftyone_pipeline_engines_fiftyone-4.4.9.0/fiftyone_pipeline_engines_fiftyone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-14 01:53:28.000000 fiftyone_pipeline_engines_fiftyone-4.4.9.0/fiftyone_pipeline_engines_fiftyone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 01:53:28.310665 fiftyone_pipeline_engines_fiftyone-4.4.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-14 01:53:20.000000 fiftyone_pipeline_engines_fiftyone-4.4.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 01:53:28.000000 fiftyone_pipeline_engines_fiftyone-4.4.9.0/version.txt
```

### Comparing `fiftyone_pipeline_engines_fiftyone-4.4.8.0/PKG-INFO` & `fiftyone_pipeline_engines_fiftyone-4.4.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone_pipeline_engines_fiftyone
-Version: 4.4.8.0
+Version: 4.4.9.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). It includes a ShareUsage engine that sends usage data to 51Degrees in zipped batches.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone/share_usage.py` & `fiftyone_pipeline_engines_fiftyone-4.4.9.0/fiftyone_pipeline_engines_fiftyone/share_usage.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone/share_usage_evidencekeyfilter.py` & `fiftyone_pipeline_engines_fiftyone-4.4.9.0/fiftyone_pipeline_engines_fiftyone/share_usage_evidencekeyfilter.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone/share_usage_tracker.py` & `fiftyone_pipeline_engines_fiftyone-4.4.9.0/fiftyone_pipeline_engines_fiftyone/share_usage_tracker.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone.egg-info/PKG-INFO` & `fiftyone_pipeline_engines_fiftyone-4.4.9.0/fiftyone_pipeline_engines_fiftyone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone-pipeline-engines-fiftyone
-Version: 4.4.8.0
+Version: 4.4.9.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). It includes a ShareUsage engine that sends usage data to 51Degrees in zipped batches.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone.egg-info/SOURCES.txt` & `fiftyone_pipeline_engines_fiftyone-4.4.9.0/fiftyone_pipeline_engines_fiftyone.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+MANIFEST.in
 setup.py
+version.txt
 fiftyone_pipeline_engines_fiftyone/__init__.py
 fiftyone_pipeline_engines_fiftyone/share_usage.py
 fiftyone_pipeline_engines_fiftyone/share_usage_evidencekeyfilter.py
 fiftyone_pipeline_engines_fiftyone/share_usage_tracker.py
 fiftyone_pipeline_engines_fiftyone.egg-info/PKG-INFO
 fiftyone_pipeline_engines_fiftyone.egg-info/SOURCES.txt
 fiftyone_pipeline_engines_fiftyone.egg-info/dependency_links.txt
```

### Comparing `fiftyone_pipeline_engines_fiftyone-4.4.8.0/setup.py` & `fiftyone_pipeline_engines_fiftyone-4.4.9.0/setup.py`

 * *Files identical despite different names*

