# Comparing `tmp/facehuggershield-0.1.1.tar.gz` & `tmp/facehuggershield-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facehuggershield-0.1.1.tar", last modified: Wed Apr 24 02:15:48 2024, max compression
+gzip compressed data, was "facehuggershield-0.1.2.tar", last modified: Wed Apr 24 02:21:08 2024, max compression
```

## Comparing `facehuggershield-0.1.1.tar` & `facehuggershield-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:15:48.957569 facehuggershield-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 02:15:45.000000 facehuggershield-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-24 02:15:48.957569 facehuggershield-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-24 02:15:45.000000 facehuggershield-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 02:15:48.957569 facehuggershield-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-24 02:15:45.000000 facehuggershield-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:15:48.957569 facehuggershield-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:15:48.957569 facehuggershield-0.1.1/src/facehuggershield.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-24 02:15:48.000000 facehuggershield-0.1.1/src/facehuggershield.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-24 02:15:48.000000 facehuggershield-0.1.1/src/facehuggershield.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:15:48.000000 facehuggershield-0.1.1/src/facehuggershield.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-24 02:15:48.000000 facehuggershield-0.1.1/src/facehuggershield.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:15:48.000000 facehuggershield-0.1.1/src/facehuggershield.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:21:08.936569 facehuggershield-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 02:21:00.000000 facehuggershield-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-24 02:21:08.936569 facehuggershield-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-24 02:21:00.000000 facehuggershield-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 02:21:08.936569 facehuggershield-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-24 02:21:00.000000 facehuggershield-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:21:08.932569 facehuggershield-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:21:08.932569 facehuggershield-0.1.2/src/facehuggershield.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-24 02:21:08.000000 facehuggershield-0.1.2/src/facehuggershield.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-24 02:21:08.000000 facehuggershield-0.1.2/src/facehuggershield.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:21:08.000000 facehuggershield-0.1.2/src/facehuggershield.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-24 02:21:08.000000 facehuggershield-0.1.2/src/facehuggershield.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:21:08.000000 facehuggershield-0.1.2/src/facehuggershield.egg-info/top_level.txt
```

### Comparing `facehuggershield-0.1.1/LICENSE` & `facehuggershield-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `facehuggershield-0.1.1/PKG-INFO` & `facehuggershield-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: facehuggershield
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/Capsize-Games/facehuggershield
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: defendatron==0.1.0
+Requires-Dist: defendatron==0.1.1
 
 # Facehugger Shield
 
 Facehugger Shield automatically locks down operations
 for specific modules. It was designed to non-destructively restrict access
 to the Huggingface library, but can be used with any library.
```

### Comparing `facehuggershield-0.1.1/README.md` & `facehuggershield-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `facehuggershield-0.1.1/setup.py` & `facehuggershield-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name="facehuggershield",
-    version="0.1.1",
+    version="0.1.2",
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
-        "defendatron==0.1.0",
+        "defendatron==0.1.1",
     ],
     dependency_links=[
     ],
 )
```

### Comparing `facehuggershield-0.1.1/src/facehuggershield.egg-info/PKG-INFO` & `facehuggershield-0.1.2/src/facehuggershield.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: facehuggershield
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/Capsize-Games/facehuggershield
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: defendatron==0.1.0
+Requires-Dist: defendatron==0.1.1
 
 # Facehugger Shield
 
 Facehugger Shield automatically locks down operations
 for specific modules. It was designed to non-destructively restrict access
 to the Huggingface library, but can be used with any library.
```

