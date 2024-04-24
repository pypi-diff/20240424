# Comparing `tmp/FuzzyTM-2.0.6.tar.gz` & `tmp/FuzzyTM-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\FuzzyTM-2.0.6.tar", last modified: Mon Apr 22 22:32:27 2024, max compression
+gzip compressed data, was "dist\FuzzyTM-2.0.7.tar", last modified: Tue Apr 23 21:07:09 2024, max compression
```

## Comparing `FuzzyTM-2.0.6.tar` & `FuzzyTM-2.0.7.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 22:32:27.912982 FuzzyTM-2.0.6/
-drwxrwxrwx   0        0        0        0 2024-04-22 22:32:27.881072 FuzzyTM-2.0.6/FuzzyTM/
--rw-rw-rw-   0        0        0    63028 2022-11-23 10:50:28.000000 FuzzyTM-2.0.6/FuzzyTM/FuzzyTM.py
--rw-rw-rw-   0        0        0      155 2022-10-19 17:02:01.000000 FuzzyTM-2.0.6/FuzzyTM/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 22:32:27.910988 FuzzyTM-2.0.6/FuzzyTM.egg-info/
--rw-rw-rw-   0        0        0     7835 2024-04-22 22:32:27.000000 FuzzyTM-2.0.6/FuzzyTM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2024-04-22 22:32:27.000000 FuzzyTM-2.0.6/FuzzyTM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 22:32:27.000000 FuzzyTM-2.0.6/FuzzyTM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-22 22:32:27.000000 FuzzyTM-2.0.6/FuzzyTM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-22 22:32:27.000000 FuzzyTM-2.0.6/FuzzyTM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    18431 2021-11-01 14:27:46.000000 FuzzyTM-2.0.6/LICENSE
--rw-rw-rw-   0        0        0     7835 2024-04-22 22:32:27.912017 FuzzyTM-2.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     7517 2024-04-22 21:30:36.000000 FuzzyTM-2.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-22 22:32:27.913979 FuzzyTM-2.0.6/setup.cfg
--rw-rw-rw-   0        0        0      924 2024-04-22 22:27:03.000000 FuzzyTM-2.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 21:07:09.908570 FuzzyTM-2.0.7/
+drwxrwxrwx   0        0        0        0 2024-04-23 21:07:09.862160 FuzzyTM-2.0.7/FuzzyTM/
+-rw-rw-rw-   0        0        0    63028 2022-11-23 10:50:28.000000 FuzzyTM-2.0.7/FuzzyTM/FuzzyTM.py
+-rw-rw-rw-   0        0        0      155 2022-10-19 17:02:01.000000 FuzzyTM-2.0.7/FuzzyTM/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 21:07:09.905578 FuzzyTM-2.0.7/FuzzyTM/analysis/
+-rw-rw-rw-   0        0        0        0 2024-04-23 21:00:12.000000 FuzzyTM-2.0.7/FuzzyTM/analysis/__init__.py
+-rw-rw-rw-   0        0        0     8215 2024-04-22 22:23:11.000000 FuzzyTM-2.0.7/FuzzyTM/analysis/topic_specificity.py
+drwxrwxrwx   0        0        0        0 2024-04-23 21:07:09.895643 FuzzyTM-2.0.7/FuzzyTM.egg-info/
+-rw-rw-rw-   0        0        0     7835 2024-04-23 21:07:09.000000 FuzzyTM-2.0.7/FuzzyTM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2024-04-23 21:07:09.000000 FuzzyTM-2.0.7/FuzzyTM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 21:07:09.000000 FuzzyTM-2.0.7/FuzzyTM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-23 21:07:09.000000 FuzzyTM-2.0.7/FuzzyTM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-23 21:07:09.000000 FuzzyTM-2.0.7/FuzzyTM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    18431 2021-11-01 14:27:46.000000 FuzzyTM-2.0.7/LICENSE
+-rw-rw-rw-   0        0        0     7835 2024-04-23 21:07:09.907570 FuzzyTM-2.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7517 2024-04-22 21:30:36.000000 FuzzyTM-2.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-23 21:07:09.908570 FuzzyTM-2.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      924 2024-04-23 21:05:01.000000 FuzzyTM-2.0.7/setup.py
```

### Comparing `FuzzyTM-2.0.6/FuzzyTM/FuzzyTM.py` & `FuzzyTM-2.0.7/FuzzyTM/FuzzyTM.py`

 * *Files identical despite different names*

### Comparing `FuzzyTM-2.0.6/FuzzyTM.egg-info/PKG-INFO` & `FuzzyTM-2.0.7/FuzzyTM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuzzyTM
-Version: 2.0.6
+Version: 2.0.7
 Summary: A Python package for Fuzzy Topic Models
 Home-page: https://github.com/ERijck/FuzzyTM
 Author: Emil Rijcken
 Author-email: emil.rijcken@gmail.com
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `FuzzyTM-2.0.6/LICENSE` & `FuzzyTM-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `FuzzyTM-2.0.6/PKG-INFO` & `FuzzyTM-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuzzyTM
-Version: 2.0.6
+Version: 2.0.7
 Summary: A Python package for Fuzzy Topic Models
 Home-page: https://github.com/ERijck/FuzzyTM
 Author: Emil Rijcken
 Author-email: emil.rijcken@gmail.com
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `FuzzyTM-2.0.6/README.md` & `FuzzyTM-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `FuzzyTM-2.0.6/setup.py` & `FuzzyTM-2.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import pathlib
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '2.0.6'
+VERSION = '2.0.7'
 PACKAGE_NAME = 'FuzzyTM'
 AUTHOR = 'Emil Rijcken'
 AUTHOR_EMAIL = 'emil.rijcken@gmail.com'
 URL = 'https://github.com/ERijck/FuzzyTM'
 
 LICENSE = 'GNU General Public License v3.0'
 DESCRIPTION = 'A Python package for Fuzzy Topic Models'
```

