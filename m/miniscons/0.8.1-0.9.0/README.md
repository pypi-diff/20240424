# Comparing `tmp/miniscons-0.8.1.tar.gz` & `tmp/miniscons-0.9.0.tar.gz`

## Comparing `miniscons-0.8.1.tar` & `miniscons-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 miniscons-0.8.1/src/__init__.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 miniscons-0.8.1/src/build.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 miniscons-0.8.1/src/compiler.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 miniscons-0.8.1/src/containers.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 miniscons-0.8.1/src/environment.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 miniscons-0.8.1/src/flag.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 miniscons-0.8.1/src/routine.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 miniscons-0.8.1/src/script.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 miniscons-0.8.1/src/target.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 miniscons-0.8.1/src/tasks.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 miniscons-0.8.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 miniscons-0.8.1/LICENSE.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 miniscons-0.8.1/README.md
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 miniscons-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 miniscons-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 miniscons-0.9.0/src/__init__.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 miniscons-0.9.0/src/build.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 miniscons-0.9.0/src/compiler.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 miniscons-0.9.0/src/containers.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 miniscons-0.9.0/src/environment.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 miniscons-0.9.0/src/flag.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 miniscons-0.9.0/src/routine.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 miniscons-0.9.0/src/script.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 miniscons-0.9.0/src/target.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 miniscons-0.9.0/src/tasks.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 miniscons-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 miniscons-0.9.0/LICENSE.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 miniscons-0.9.0/README.md
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 miniscons-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 miniscons-0.9.0/PKG-INFO
```

### Comparing `miniscons-0.8.1/src/build.py` & `miniscons-0.9.0/src/build.py`

 * *Files identical despite different names*

### Comparing `miniscons-0.8.1/src/environment.py` & `miniscons-0.9.0/src/environment.py`

 * *Files identical despite different names*

### Comparing `miniscons-0.8.1/src/script.py` & `miniscons-0.9.0/src/script.py`

 * *Files identical despite different names*

### Comparing `miniscons-0.8.1/src/target.py` & `miniscons-0.9.0/src/target.py`

 * *Files identical despite different names*

### Comparing `miniscons-0.8.1/src/tasks.py` & `miniscons-0.9.0/src/tasks.py`

 * *Files identical despite different names*

### Comparing `miniscons-0.8.1/LICENSE.md` & `miniscons-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `miniscons-0.8.1/pyproject.toml` & `miniscons-0.9.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "miniscons"
 description = "SCons builders."
-version = "0.8.1"
+version = "0.9.0"
 
 keywords = ["SCons", "SConstruct", "builders"]
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 requires-python = ">=3.8"
-dependencies = ["SCons==4.3.0"]
+dependencies = ["psutil==5.9.1", "SCons==4.3.0"]
 
 [project.optional-dependencies]
 all = [
     "autoflake==1.4",
     "black==22.3.0",
     "build==1.2.1",
     "bump2version==1.0.1",
@@ -67,17 +67,24 @@
 src = "miniscons"
 
 [tool.thx.jobs]
 lint = [
     "npx cspell . --dot",
     "pylint src --disable=C0114,C0115,C0116,C0411,C3001",
     "mypy -m src --ignore-missing-import",
+    "trufflehog3",
 ]
 
 format = [
     "black .",
     "isort . --no-sections --remove-redundant-aliases",
     "npx prettier . --write",
 ]
 
 test = "pytest . --doctest-modules --cov --cov-report=xml"
 docs = "doxygen"
+
+[tool.coverage.run]
+data_file = "coverage/.coverage"
+
+[tool.coverage.xml]
+output = "coverage/cobertura.xml"
```

### Comparing `miniscons-0.8.1/PKG-INFO` & `miniscons-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: miniscons
-Version: 0.8.1
+Version: 0.9.0
 Summary: SCons builders.
 Project-URL: Homepage, https://github.com/JoelLefkowitz/miniscons
 Author-email: Joel Lefkowitz <joellefkowitz@hotmail.com>
 License: # MIT License
         
         Copyright (c) 2024 Joel Lefkowitz
         
@@ -28,14 +28,15 @@
 Keywords: SCons,SConstruct,builders
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Requires-Dist: psutil==5.9.1
 Requires-Dist: scons==4.3.0
 Provides-Extra: all
 Requires-Dist: autoflake==1.4; extra == 'all'
 Requires-Dist: black==22.3.0; extra == 'all'
 Requires-Dist: build==1.2.1; extra == 'all'
 Requires-Dist: bump2version==1.0.1; extra == 'all'
 Requires-Dist: isort==5.10.1; extra == 'all'
```

