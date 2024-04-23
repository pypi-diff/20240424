# Comparing `tmp/gravithon-0.0.8.tar.gz` & `tmp/gravithon-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravithon-0.0.8.tar", last modified: Sun Apr 21 21:31:29 2024, max compression
+gzip compressed data, was "gravithon-0.0.9.tar", last modified: Tue Apr 23 23:05:44 2024, max compression
```

## Comparing `gravithon-0.0.8.tar` & `gravithon-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 yehuda    (1000) yehuda    (1000)        0 2024-04-21 21:31:29.098492 gravithon-0.0.8/
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)     1071 2024-03-22 09:00:56.000000 gravithon-0.0.8/LICENSE
--rw-r--r--   0 yehuda    (1000) yehuda    (1000)     1006 2024-04-21 21:31:29.098492 gravithon-0.0.8/PKG-INFO
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      370 2024-04-21 21:31:07.000000 gravithon-0.0.8/README.md
-drwxrwxr-x   0 yehuda    (1000) yehuda    (1000)        0 2024-04-21 21:31:29.098492 gravithon-0.0.8/gravithon.egg-info/
--rw-r--r--   0 yehuda    (1000) yehuda    (1000)     1006 2024-04-21 21:31:29.000000 gravithon-0.0.8/gravithon.egg-info/PKG-INFO
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      210 2024-04-21 21:31:29.000000 gravithon-0.0.8/gravithon.egg-info/SOURCES.txt
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)        1 2024-04-21 21:31:29.000000 gravithon-0.0.8/gravithon.egg-info/dependency_links.txt
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)       38 2024-04-21 21:31:29.000000 gravithon-0.0.8/gravithon.egg-info/requires.txt
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)        1 2024-04-21 21:31:29.000000 gravithon-0.0.8/gravithon.egg-info/top_level.txt
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      865 2024-04-21 21:31:23.000000 gravithon-0.0.8/pyproject.toml
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)       38 2024-04-21 21:31:29.098492 gravithon-0.0.8/setup.cfg
-drwxrwxr-x   0 yehuda    (1000) yehuda    (1000)        0 2024-04-21 21:31:29.098492 gravithon-0.0.8/tests/
--rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      131 2024-03-29 13:24:59.000000 gravithon-0.0.8/tests/test.py
+drwxrwxr-x   0 yehuda    (1000) yehuda    (1000)        0 2024-04-23 23:05:44.838573 gravithon-0.0.9/
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)     1071 2024-03-22 09:00:56.000000 gravithon-0.0.9/LICENSE
+-rw-r--r--   0 yehuda    (1000) yehuda    (1000)     1007 2024-04-23 23:05:44.838573 gravithon-0.0.9/PKG-INFO
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      370 2024-04-21 21:31:07.000000 gravithon-0.0.9/README.md
+drwxrwxr-x   0 yehuda    (1000) yehuda    (1000)        0 2024-04-23 23:05:44.838573 gravithon-0.0.9/gravithon.egg-info/
+-rw-r--r--   0 yehuda    (1000) yehuda    (1000)     1007 2024-04-23 23:05:44.000000 gravithon-0.0.9/gravithon.egg-info/PKG-INFO
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      210 2024-04-23 23:05:44.000000 gravithon-0.0.9/gravithon.egg-info/SOURCES.txt
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)        1 2024-04-23 23:05:44.000000 gravithon-0.0.9/gravithon.egg-info/dependency_links.txt
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)       39 2024-04-23 23:05:44.000000 gravithon-0.0.9/gravithon.egg-info/requires.txt
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)        1 2024-04-23 23:05:44.000000 gravithon-0.0.9/gravithon.egg-info/top_level.txt
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      866 2024-04-23 23:05:34.000000 gravithon-0.0.9/pyproject.toml
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)       38 2024-04-23 23:05:44.838573 gravithon-0.0.9/setup.cfg
+drwxrwxr-x   0 yehuda    (1000) yehuda    (1000)        0 2024-04-23 23:05:44.838573 gravithon-0.0.9/tests/
+-rw-rw-r--   0 yehuda    (1000) yehuda    (1000)      131 2024-03-29 13:24:59.000000 gravithon-0.0.9/tests/test.py
```

### Comparing `gravithon-0.0.8/LICENSE` & `gravithon-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gravithon-0.0.8/PKG-INFO` & `gravithon-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gravithon
-Version: 0.0.8
+Version: 0.0.9
 Summary: Create multy-dimensional python spaces
 Author-email: Yehuda Elyasaf <30yehuda26@gmail.com>
 Maintainer-email: Yehuda Elyasaf <30yehuda26@gmail.com>
 Project-URL: Homepage, https://github.com/YehudaElyasaf/gravithon
 Project-URL: Issues, https://github.com/YehudaElyasaf/gravithon/issues
 Keywords: physics,2d,3d,engine
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: multipledispatch
-Requires-Dist: tkinter
 Requires-Dist: Pillow
+Requires-Dist: datetime
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-C06524)](https://github.com/YehudaElyasaf/gravithon/blob/master/LICENSE)
 [![PyPI - Version](https://img.shields.io/pypi/v/gravithon.svg)](https://pypi.org/project/gravithon/)
 
 <img src="https://github.com/YehudaElyasaf/gravithon/blob/master/logo/logo.png?raw=True" alt="Logo" width="300">
 
 <!--
```

### Comparing `gravithon-0.0.8/gravithon.egg-info/PKG-INFO` & `gravithon-0.0.9/gravithon.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gravithon
-Version: 0.0.8
+Version: 0.0.9
 Summary: Create multy-dimensional python spaces
 Author-email: Yehuda Elyasaf <30yehuda26@gmail.com>
 Maintainer-email: Yehuda Elyasaf <30yehuda26@gmail.com>
 Project-URL: Homepage, https://github.com/YehudaElyasaf/gravithon
 Project-URL: Issues, https://github.com/YehudaElyasaf/gravithon/issues
 Keywords: physics,2d,3d,engine
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: multipledispatch
-Requires-Dist: tkinter
 Requires-Dist: Pillow
+Requires-Dist: datetime
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-C06524)](https://github.com/YehudaElyasaf/gravithon/blob/master/LICENSE)
 [![PyPI - Version](https://img.shields.io/pypi/v/gravithon.svg)](https://pypi.org/project/gravithon/)
 
 <img src="https://github.com/YehudaElyasaf/gravithon/blob/master/logo/logo.png?raw=True" alt="Logo" width="300">
 
 <!--
```

### Comparing `gravithon-0.0.8/pyproject.toml` & `gravithon-0.0.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 package-data = { "sample" = ["*.dat"] }
 py-modules = []
 
 
 [project]
 name = 'gravithon'
 keywords = ['physics', '2d', '3d', 'engine'] #TODO
-version = '0.0.8'
+version = '0.0.9'
 description = 'Create multy-dimensional python spaces' #TODO
 readme = 'README.md'
 
 dependencies = [
     'numpy',
     'multipledispatch',
-    'tkinter',
-    'Pillow'
+    'Pillow',
+    'datetime'
 ]
 
 authors = [
     { name = 'Yehuda Elyasaf', email = '30yehuda26@gmail.com' },
 ]
 maintainers = [
     { name = 'Yehuda Elyasaf', email = '30yehuda26@gmail.com' },
```

