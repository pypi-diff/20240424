# Comparing `tmp/decthings-api-0.0.1.tar.gz` & `tmp/decthings_api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decthings-api-0.0.1.tar", last modified: Mon Apr  1 22:45:44 2024, max compression
+gzip compressed data, was "decthings_api-0.0.2.tar", last modified: Wed Apr 24 11:41:15 2024, max compression
```

## Comparing `decthings-api-0.0.1.tar` & `decthings_api-0.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-01 22:45:44.660560 decthings-api-0.0.1/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1066 2024-04-01 22:37:02.000000 decthings-api-0.0.1/LICENSE
--rw-r--r--   0 viktor    (1000) viktor    (1000)     1145 2024-04-01 22:45:44.660560 decthings-api-0.0.1/PKG-INFO
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      657 2024-04-01 22:41:20.000000 decthings-api-0.0.1/README.md
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      460 2024-04-01 22:45:26.000000 decthings-api-0.0.1/pyproject.toml
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       38 2024-04-01 22:45:44.660560 decthings-api-0.0.1/setup.cfg
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-01 22:45:44.648560 decthings-api-0.0.1/src/
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-01 22:45:44.652560 decthings-api-0.0.1/src/decthings_api/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)        0 2024-04-01 19:18:41.000000 decthings-api-0.0.1/src/decthings_api/__init__.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     4627 2024-04-01 19:18:41.000000 decthings-api-0.0.1/src/decthings_api/client.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     4634 2024-04-01 19:18:41.000000 decthings-api-0.0.1/src/decthings_api/client_sync.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1440 2024-04-01 19:18:41.000000 decthings-api-0.0.1/src/decthings_api/event.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     3627 2024-04-01 19:18:41.000000 decthings-api-0.0.1/src/decthings_api/protocol.py
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-01 22:45:44.660560 decthings-api-0.0.1/src/decthings_api/rpc_impl/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1746 2024-04-01 22:29:43.000000 decthings-api-0.0.1/src/decthings_api/rpc_impl/convert.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    10151 2024-04-01 22:34:04.000000 decthings-api-0.0.1/src/decthings_api/rpc_impl/dataset.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    16281 2024-04-01 22:29:43.000000 decthings-api-0.0.1/src/decthings_api/rpc_impl/debug.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    14561 2024-04-01 19:18:41.000000 decthings-api-0.0.1/src/decthings_api/rpc_impl/fs.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     4395 2024-04-01 19:18:41.000000 decthings-api-0.0.1/src/decthings_api/rpc_impl/language.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    23489 2024-04-01 22:29:43.000000 decthings-api-0.0.1/src/decthings_api/rpc_impl/model.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1873 2024-04-01 19:18:41.000000 decthings-api-0.0.1/src/decthings_api/rpc_impl/persistent_launcher.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     8105 2024-04-01 19:18:41.000000 decthings-api-0.0.1/src/decthings_api/rpc_impl/spawned.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     4536 2024-04-01 19:18:41.000000 decthings-api-0.0.1/src/decthings_api/rpc_impl/team.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     7673 2024-04-01 19:18:41.000000 decthings-api-0.0.1/src/decthings_api/rpc_impl/terminal.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     2598 2024-04-01 19:18:41.000000 decthings-api-0.0.1/src/decthings_api/rpc_impl/user.py
--rw-r--r--   0 viktor    (1000) viktor    (1000)    18913 2024-04-01 22:14:58.000000 decthings-api-0.0.1/src/decthings_api/tensor.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1262 2024-04-01 19:18:41.000000 decthings-api-0.0.1/src/decthings_api/varint.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     8729 2024-04-01 19:18:41.000000 decthings-api-0.0.1/src/decthings_api/ws.py
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-01 22:45:44.660560 decthings-api-0.0.1/src/decthings_api.egg-info/
--rw-r--r--   0 viktor    (1000) viktor    (1000)     1145 2024-04-01 22:45:44.000000 decthings-api-0.0.1/src/decthings_api.egg-info/PKG-INFO
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      881 2024-04-01 22:45:44.000000 decthings-api-0.0.1/src/decthings_api.egg-info/SOURCES.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)        1 2024-04-01 22:45:44.000000 decthings-api-0.0.1/src/decthings_api.egg-info/dependency_links.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       38 2024-04-01 22:45:44.000000 decthings-api-0.0.1/src/decthings_api.egg-info/requires.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       14 2024-04-01 22:45:44.000000 decthings-api-0.0.1/src/decthings_api.egg-info/top_level.txt
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-24 11:41:15.516888 decthings_api-0.0.2/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1066 2024-04-24 11:36:19.000000 decthings_api-0.0.2/LICENSE
+-rw-r--r--   0 viktor    (1000) viktor    (1000)     1146 2024-04-24 11:41:15.512889 decthings_api-0.0.2/PKG-INFO
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      658 2024-04-24 11:36:19.000000 decthings_api-0.0.2/README.md
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      460 2024-04-24 11:40:53.000000 decthings_api-0.0.2/pyproject.toml
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       38 2024-04-24 11:41:15.516888 decthings_api-0.0.2/setup.cfg
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-24 11:41:15.508889 decthings_api-0.0.2/src/
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-24 11:41:15.512889 decthings_api-0.0.2/src/decthings_api/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      257 2024-04-24 11:40:28.000000 decthings_api-0.0.2/src/decthings_api/__init__.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     4627 2024-04-24 11:36:19.000000 decthings_api-0.0.2/src/decthings_api/client.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     4634 2024-04-24 11:36:19.000000 decthings_api-0.0.2/src/decthings_api/client_sync.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1440 2024-04-24 11:36:19.000000 decthings_api-0.0.2/src/decthings_api/event.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     3627 2024-04-24 11:36:19.000000 decthings_api-0.0.2/src/decthings_api/protocol.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-24 11:41:15.512889 decthings_api-0.0.2/src/decthings_api/rpc_impl/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1746 2024-04-24 11:36:19.000000 decthings_api-0.0.2/src/decthings_api/rpc_impl/convert.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    10151 2024-04-24 11:36:19.000000 decthings_api-0.0.2/src/decthings_api/rpc_impl/dataset.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    16281 2024-04-24 11:36:19.000000 decthings_api-0.0.2/src/decthings_api/rpc_impl/debug.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    14561 2024-04-24 11:36:19.000000 decthings_api-0.0.2/src/decthings_api/rpc_impl/fs.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     4395 2024-04-24 11:36:19.000000 decthings_api-0.0.2/src/decthings_api/rpc_impl/language.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    23489 2024-04-24 11:36:19.000000 decthings_api-0.0.2/src/decthings_api/rpc_impl/model.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1873 2024-04-24 11:36:19.000000 decthings_api-0.0.2/src/decthings_api/rpc_impl/persistent_launcher.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     8105 2024-04-24 11:36:19.000000 decthings_api-0.0.2/src/decthings_api/rpc_impl/spawned.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     4536 2024-04-24 11:36:19.000000 decthings_api-0.0.2/src/decthings_api/rpc_impl/team.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     7673 2024-04-24 11:36:19.000000 decthings_api-0.0.2/src/decthings_api/rpc_impl/terminal.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     2598 2024-04-24 11:36:19.000000 decthings_api-0.0.2/src/decthings_api/rpc_impl/user.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    18913 2024-04-24 11:36:19.000000 decthings_api-0.0.2/src/decthings_api/tensor.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1262 2024-04-24 11:36:19.000000 decthings_api-0.0.2/src/decthings_api/varint.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     8729 2024-04-24 11:36:19.000000 decthings_api-0.0.2/src/decthings_api/ws.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-24 11:41:15.512889 decthings_api-0.0.2/src/decthings_api.egg-info/
+-rw-r--r--   0 viktor    (1000) viktor    (1000)     1146 2024-04-24 11:41:15.000000 decthings_api-0.0.2/src/decthings_api.egg-info/PKG-INFO
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      881 2024-04-24 11:41:15.000000 decthings_api-0.0.2/src/decthings_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)        1 2024-04-24 11:41:15.000000 decthings_api-0.0.2/src/decthings_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       38 2024-04-24 11:41:15.000000 decthings_api-0.0.2/src/decthings_api.egg-info/requires.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       14 2024-04-24 11:41:15.000000 decthings_api-0.0.2/src/decthings_api.egg-info/top_level.txt
```

### Comparing `decthings-api-0.0.1/LICENSE` & `decthings_api-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `decthings-api-0.0.1/PKG-INFO` & `decthings_api-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decthings-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: Official Python API client for Decthings
 Project-URL: Homepage, https://github.com/decthings/api-client-py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -22,12 +22,12 @@
 [Decthings](https://decthings.com) is a cloud-based API for artificial intelligence and machine learning. This package is officially supported by Decthings.
 
 `pip install decthings-api`
 
 ---
 #### Documentation
 
-Documentation for this package is available [here](https://decthings.com/docs/api-python).
+Documentation for this package is available [here](https://decthings.com/reference/python).
 
 ---
 
 With Decthings, you can create AI models that run in the cloud. Then, use an API client to send input data and receive the output.
```

### Comparing `decthings-api-0.0.1/README.md` & `decthings_api-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 [Decthings](https://decthings.com) is a cloud-based API for artificial intelligence and machine learning. This package is officially supported by Decthings.
 
 `pip install decthings-api`
 
 ---
 #### Documentation
 
-Documentation for this package is available [here](https://decthings.com/docs/api-python).
+Documentation for this package is available [here](https://decthings.com/reference/python).
 
 ---
 
 With Decthings, you can create AI models that run in the cloud. Then, use an API client to send input data and receive the output.
```

### Comparing `decthings-api-0.0.1/src/decthings_api/client.py` & `decthings_api-0.0.2/src/decthings_api/client.py`

 * *Files identical despite different names*

### Comparing `decthings-api-0.0.1/src/decthings_api/client_sync.py` & `decthings_api-0.0.2/src/decthings_api/client_sync.py`

 * *Files identical despite different names*

### Comparing `decthings-api-0.0.1/src/decthings_api/event.py` & `decthings_api-0.0.2/src/decthings_api/event.py`

 * *Files identical despite different names*

### Comparing `decthings-api-0.0.1/src/decthings_api/protocol.py` & `decthings_api-0.0.2/src/decthings_api/protocol.py`

 * *Files identical despite different names*

### Comparing `decthings-api-0.0.1/src/decthings_api/rpc_impl/convert.py` & `decthings_api-0.0.2/src/decthings_api/rpc_impl/convert.py`

 * *Files identical despite different names*

### Comparing `decthings-api-0.0.1/src/decthings_api/rpc_impl/dataset.py` & `decthings_api-0.0.2/src/decthings_api/rpc_impl/dataset.py`

 * *Files identical despite different names*

### Comparing `decthings-api-0.0.1/src/decthings_api/rpc_impl/debug.py` & `decthings_api-0.0.2/src/decthings_api/rpc_impl/debug.py`

 * *Files identical despite different names*

### Comparing `decthings-api-0.0.1/src/decthings_api/rpc_impl/fs.py` & `decthings_api-0.0.2/src/decthings_api/rpc_impl/fs.py`

 * *Files identical despite different names*

### Comparing `decthings-api-0.0.1/src/decthings_api/rpc_impl/language.py` & `decthings_api-0.0.2/src/decthings_api/rpc_impl/language.py`

 * *Files identical despite different names*

### Comparing `decthings-api-0.0.1/src/decthings_api/rpc_impl/model.py` & `decthings_api-0.0.2/src/decthings_api/rpc_impl/model.py`

 * *Files identical despite different names*

### Comparing `decthings-api-0.0.1/src/decthings_api/rpc_impl/persistent_launcher.py` & `decthings_api-0.0.2/src/decthings_api/rpc_impl/persistent_launcher.py`

 * *Files identical despite different names*

### Comparing `decthings-api-0.0.1/src/decthings_api/rpc_impl/spawned.py` & `decthings_api-0.0.2/src/decthings_api/rpc_impl/spawned.py`

 * *Files identical despite different names*

### Comparing `decthings-api-0.0.1/src/decthings_api/rpc_impl/team.py` & `decthings_api-0.0.2/src/decthings_api/rpc_impl/team.py`

 * *Files identical despite different names*

### Comparing `decthings-api-0.0.1/src/decthings_api/rpc_impl/terminal.py` & `decthings_api-0.0.2/src/decthings_api/rpc_impl/terminal.py`

 * *Files identical despite different names*

### Comparing `decthings-api-0.0.1/src/decthings_api/rpc_impl/user.py` & `decthings_api-0.0.2/src/decthings_api/rpc_impl/user.py`

 * *Files identical despite different names*

### Comparing `decthings-api-0.0.1/src/decthings_api/tensor.py` & `decthings_api-0.0.2/src/decthings_api/tensor.py`

 * *Files identical despite different names*

### Comparing `decthings-api-0.0.1/src/decthings_api/varint.py` & `decthings_api-0.0.2/src/decthings_api/varint.py`

 * *Files identical despite different names*

### Comparing `decthings-api-0.0.1/src/decthings_api/ws.py` & `decthings_api-0.0.2/src/decthings_api/ws.py`

 * *Files identical despite different names*

### Comparing `decthings-api-0.0.1/src/decthings_api.egg-info/PKG-INFO` & `decthings_api-0.0.2/src/decthings_api.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decthings-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: Official Python API client for Decthings
 Project-URL: Homepage, https://github.com/decthings/api-client-py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -22,12 +22,12 @@
 [Decthings](https://decthings.com) is a cloud-based API for artificial intelligence and machine learning. This package is officially supported by Decthings.
 
 `pip install decthings-api`
 
 ---
 #### Documentation
 
-Documentation for this package is available [here](https://decthings.com/docs/api-python).
+Documentation for this package is available [here](https://decthings.com/reference/python).
 
 ---
 
 With Decthings, you can create AI models that run in the cloud. Then, use an API client to send input data and receive the output.
```

### Comparing `decthings-api-0.0.1/src/decthings_api.egg-info/SOURCES.txt` & `decthings_api-0.0.2/src/decthings_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

