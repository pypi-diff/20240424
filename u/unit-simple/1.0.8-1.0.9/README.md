# Comparing `tmp/unit_simple-1.0.8.tar.gz` & `tmp/unit_simple-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unit_simple-1.0.8.tar", last modified: Fri Mar 22 22:18:14 2024, max compression
+gzip compressed data, was "unit_simple-1.0.9.tar", last modified: Fri Apr  5 15:32:55 2024, max compression
```

## Comparing `unit_simple-1.0.8.tar` & `unit_simple-1.0.9.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-03-22 22:18:14.475212 unit_simple-1.0.8/
--rw-r--r--   0 gitlab-runner   (993) gitlab-runner   (993)     4992 2024-03-22 22:18:14.475212 unit_simple-1.0.8/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     4576 2024-03-22 21:53:05.000000 unit_simple-1.0.8/README.md
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      571 2024-03-22 22:18:02.000000 unit_simple-1.0.8/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)       38 2024-03-22 22:18:14.475212 unit_simple-1.0.8/setup.cfg
-drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-03-22 22:18:14.475212 unit_simple-1.0.8/unit_simple.egg-info/
--rw-r--r--   0 gitlab-runner   (993) gitlab-runner   (993)     4992 2024-03-22 22:18:14.000000 unit_simple-1.0.8/unit_simple.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      179 2024-03-22 22:18:14.000000 unit_simple-1.0.8/unit_simple.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)        1 2024-03-22 22:18:14.000000 unit_simple-1.0.8/unit_simple.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)       12 2024-03-22 22:18:14.000000 unit_simple-1.0.8/unit_simple.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     8671 2024-03-05 22:07:55.000000 unit_simple-1.0.8/unit_simple.py
+drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-04-05 15:32:55.879851 unit_simple-1.0.9/
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     1211 2024-04-05 15:32:44.000000 unit_simple-1.0.9/LICENSE.md
+-rw-r--r--   0 gitlab-runner   (993) gitlab-runner   (993)     6430 2024-04-05 15:32:55.879851 unit_simple-1.0.9/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     4576 2024-03-22 21:53:05.000000 unit_simple-1.0.9/README.md
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      603 2024-04-05 15:32:44.000000 unit_simple-1.0.9/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)       38 2024-04-05 15:32:55.879851 unit_simple-1.0.9/setup.cfg
+drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-04-05 15:32:55.879851 unit_simple-1.0.9/unit_simple.egg-info/
+-rw-r--r--   0 gitlab-runner   (993) gitlab-runner   (993)     6430 2024-04-05 15:32:55.000000 unit_simple-1.0.9/unit_simple.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      190 2024-04-05 15:32:55.000000 unit_simple-1.0.9/unit_simple.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)        1 2024-04-05 15:32:55.000000 unit_simple-1.0.9/unit_simple.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)       12 2024-04-05 15:32:55.000000 unit_simple-1.0.9/unit_simple.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     8671 2024-03-05 22:07:55.000000 unit_simple-1.0.9/unit_simple.py
```

### Comparing `unit_simple-1.0.8/PKG-INFO` & `unit_simple-1.0.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: unit_simple
-Version: 1.0.8
-Summary: A simple measurement unit API to handle basic unit conversions.
-Author-email: Samuel Andrés <samuel.andres@yahoo.fr>
-Project-URL: Homepage, https://github.com/SamuelAndresPascal/cosmoloj-py
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-
 # Simple Unit (Python implementation)
 
 [![Anaconda-Server Badge](https://anaconda.org/cosmoloj/unit_simple/badges/version.svg)](https://anaconda.org/cosmoloj/unit_simple)
 [![PyPI repository Badge](https://badge.fury.io/py/unit_simple.svg)](https://badge.fury.io/py/unit_simple)
 
 * [Standard usage](#Utilisation-standard)
 * [Operator overloading usage](#Utilisation-avec-surcharge-des-opérateurs)
@@ -221,8 +210,8 @@
 ms = m / s
 kmh = km / h
 
 msToKmh = ms >> kmh
 
 msToKmh(100.) # 360
 (~msToKmh)(18.) # 5
-```
+```
```

### Comparing `unit_simple-1.0.8/pyproject.toml` & `unit_simple-1.0.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unit_simple"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="Samuel Andrés", email="samuel.andres@yahoo.fr" },
 ]
 description = "A simple measurement unit API to handle basic unit conversions."
 readme = "README.md"
+license = {file = "LICENSE.md"}
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 [tool.setuptools]
```

### Comparing `unit_simple-1.0.8/unit_simple.egg-info/PKG-INFO` & `unit_simple-1.0.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,43 @@
 Metadata-Version: 2.1
 Name: unit_simple
-Version: 1.0.8
+Version: 1.0.9
 Summary: A simple measurement unit API to handle basic unit conversions.
 Author-email: Samuel Andrés <samuel.andres@yahoo.fr>
+License: This is free and unencumbered software released into the public domain.
+        
+        Anyone is free to copy, modify, publish, use, compile, sell, or
+        distribute this software, either in source code form or as a compiled
+        binary, for any purpose, commercial or non-commercial, and by any
+        means.
+        
+        In jurisdictions that recognize copyright laws, the author or authors
+        of this software dedicate any and all copyright interest in the
+        software to the public domain. We make this dedication for the benefit
+        of the public at large and to the detriment of our heirs and
+        successors. We intend this dedication to be an overt act of
+        relinquishment in perpetuity of all present and future rights to this
+        software under copyright law.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+        EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+        MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+        IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
+        OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+        ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+        OTHER DEALINGS IN THE SOFTWARE.
+        
+        For more information, please refer to <https://unlicense.org>
+        
 Project-URL: Homepage, https://github.com/SamuelAndresPascal/cosmoloj-py
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 
 # Simple Unit (Python implementation)
 
 [![Anaconda-Server Badge](https://anaconda.org/cosmoloj/unit_simple/badges/version.svg)](https://anaconda.org/cosmoloj/unit_simple)
 [![PyPI repository Badge](https://badge.fury.io/py/unit_simple.svg)](https://badge.fury.io/py/unit_simple)
 
 * [Standard usage](#Utilisation-standard)
```

### Comparing `unit_simple-1.0.8/unit_simple.py` & `unit_simple-1.0.9/unit_simple.py`

 * *Files identical despite different names*

