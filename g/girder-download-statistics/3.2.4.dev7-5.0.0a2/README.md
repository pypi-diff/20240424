# Comparing `tmp/girder-download-statistics-3.2.4.dev7.tar.gz` & `tmp/girder-download-statistics-5.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-download-statistics-3.2.4.dev7.tar", last modified: Wed Apr 24 19:12:21 2024, max compression
+gzip compressed data, was "girder-download-statistics-5.0.0a2.tar", last modified: Fri Apr 12 16:30:01 2024, max compression
```

## Comparing `girder-download-statistics-3.2.4.dev7.tar` & `girder-download-statistics-5.0.0a2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:21.066557 girder-download-statistics-3.2.4.dev7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      527 2024-04-24 19:12:21.066557 girder-download-statistics-3.2.4.dev7/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:21.062557 girder-download-statistics-3.2.4.dev7/girder_download_statistics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1147 2024-04-24 19:11:47.000000 girder-download-statistics-3.2.4.dev7/girder_download_statistics/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:21.066557 girder-download-statistics-3.2.4.dev7/girder_download_statistics.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      527 2024-04-24 19:12:20.000000 girder-download-statistics-3.2.4.dev7/girder_download_statistics.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      533 2024-04-24 19:12:21.000000 girder-download-statistics-3.2.4.dev7/girder_download_statistics.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:12:20.000000 girder-download-statistics-3.2.4.dev7/girder_download_statistics.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       90 2024-04-24 19:12:20.000000 girder-download-statistics-3.2.4.dev7/girder_download_statistics.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:12:20.000000 girder-download-statistics-3.2.4.dev7/girder_download_statistics.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-24 19:12:20.000000 girder-download-statistics-3.2.4.dev7/girder_download_statistics.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2024-04-24 19:12:20.000000 girder-download-statistics-3.2.4.dev7/girder_download_statistics.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       64 2024-04-24 19:11:47.000000 girder-download-statistics-3.2.4.dev7/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:21.066557 girder-download-statistics-3.2.4.dev7/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:11:47.000000 girder-download-statistics-3.2.4.dev7/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6503 2024-04-24 19:11:47.000000 girder-download-statistics-3.2.4.dev7/plugin_tests/download_statistics_test.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:21.066557 girder-download-statistics-3.2.4.dev7/plugin_tests/files/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2024-04-24 19:11:47.000000 girder-download-statistics-3.2.4.dev7/plugin_tests/files/txt1.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2024-04-24 19:11:47.000000 girder-download-statistics-3.2.4.dev7/plugin_tests/files/txt2.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-24 19:12:21.066557 girder-download-statistics-3.2.4.dev7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1625 2024-04-24 19:11:47.000000 girder-download-statistics-3.2.4.dev7/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:30:01.376257 girder-download-statistics-5.0.0a2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2024-04-12 16:30:01.372256 girder-download-statistics-5.0.0a2/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:30:01.372256 girder-download-statistics-5.0.0a2/girder_download_statistics/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1147 2024-04-12 16:27:18.000000 girder-download-statistics-5.0.0a2/girder_download_statistics/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:30:01.372256 girder-download-statistics-5.0.0a2/girder_download_statistics.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2024-04-12 16:30:01.000000 girder-download-statistics-5.0.0a2/girder_download_statistics.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      533 2024-04-12 16:30:01.000000 girder-download-statistics-5.0.0a2/girder_download_statistics.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:30:01.000000 girder-download-statistics-5.0.0a2/girder_download_statistics.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       90 2024-04-12 16:30:01.000000 girder-download-statistics-5.0.0a2/girder_download_statistics.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:30:01.000000 girder-download-statistics-5.0.0a2/girder_download_statistics.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-12 16:30:01.000000 girder-download-statistics-5.0.0a2/girder_download_statistics.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2024-04-12 16:30:01.000000 girder-download-statistics-5.0.0a2/girder_download_statistics.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       64 2024-04-12 16:27:18.000000 girder-download-statistics-5.0.0a2/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:30:01.372256 girder-download-statistics-5.0.0a2/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:27:18.000000 girder-download-statistics-5.0.0a2/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6503 2024-04-12 16:27:18.000000 girder-download-statistics-5.0.0a2/plugin_tests/download_statistics_test.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:30:01.372256 girder-download-statistics-5.0.0a2/plugin_tests/files/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2024-04-12 16:27:18.000000 girder-download-statistics-5.0.0a2/plugin_tests/files/txt1.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2024-04-12 16:27:18.000000 girder-download-statistics-5.0.0a2/plugin_tests/files/txt2.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 16:30:01.376257 girder-download-statistics-5.0.0a2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1625 2024-04-12 16:27:18.000000 girder-download-statistics-5.0.0a2/setup.py
```

### Comparing `girder-download-statistics-3.2.4.dev7/PKG-INFO` & `girder-download-statistics-5.0.0a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-download-statistics
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Record file download statistics
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-download-statistics-3.2.4.dev7/girder_download_statistics/__init__.py` & `girder-download-statistics-5.0.0a2/girder_download_statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-download-statistics-3.2.4.dev7/girder_download_statistics.egg-info/PKG-INFO` & `girder-download-statistics-5.0.0a2/girder_download_statistics.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-download-statistics
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Record file download statistics
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-download-statistics-3.2.4.dev7/girder_download_statistics.egg-info/SOURCES.txt` & `girder-download-statistics-5.0.0a2/girder_download_statistics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-download-statistics-3.2.4.dev7/plugin_tests/download_statistics_test.py` & `girder-download-statistics-5.0.0a2/plugin_tests/download_statistics_test.py`

 * *Files identical despite different names*

### Comparing `girder-download-statistics-3.2.4.dev7/setup.py` & `girder-download-statistics-5.0.0a2/setup.py`

 * *Files identical despite different names*

