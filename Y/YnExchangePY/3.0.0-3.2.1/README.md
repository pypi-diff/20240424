# Comparing `tmp/YnExchangePY-3.0.0.tar.gz` & `tmp/YnExchangePY-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YnExchangePY-3.0.0.tar", last modified: Tue Apr 23 18:42:58 2024, max compression
+gzip compressed data, was "YnExchangePY-3.2.1.tar", last modified: Wed Apr 24 10:59:47 2024, max compression
```

## Comparing `YnExchangePY-3.0.0.tar` & `YnExchangePY-3.2.1.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 18:42:58.021059 YnExchangePY-3.0.0/
--rw-rw-rw-   0        0        0     3732 2024-04-23 18:42:58.020059 YnExchangePY-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3369 2024-04-19 14:49:08.000000 YnExchangePY-3.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 18:42:58.018067 YnExchangePY-3.0.0/YnExchangePY.egg-info/
--rw-rw-rw-   0        0        0     3732 2024-04-23 18:42:57.000000 YnExchangePY-3.0.0/YnExchangePY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-23 18:42:57.000000 YnExchangePY-3.0.0/YnExchangePY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 18:42:57.000000 YnExchangePY-3.0.0/YnExchangePY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-23 18:42:57.000000 YnExchangePY-3.0.0/YnExchangePY.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 18:42:57.000000 YnExchangePY-3.0.0/YnExchangePY.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 18:42:58.021059 YnExchangePY-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0      674 2024-04-23 18:11:36.000000 YnExchangePY-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:59:47.447939 YnExchangePY-3.2.1/
+-rw-rw-rw-   0        0        0     3732 2024-04-24 10:59:47.446940 YnExchangePY-3.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3369 2024-04-19 14:49:08.000000 YnExchangePY-3.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 10:59:47.407961 YnExchangePY-3.2.1/YN_Exchange/
+-rw-rw-rw-   0        0        0      967 2024-04-24 10:28:56.000000 YnExchangePY-3.2.1/YN_Exchange/__init__.py
+-rw-rw-rw-   0        0        0    31848 2024-04-24 10:58:24.000000 YnExchangePY-3.2.1/YN_Exchange/yn_exchange.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:59:47.445940 YnExchangePY-3.2.1/YnExchangePY.egg-info/
+-rw-rw-rw-   0        0        0     3732 2024-04-24 10:59:46.000000 YnExchangePY-3.2.1/YnExchangePY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-04-24 10:59:46.000000 YnExchangePY-3.2.1/YnExchangePY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 10:59:46.000000 YnExchangePY-3.2.1/YnExchangePY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-24 10:59:46.000000 YnExchangePY-3.2.1/YnExchangePY.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-24 10:59:46.000000 YnExchangePY-3.2.1/YnExchangePY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 10:59:47.447939 YnExchangePY-3.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      674 2024-04-24 10:58:33.000000 YnExchangePY-3.2.1/setup.py
```

### Comparing `YnExchangePY-3.0.0/PKG-INFO` & `YnExchangePY-3.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YnExchangePY
-Version: 3.0.0
+Version: 3.2.1
 Author: Yasha Najafi(YN)
 Author-email: <najafiyasha@gmail.com>
 Keywords: python,crypto,prices,crypto calculations,api,calculations
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: bs4
```

### Comparing `YnExchangePY-3.0.0/README.md` & `YnExchangePY-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `YnExchangePY-3.0.0/YnExchangePY.egg-info/PKG-INFO` & `YnExchangePY-3.2.1/YnExchangePY.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YnExchangePY
-Version: 3.0.0
+Version: 3.2.1
 Author: Yasha Najafi(YN)
 Author-email: <najafiyasha@gmail.com>
 Keywords: python,crypto,prices,crypto calculations,api,calculations
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: bs4
```

### Comparing `YnExchangePY-3.0.0/setup.py` & `YnExchangePY-3.2.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '3.0.0'
+VERSION = '3.2.1'
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     LONG_DESCRIPTION = "\n" + fh.read()
 
 
 # Setting up
```

