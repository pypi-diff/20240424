# Comparing `tmp/decthings_model-0.0.3.tar.gz` & `tmp/decthings_model-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decthings_model-0.0.3.tar", last modified: Tue Apr 16 09:15:40 2024, max compression
+gzip compressed data, was "decthings_model-0.0.4.tar", last modified: Wed Apr 24 11:47:35 2024, max compression
```

## Comparing `decthings_model-0.0.3.tar` & `decthings_model-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-16 09:15:40.666765 decthings_model-0.0.3/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1066 2024-04-16 09:05:15.000000 decthings_model-0.0.3/LICENSE
--rw-r--r--   0 viktor    (1000) viktor    (1000)     1464 2024-04-16 09:15:40.666765 decthings_model-0.0.3/PKG-INFO
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1029 2024-04-16 09:05:15.000000 decthings_model-0.0.3/README.md
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      421 2024-04-16 09:15:23.000000 decthings_model-0.0.3/pyproject.toml
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       38 2024-04-16 09:15:40.666765 decthings_model-0.0.3/setup.cfg
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-16 09:15:40.666765 decthings_model-0.0.3/src/
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-16 09:15:40.666765 decthings_model-0.0.3/src/decthings_model/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       21 2024-04-16 09:09:55.000000 decthings_model-0.0.3/src/decthings_model/__init__.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       34 2024-04-16 09:05:15.000000 decthings_model-0.0.3/src/decthings_model/__main__.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    11294 2024-04-16 09:05:15.000000 decthings_model-0.0.3/src/decthings_model/model.py
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-16 09:15:40.666765 decthings_model-0.0.3/src/decthings_model/run/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     6642 2024-04-16 09:05:15.000000 decthings_model-0.0.3/src/decthings_model/run/dataloader.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    14621 2024-04-16 09:05:15.000000 decthings_model-0.0.3/src/decthings_model/run/run.py
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-16 09:15:40.666765 decthings_model-0.0.3/src/decthings_model.egg-info/
--rw-r--r--   0 viktor    (1000) viktor    (1000)     1464 2024-04-16 09:15:40.000000 decthings_model-0.0.3/src/decthings_model.egg-info/PKG-INFO
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      408 2024-04-16 09:15:40.000000 decthings_model-0.0.3/src/decthings_model.egg-info/SOURCES.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)        1 2024-04-16 09:15:40.000000 decthings_model-0.0.3/src/decthings_model.egg-info/dependency_links.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       21 2024-04-16 09:15:40.000000 decthings_model-0.0.3/src/decthings_model.egg-info/requires.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       16 2024-04-16 09:15:40.000000 decthings_model-0.0.3/src/decthings_model.egg-info/top_level.txt
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-24 11:47:35.325650 decthings_model-0.0.4/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1066 2024-04-16 09:05:15.000000 decthings_model-0.0.4/LICENSE
+-rw-r--r--   0 viktor    (1000) viktor    (1000)     1464 2024-04-24 11:47:35.325650 decthings_model-0.0.4/PKG-INFO
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1029 2024-04-18 15:37:50.000000 decthings_model-0.0.4/README.md
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      421 2024-04-24 11:47:16.000000 decthings_model-0.0.4/pyproject.toml
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       38 2024-04-24 11:47:35.325650 decthings_model-0.0.4/setup.cfg
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-24 11:47:35.325650 decthings_model-0.0.4/src/
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-24 11:47:35.325650 decthings_model-0.0.4/src/decthings_model/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      133 2024-04-24 11:43:09.000000 decthings_model-0.0.4/src/decthings_model/__init__.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       34 2024-04-16 09:05:15.000000 decthings_model-0.0.4/src/decthings_model/__main__.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    11294 2024-04-16 09:05:15.000000 decthings_model-0.0.4/src/decthings_model/model.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-24 11:47:35.325650 decthings_model-0.0.4/src/decthings_model/run/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     6642 2024-04-16 09:05:15.000000 decthings_model-0.0.4/src/decthings_model/run/dataloader.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    14621 2024-04-16 09:05:15.000000 decthings_model-0.0.4/src/decthings_model/run/run.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-24 11:47:35.325650 decthings_model-0.0.4/src/decthings_model.egg-info/
+-rw-r--r--   0 viktor    (1000) viktor    (1000)     1464 2024-04-24 11:47:35.000000 decthings_model-0.0.4/src/decthings_model.egg-info/PKG-INFO
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      408 2024-04-24 11:47:35.000000 decthings_model-0.0.4/src/decthings_model.egg-info/SOURCES.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)        1 2024-04-24 11:47:35.000000 decthings_model-0.0.4/src/decthings_model.egg-info/dependency_links.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       21 2024-04-24 11:47:35.000000 decthings_model-0.0.4/src/decthings_model.egg-info/requires.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       16 2024-04-24 11:47:35.000000 decthings_model-0.0.4/src/decthings_model.egg-info/top_level.txt
```

### Comparing `decthings_model-0.0.3/LICENSE` & `decthings_model-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `decthings_model-0.0.3/PKG-INFO` & `decthings_model-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decthings-model
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create a Decthings model using Python
 Project-URL: Homepage, https://github.com/decthings/model-py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `decthings_model-0.0.3/README.md` & `decthings_model-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `decthings_model-0.0.3/src/decthings_model/model.py` & `decthings_model-0.0.4/src/decthings_model/model.py`

 * *Files identical despite different names*

### Comparing `decthings_model-0.0.3/src/decthings_model/run/dataloader.py` & `decthings_model-0.0.4/src/decthings_model/run/dataloader.py`

 * *Files identical despite different names*

### Comparing `decthings_model-0.0.3/src/decthings_model/run/run.py` & `decthings_model-0.0.4/src/decthings_model/run/run.py`

 * *Files identical despite different names*

### Comparing `decthings_model-0.0.3/src/decthings_model.egg-info/PKG-INFO` & `decthings_model-0.0.4/src/decthings_model.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decthings-model
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create a Decthings model using Python
 Project-URL: Homepage, https://github.com/decthings/model-py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

