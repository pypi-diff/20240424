# Comparing `tmp/kungfupanda-0.23.tar.gz` & `tmp/kungfupanda-0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kungfupanda-0.23.tar", last modified: Wed Apr 24 09:21:08 2024, max compression
+gzip compressed data, was "kungfupanda-0.24.tar", last modified: Wed Apr 24 09:37:17 2024, max compression
```

## Comparing `kungfupanda-0.23.tar` & `kungfupanda-0.24.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-24 09:21:08.957656 kungfupanda-0.23/
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       36 2024-04-24 08:31:59.000000 kungfupanda-0.23/MANIFEST.in
--rw-r--r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      522 2024-04-24 09:21:08.957656 kungfupanda-0.23/PKG-INFO
-drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-24 09:21:08.953656 kungfupanda-0.23/kungfupanda/
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)     1660 2024-04-23 19:01:49.000000 kungfupanda-0.23/kungfupanda/__init__.py
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)    15325 2024-04-24 09:17:38.000000 kungfupanda-0.23/kungfupanda/kungfupanda.py
-drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-24 09:21:08.953656 kungfupanda-0.23/kungfupanda/resources/
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)  1974158 2024-04-23 19:03:43.000000 kungfupanda-0.23/kungfupanda/resources/gif_1.gif
-drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-24 09:21:08.957656 kungfupanda-0.23/kungfupanda.egg-info/
--rw-r--r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      522 2024-04-24 09:21:08.000000 kungfupanda-0.23/kungfupanda.egg-info/PKG-INFO
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      277 2024-04-24 09:21:08.000000 kungfupanda-0.23/kungfupanda.egg-info/SOURCES.txt
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)        1 2024-04-24 09:21:08.000000 kungfupanda-0.23/kungfupanda.egg-info/dependency_links.txt
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       21 2024-04-24 09:21:08.000000 kungfupanda-0.23/kungfupanda.egg-info/requires.txt
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       12 2024-04-24 09:21:08.000000 kungfupanda-0.23/kungfupanda.egg-info/top_level.txt
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       38 2024-04-24 09:21:08.957656 kungfupanda-0.23/setup.cfg
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      702 2024-04-24 09:05:50.000000 kungfupanda-0.23/setup.py
+drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-24 09:37:17.547762 kungfupanda-0.24/
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       36 2024-04-24 08:31:59.000000 kungfupanda-0.24/MANIFEST.in
+-rw-r--r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      522 2024-04-24 09:37:17.547762 kungfupanda-0.24/PKG-INFO
+drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-24 09:37:17.543762 kungfupanda-0.24/kungfupanda/
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)     1649 2024-04-24 09:35:15.000000 kungfupanda-0.24/kungfupanda/__init__.py
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)    15325 2024-04-24 09:17:38.000000 kungfupanda-0.24/kungfupanda/kungfupanda.py
+drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-24 09:37:17.543762 kungfupanda-0.24/kungfupanda/resources/
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)  1974158 2024-04-23 19:03:43.000000 kungfupanda-0.24/kungfupanda/resources/gif_1.gif
+drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-24 09:37:17.547762 kungfupanda-0.24/kungfupanda.egg-info/
+-rw-r--r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      522 2024-04-24 09:37:17.000000 kungfupanda-0.24/kungfupanda.egg-info/PKG-INFO
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      277 2024-04-24 09:37:17.000000 kungfupanda-0.24/kungfupanda.egg-info/SOURCES.txt
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)        1 2024-04-24 09:37:17.000000 kungfupanda-0.24/kungfupanda.egg-info/dependency_links.txt
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       21 2024-04-24 09:37:17.000000 kungfupanda-0.24/kungfupanda.egg-info/requires.txt
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       12 2024-04-24 09:37:17.000000 kungfupanda-0.24/kungfupanda.egg-info/top_level.txt
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       38 2024-04-24 09:37:17.547762 kungfupanda-0.24/setup.cfg
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      702 2024-04-24 09:37:10.000000 kungfupanda-0.24/setup.py
```

### Comparing `kungfupanda-0.23/PKG-INFO` & `kungfupanda-0.24/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kungfupanda
-Version: 0.23
+Version: 0.24
 Summary: A simple package to make everything easy for programmers to do everything the cool way
 Home-page: 
 Author: The Big Fat Panda
 Author-email: po_the_big_fat_panda@gmail.com
 Requires-Dist: pandas
 Requires-Dist: opencv-python
```

### Comparing `kungfupanda-0.23/kungfupanda/__init__.py` & `kungfupanda-0.24/kungfupanda/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from kungfupanda.kungfupanda import who_is_dragon_warrior,wuxi_finger_hold
+from kungfupanda import who_is_dragon_warrior,wuxi_finger_hold
 from pandas import *
 
+
 print(r"""
 __          __  _                            _          _   _          
 \ \        / / | |                          | |        | | | |         
  \ \  /\  / /__| | ___ ___  _ __ ___   ___  | |_ ___   | |_| |__   ___ 
   \ \/  \/ / _ \ |/ __/ _ \| '_ ` _ \ / _ \ | __/ _ \  | __| '_ \ / _ \
    \  /\  /  __/ | (_| (_) | | | | | |  __/ | || (_) | | |_| | | |  __/
     \/  \/ \___|_|\___\___/|_| |_| |_|\___|  \__\___/   \__|_| |_|\___|
```

### Comparing `kungfupanda-0.23/kungfupanda/kungfupanda.py` & `kungfupanda-0.24/kungfupanda/kungfupanda.py`

 * *Files identical despite different names*

### Comparing `kungfupanda-0.23/kungfupanda/resources/gif_1.gif` & `kungfupanda-0.24/kungfupanda/resources/gif_1.gif`

 * *Files identical despite different names*

### Comparing `kungfupanda-0.23/kungfupanda.egg-info/PKG-INFO` & `kungfupanda-0.24/kungfupanda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kungfupanda
-Version: 0.23
+Version: 0.24
 Summary: A simple package to make everything easy for programmers to do everything the cool way
 Home-page: 
 Author: The Big Fat Panda
 Author-email: po_the_big_fat_panda@gmail.com
 Requires-Dist: pandas
 Requires-Dist: opencv-python
```

### Comparing `kungfupanda-0.23/setup.py` & `kungfupanda-0.24/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='kungfupanda',
-    version='0.23',
+    version='0.24',
     author='The Big Fat Panda',
     author_email='po_the_big_fat_panda@gmail.com',
     description="A simple package to make everything easy for programmers to do everything the cool way",
     long_description="""A simple package for people who are not bound by societal rules, made by a cute panda trained to be a dragon warrior. For the full story, watch the original trilogy:
     - Kung Fu Panda 1
     - Kung Fu Panda 2
     - Kung Fu Panda 3
```

