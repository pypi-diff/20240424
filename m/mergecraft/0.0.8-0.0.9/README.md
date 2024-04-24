# Comparing `tmp/mergecraft-0.0.8.tar.gz` & `tmp/mergecraft-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mergecraft-0.0.8.tar", last modified: Wed Apr 24 10:27:17 2024, max compression
+gzip compressed data, was "mergecraft-0.0.9.tar", last modified: Wed Apr 24 10:34:07 2024, max compression
```

## Comparing `mergecraft-0.0.8.tar` & `mergecraft-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:27:17.528295 mergecraft-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-24 10:27:04.000000 mergecraft-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-24 10:27:17.528295 mergecraft-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-24 10:27:04.000000 mergecraft-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:27:17.528295 mergecraft-0.0.8/mergecraft/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:27:04.000000 mergecraft-0.0.8/mergecraft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-24 10:27:04.000000 mergecraft-0.0.8/mergecraft/mergecraft.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:27:17.528295 mergecraft-0.0.8/mergecraft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-24 10:27:17.000000 mergecraft-0.0.8/mergecraft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-24 10:27:17.000000 mergecraft-0.0.8/mergecraft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:27:17.000000 mergecraft-0.0.8/mergecraft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 10:27:17.000000 mergecraft-0.0.8/mergecraft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 10:27:17.000000 mergecraft-0.0.8/mergecraft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 10:27:17.000000 mergecraft-0.0.8/mergecraft.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 10:27:17.528295 mergecraft-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-24 10:27:04.000000 mergecraft-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:34:07.042873 mergecraft-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-24 10:33:55.000000 mergecraft-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-24 10:34:07.042873 mergecraft-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-24 10:33:55.000000 mergecraft-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:34:07.042873 mergecraft-0.0.9/mergecraft/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:55.000000 mergecraft-0.0.9/mergecraft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-24 10:33:55.000000 mergecraft-0.0.9/mergecraft/mergecraft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:34:07.042873 mergecraft-0.0.9/mergecraft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-24 10:34:07.000000 mergecraft-0.0.9/mergecraft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-24 10:34:07.000000 mergecraft-0.0.9/mergecraft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:34:07.000000 mergecraft-0.0.9/mergecraft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 10:34:07.000000 mergecraft-0.0.9/mergecraft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 10:34:07.000000 mergecraft-0.0.9/mergecraft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 10:34:07.000000 mergecraft-0.0.9/mergecraft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 10:34:07.042873 mergecraft-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-24 10:33:55.000000 mergecraft-0.0.9/setup.py
```

### Comparing `mergecraft-0.0.8/LICENSE` & `mergecraft-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mergecraft-0.0.8/PKG-INFO` & `mergecraft-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mergecraft
-Version: 0.0.8
+Version: 0.0.9
 Summary: A command-line tool to merge files into a temporary file and open in VS Code. Designed to support AI-driven development.
 Home-page: https://github.com/josenerydev/mergecraft
 Author: José Nery
 Author-email: josenerydev@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pathspec
+Requires-Dist: PyYAML
 
 # mergecraft 🚀
 
 [![Upload Python Package](https://github.com/josenerydev/mergecraft/actions/workflows/python-publish.yml/badge.svg)](https://github.com/josenerydev/mergecraft/actions/workflows/python-publish.yml)
 ![GitHub](https://img.shields.io/github/license/josenerydev/mergecraft)
 ![PyPI](https://img.shields.io/pypi/v/mergecraft)
 ![Python Version](https://img.shields.io/pypi/pyversions/mergecraft)
```

### Comparing `mergecraft-0.0.8/README.md` & `mergecraft-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mergecraft-0.0.8/mergecraft/mergecraft.py` & `mergecraft-0.0.9/mergecraft/mergecraft.py`

 * *Files identical despite different names*

### Comparing `mergecraft-0.0.8/mergecraft.egg-info/PKG-INFO` & `mergecraft-0.0.9/mergecraft.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mergecraft
-Version: 0.0.8
+Version: 0.0.9
 Summary: A command-line tool to merge files into a temporary file and open in VS Code. Designed to support AI-driven development.
 Home-page: https://github.com/josenerydev/mergecraft
 Author: José Nery
 Author-email: josenerydev@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pathspec
+Requires-Dist: PyYAML
 
 # mergecraft 🚀
 
 [![Upload Python Package](https://github.com/josenerydev/mergecraft/actions/workflows/python-publish.yml/badge.svg)](https://github.com/josenerydev/mergecraft/actions/workflows/python-publish.yml)
 ![GitHub](https://img.shields.io/github/license/josenerydev/mergecraft)
 ![PyPI](https://img.shields.io/pypi/v/mergecraft)
 ![Python Version](https://img.shields.io/pypi/pyversions/mergecraft)
```

### Comparing `mergecraft-0.0.8/setup.py` & `mergecraft-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mergecraft",
-    version="0.0.8",
+    version="0.0.9",
     description="A command-line tool to merge files into a temporary file and open in VS Code. Designed to support AI-driven development.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="José Nery",
     author_email="josenerydev@gmail.com",
     url="https://github.com/josenerydev/mergecraft",
     packages=find_packages(),
-    install_requires=["pathspec"],
+    install_requires=["pathspec","PyYAML"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
```

