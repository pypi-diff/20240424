# Comparing `tmp/finalsa-s3-client-0.0.1.tar.gz` & `tmp/finalsa_s3_client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finalsa-s3-client-0.0.1.tar", last modified: Fri Apr 12 04:26:46 2024, max compression
+gzip compressed data, was "finalsa_s3_client-0.0.2.tar", last modified: Wed Apr 24 12:57:25 2024, max compression
```

## Comparing `finalsa-s3-client-0.0.1.tar` & `finalsa_s3_client-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:26:46.370593 finalsa-s3-client-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-12 04:26:38.000000 finalsa-s3-client-0.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-12 04:26:46.370593 finalsa-s3-client-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 04:26:38.000000 finalsa-s3-client-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:26:46.362593 finalsa-s3-client-0.0.1/finalsa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:26:46.362593 finalsa-s3-client-0.0.1/finalsa/s3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:26:46.366593 finalsa-s3-client-0.0.1/finalsa/s3/client/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-12 04:26:38.000000 finalsa-s3-client-0.0.1/finalsa/s3/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:26:46.366593 finalsa-s3-client-0.0.1/finalsa/s3/client/client/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-12 04:26:38.000000 finalsa-s3-client-0.0.1/finalsa/s3/client/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-12 04:26:38.000000 finalsa-s3-client-0.0.1/finalsa/s3/client/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:26:46.366593 finalsa-s3-client-0.0.1/finalsa/s3/client/interface/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 04:26:38.000000 finalsa-s3-client-0.0.1/finalsa/s3/client/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-12 04:26:38.000000 finalsa-s3-client-0.0.1/finalsa/s3/client/interface/client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 04:26:38.000000 finalsa-s3-client-0.0.1/finalsa/s3/client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:26:46.366593 finalsa-s3-client-0.0.1/finalsa/s3/client/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-12 04:26:38.000000 finalsa-s3-client-0.0.1/finalsa/s3/client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-12 04:26:38.000000 finalsa-s3-client-0.0.1/finalsa/s3/client/tests/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:26:46.370593 finalsa-s3-client-0.0.1/finalsa_s3_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-12 04:26:46.000000 finalsa-s3-client-0.0.1/finalsa_s3_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-12 04:26:46.000000 finalsa-s3-client-0.0.1/finalsa_s3_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 04:26:46.000000 finalsa-s3-client-0.0.1/finalsa_s3_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 04:26:46.000000 finalsa-s3-client-0.0.1/finalsa_s3_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 04:26:46.000000 finalsa-s3-client-0.0.1/finalsa_s3_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 04:26:46.000000 finalsa-s3-client-0.0.1/finalsa_s3_client.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-12 04:26:46.370593 finalsa-s3-client-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-12 04:26:38.000000 finalsa-s3-client-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:26:46.370593 finalsa-s3-client-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-12 04:26:38.000000 finalsa-s3-client-0.0.1/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:25.235166 finalsa_s3_client-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-24 12:57:25.235166 finalsa_s3_client-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:25.227166 finalsa_s3_client-0.0.2/finalsa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:25.227166 finalsa_s3_client-0.0.2/finalsa/s3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:25.231166 finalsa_s3_client-0.0.2/finalsa/s3/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/finalsa/s3/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:25.231166 finalsa_s3_client-0.0.2/finalsa/s3/client/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/finalsa/s3/client/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/finalsa/s3/client/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:25.231166 finalsa_s3_client-0.0.2/finalsa/s3/client/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/finalsa/s3/client/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/finalsa/s3/client/interface/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/finalsa/s3/client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:25.231166 finalsa_s3_client-0.0.2/finalsa/s3/client/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/finalsa/s3/client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/finalsa/s3/client/tests/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:25.231166 finalsa_s3_client-0.0.2/finalsa_s3_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-24 12:57:25.000000 finalsa_s3_client-0.0.2/finalsa_s3_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-24 12:57:25.000000 finalsa_s3_client-0.0.2/finalsa_s3_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:57:25.000000 finalsa_s3_client-0.0.2/finalsa_s3_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 12:57:25.000000 finalsa_s3_client-0.0.2/finalsa_s3_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-24 12:57:25.000000 finalsa_s3_client-0.0.2/finalsa_s3_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:57:25.000000 finalsa_s3_client-0.0.2/finalsa_s3_client.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-24 12:57:25.235166 finalsa_s3_client-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:25.231166 finalsa_s3_client-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-24 12:57:15.000000 finalsa_s3_client-0.0.2/tests/test_client.py
```

### Comparing `finalsa-s3-client-0.0.1/LICENSE.md` & `finalsa_s3_client-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `finalsa-s3-client-0.0.1/PKG-INFO` & `finalsa_s3_client-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: finalsa-s3-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: An utils package for using s3
-Home-page: https://github.com/finalsa/s3-client
+Home-page: https://github.com/finalsa/finalsa-s3-client
 Author: Luis Jimenez
 Author-email: luis@finalsa.com
 License: MIT
 Keywords: s3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `finalsa-s3-client-0.0.1/finalsa/s3/client/client/client.py` & `finalsa_s3_client-0.0.2/finalsa/s3/client/client/client.py`

 * *Files identical despite different names*

### Comparing `finalsa-s3-client-0.0.1/finalsa/s3/client/interface/client.py` & `finalsa_s3_client-0.0.2/finalsa/s3/client/interface/client.py`

 * *Files identical despite different names*

### Comparing `finalsa-s3-client-0.0.1/finalsa/s3/client/tests/client.py` & `finalsa_s3_client-0.0.2/finalsa/s3/client/tests/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,7 +27,10 @@
         self.buckets[bucket] = {}
 
     def delete_bucket(self, bucket: str):
         del self.buckets[bucket]
 
     def get_bucket_location(self, bucket: str) -> str:
         return "us-east-1"
+
+    def clear(self):
+        self.buckets = {}
```

### Comparing `finalsa-s3-client-0.0.1/finalsa_s3_client.egg-info/PKG-INFO` & `finalsa_s3_client-0.0.2/finalsa_s3_client.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: finalsa-s3-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: An utils package for using s3
-Home-page: https://github.com/finalsa/s3-client
+Home-page: https://github.com/finalsa/finalsa-s3-client
 Author: Luis Jimenez
 Author-email: luis@finalsa.com
 License: MIT
 Keywords: s3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `finalsa-s3-client-0.0.1/finalsa_s3_client.egg-info/SOURCES.txt` & `finalsa_s3_client-0.0.2/finalsa_s3_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finalsa-s3-client-0.0.1/setup.py` & `finalsa_s3_client-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import os
 import re
 
 from setuptools import setup
 
 PACKAGE = "finalsa-s3-client"
-URL = "https://github.com/finalsa/s3-client"
+URL = "https://github.com/finalsa/finalsa-s3-client"
 PACKAGE_FOLDER = "finalsa/s3/client"
 
 def get_version(package):
     """
     Return package version as listed in `__version__` in `init.py`.
     """
     with open(os.path.join(package, "__init__.py")) as f:
```

### Comparing `finalsa-s3-client-0.0.1/tests/test_client.py` & `finalsa_s3_client-0.0.2/tests/test_client.py`

 * *Files identical despite different names*

