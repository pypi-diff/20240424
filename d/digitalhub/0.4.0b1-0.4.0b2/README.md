# Comparing `tmp/digitalhub-0.4.0b1.tar.gz` & `tmp/digitalhub-0.4.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub-0.4.0b1.tar", last modified: Fri Apr 19 08:57:50 2024, max compression
+gzip compressed data, was "digitalhub-0.4.0b2.tar", last modified: Wed Apr 24 07:50:19 2024, max compression
```

## Comparing `digitalhub-0.4.0b1.tar` & `digitalhub-0.4.0b2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:57:50.414500 digitalhub-0.4.0b1/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub-0.4.0b1/LICENSE.txt
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14790 2024-04-19 08:57:50.414500 digitalhub-0.4.0b1/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      510 2024-04-19 08:34:18.000000 digitalhub-0.4.0b1/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:57:50.410501 digitalhub-0.4.0b1/digitalhub/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2225 2024-04-19 08:14:48.000000 digitalhub-0.4.0b1/digitalhub/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:57:50.414500 digitalhub-0.4.0b1/digitalhub.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14790 2024-04-19 08:57:50.000000 digitalhub-0.4.0b1/digitalhub.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      421 2024-04-19 08:57:50.000000 digitalhub-0.4.0b1/digitalhub.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-04-19 08:57:50.000000 digitalhub-0.4.0b1/digitalhub.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      166 2024-04-19 08:57:50.000000 digitalhub-0.4.0b1/digitalhub.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       35 2024-04-19 08:57:50.000000 digitalhub-0.4.0b1/digitalhub.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1547 2024-04-19 08:46:19.000000 digitalhub-0.4.0b1/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-04-19 08:57:50.414500 digitalhub-0.4.0b1/setup.cfg
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:57:50.414500 digitalhub-0.4.0b1/test/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2511 2024-04-09 11:48:32.000000 digitalhub-0.4.0b1/test/test_crud_artifacts.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2504 2024-04-09 11:48:32.000000 digitalhub-0.4.0b1/test/test_crud_dataitems.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2769 2024-04-09 11:48:34.000000 digitalhub-0.4.0b1/test/test_crud_functions.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2220 2024-04-09 11:48:34.000000 digitalhub-0.4.0b1/test/test_crud_runs.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2111 2024-04-09 11:48:32.000000 digitalhub-0.4.0b1/test/test_crud_tasks.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1269 2024-03-22 13:56:51.000000 digitalhub-0.4.0b1/test/test_imports.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1086 2024-03-25 07:51:29.000000 digitalhub-0.4.0b1/test/testkfp.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      619 2024-03-25 10:18:34.000000 digitalhub-0.4.0b1/test/testkfp_pipeline.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:19.509784 digitalhub-0.4.0b2/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub-0.4.0b2/LICENSE.txt
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14790 2024-04-24 07:50:19.505784 digitalhub-0.4.0b2/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      510 2024-04-23 09:36:04.000000 digitalhub-0.4.0b2/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:19.505784 digitalhub-0.4.0b2/digitalhub/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2225 2024-04-23 09:36:04.000000 digitalhub-0.4.0b2/digitalhub/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:19.505784 digitalhub-0.4.0b2/digitalhub.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14790 2024-04-24 07:50:19.000000 digitalhub-0.4.0b2/digitalhub.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      421 2024-04-24 07:50:19.000000 digitalhub-0.4.0b2/digitalhub.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-04-24 07:50:19.000000 digitalhub-0.4.0b2/digitalhub.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      166 2024-04-24 07:50:19.000000 digitalhub-0.4.0b2/digitalhub.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       35 2024-04-24 07:50:19.000000 digitalhub-0.4.0b2/digitalhub.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1547 2024-04-23 13:34:39.000000 digitalhub-0.4.0b2/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-04-24 07:50:19.509784 digitalhub-0.4.0b2/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:50:19.505784 digitalhub-0.4.0b2/test/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2511 2024-04-09 11:48:32.000000 digitalhub-0.4.0b2/test/test_crud_artifacts.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2504 2024-04-09 11:48:32.000000 digitalhub-0.4.0b2/test/test_crud_dataitems.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2769 2024-04-09 11:48:34.000000 digitalhub-0.4.0b2/test/test_crud_functions.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2220 2024-04-09 11:48:34.000000 digitalhub-0.4.0b2/test/test_crud_runs.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2111 2024-04-09 11:48:32.000000 digitalhub-0.4.0b2/test/test_crud_tasks.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1269 2024-03-22 13:56:51.000000 digitalhub-0.4.0b2/test/test_imports.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1086 2024-03-25 07:51:29.000000 digitalhub-0.4.0b2/test/testkfp.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      619 2024-03-25 10:18:34.000000 digitalhub-0.4.0b2/test/testkfp_pipeline.py
```

### Comparing `digitalhub-0.4.0b1/LICENSE.txt` & `digitalhub-0.4.0b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b1/PKG-INFO` & `digitalhub-0.4.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub
-Version: 0.4.0b1
+Version: 0.4.0b2
 Summary: Python SDK for DigitalHub
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `digitalhub-0.4.0b1/digitalhub/__init__.py` & `digitalhub-0.4.0b2/digitalhub/__init__.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b1/digitalhub.egg-info/PKG-INFO` & `digitalhub-0.4.0b2/digitalhub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub
-Version: 0.4.0b1
+Version: 0.4.0b2
 Summary: Python SDK for DigitalHub
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `digitalhub-0.4.0b1/pyproject.toml` & `digitalhub-0.4.0b2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub"
-version = "0.4.0b1"
+version = "0.4.0b2"
 description = "Python SDK for DigitalHub"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -48,15 +48,15 @@
 [tool.ruff.extend-per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
 
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

### Comparing `digitalhub-0.4.0b1/test/test_crud_artifacts.py` & `digitalhub-0.4.0b2/test/test_crud_artifacts.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b1/test/test_crud_dataitems.py` & `digitalhub-0.4.0b2/test/test_crud_dataitems.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b1/test/test_crud_functions.py` & `digitalhub-0.4.0b2/test/test_crud_functions.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b1/test/test_crud_runs.py` & `digitalhub-0.4.0b2/test/test_crud_runs.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b1/test/test_crud_tasks.py` & `digitalhub-0.4.0b2/test/test_crud_tasks.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b1/test/test_imports.py` & `digitalhub-0.4.0b2/test/test_imports.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b1/test/testkfp.py` & `digitalhub-0.4.0b2/test/testkfp.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b1/test/testkfp_pipeline.py` & `digitalhub-0.4.0b2/test/testkfp_pipeline.py`

 * *Files identical despite different names*

