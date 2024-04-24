# Comparing `tmp/taxref-0.0.8.tar.gz` & `tmp/taxref-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taxref-0.0.8.tar", last modified: Mon Apr  8 07:08:19 2024, max compression
+gzip compressed data, was "taxref-0.0.9.tar", last modified: Thu Apr 18 19:44:56 2024, max compression
```

## Comparing `taxref-0.0.8.tar` & `taxref-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-04-08 07:08:19.701881 taxref-0.0.8/
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     1211 2024-04-08 07:08:07.000000 taxref-0.0.8/LICENSE.md
--rw-r--r--   0 gitlab-runner   (993) gitlab-runner   (993)      607 2024-04-08 07:08:19.701881 taxref-0.0.8/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      210 2023-11-24 00:25:28.000000 taxref-0.0.8/README.md
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      541 2024-04-08 07:08:07.000000 taxref-0.0.8/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)       38 2024-04-08 07:08:19.701881 taxref-0.0.8/setup.cfg
-drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-04-08 07:08:19.701881 taxref-0.0.8/taxref.egg-info/
--rw-r--r--   0 gitlab-runner   (993) gitlab-runner   (993)      607 2024-04-08 07:08:19.000000 taxref-0.0.8/taxref.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      184 2024-04-08 07:08:19.000000 taxref-0.0.8/taxref.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)        1 2024-04-08 07:08:19.000000 taxref-0.0.8/taxref.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)       23 2024-04-08 07:08:19.000000 taxref-0.0.8/taxref.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     3699 2023-11-21 21:18:39.000000 taxref-0.0.8/taxref11.py
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      455 2023-11-24 22:14:28.000000 taxref-0.0.8/taxref_common.py
+drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-04-18 19:44:56.507924 taxref-0.0.9/
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     1211 2024-04-18 19:44:43.000000 taxref-0.0.9/LICENSE.md
+-rw-r--r--   0 gitlab-runner   (993) gitlab-runner   (993)      607 2024-04-18 19:44:56.507924 taxref-0.0.9/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      210 2023-11-24 00:25:28.000000 taxref-0.0.9/README.md
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      551 2024-04-18 19:44:43.000000 taxref-0.0.9/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)       38 2024-04-18 19:44:56.507924 taxref-0.0.9/setup.cfg
+drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-04-18 19:44:56.495924 taxref-0.0.9/src/
+drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-04-18 19:44:56.495924 taxref-0.0.9/src/taxref/
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-04-17 21:02:58.000000 taxref-0.0.9/src/taxref/__init__.py
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     3699 2024-04-17 21:02:58.000000 taxref-0.0.9/src/taxref/taxref11.py
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      455 2024-04-17 21:02:58.000000 taxref-0.0.9/src/taxref/taxref_common.py
+drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-04-18 19:44:56.507924 taxref-0.0.9/src/taxref.egg-info/
+-rw-r--r--   0 gitlab-runner   (993) gitlab-runner   (993)      607 2024-04-18 19:44:56.000000 taxref-0.0.9/src/taxref.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      258 2024-04-18 19:44:56.000000 taxref-0.0.9/src/taxref.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)        1 2024-04-18 19:44:56.000000 taxref-0.0.9/src/taxref.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)        7 2024-04-18 19:44:56.000000 taxref-0.0.9/src/taxref.egg-info/top_level.txt
+drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-04-18 19:44:56.495924 taxref-0.0.9/test/
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     1234 2024-04-17 21:13:26.000000 taxref-0.0.9/test/test.py
```

### Comparing `taxref-0.0.8/LICENSE.md` & `taxref-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `taxref-0.0.8/PKG-INFO` & `taxref-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taxref
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple taxref toolbox.
 Author-email: Samuel Andrés <samuel.andres@yahoo.fr>
 Project-URL: Homepage, https://github.com/SamuelAndresPascal/cosmoloj-py
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `taxref-0.0.8/pyproject.toml` & `taxref-0.0.9/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "taxref"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Samuel Andrés", email="samuel.andres@yahoo.fr" },
 ]
 description = "A simple taxref toolbox."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
-[tool.setuptools]
-py-modules = ["taxref_common", "taxref11"]
+[tool.pytest.ini_options]
+addopts = [
+    "--import-mode=importlib",
+]
 
 [project.urls]
 "Homepage" = "https://github.com/SamuelAndresPascal/cosmoloj-py"
```

### Comparing `taxref-0.0.8/taxref.egg-info/PKG-INFO` & `taxref-0.0.9/src/taxref.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taxref
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple taxref toolbox.
 Author-email: Samuel Andrés <samuel.andres@yahoo.fr>
 Project-URL: Homepage, https://github.com/SamuelAndresPascal/cosmoloj-py
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `taxref-0.0.8/taxref11.py` & `taxref-0.0.9/src/taxref/taxref11.py`

 * *Files identical despite different names*

