# Comparing `tmp/facehuggershield-0.1.0.tar.gz` & `tmp/facehuggershield-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facehuggershield-0.1.0.tar", last modified: Wed Apr 24 00:56:11 2024, max compression
+gzip compressed data, was "facehuggershield-0.1.1.tar", last modified: Wed Apr 24 02:15:48 2024, max compression
```

## Comparing `facehuggershield-0.1.0.tar` & `facehuggershield-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:56:11.453901 facehuggershield-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 00:55:56.000000 facehuggershield-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-24 00:56:11.453901 facehuggershield-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-24 00:55:56.000000 facehuggershield-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 00:56:11.453901 facehuggershield-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-24 00:55:56.000000 facehuggershield-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:56:11.453901 facehuggershield-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:56:11.453901 facehuggershield-0.1.0/src/facehuggershield.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-24 00:56:11.000000 facehuggershield-0.1.0/src/facehuggershield.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-24 00:56:11.000000 facehuggershield-0.1.0/src/facehuggershield.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 00:56:11.000000 facehuggershield-0.1.0/src/facehuggershield.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 00:56:11.000000 facehuggershield-0.1.0/src/facehuggershield.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:15:48.957569 facehuggershield-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 02:15:45.000000 facehuggershield-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-24 02:15:48.957569 facehuggershield-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-24 02:15:45.000000 facehuggershield-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 02:15:48.957569 facehuggershield-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-24 02:15:45.000000 facehuggershield-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:15:48.957569 facehuggershield-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:15:48.957569 facehuggershield-0.1.1/src/facehuggershield.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-24 02:15:48.000000 facehuggershield-0.1.1/src/facehuggershield.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-24 02:15:48.000000 facehuggershield-0.1.1/src/facehuggershield.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:15:48.000000 facehuggershield-0.1.1/src/facehuggershield.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-24 02:15:48.000000 facehuggershield-0.1.1/src/facehuggershield.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:15:48.000000 facehuggershield-0.1.1/src/facehuggershield.egg-info/top_level.txt
```

### Comparing `facehuggershield-0.1.0/LICENSE` & `facehuggershield-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `facehuggershield-0.1.0/PKG-INFO` & `facehuggershield-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: facehuggershield
-Version: 0.1.0
+Version: 0.1.1
 Home-page: https://github.com/Capsize-Games/facehuggershield
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: defendatron==0.1.0
 
 # Facehugger Shield
 
-
-![img.png](img.png)
-
-
 Facehugger Shield automatically locks down operations
 for specific modules. It was designed to non-destructively restrict access
 to the Huggingface library, but can be used with any library.
 
 ---
 
+![img.png](img.png)
+
+[![Upload Python Package](https://github.com/Capsize-Games/facehuggershield/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Capsize-Games/facehuggershield/actions/workflows/python-publish.yml)
+
+---
+
 ## Usage
 
 Facehugger Shield was specifically designed to override Huggingface libraries, so the following examples show how to do that.
 
 
 Install with Huggingface libraries (or any other library you want to restrict).
```

### Comparing `facehuggershield-0.1.0/README.md` & `facehuggershield-0.1.1/src/facehuggershield.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,33 @@
-# Facehugger Shield
-
-
-![img.png](img.png)
+Metadata-Version: 2.1
+Name: facehuggershield
+Version: 0.1.1
+Home-page: https://github.com/Capsize-Games/facehuggershield
+Author: Capsize LLC
+Author-email: contact@capsizegames.com
+License: GPL-3.0
+Requires-Python: >=3.10.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: defendatron==0.1.0
 
+# Facehugger Shield
 
 Facehugger Shield automatically locks down operations
 for specific modules. It was designed to non-destructively restrict access
 to the Huggingface library, but can be used with any library.
 
 ---
 
+![img.png](img.png)
+
+[![Upload Python Package](https://github.com/Capsize-Games/facehuggershield/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Capsize-Games/facehuggershield/actions/workflows/python-publish.yml)
+
+---
+
 ## Usage
 
 Facehugger Shield was specifically designed to override Huggingface libraries, so the following examples show how to do that.
 
 
 Install with Huggingface libraries (or any other library you want to restrict).
```

### Comparing `facehuggershield-0.1.0/setup.py` & `facehuggershield-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name="facehuggershield",
-    version="0.1.0",
+    version="0.1.1",
     author="Capsize LLC",
     description="",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="",
     license="GPL-3.0",
     author_email="contact@capsizegames.com",
     url="https://github.com/Capsize-Games/facehuggershield",
     package_dir={"": "src"},
     packages=find_packages("src"),
     python_requires=">=3.10.0",
     install_requires=[
+        "defendatron==0.1.0",
     ],
     dependency_links=[
-        "defendron==0.1.0",
     ],
 )
```

### Comparing `facehuggershield-0.1.0/src/facehuggershield.egg-info/PKG-INFO` & `facehuggershield-0.1.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,21 @@
-Metadata-Version: 2.1
-Name: facehuggershield
-Version: 0.1.0
-Home-page: https://github.com/Capsize-Games/facehuggershield
-Author: Capsize LLC
-Author-email: contact@capsizegames.com
-License: GPL-3.0
-Requires-Python: >=3.10.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Facehugger Shield
 
-
-![img.png](img.png)
-
-
 Facehugger Shield automatically locks down operations
 for specific modules. It was designed to non-destructively restrict access
 to the Huggingface library, but can be used with any library.
 
 ---
 
+![img.png](img.png)
+
+[![Upload Python Package](https://github.com/Capsize-Games/facehuggershield/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Capsize-Games/facehuggershield/actions/workflows/python-publish.yml)
+
+---
+
 ## Usage
 
 Facehugger Shield was specifically designed to override Huggingface libraries, so the following examples show how to do that.
 
 
 Install with Huggingface libraries (or any other library you want to restrict).
```

