# Comparing `tmp/kungfupanda-0.7.tar.gz` & `tmp/kungfupanda-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kungfupanda-0.7.tar", last modified: Sun Apr 21 19:35:46 2024, max compression
+gzip compressed data, was "kungfupanda-0.8.tar", last modified: Sun Apr 21 19:54:14 2024, max compression
```

## Comparing `kungfupanda-0.7.tar` & `kungfupanda-0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-21 19:35:46.167822 kungfupanda-0.7/
--rw-r--r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      571 2024-04-21 19:35:46.167822 kungfupanda-0.7/PKG-INFO
-drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-21 19:35:46.163822 kungfupanda-0.7/kungfupanda/
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       72 2024-04-21 19:28:01.000000 kungfupanda-0.7/kungfupanda/__init__.py
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)    17978 2024-04-21 19:34:04.000000 kungfupanda-0.7/kungfupanda/kungfupanda.py
-drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-21 19:35:46.167822 kungfupanda-0.7/kungfupanda.egg-info/
--rw-r--r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      571 2024-04-21 19:35:46.000000 kungfupanda-0.7/kungfupanda.egg-info/PKG-INFO
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      271 2024-04-21 19:35:46.000000 kungfupanda-0.7/kungfupanda.egg-info/SOURCES.txt
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)        1 2024-04-21 19:35:46.000000 kungfupanda-0.7/kungfupanda.egg-info/dependency_links.txt
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       80 2024-04-21 19:35:46.000000 kungfupanda-0.7/kungfupanda.egg-info/entry_points.txt
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       45 2024-04-21 19:35:46.000000 kungfupanda-0.7/kungfupanda.egg-info/requires.txt
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       12 2024-04-21 19:35:46.000000 kungfupanda-0.7/kungfupanda.egg-info/top_level.txt
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       38 2024-04-21 19:35:46.167822 kungfupanda-0.7/setup.cfg
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      851 2024-04-21 19:34:14.000000 kungfupanda-0.7/setup.py
+drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-21 19:54:14.089017 kungfupanda-0.8/
+-rw-r--r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      571 2024-04-21 19:54:14.089017 kungfupanda-0.8/PKG-INFO
+drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-21 19:54:14.089017 kungfupanda-0.8/kungfupanda/
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       38 2024-04-21 19:54:04.000000 kungfupanda-0.8/kungfupanda/__init__.py
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)    17910 2024-04-21 19:54:00.000000 kungfupanda-0.8/kungfupanda/kungfupanda.py
+drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-21 19:54:14.089017 kungfupanda-0.8/kungfupanda.egg-info/
+-rw-r--r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      571 2024-04-21 19:54:13.000000 kungfupanda-0.8/kungfupanda.egg-info/PKG-INFO
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      271 2024-04-21 19:54:14.000000 kungfupanda-0.8/kungfupanda.egg-info/SOURCES.txt
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)        1 2024-04-21 19:54:13.000000 kungfupanda-0.8/kungfupanda.egg-info/dependency_links.txt
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       80 2024-04-21 19:54:13.000000 kungfupanda-0.8/kungfupanda.egg-info/entry_points.txt
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       45 2024-04-21 19:54:13.000000 kungfupanda-0.8/kungfupanda.egg-info/requires.txt
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       12 2024-04-21 19:54:13.000000 kungfupanda-0.8/kungfupanda.egg-info/top_level.txt
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       38 2024-04-21 19:54:14.089017 kungfupanda-0.8/setup.cfg
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      851 2024-04-21 19:54:09.000000 kungfupanda-0.8/setup.py
```

### Comparing `kungfupanda-0.7/PKG-INFO` & `kungfupanda-0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kungfupanda
-Version: 0.7
+Version: 0.8
 Summary: A simple package to make everything easy for programmers for doing everything the cool way
 Home-page: 
 Author: The big fat panda
 Author-email: po_the_big_fat_panda@gmail.com
 Requires-Dist: requests>=2.25.1
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: pandas>=2.2.2
```

### Comparing `kungfupanda-0.7/kungfupanda/kungfupanda.py` & `kungfupanda-0.8/kungfupanda/kungfupanda.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 from pandas import *
 
 # Mirror all functions/classes from pandas
-__all__ = [name for name in dir() if not name.startswith('_')]
+kungfupanda = pd
 
 def who_is_dragon_warrior():
     print("""
             *********************++++***++++++**++++++**++++++++++++++++++++++*+++++++++++++++++++++++++++++++++++++++++++++++++++++
             *********************++*++**+++++++**+++++*++++++++++++++*++++++++*+++++++++++++++++++++++++++++++++++++++++++++++++++++
             *****************************+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
             ******************************+***+++++++++++++++++*++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
@@ -126,16 +126,15 @@
             %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%#%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%@%%%@@
             @%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%#%#%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%@%%@@@
             %%%%%%%%%%%%%%%@%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%#####%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%@%%%%@%%
             
             
                   """)
     
-def print_message():
-     print("""__          __  _                            _          _   _          
+    print("""__          __  _                            _          _   _          
         \ \        / / | |                          | |        | | | |         
          \ \  /\  / /__| | ___ ___  _ __ ___   ___  | |_ ___   | |_| |__   ___ 
           \ \/  \/ / _ \ |/ __/ _ \| '_ ` _ \ / _ \ | __/ _ \  | __| '_ \ / _ \
            \  /\  /  __/ | (_| (_) | | | | | |  __/ | || (_) | | |_| | | |  __/
             \/  \/ \___|_|\___\___/|_| |_| |_|\___|  \__\___/   \__|_| |_|\___|
```

### Comparing `kungfupanda-0.7/kungfupanda.egg-info/PKG-INFO` & `kungfupanda-0.8/kungfupanda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kungfupanda
-Version: 0.7
+Version: 0.8
 Summary: A simple package to make everything easy for programmers for doing everything the cool way
 Home-page: 
 Author: The big fat panda
 Author-email: po_the_big_fat_panda@gmail.com
 Requires-Dist: requests>=2.25.1
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: pandas>=2.2.2
```

### Comparing `kungfupanda-0.7/setup.py` & `kungfupanda-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='kungfupanda',
-    version='0.7',
+    version='0.8',
     author='The big fat panda',
     author_email='po_the_big_fat_panda@gmail.com',
     description="A simple package to make everything easy for programmers for doing everything the cool way",
     long_description="""A simple package for the people who are not bound by society rules 
     made by an cute panda who trained to be a dragon warrior
     For all the story watch the original triology
     Kung Fu Panda 1
```

