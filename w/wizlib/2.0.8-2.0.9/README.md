# Comparing `tmp/wizlib-2.0.8.tar.gz` & `tmp/wizlib-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizlib-2.0.8.tar", max compression
+gzip compressed data, was "wizlib-2.0.9.tar", max compression
```

## Comparing `wizlib-2.0.8.tar` & `wizlib-2.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     5320 2023-11-25 21:45:01.983618 wizlib-2.0.8/README.md
--rw-r--r--   0        0        0      696 2023-11-25 21:45:18.092446 wizlib-2.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-25 21:45:02.010617 wizlib-2.0.8/wizlib/__init__.py
--rw-r--r--   0        0        0     2794 2023-11-25 21:45:01.984618 wizlib-2.0.8/wizlib/app.py
--rw-r--r--   0        0        0     4424 2023-11-25 21:45:01.984618 wizlib-2.0.8/wizlib/class_family.py
--rw-r--r--   0        0        0     1304 2023-11-25 21:45:01.984618 wizlib-2.0.8/wizlib/command.py
--rw-r--r--   0        0        0     2600 2023-11-25 21:45:01.984618 wizlib-2.0.8/wizlib/config_handler.py
--rw-r--r--   0        0        0       46 2023-11-25 21:45:01.984618 wizlib-2.0.8/wizlib/error.py
--rw-r--r--   0        0        0      306 2023-11-25 21:45:01.984618 wizlib-2.0.8/wizlib/handler.py
--rw-r--r--   0        0        0      597 2023-11-25 21:45:01.984618 wizlib-2.0.8/wizlib/input_handler.py
--rw-r--r--   0        0        0     1505 2023-11-25 21:45:01.984618 wizlib-2.0.8/wizlib/parser.py
--rw-r--r--   0        0        0     1754 2023-11-25 21:45:01.984618 wizlib-2.0.8/wizlib/rlinput.py
--rw-r--r--   0        0        0      272 2023-11-25 21:45:01.984618 wizlib-2.0.8/wizlib/super_wrapper.py
--rw-r--r--   0        0        0     5921 1970-01-01 00:00:00.000000 wizlib-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     5320 2023-11-26 21:00:11.298215 wizlib-2.0.9/README.md
+-rw-r--r--   0        0        0      696 2023-11-26 21:00:27.610307 wizlib-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-26 21:00:11.325215 wizlib-2.0.9/wizlib/__init__.py
+-rw-r--r--   0        0        0     2794 2023-11-26 21:00:11.299215 wizlib-2.0.9/wizlib/app.py
+-rw-r--r--   0        0        0     4424 2023-11-26 21:00:11.299215 wizlib-2.0.9/wizlib/class_family.py
+-rw-r--r--   0        0        0     1304 2023-11-26 21:00:11.299215 wizlib-2.0.9/wizlib/command.py
+-rw-r--r--   0        0        0     2639 2023-11-26 21:00:11.299215 wizlib-2.0.9/wizlib/config_handler.py
+-rw-r--r--   0        0        0       46 2023-11-26 21:00:11.299215 wizlib-2.0.9/wizlib/error.py
+-rw-r--r--   0        0        0      306 2023-11-26 21:00:11.299215 wizlib-2.0.9/wizlib/handler.py
+-rw-r--r--   0        0        0      597 2023-11-26 21:00:11.299215 wizlib-2.0.9/wizlib/input_handler.py
+-rw-r--r--   0        0        0     1505 2023-11-26 21:00:11.299215 wizlib-2.0.9/wizlib/parser.py
+-rw-r--r--   0        0        0     1754 2023-11-26 21:00:11.299215 wizlib-2.0.9/wizlib/rlinput.py
+-rw-r--r--   0        0        0      272 2023-11-26 21:00:11.299215 wizlib-2.0.9/wizlib/super_wrapper.py
+-rw-r--r--   0        0        0     5921 1970-01-01 00:00:00.000000 wizlib-2.0.9/PKG-INFO
```

### Comparing `wizlib-2.0.8/README.md` & `wizlib-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `wizlib-2.0.8/pyproject.toml` & `wizlib-2.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wizlib"
-version = "2.0.8"
+version = "2.0.9"
 description = "Framework for flexible and powerful command-line applications"
 authors = ["Steampunk Wizard <wizlib@steampunkwizard.ca>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
```

### Comparing `wizlib-2.0.8/wizlib/app.py` & `wizlib-2.0.9/wizlib/app.py`

 * *Files identical despite different names*

### Comparing `wizlib-2.0.8/wizlib/class_family.py` & `wizlib-2.0.9/wizlib/class_family.py`

 * *Files identical despite different names*

### Comparing `wizlib-2.0.8/wizlib/command.py` & `wizlib-2.0.9/wizlib/command.py`

 * *Files identical despite different names*

### Comparing `wizlib-2.0.8/wizlib/config_handler.py` & `wizlib-2.0.9/wizlib/config_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,11 +76,12 @@
 
     @classmethod
     def fake(cls, **vals):
         """Return a fake ConfigHandler with forced values, for testing"""
         handler = cls()
 
         def fake_env(name):
-            if name in vals:
-                return vals[name]
+            key = name.replace('-', '_')
+            if key in vals:
+                return vals[key]
         handler.env = fake_env
         return handler
```

### Comparing `wizlib-2.0.8/wizlib/input_handler.py` & `wizlib-2.0.9/wizlib/input_handler.py`

 * *Files identical despite different names*

### Comparing `wizlib-2.0.8/wizlib/parser.py` & `wizlib-2.0.9/wizlib/parser.py`

 * *Files identical despite different names*

### Comparing `wizlib-2.0.8/wizlib/rlinput.py` & `wizlib-2.0.9/wizlib/rlinput.py`

 * *Files identical despite different names*

### Comparing `wizlib-2.0.8/PKG-INFO` & `wizlib-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizlib
-Version: 2.0.8
+Version: 2.0.9
 Summary: Framework for flexible and powerful command-line applications
 License: MIT
 Author: Steampunk Wizard
 Author-email: wizlib@steampunkwizard.ca
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

