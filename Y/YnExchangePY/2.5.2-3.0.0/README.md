# Comparing `tmp/YnExchangePY-2.5.2.tar.gz` & `tmp/YnExchangePY-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YnExchangePY-2.5.2.tar", last modified: Fri Apr 19 14:53:39 2024, max compression
+gzip compressed data, was "YnExchangePY-3.0.0.tar", last modified: Tue Apr 23 18:42:58 2024, max compression
```

## Comparing `YnExchangePY-2.5.2.tar` & `YnExchangePY-3.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 14:53:39.822461 YnExchangePY-2.5.2/
--rw-rw-rw-   0        0        0     3732 2024-04-19 14:53:39.822461 YnExchangePY-2.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     3369 2024-04-19 14:49:08.000000 YnExchangePY-2.5.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 14:53:39.804345 YnExchangePY-2.5.2/YnExchangePY.egg-info/
--rw-rw-rw-   0        0        0     3732 2024-04-19 14:53:38.000000 YnExchangePY-2.5.2/YnExchangePY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-19 14:53:38.000000 YnExchangePY-2.5.2/YnExchangePY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 14:53:38.000000 YnExchangePY-2.5.2/YnExchangePY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-19 14:53:38.000000 YnExchangePY-2.5.2/YnExchangePY.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 14:53:38.000000 YnExchangePY-2.5.2/YnExchangePY.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 14:53:39.822461 YnExchangePY-2.5.2/setup.cfg
--rw-rw-rw-   0        0        0      674 2024-04-19 14:46:26.000000 YnExchangePY-2.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:42:58.021059 YnExchangePY-3.0.0/
+-rw-rw-rw-   0        0        0     3732 2024-04-23 18:42:58.020059 YnExchangePY-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3369 2024-04-19 14:49:08.000000 YnExchangePY-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 18:42:58.018067 YnExchangePY-3.0.0/YnExchangePY.egg-info/
+-rw-rw-rw-   0        0        0     3732 2024-04-23 18:42:57.000000 YnExchangePY-3.0.0/YnExchangePY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-23 18:42:57.000000 YnExchangePY-3.0.0/YnExchangePY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 18:42:57.000000 YnExchangePY-3.0.0/YnExchangePY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-23 18:42:57.000000 YnExchangePY-3.0.0/YnExchangePY.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 18:42:57.000000 YnExchangePY-3.0.0/YnExchangePY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 18:42:58.021059 YnExchangePY-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      674 2024-04-23 18:11:36.000000 YnExchangePY-3.0.0/setup.py
```

### Comparing `YnExchangePY-2.5.2/PKG-INFO` & `YnExchangePY-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YnExchangePY
-Version: 2.5.2
+Version: 3.0.0
 Author: Yasha Najafi(YN)
 Author-email: <najafiyasha@gmail.com>
 Keywords: python,crypto,prices,crypto calculations,api,calculations
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: bs4
```

### Comparing `YnExchangePY-2.5.2/README.md` & `YnExchangePY-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `YnExchangePY-2.5.2/YnExchangePY.egg-info/PKG-INFO` & `YnExchangePY-3.0.0/YnExchangePY.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YnExchangePY
-Version: 2.5.2
+Version: 3.0.0
 Author: Yasha Najafi(YN)
 Author-email: <najafiyasha@gmail.com>
 Keywords: python,crypto,prices,crypto calculations,api,calculations
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: bs4
```

### Comparing `YnExchangePY-2.5.2/setup.py` & `YnExchangePY-3.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '2.5.2'
+VERSION = '3.0.0'
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     LONG_DESCRIPTION = "\n" + fh.read()
 
 
 # Setting up
```

