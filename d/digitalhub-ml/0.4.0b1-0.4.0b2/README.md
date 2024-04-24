# Comparing `tmp/digitalhub_ml-0.4.0b1.tar.gz` & `tmp/digitalhub_ml-0.4.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub_ml-0.4.0b1.tar", last modified: Fri Apr 19 08:59:16 2024, max compression
+gzip compressed data, was "digitalhub_ml-0.4.0b2.tar", last modified: Wed Apr 24 07:53:14 2024, max compression
```

## Comparing `digitalhub_ml-0.4.0b1.tar` & `digitalhub_ml-0.4.0b2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:59:16.567960 digitalhub_ml-0.4.0b1/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      938 2024-04-19 08:59:16.567960 digitalhub_ml-0.4.0b1/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      462 2024-04-19 08:38:22.000000 digitalhub_ml-0.4.0b1/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:59:16.567960 digitalhub_ml-0.4.0b1/digitalhub_ml/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      304 2024-04-19 08:14:48.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:59:16.567960 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:38:37.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:59:16.567960 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/models/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:40:22.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/models/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6252 2024-04-19 08:14:48.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/models/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6786 2024-04-19 08:14:48.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/models/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      318 2024-04-17 12:32:27.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/models/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      557 2024-04-17 12:32:27.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/models/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      209 2024-02-15 10:15:41.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/models/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:59:16.567960 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:33:48.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6049 2024-04-19 08:14:48.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5788 2024-04-19 08:14:48.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      988 2024-04-19 08:14:48.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      991 2024-04-17 12:32:27.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:59:16.567960 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-23 14:34:03.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/runs/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      405 2024-04-19 08:14:48.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      313 2024-03-14 13:46:16.000000 digitalhub_ml-0.4.0b1/digitalhub_ml/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:59:16.567960 digitalhub_ml-0.4.0b1/digitalhub_ml.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      938 2024-04-19 08:59:16.000000 digitalhub_ml-0.4.0b1/digitalhub_ml.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      864 2024-04-19 08:59:16.000000 digitalhub_ml-0.4.0b1/digitalhub_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-04-19 08:59:16.000000 digitalhub_ml-0.4.0b1/digitalhub_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-19 08:59:16.000000 digitalhub_ml-0.4.0b1/digitalhub_ml.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       19 2024-04-19 08:59:16.000000 digitalhub_ml-0.4.0b1/digitalhub_ml.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1054 2024-04-19 08:46:19.000000 digitalhub_ml-0.4.0b1/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-04-19 08:59:16.567960 digitalhub_ml-0.4.0b1/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:53:14.943603 digitalhub_ml-0.4.0b2/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      938 2024-04-24 07:53:14.943603 digitalhub_ml-0.4.0b2/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      462 2024-04-23 09:36:04.000000 digitalhub_ml-0.4.0b2/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:53:14.939603 digitalhub_ml-0.4.0b2/digitalhub_ml/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      304 2024-04-19 08:14:48.000000 digitalhub_ml-0.4.0b2/digitalhub_ml/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:53:14.943603 digitalhub_ml-0.4.0b2/digitalhub_ml/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:38:37.000000 digitalhub_ml-0.4.0b2/digitalhub_ml/entities/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:53:14.943603 digitalhub_ml-0.4.0b2/digitalhub_ml/entities/models/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:40:22.000000 digitalhub_ml-0.4.0b2/digitalhub_ml/entities/models/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6252 2024-04-19 08:14:48.000000 digitalhub_ml-0.4.0b2/digitalhub_ml/entities/models/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6786 2024-04-23 09:36:04.000000 digitalhub_ml-0.4.0b2/digitalhub_ml/entities/models/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      318 2024-04-23 09:36:04.000000 digitalhub_ml-0.4.0b2/digitalhub_ml/entities/models/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      557 2024-04-23 09:36:04.000000 digitalhub_ml-0.4.0b2/digitalhub_ml/entities/models/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      209 2024-02-15 10:15:41.000000 digitalhub_ml-0.4.0b2/digitalhub_ml/entities/models/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:53:14.943603 digitalhub_ml-0.4.0b2/digitalhub_ml/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:33:48.000000 digitalhub_ml-0.4.0b2/digitalhub_ml/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6049 2024-04-19 08:14:48.000000 digitalhub_ml-0.4.0b2/digitalhub_ml/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5788 2024-04-23 09:36:04.000000 digitalhub_ml-0.4.0b2/digitalhub_ml/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      988 2024-04-23 09:36:04.000000 digitalhub_ml-0.4.0b2/digitalhub_ml/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      991 2024-04-23 09:36:04.000000 digitalhub_ml-0.4.0b2/digitalhub_ml/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:53:14.943603 digitalhub_ml-0.4.0b2/digitalhub_ml/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-23 14:34:03.000000 digitalhub_ml-0.4.0b2/digitalhub_ml/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_ml-0.4.0b2/digitalhub_ml/entities/runs/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      405 2024-04-19 08:14:48.000000 digitalhub_ml-0.4.0b2/digitalhub_ml/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      313 2024-03-14 13:46:16.000000 digitalhub_ml-0.4.0b2/digitalhub_ml/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:53:14.943603 digitalhub_ml-0.4.0b2/digitalhub_ml.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      938 2024-04-24 07:53:14.000000 digitalhub_ml-0.4.0b2/digitalhub_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      864 2024-04-24 07:53:14.000000 digitalhub_ml-0.4.0b2/digitalhub_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-04-24 07:53:14.000000 digitalhub_ml-0.4.0b2/digitalhub_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-24 07:53:14.000000 digitalhub_ml-0.4.0b2/digitalhub_ml.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       19 2024-04-24 07:53:14.000000 digitalhub_ml-0.4.0b2/digitalhub_ml.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1054 2024-04-23 13:34:39.000000 digitalhub_ml-0.4.0b2/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-04-24 07:53:14.943603 digitalhub_ml-0.4.0b2/setup.cfg
```

### Comparing `digitalhub_ml-0.4.0b1/PKG-INFO` & `digitalhub_ml-0.4.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-ml
-Version: 0.4.0b1
+Version: 0.4.0b2
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
```

### Comparing `digitalhub_ml-0.4.0b1/digitalhub_ml/entities/models/crud.py` & `digitalhub_ml-0.4.0b2/digitalhub_ml/entities/models/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.4.0b1/digitalhub_ml/entities/models/entity.py` & `digitalhub_ml-0.4.0b2/digitalhub_ml/entities/models/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.4.0b1/digitalhub_ml/entities/models/spec.py` & `digitalhub_ml-0.4.0b2/digitalhub_ml/entities/models/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.4.0b1/digitalhub_ml/entities/projects/crud.py` & `digitalhub_ml-0.4.0b2/digitalhub_ml/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.4.0b1/digitalhub_ml/entities/projects/entity.py` & `digitalhub_ml-0.4.0b2/digitalhub_ml/entities/projects/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.4.0b1/digitalhub_ml/entities/projects/spec.py` & `digitalhub_ml-0.4.0b2/digitalhub_ml/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.4.0b1/digitalhub_ml/entities/registries.py` & `digitalhub_ml-0.4.0b2/digitalhub_ml/entities/registries.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.4.0b1/digitalhub_ml.egg-info/PKG-INFO` & `digitalhub_ml-0.4.0b2/digitalhub_ml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-ml
-Version: 0.4.0b1
+Version: 0.4.0b2
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
```

### Comparing `digitalhub_ml-0.4.0b1/digitalhub_ml.egg-info/SOURCES.txt` & `digitalhub_ml-0.4.0b2/digitalhub_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.4.0b1/pyproject.toml` & `digitalhub_ml-0.4.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-ml"
-version = "0.4.0b1"
+version = "0.4.0b2"
 description = "Python SDK for DHCore"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -23,15 +23,15 @@
     "digitalhub-data~=0.3",
 ]
 
 [tool.setuptools.packages.find]
 exclude = ["modules*"]
 
 [tool.bumpver]
-current_version = "0.4.0b1"
+current_version = "0.4.0b2"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

