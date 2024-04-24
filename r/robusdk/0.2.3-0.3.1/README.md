# Comparing `tmp/robusdk-0.2.3.tar.gz` & `tmp/robusdk-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robusdk-0.2.3.tar", last modified: Thu Dec 21 02:45:10 2023, max compression
+gzip compressed data, was "robusdk-0.3.1.tar", last modified: Wed Apr 24 03:58:24 2024, max compression
```

## Comparing `robusdk-0.2.3.tar` & `robusdk-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-12-21 02:45:10.653852 robusdk-0.2.3/
--rw-r--r--   0 debian    (1000) debian    (1000)       18 2023-12-21 01:21:17.000000 robusdk-0.2.3/MANIFEST.in
--rw-r--r--   0 debian    (1000) debian    (1000)     2981 2023-12-21 02:45:10.653852 robusdk-0.2.3/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)     2728 2023-12-21 01:21:17.000000 robusdk-0.2.3/readme.md
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-12-21 02:45:10.649852 robusdk-0.2.3/robusdk/
--rw-r--r--   0 debian    (1000) debian    (1000)      150 2023-12-21 01:21:17.000000 robusdk-0.2.3/robusdk/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)      879 2023-12-21 01:21:17.000000 robusdk-0.2.3/robusdk/awaitable.py
--rw-r--r--   0 debian    (1000) debian    (1000)      477 2023-12-21 01:21:17.000000 robusdk-0.2.3/robusdk/coroutine.py
--rw-r--r--   0 debian    (1000) debian    (1000)      438 2023-12-21 01:21:17.000000 robusdk-0.2.3/robusdk/ksy.py
--rw-r--r--   0 debian    (1000) debian    (1000)      496 2023-12-21 01:21:17.000000 robusdk-0.2.3/robusdk/logger.py
--rw-r--r--   0 debian    (1000) debian    (1000)     5561 2023-12-21 01:21:17.000000 robusdk-0.2.3/robusdk/main.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1197 2023-12-21 01:21:17.000000 robusdk-0.2.3/robusdk/sequence.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2023-12-21 02:45:10.653852 robusdk-0.2.3/robusdk.egg-info/
--rw-r--r--   0 debian    (1000) debian    (1000)     2981 2023-12-21 02:45:10.000000 robusdk-0.2.3/robusdk.egg-info/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)      315 2023-12-21 02:45:10.000000 robusdk-0.2.3/robusdk.egg-info/SOURCES.txt
--rw-r--r--   0 debian    (1000) debian    (1000)        1 2023-12-21 02:45:10.000000 robusdk-0.2.3/robusdk.egg-info/dependency_links.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       44 2023-12-21 02:45:10.000000 robusdk-0.2.3/robusdk.egg-info/requires.txt
--rw-r--r--   0 debian    (1000) debian    (1000)        8 2023-12-21 02:45:10.000000 robusdk-0.2.3/robusdk.egg-info/top_level.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       38 2023-12-21 02:45:10.653852 robusdk-0.2.3/setup.cfg
--rw-r--r--   0 debian    (1000) debian    (1000)      706 2023-12-21 02:44:40.000000 robusdk-0.2.3/setup.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-04-24 03:58:24.236567 robusdk-0.3.1/
+-rw-r--r--   0 debian    (1000) debian    (1000)       18 2024-04-24 03:29:02.000000 robusdk-0.3.1/MANIFEST.in
+-rw-r--r--   0 debian    (1000) debian    (1000)     2981 2024-04-24 03:58:24.236567 robusdk-0.3.1/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)     2728 2024-04-24 03:29:02.000000 robusdk-0.3.1/readme.md
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-04-24 03:58:24.236567 robusdk-0.3.1/robusdk/
+-rw-r--r--   0 debian    (1000) debian    (1000)      150 2024-04-24 03:29:02.000000 robusdk-0.3.1/robusdk/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      879 2024-04-24 03:29:02.000000 robusdk-0.3.1/robusdk/awaitable.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      477 2024-04-24 03:29:02.000000 robusdk-0.3.1/robusdk/coroutine.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      438 2024-04-24 03:29:02.000000 robusdk-0.3.1/robusdk/ksy.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      496 2024-04-24 03:29:02.000000 robusdk-0.3.1/robusdk/logger.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     5561 2024-04-24 03:29:02.000000 robusdk-0.3.1/robusdk/main.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1197 2024-04-24 03:29:02.000000 robusdk-0.3.1/robusdk/sequence.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-04-24 03:58:24.236567 robusdk-0.3.1/robusdk.egg-info/
+-rw-r--r--   0 debian    (1000) debian    (1000)     2981 2024-04-24 03:58:24.000000 robusdk-0.3.1/robusdk.egg-info/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)      315 2024-04-24 03:58:24.000000 robusdk-0.3.1/robusdk.egg-info/SOURCES.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)        1 2024-04-24 03:58:24.000000 robusdk-0.3.1/robusdk.egg-info/dependency_links.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       44 2024-04-24 03:58:24.000000 robusdk-0.3.1/robusdk.egg-info/requires.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)        8 2024-04-24 03:58:24.000000 robusdk-0.3.1/robusdk.egg-info/top_level.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       38 2024-04-24 03:58:24.236567 robusdk-0.3.1/setup.cfg
+-rw-r--r--   0 debian    (1000) debian    (1000)      706 2024-04-24 03:57:20.000000 robusdk-0.3.1/setup.py
```

### Comparing `robusdk-0.2.3/PKG-INFO` & `robusdk-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robusdk
-Version: 0.2.3
+Version: 0.3.1
 Summary: robusdk
 Home-page: http://255.255.255.255/
 Author: robusdk
 Author-email: root@localhost.localdomain
 License: UNLISENCED
 Keywords: robusdk
 Platform: any
```

### Comparing `robusdk-0.2.3/readme.md` & `robusdk-0.3.1/readme.md`

 * *Files identical despite different names*

### Comparing `robusdk-0.2.3/robusdk/awaitable.py` & `robusdk-0.3.1/robusdk/awaitable.py`

 * *Files identical despite different names*

### Comparing `robusdk-0.2.3/robusdk/main.py` & `robusdk-0.3.1/robusdk/main.py`

 * *Files identical despite different names*

### Comparing `robusdk-0.2.3/robusdk/sequence.py` & `robusdk-0.3.1/robusdk/sequence.py`

 * *Files identical despite different names*

### Comparing `robusdk-0.2.3/robusdk.egg-info/PKG-INFO` & `robusdk-0.3.1/robusdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robusdk
-Version: 0.2.3
+Version: 0.3.1
 Summary: robusdk
 Home-page: http://255.255.255.255/
 Author: robusdk
 Author-email: root@localhost.localdomain
 License: UNLISENCED
 Keywords: robusdk
 Platform: any
```

### Comparing `robusdk-0.2.3/setup.py` & `robusdk-0.3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 name = 'robusdk'
 
 setup(
     name = name,
-    version = '0.2.3',
+    version = '0.3.1',
     keywords = [name],
     description = name,
     long_description=(Path(__file__).parent / 'readme.md').read_text(),
     long_description_content_type='text/markdown',
     license = 'UNLISENCED',
     url = 'http://255.255.255.255/',
     author = name,
```

