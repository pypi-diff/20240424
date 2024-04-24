# Comparing `tmp/hebill-1.2.2.tar.gz` & `tmp/hebill-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hebill-1.2.2.tar", last modified: Wed Apr 24 03:18:45 2024, max compression
+gzip compressed data, was "hebill-1.2.3.tar", last modified: Wed Apr 24 03:23:46 2024, max compression
```

## Comparing `hebill-1.2.2.tar` & `hebill-1.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 03:18:45.123378 hebill-1.2.2/
--rw-rw-rw-   0        0        0      924 2024-04-24 03:18:45.122380 hebill-1.2.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 03:18:45.116859 hebill-1.2.2/hebill/
--rw-rw-rw-   0        0        0      341 2024-04-24 03:12:13.000000 hebill-1.2.2/hebill/__init__.py
--rw-rw-rw-   0        0        0      267 2024-04-24 02:57:28.000000 hebill-1.2.2/hebill/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-24 03:18:45.122380 hebill-1.2.2/hebill.egg-info/
--rw-rw-rw-   0        0        0      924 2024-04-24 03:18:45.000000 hebill-1.2.2/hebill.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2024-04-24 03:18:45.000000 hebill-1.2.2/hebill.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 03:18:45.000000 hebill-1.2.2/hebill.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2024-04-24 03:18:45.000000 hebill-1.2.2/hebill.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-24 03:18:45.000000 hebill-1.2.2/hebill.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      592 2024-04-24 03:18:44.000000 hebill-1.2.2/pack_upload_setup.py
--rw-rw-rw-   0        0        0       42 2024-04-24 03:18:45.123378 hebill-1.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 03:23:46.547122 hebill-1.2.3/
+-rw-rw-rw-   0        0        0      924 2024-04-24 03:23:46.547122 hebill-1.2.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 03:23:46.540605 hebill-1.2.3/hebill/
+-rw-rw-rw-   0        0        0      341 2024-04-24 03:12:13.000000 hebill-1.2.3/hebill/__init__.py
+-rw-rw-rw-   0        0        0      267 2024-04-24 03:23:45.000000 hebill-1.2.3/hebill/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:23:46.544605 hebill-1.2.3/hebill.egg-info/
+-rw-rw-rw-   0        0        0      924 2024-04-24 03:23:46.000000 hebill-1.2.3/hebill.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2024-04-24 03:23:46.000000 hebill-1.2.3/hebill.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 03:23:46.000000 hebill-1.2.3/hebill.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2024-04-24 03:23:46.000000 hebill-1.2.3/hebill.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 03:23:46.000000 hebill-1.2.3/hebill.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      592 2024-04-24 03:23:45.000000 hebill-1.2.3/pack_upload_setup.py
+-rw-rw-rw-   0        0        0       42 2024-04-24 03:23:46.547122 hebill-1.2.3/setup.cfg
```

### Comparing `hebill-1.2.2/PKG-INFO` & `hebill-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hebill
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python Hebill
 Requires-Python: >=3.12
 Description-Content-Type: text/plain
 Requires-Dist: psutil==5.9.8
 Requires-Dist: pillow==10.3.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: wxpython==4.2.1
```

### Comparing `hebill-1.2.2/hebill.egg-info/PKG-INFO` & `hebill-1.2.3/hebill.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hebill
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python Hebill
 Requires-Python: >=3.12
 Description-Content-Type: text/plain
 Requires-Dist: psutil==5.9.8
 Requires-Dist: pillow==10.3.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: wxpython==4.2.1
```

### Comparing `hebill-1.2.2/pack_upload_setup.py` & `hebill-1.2.3/pack_upload_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 setup(
     name='hebill',
-    version='1.2.2',
+    version='1.2.3',
     description='Python Hebill',
     long_description=open(r'D:\SDK\GitHub\python_hebill\hebill\README.MD', encoding='utf-8').read(),
     long_description_content_type='text/plain',
     packages=[
         'hebill',
     ],
     install_requires=[
```

