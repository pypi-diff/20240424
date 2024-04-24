# Comparing `tmp/mergecraft-0.0.4.tar.gz` & `tmp/mergecraft-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mergecraft-0.0.4.tar", last modified: Wed Apr 24 10:00:54 2024, max compression
+gzip compressed data, was "mergecraft-0.0.5.tar", last modified: Wed Apr 24 10:06:15 2024, max compression
```

## Comparing `mergecraft-0.0.4.tar` & `mergecraft-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:00:54.239794 mergecraft-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-24 10:00:43.000000 mergecraft-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-24 10:00:54.239794 mergecraft-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-24 10:00:43.000000 mergecraft-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:00:54.235794 mergecraft-0.0.4/mergecraft/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:00:43.000000 mergecraft-0.0.4/mergecraft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-24 10:00:43.000000 mergecraft-0.0.4/mergecraft/mergecraft.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:00:54.235794 mergecraft-0.0.4/mergecraft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-24 10:00:54.000000 mergecraft-0.0.4/mergecraft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-24 10:00:54.000000 mergecraft-0.0.4/mergecraft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:00:54.000000 mergecraft-0.0.4/mergecraft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 10:00:54.000000 mergecraft-0.0.4/mergecraft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 10:00:54.000000 mergecraft-0.0.4/mergecraft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 10:00:54.000000 mergecraft-0.0.4/mergecraft.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 10:00:54.239794 mergecraft-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-24 10:00:43.000000 mergecraft-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:06:15.279684 mergecraft-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-24 10:06:03.000000 mergecraft-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-24 10:06:15.279684 mergecraft-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-24 10:06:03.000000 mergecraft-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:06:15.279684 mergecraft-0.0.5/mergecraft/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:06:03.000000 mergecraft-0.0.5/mergecraft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-24 10:06:03.000000 mergecraft-0.0.5/mergecraft/mergecraft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:06:15.279684 mergecraft-0.0.5/mergecraft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-24 10:06:15.000000 mergecraft-0.0.5/mergecraft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-24 10:06:15.000000 mergecraft-0.0.5/mergecraft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:06:15.000000 mergecraft-0.0.5/mergecraft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 10:06:15.000000 mergecraft-0.0.5/mergecraft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 10:06:15.000000 mergecraft-0.0.5/mergecraft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 10:06:15.000000 mergecraft-0.0.5/mergecraft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 10:06:15.279684 mergecraft-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-24 10:06:03.000000 mergecraft-0.0.5/setup.py
```

### Comparing `mergecraft-0.0.4/LICENSE` & `mergecraft-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mergecraft-0.0.4/PKG-INFO` & `mergecraft-0.0.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mergecraft
-Version: 0.0.4
-Summary: A command-line tool to merge files into a temporary file and open in VS Code.
+Version: 0.0.5
+Summary: A command-line tool to merge files into a temporary file and open in VS Code. Designed to support AI-driven development.
 Home-page: https://github.com/josenerydev/mergecraft
 Author: José Nery
 Author-email: josenerydev@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pathspec
 
 # mergecraft 🚀
 
+[![Upload Python Package](https://github.com/josenerydev/mergecraft/actions/workflows/python-publish.yml/badge.svg)](https://github.com/josenerydev/mergecraft/actions/workflows/python-publish.yml)
 ![GitHub](https://img.shields.io/github/license/josenerydev/mergecraft)
 ![PyPI](https://img.shields.io/pypi/v/mergecraft)
 ![Python Version](https://img.shields.io/pypi/pyversions/mergecraft)
 
 `mergecraft` is a command-line tool engineered to assist development teams by merging files into a single temporary file and then opening it in Visual Studio Code. This tool is particularly useful in AI-driven development environments, where understanding the broader context of code changes is crucial.
 
 ## 🌟 Introduction to AI-Driven Development with mergecraft
```

### Comparing `mergecraft-0.0.4/README.md` & `mergecraft-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # mergecraft 🚀
 
+[![Upload Python Package](https://github.com/josenerydev/mergecraft/actions/workflows/python-publish.yml/badge.svg)](https://github.com/josenerydev/mergecraft/actions/workflows/python-publish.yml)
 ![GitHub](https://img.shields.io/github/license/josenerydev/mergecraft)
 ![PyPI](https://img.shields.io/pypi/v/mergecraft)
 ![Python Version](https://img.shields.io/pypi/pyversions/mergecraft)
 
 `mergecraft` is a command-line tool engineered to assist development teams by merging files into a single temporary file and then opening it in Visual Studio Code. This tool is particularly useful in AI-driven development environments, where understanding the broader context of code changes is crucial.
 
 ## 🌟 Introduction to AI-Driven Development with mergecraft
@@ -86,8 +87,8 @@
 
 ## 🎯 AI in Development: The Role of mergecraft
 
 `mergecraft` supports AI-driven development by automating routine tasks like file merging, aiding in documentation, and streamlining code reviews. It helps bridge the gap between developers' needs for consistency and the requirements of fast-paced technology environments, making it an indispensable tool for modern development teams.
 
 ## 📜 License
 
-`mergecraft` is released under the MIT License. See the LICENSE file for more details.
+`mergecraft` is released under the MIT License. See the LICENSE file for more details.
```

### Comparing `mergecraft-0.0.4/mergecraft/mergecraft.py` & `mergecraft-0.0.5/mergecraft/mergecraft.py`

 * *Files identical despite different names*

### Comparing `mergecraft-0.0.4/mergecraft.egg-info/PKG-INFO` & `mergecraft-0.0.5/mergecraft.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mergecraft
-Version: 0.0.4
-Summary: A command-line tool to merge files into a temporary file and open in VS Code.
+Version: 0.0.5
+Summary: A command-line tool to merge files into a temporary file and open in VS Code. Designed to support AI-driven development.
 Home-page: https://github.com/josenerydev/mergecraft
 Author: José Nery
 Author-email: josenerydev@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pathspec
 
 # mergecraft 🚀
 
+[![Upload Python Package](https://github.com/josenerydev/mergecraft/actions/workflows/python-publish.yml/badge.svg)](https://github.com/josenerydev/mergecraft/actions/workflows/python-publish.yml)
 ![GitHub](https://img.shields.io/github/license/josenerydev/mergecraft)
 ![PyPI](https://img.shields.io/pypi/v/mergecraft)
 ![Python Version](https://img.shields.io/pypi/pyversions/mergecraft)
 
 `mergecraft` is a command-line tool engineered to assist development teams by merging files into a single temporary file and then opening it in Visual Studio Code. This tool is particularly useful in AI-driven development environments, where understanding the broader context of code changes is crucial.
 
 ## 🌟 Introduction to AI-Driven Development with mergecraft
```

### Comparing `mergecraft-0.0.4/setup.py` & `mergecraft-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mergecraft",
-    version="0.0.4",
-    description="A command-line tool to merge files into a temporary file and open in VS Code.",
+    version="0.0.5",
+    description="A command-line tool to merge files into a temporary file and open in VS Code. Designed to support AI-driven development.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="José Nery",
     author_email="josenerydev@gmail.com",
     url="https://github.com/josenerydev/mergecraft",
     packages=find_packages(),
     install_requires=["pathspec"],
```

