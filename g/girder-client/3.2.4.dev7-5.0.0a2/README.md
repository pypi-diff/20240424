# Comparing `tmp/girder-client-3.2.4.dev7.tar.gz` & `tmp/girder_client-5a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-client-3.2.4.dev7.tar", last modified: Wed Apr 24 19:14:11 2024, max compression
+gzip compressed data, was "girder_client-5a2.tar", last modified: Fri Apr 12 16:33:43 2024, max compression
```

## Comparing `girder-client-3.2.4.dev7.tar` & `girder_client-5a2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:14:11.534411 girder-client-3.2.4.dev7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      964 2024-04-24 19:14:11.534411 girder-client-3.2.4.dev7/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2024-04-24 19:11:47.000000 girder-client-3.2.4.dev7/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:14:11.534411 girder-client-3.2.4.dev7/girder_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    68223 2024-04-24 19:11:47.000000 girder-client-3.2.4.dev7/girder_client/__init__.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    13535 2024-04-24 19:11:47.000000 girder-client-3.2.4.dev7/girder_client/cli.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:14:11.534411 girder-client-3.2.4.dev7/girder_client.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      964 2024-04-24 19:14:11.000000 girder-client-3.2.4.dev7/girder_client.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      326 2024-04-24 19:14:11.000000 girder-client-3.2.4.dev7/girder_client.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:14:11.000000 girder-client-3.2.4.dev7/girder_client.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       93 2024-04-24 19:14:11.000000 girder-client-3.2.4.dev7/girder_client.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:14:11.000000 girder-client-3.2.4.dev7/girder_client.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       55 2024-04-24 19:14:11.000000 girder-client-3.2.4.dev7/girder_client.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-04-24 19:14:11.000000 girder-client-3.2.4.dev7/girder_client.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-24 19:14:11.534411 girder-client-3.2.4.dev7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1810 2024-04-24 19:11:47.000000 girder-client-3.2.4.dev7/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:33:43.453869 girder_client-5a2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2024-04-12 16:33:43.453869 girder_client-5a2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2024-04-12 16:27:17.000000 girder_client-5a2/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:33:43.453869 girder_client-5a2/girder_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    68223 2024-04-12 16:27:17.000000 girder_client-5a2/girder_client/__init__.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    13535 2024-04-12 16:27:17.000000 girder_client-5a2/girder_client/cli.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:33:43.453869 girder_client-5a2/girder_client.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2024-04-12 16:33:43.000000 girder_client-5a2/girder_client.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      326 2024-04-12 16:33:43.000000 girder_client-5a2/girder_client.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:33:43.000000 girder_client-5a2/girder_client.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       93 2024-04-12 16:33:43.000000 girder_client-5a2/girder_client.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:33:43.000000 girder_client-5a2/girder_client.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       55 2024-04-12 16:33:43.000000 girder_client-5a2/girder_client.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-04-12 16:33:43.000000 girder_client-5a2/girder_client.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 16:33:43.453869 girder_client-5a2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1810 2024-04-12 16:27:17.000000 girder_client-5a2/setup.py
```

### Comparing `girder-client-3.2.4.dev7/PKG-INFO` & `girder_client-5a2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-client
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Python client for interacting with Girder servers
 Home-page: http://girder.readthedocs.org/en/latest/python-client.html
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `girder-client-3.2.4.dev7/girder_client/__init__.py` & `girder_client-5a2/girder_client/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-client-3.2.4.dev7/girder_client/cli.py` & `girder_client-5a2/girder_client/cli.py`

 * *Files identical despite different names*

### Comparing `girder-client-3.2.4.dev7/girder_client.egg-info/PKG-INFO` & `girder_client-5a2/girder_client.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-client
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Python client for interacting with Girder servers
 Home-page: http://girder.readthedocs.org/en/latest/python-client.html
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `girder-client-3.2.4.dev7/setup.py` & `girder_client-5a2/setup.py`

 * *Files identical despite different names*

