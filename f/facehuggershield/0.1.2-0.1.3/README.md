# Comparing `tmp/facehuggershield-0.1.2.tar.gz` & `tmp/facehuggershield-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facehuggershield-0.1.2.tar", last modified: Wed Apr 24 02:21:08 2024, max compression
+gzip compressed data, was "facehuggershield-0.1.3.tar", last modified: Wed Apr 24 02:28:14 2024, max compression
```

## Comparing `facehuggershield-0.1.2.tar` & `facehuggershield-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:21:08.936569 facehuggershield-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 02:21:00.000000 facehuggershield-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-24 02:21:08.936569 facehuggershield-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-24 02:21:00.000000 facehuggershield-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 02:21:08.936569 facehuggershield-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-24 02:21:00.000000 facehuggershield-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:21:08.932569 facehuggershield-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:21:08.932569 facehuggershield-0.1.2/src/facehuggershield.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-24 02:21:08.000000 facehuggershield-0.1.2/src/facehuggershield.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-24 02:21:08.000000 facehuggershield-0.1.2/src/facehuggershield.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:21:08.000000 facehuggershield-0.1.2/src/facehuggershield.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-24 02:21:08.000000 facehuggershield-0.1.2/src/facehuggershield.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:21:08.000000 facehuggershield-0.1.2/src/facehuggershield.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:28:14.127005 facehuggershield-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 02:28:04.000000 facehuggershield-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-24 02:28:14.123005 facehuggershield-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-24 02:28:04.000000 facehuggershield-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 02:28:14.127005 facehuggershield-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-24 02:28:04.000000 facehuggershield-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:28:14.123005 facehuggershield-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:28:14.123005 facehuggershield-0.1.3/src/facehuggershield.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-24 02:28:14.000000 facehuggershield-0.1.3/src/facehuggershield.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-24 02:28:14.000000 facehuggershield-0.1.3/src/facehuggershield.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:28:14.000000 facehuggershield-0.1.3/src/facehuggershield.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-24 02:28:14.000000 facehuggershield-0.1.3/src/facehuggershield.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:28:14.000000 facehuggershield-0.1.3/src/facehuggershield.egg-info/top_level.txt
```

### Comparing `facehuggershield-0.1.2/LICENSE` & `facehuggershield-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `facehuggershield-0.1.2/PKG-INFO` & `facehuggershield-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facehuggershield
-Version: 0.1.2
+Version: 0.1.3
 Home-page: https://github.com/Capsize-Games/facehuggershield
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `facehuggershield-0.1.2/README.md` & `facehuggershield-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `facehuggershield-0.1.2/setup.py` & `facehuggershield-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="facehuggershield",
-    version="0.1.2",
+    version="0.1.3",
     author="Capsize LLC",
     description="",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="",
     license="GPL-3.0",
     author_email="contact@capsizegames.com",
```

### Comparing `facehuggershield-0.1.2/src/facehuggershield.egg-info/PKG-INFO` & `facehuggershield-0.1.3/src/facehuggershield.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facehuggershield
-Version: 0.1.2
+Version: 0.1.3
 Home-page: https://github.com/Capsize-Games/facehuggershield
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

