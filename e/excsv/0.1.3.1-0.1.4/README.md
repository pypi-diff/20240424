# Comparing `tmp/excsv-0.1.3.1.tar.gz` & `tmp/excsv-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excsv-0.1.3.1.tar", last modified: Tue Apr 23 22:12:25 2024, max compression
+gzip compressed data, was "excsv-0.1.4.tar", last modified: Tue Apr 23 22:29:32 2024, max compression
```

## Comparing `excsv-0.1.3.1.tar` & `excsv-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2024-04-23 22:12:25.316672 excsv-0.1.3.1/
--rw-r--r--   0 dan        (502) staff       (20)     4141 2024-04-23 22:12:25.316304 excsv-0.1.3.1/PKG-INFO
--rw-r--r--   0 dan        (502) staff       (20)     3215 2024-03-19 22:32:52.000000 excsv-0.1.3.1/README.md
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2024-04-23 22:12:25.313065 excsv-0.1.3.1/excsv/
--rw-r--r--   0 dan        (502) staff       (20)        0 2024-03-14 22:44:15.000000 excsv-0.1.3.1/excsv/__init__.py
--rw-r--r--   0 dan        (502) staff       (20)       59 2024-03-14 22:41:59.000000 excsv-0.1.3.1/excsv/__main__.py
--rwxr-xr-x   0 dan        (502) staff       (20)     9727 2024-03-19 22:32:52.000000 excsv-0.1.3.1/excsv/cli.py
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2024-04-23 22:12:25.315336 excsv-0.1.3.1/excsv.egg-info/
--rw-r--r--   0 dan        (502) staff       (20)     4141 2024-04-23 22:12:25.000000 excsv-0.1.3.1/excsv.egg-info/PKG-INFO
--rw-r--r--   0 dan        (502) staff       (20)      243 2024-04-23 22:12:25.000000 excsv-0.1.3.1/excsv.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (502) staff       (20)        1 2024-04-23 22:12:25.000000 excsv-0.1.3.1/excsv.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (502) staff       (20)       40 2024-04-23 22:12:25.000000 excsv-0.1.3.1/excsv.egg-info/entry_points.txt
--rw-r--r--   0 dan        (502) staff       (20)      178 2024-04-23 22:12:25.000000 excsv-0.1.3.1/excsv.egg-info/requires.txt
--rw-r--r--   0 dan        (502) staff       (20)        6 2024-04-23 22:12:25.000000 excsv-0.1.3.1/excsv.egg-info/top_level.txt
--rw-r--r--   0 dan        (502) staff       (20)       38 2024-04-23 22:12:25.316748 excsv-0.1.3.1/setup.cfg
--rw-r--r--   0 dan        (502) staff       (20)     1354 2024-04-23 22:11:47.000000 excsv-0.1.3.1/setup.py
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2024-04-23 22:29:32.860763 excsv-0.1.4/
+-rw-r--r--   0 dan        (502) staff       (20)     4139 2024-04-23 22:29:32.860141 excsv-0.1.4/PKG-INFO
+-rw-r--r--   0 dan        (502) staff       (20)     3215 2024-04-23 22:27:20.000000 excsv-0.1.4/README.md
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2024-04-23 22:29:32.853487 excsv-0.1.4/excsv/
+-rw-r--r--   0 dan        (502) staff       (20)        0 2024-03-14 22:44:15.000000 excsv-0.1.4/excsv/__init__.py
+-rwxr-xr-x   0 dan        (502) staff       (20)     9727 2024-04-23 22:27:20.000000 excsv-0.1.4/excsv/cli.py
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2024-04-23 22:29:32.858184 excsv-0.1.4/excsv/utils/
+-rw-r--r--   0 dan        (502) staff       (20)        0 2024-04-23 22:28:36.000000 excsv-0.1.4/excsv/utils/__init__.py
+-rw-r--r--   0 dan        (502) staff       (20)     1040 2024-04-23 22:27:20.000000 excsv-0.1.4/excsv/utils/excel.py
+-rw-r--r--   0 dan        (502) staff       (20)     1568 2024-03-15 23:29:59.000000 excsv-0.1.4/excsv/utils/infer.py
+-rw-r--r--   0 dan        (502) staff       (20)      669 2024-04-23 22:27:20.000000 excsv-0.1.4/excsv/utils/listing.py
+-rw-r--r--   0 dan        (502) staff       (20)      298 2024-03-15 23:29:59.000000 excsv-0.1.4/excsv/utils/text.py
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2024-04-23 22:29:32.859183 excsv-0.1.4/excsv.egg-info/
+-rw-r--r--   0 dan        (502) staff       (20)     4139 2024-04-23 22:29:32.000000 excsv-0.1.4/excsv.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (502) staff       (20)      334 2024-04-23 22:29:32.000000 excsv-0.1.4/excsv.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (502) staff       (20)        1 2024-04-23 22:29:32.000000 excsv-0.1.4/excsv.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (502) staff       (20)       40 2024-04-23 22:29:32.000000 excsv-0.1.4/excsv.egg-info/entry_points.txt
+-rw-r--r--   0 dan        (502) staff       (20)      178 2024-04-23 22:29:32.000000 excsv-0.1.4/excsv.egg-info/requires.txt
+-rw-r--r--   0 dan        (502) staff       (20)        6 2024-04-23 22:29:32.000000 excsv-0.1.4/excsv.egg-info/top_level.txt
+-rw-r--r--   0 dan        (502) staff       (20)       38 2024-04-23 22:29:32.860853 excsv-0.1.4/setup.cfg
+-rw-r--r--   0 dan        (502) staff       (20)     1401 2024-04-23 22:28:36.000000 excsv-0.1.4/setup.py
```

### Comparing `excsv-0.1.3.1/PKG-INFO` & `excsv-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excsv
-Version: 0.1.3.1
+Version: 0.1.4
 Summary: A command-line utility for converting CSV files into Excel sheets.
 Home-page: https://github.com/dannguyen/excsv
 Author: Dan Nguyen
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.dannguyen/dannguyen/excsv/issues
 Project-URL: CI, https://github.com/dannguyen/excsv/actions
 Project-URL: Changelog, https://github.com/dannguyen/excsv/releases
```

### Comparing `excsv-0.1.3.1/README.md` & `excsv-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `excsv-0.1.3.1/excsv/cli.py` & `excsv-0.1.4/excsv/cli.py`

 * *Files identical despite different names*

### Comparing `excsv-0.1.3.1/excsv.egg-info/PKG-INFO` & `excsv-0.1.4/excsv.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excsv
-Version: 0.1.3.1
+Version: 0.1.4
 Summary: A command-line utility for converting CSV files into Excel sheets.
 Home-page: https://github.com/dannguyen/excsv
 Author: Dan Nguyen
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.dannguyen/dannguyen/excsv/issues
 Project-URL: CI, https://github.com/dannguyen/excsv/actions
 Project-URL: Changelog, https://github.com/dannguyen/excsv/releases
```

### Comparing `excsv-0.1.3.1/setup.py` & `excsv-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 import os
 
-VERSION = "0.1.3.1"
+VERSION = "0.1.4"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
@@ -22,15 +22,15 @@
     project_urls={
         "Issues": "https://github.dannguyen/dannguyen/excsv/issues",
         "CI": "https://github.com/dannguyen/excsv/actions",
         "Changelog": "https://github.com/dannguyen/excsv/releases",
     },
     license="Apache License, Version 2.0",
     version=VERSION,
-    packages=["excsv"],
+    packages=find_packages(exclude=["tests", "tests.*"]),
     entry_points="""
         [console_scripts]
         excsv=excsv.cli:cli
     """,
     install_requires=[
         "click>=8.1",
         "hyperloglog",
```

