# Comparing `tmp/excsv-0.1.2.tar.gz` & `tmp/excsv-0.1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excsv-0.1.2.tar", last modified: Fri Mar 15 22:57:24 2024, max compression
+gzip compressed data, was "excsv-0.1.3.1.tar", last modified: Tue Apr 23 22:12:25 2024, max compression
```

## Comparing `excsv-0.1.2.tar` & `excsv-0.1.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2024-03-15 22:57:24.269687 excsv-0.1.2/
--rw-r--r--   0 dan        (502) staff       (20)     2825 2024-03-15 22:57:24.269281 excsv-0.1.2/PKG-INFO
--rw-r--r--   0 dan        (502) staff       (20)     2296 2024-03-15 22:56:01.000000 excsv-0.1.2/README.md
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2024-03-15 22:57:24.267049 excsv-0.1.2/excsv/
--rw-r--r--   0 dan        (502) staff       (20)        0 2024-03-15 14:59:45.000000 excsv-0.1.2/excsv/__init__.py
--rw-r--r--   0 dan        (502) staff       (20)       59 2024-03-15 14:59:45.000000 excsv-0.1.2/excsv/__main__.py
--rwxr-xr-x   0 dan        (502) staff       (20)     6720 2024-03-15 22:55:03.000000 excsv-0.1.2/excsv/cli.py
-drwxr-xr-x   0 dan        (502) staff       (20)        0 2024-03-15 22:57:24.268871 excsv-0.1.2/excsv.egg-info/
--rw-r--r--   0 dan        (502) staff       (20)     2825 2024-03-15 22:57:24.000000 excsv-0.1.2/excsv.egg-info/PKG-INFO
--rw-r--r--   0 dan        (502) staff       (20)      243 2024-03-15 22:57:24.000000 excsv-0.1.2/excsv.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (502) staff       (20)        1 2024-03-15 22:57:24.000000 excsv-0.1.2/excsv.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (502) staff       (20)       59 2024-03-15 22:57:24.000000 excsv-0.1.2/excsv.egg-info/entry_points.txt
--rw-r--r--   0 dan        (502) staff       (20)       33 2024-03-15 22:57:24.000000 excsv-0.1.2/excsv.egg-info/requires.txt
--rw-r--r--   0 dan        (502) staff       (20)        6 2024-03-15 22:57:24.000000 excsv-0.1.2/excsv.egg-info/top_level.txt
--rw-r--r--   0 dan        (502) staff       (20)       38 2024-03-15 22:57:24.269805 excsv-0.1.2/setup.cfg
--rw-r--r--   0 dan        (502) staff       (20)     1130 2024-03-15 22:56:41.000000 excsv-0.1.2/setup.py
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2024-04-23 22:12:25.316672 excsv-0.1.3.1/
+-rw-r--r--   0 dan        (502) staff       (20)     4141 2024-04-23 22:12:25.316304 excsv-0.1.3.1/PKG-INFO
+-rw-r--r--   0 dan        (502) staff       (20)     3215 2024-03-19 22:32:52.000000 excsv-0.1.3.1/README.md
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2024-04-23 22:12:25.313065 excsv-0.1.3.1/excsv/
+-rw-r--r--   0 dan        (502) staff       (20)        0 2024-03-14 22:44:15.000000 excsv-0.1.3.1/excsv/__init__.py
+-rw-r--r--   0 dan        (502) staff       (20)       59 2024-03-14 22:41:59.000000 excsv-0.1.3.1/excsv/__main__.py
+-rwxr-xr-x   0 dan        (502) staff       (20)     9727 2024-03-19 22:32:52.000000 excsv-0.1.3.1/excsv/cli.py
+drwxr-xr-x   0 dan        (502) staff       (20)        0 2024-04-23 22:12:25.315336 excsv-0.1.3.1/excsv.egg-info/
+-rw-r--r--   0 dan        (502) staff       (20)     4141 2024-04-23 22:12:25.000000 excsv-0.1.3.1/excsv.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (502) staff       (20)      243 2024-04-23 22:12:25.000000 excsv-0.1.3.1/excsv.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (502) staff       (20)        1 2024-04-23 22:12:25.000000 excsv-0.1.3.1/excsv.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (502) staff       (20)       40 2024-04-23 22:12:25.000000 excsv-0.1.3.1/excsv.egg-info/entry_points.txt
+-rw-r--r--   0 dan        (502) staff       (20)      178 2024-04-23 22:12:25.000000 excsv-0.1.3.1/excsv.egg-info/requires.txt
+-rw-r--r--   0 dan        (502) staff       (20)        6 2024-04-23 22:12:25.000000 excsv-0.1.3.1/excsv.egg-info/top_level.txt
+-rw-r--r--   0 dan        (502) staff       (20)       38 2024-04-23 22:12:25.316748 excsv-0.1.3.1/setup.cfg
+-rw-r--r--   0 dan        (502) staff       (20)     1354 2024-04-23 22:11:47.000000 excsv-0.1.3.1/setup.py
```

### Comparing `excsv-0.1.2/PKG-INFO` & `excsv-0.1.3.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: excsv
-Version: 0.1.2
-Summary: A command-line utility for converting CSV files into Excel sheets.
-Home-page: https://github.com/dannguyen/excsv
-Author: Dan Nguyen
-License: Apache License, Version 2.0
-Project-URL: Issues, https://github.dannguyen/dannguyen/excsv/issues
-Project-URL: CI, https://github.com/dannguyen/excsv/actions
-Project-URL: Changelog, https://github.com/dannguyen/excsv/releases
-Platform: UNKNOWN
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-
 # excsv
 
 A command-line utility for converting CSV files into Excel sheets. 
 
 (Other utilities included)
 
 
@@ -28,28 +13,54 @@
 pip install excsv
 ```
 
 
 Basic usage:
 
 ```bash
-excsv mydata.csv > mysheet.xlsx
-
-# or if you dislike unix redirect operator
+# input file as argument, output file as -o
 excsv mydata.csv -o mysheet.xlsx
 
-# or full unix style
-cat mydata.csv | excsv > mysheet.xlsx
+
+cat mydata.csv | excsv -o mysheet.xlsx
 ```
 
 
 ## Notes and TODOS
 
+### 2024-03-19
+
+- consider switching openpyxl to xlswriter for creating excel files: https://xlsxwriter.readthedocs.io/working_with_memory.html
+    - use openpyxl for testing only
+
+
+
 ### 2024-03-15
 
+### Similar libraries
+
+- [deztec/csv2excel](https://github.com/deztec/csv2excel): 
+
+    > .NET command line tool to convert delimited files to Microsoft Excel format (xls/xlsx) without Microsoft Excel having to be installed.
+
+    `$ csv2excel.exe -i input.csv`
+
+- [mentax/csv2xlsx](https://github.com/mentax/csv2xlsx):
+    ~~~sh
+    $ csv2xlsx --template example/template.xlsx \
+        --sheet Sheet_1 --sheet Sheet_2 \
+        --row 2 \
+        --output result.xlsx data.csv data2.csv`
+    ~~~
+
+### TODOS 2024-03-15
+
+- Use write_only mode for faster performance: https://openpyxl.readthedocs.io/en/latest/optimized.html
+>>>>>>> 9a8c8b5 (f)
+
 - Rudimentary functionality as I decide whether or not to implement features that are already done best in xsv and csvkit.
 
 - Change focus to tools/functions that are most needed when populating a spreadsheet, such as removing bad characters/control characters, unintended excess whitespace, renaming headers, etc.
 
 Things to add:
 - `excel` option flags to configure frozen header, filters (yes/no), font formatting, and setting every field to the width of its longest values
     - let user name sheet name
@@ -70,14 +81,18 @@
     - clean up header names, strip whitespace from headers/values, etc.
     - allow user to specify when data starts and ends (i.e. to ignore first/final few rows of metadata)
 
 - `head/tail`:
     - quickly inspect the first/last few rows
 
 
+- `probe`:
+    - add min, max, most common value, longest value (chars)
+    - detect file size, if large, use count-min-sketch and hyperloglog
+
 
 ## Dev and Testing
 
 
 ```sh
 # install locally
 $ pip install -e .
@@ -91,9 +106,7 @@
 
 
 # skip alpha tests
 $ pytest -m 'not alpha'
 ```
 
 
-
-
```

### Comparing `excsv-0.1.2/setup.py` & `excsv-0.1.3.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.1.2"
+VERSION = "0.1.3.1"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
@@ -27,12 +27,27 @@
     license="Apache License, Version 2.0",
     version=VERSION,
     packages=["excsv"],
     entry_points="""
         [console_scripts]
         excsv=excsv.cli:cli
     """,
-    install_requires=["click"],
-    #    extras_require={"test": ["pytest", "pytest-icdiff", "cogapp", "PyYAML", "ruff"]},
-    extras_require={"test": ["pytest", "pytest-mock"]},
+    install_requires=[
+        "click>=8.1",
+        "hyperloglog",
+        "rich_click",
+        "openpyxl",
+        "click-default-group>=1.2.3",
+        "setuptools",
+        "pip",
+        "pyreadline3; sys_platform == 'win32'",
+    ],
+    extras_require={
+        "test": [
+            "pytest",
+            "pytest-mock",
+            "black>=24.2.0",
+            "types-click",
+        ]
+    },
     python_requires=">=3.8",
 )
```

