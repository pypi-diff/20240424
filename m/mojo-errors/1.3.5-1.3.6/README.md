# Comparing `tmp/mojo_errors-1.3.5.tar.gz` & `tmp/mojo_errors-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_errors-1.3.5.tar", max compression
+gzip compressed data, was "mojo_errors-1.3.6.tar", max compression
```

## Comparing `mojo_errors-1.3.5.tar` & `mojo_errors-1.3.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1083 2024-01-26 02:55:15.327504 mojo_errors-1.3.5/LICENSE.txt
--rw-r--r--   0        0        0      154 2024-01-29 05:14:53.461749 mojo_errors-1.3.5/README.rst
--rw-r--r--   0        0        0      663 2024-03-09 19:49:50.816983 mojo_errors-1.3.5/pyproject.toml
--rw-r--r--   0        0        0     5281 2024-01-26 02:55:15.328551 mojo_errors-1.3.5/source/packages/mojo/errors/exceptions.py
--rw-r--r--   0        0        0    11785 2024-03-09 19:49:42.773416 mojo_errors-1.3.5/source/packages/mojo/errors/xtraceback.py
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 mojo_errors-1.3.5/setup.py
--rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 mojo_errors-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-26 02:55:15.327504 mojo_errors-1.3.6/LICENSE.txt
+-rw-r--r--   0        0        0      154 2024-01-29 05:14:53.461749 mojo_errors-1.3.6/README.rst
+-rw-r--r--   0        0        0      663 2024-04-24 03:49:12.060446 mojo_errors-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0     5281 2024-01-26 02:55:15.328551 mojo_errors-1.3.6/source/packages/mojo/errors/exceptions.py
+-rw-r--r--   0        0        0    11785 2024-03-09 19:49:42.773416 mojo_errors-1.3.6/source/packages/mojo/errors/xtraceback.py
+-rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 mojo_errors-1.3.6/setup.py
+-rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 mojo_errors-1.3.6/PKG-INFO
```

### Comparing `mojo_errors-1.3.5/LICENSE.txt` & `mojo_errors-1.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_errors-1.3.5/pyproject.toml` & `mojo_errors-1.3.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mojo-errors"
 description = "Automation Mojo Errors Module"
-version = "1.3.5"
+version = "1.3.6"
 authors = []
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
```

### Comparing `mojo_errors-1.3.5/source/packages/mojo/errors/exceptions.py` & `mojo_errors-1.3.6/source/packages/mojo/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `mojo_errors-1.3.5/source/packages/mojo/errors/xtraceback.py` & `mojo_errors-1.3.6/source/packages/mojo/errors/xtraceback.py`

 * *Files identical despite different names*

### Comparing `mojo_errors-1.3.5/setup.py` & `mojo_errors-1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['mojo', 'mojo.errors']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'mojo-errors',
-    'version': '1.3.5',
+    'version': '1.3.6',
     'description': 'Automation Mojo Errors Module',
     'long_description': '==============================\nAutomation Mojo Errors Package\n==============================\nPython package that provides a common source of error types.\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mojo_errors-1.3.5/PKG-INFO` & `mojo_errors-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mojo-errors
-Version: 1.3.5
+Version: 1.3.6
 Summary: Automation Mojo Errors Module
 License: LICENSE.txt
 Keywords: python
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
```

