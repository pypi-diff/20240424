# Comparing `tmp/girder-virtual-folders-3.2.4.dev7.tar.gz` & `tmp/girder_virtual_folders-5a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-virtual-folders-3.2.4.dev7.tar", last modified: Wed Apr 24 19:14:03 2024, max compression
+gzip compressed data, was "girder_virtual_folders-5a2.tar", last modified: Fri Apr 12 16:33:13 2024, max compression
```

## Comparing `girder-virtual-folders-3.2.4.dev7.tar` & `girder_virtual_folders-5a2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:14:02.994424 girder-virtual-folders-3.2.4.dev7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      559 2024-04-24 19:14:02.994424 girder-virtual-folders-3.2.4.dev7/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:14:02.990424 girder-virtual-folders-3.2.4.dev7/girder_virtual_folders/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8194 2024-04-24 19:11:47.000000 girder-virtual-folders-3.2.4.dev7/girder_virtual_folders/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:14:02.994424 girder-virtual-folders-3.2.4.dev7/girder_virtual_folders.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      559 2024-04-24 19:14:02.000000 girder-virtual-folders-3.2.4.dev7/girder_virtual_folders.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      441 2024-04-24 19:14:02.000000 girder-virtual-folders-3.2.4.dev7/girder_virtual_folders.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:14:02.000000 girder-virtual-folders-3.2.4.dev7/girder_virtual_folders.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       78 2024-04-24 19:14:02.000000 girder-virtual-folders-3.2.4.dev7/girder_virtual_folders.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:14:02.000000 girder-virtual-folders-3.2.4.dev7/girder_virtual_folders.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-24 19:14:02.000000 girder-virtual-folders-3.2.4.dev7/girder_virtual_folders.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       23 2024-04-24 19:14:02.000000 girder-virtual-folders-3.2.4.dev7/girder_virtual_folders.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2024-04-24 19:11:47.000000 girder-virtual-folders-3.2.4.dev7/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:14:02.994424 girder-virtual-folders-3.2.4.dev7/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:11:47.000000 girder-virtual-folders-3.2.4.dev7/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6178 2024-04-24 19:11:47.000000 girder-virtual-folders-3.2.4.dev7/plugin_tests/virtual_folders_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-24 19:14:02.994424 girder-virtual-folders-3.2.4.dev7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1645 2024-04-24 19:11:47.000000 girder-virtual-folders-3.2.4.dev7/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:33:13.605667 girder_virtual_folders-5a2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      556 2024-04-12 16:33:13.605667 girder_virtual_folders-5a2/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:33:13.605667 girder_virtual_folders-5a2/girder_virtual_folders/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8194 2024-04-12 16:27:18.000000 girder_virtual_folders-5a2/girder_virtual_folders/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:33:13.605667 girder_virtual_folders-5a2/girder_virtual_folders.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      556 2024-04-12 16:33:13.000000 girder_virtual_folders-5a2/girder_virtual_folders.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      441 2024-04-12 16:33:13.000000 girder_virtual_folders-5a2/girder_virtual_folders.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:33:13.000000 girder_virtual_folders-5a2/girder_virtual_folders.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       78 2024-04-12 16:33:13.000000 girder_virtual_folders-5a2/girder_virtual_folders.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:33:13.000000 girder_virtual_folders-5a2/girder_virtual_folders.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-12 16:33:13.000000 girder_virtual_folders-5a2/girder_virtual_folders.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       23 2024-04-12 16:33:13.000000 girder_virtual_folders-5a2/girder_virtual_folders.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2024-04-12 16:27:18.000000 girder_virtual_folders-5a2/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:33:13.605667 girder_virtual_folders-5a2/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:27:18.000000 girder_virtual_folders-5a2/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6178 2024-04-12 16:27:18.000000 girder_virtual_folders-5a2/plugin_tests/virtual_folders_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 16:33:13.605667 girder_virtual_folders-5a2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1645 2024-04-12 16:27:18.000000 girder_virtual_folders-5a2/setup.py
```

### Comparing `girder-virtual-folders-3.2.4.dev7/PKG-INFO` & `girder_virtual_folders-5a2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-virtual-folders
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Allows folders to list child items using arbitrary database queries
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-virtual-folders-3.2.4.dev7/girder_virtual_folders/__init__.py` & `girder_virtual_folders-5a2/girder_virtual_folders/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-virtual-folders-3.2.4.dev7/girder_virtual_folders.egg-info/PKG-INFO` & `girder_virtual_folders-5a2/girder_virtual_folders.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-virtual-folders
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Allows folders to list child items using arbitrary database queries
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-virtual-folders-3.2.4.dev7/plugin_tests/virtual_folders_test.py` & `girder_virtual_folders-5a2/plugin_tests/virtual_folders_test.py`

 * *Files identical despite different names*

### Comparing `girder-virtual-folders-3.2.4.dev7/setup.py` & `girder_virtual_folders-5a2/setup.py`

 * *Files identical despite different names*

