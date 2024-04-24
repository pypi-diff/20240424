# Comparing `tmp/isupermath-0.0.1.tar.gz` & `tmp/isupermath-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isupermath-0.0.1.tar", last modified: Mon Mar 25 10:23:34 2024, max compression
+gzip compressed data, was "isupermath-0.0.2.tar", last modified: Wed Apr 24 16:41:56 2024, max compression
```

## Comparing `isupermath-0.0.1.tar` & `isupermath-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 10:23:34.015492 isupermath-0.0.1/
--rw-rw-rw-   0        0        0     1064 2024-03-23 18:00:29.000000 isupermath-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      590 2024-03-25 10:23:34.006545 isupermath-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-25 10:23:33.973665 isupermath-0.0.1/isupermath/
--rw-rw-rw-   0        0        0        0 2024-03-25 09:38:34.000000 isupermath-0.0.1/isupermath/__init__.py
--rw-rw-rw-   0        0        0     2510 2024-03-25 09:37:53.000000 isupermath-0.0.1/isupermath/fn.py
-drwxrwxrwx   0        0        0        0 2024-03-25 10:23:34.006545 isupermath-0.0.1/isupermath.egg-info/
--rw-rw-rw-   0        0        0      590 2024-03-25 10:23:33.000000 isupermath-0.0.1/isupermath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2024-03-25 10:23:33.000000 isupermath-0.0.1/isupermath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 10:23:33.000000 isupermath-0.0.1/isupermath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-03-25 10:23:33.000000 isupermath-0.0.1/isupermath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-25 10:23:34.015492 isupermath-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      857 2024-03-25 10:22:42.000000 isupermath-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:41:56.056089 isupermath-0.0.2/
+-rw-rw-rw-   0        0        0     1064 2024-03-23 18:00:29.000000 isupermath-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      602 2024-04-24 16:41:56.056089 isupermath-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 16:41:56.046797 isupermath-0.0.2/isupermath.egg-info/
+-rw-rw-rw-   0        0        0      602 2024-04-24 16:41:55.000000 isupermath-0.0.2/isupermath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2024-04-24 16:41:55.000000 isupermath-0.0.2/isupermath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 16:41:55.000000 isupermath-0.0.2/isupermath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 16:41:55.000000 isupermath-0.0.2/isupermath.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 16:41:55.000000 isupermath-0.0.2/isupermath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 16:41:56.056089 isupermath-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      851 2024-04-24 16:41:23.000000 isupermath-0.0.2/setup.py
```

### Comparing `isupermath-0.0.1/LICENSE.txt` & `isupermath-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `isupermath-0.0.1/PKG-INFO` & `isupermath-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: isupermath
-Version: 0.0.1
+Version: 0.0.2
 Summary: isupermath
 Author: Iffiisyed
 Author-email: iffiisyed@gmail.com
-Keywords: arithmetic,supermath,mathematics,python tutorial,iffiisyed
+Keywords: csv,read_csv,readfile,iffiisyed
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: pandas
 
-A package to perform basic maths
+A package to read csv file and make it dataframe
```

### Comparing `isupermath-0.0.1/isupermath.egg-info/PKG-INFO` & `isupermath-0.0.2/isupermath.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: isupermath
-Version: 0.0.1
+Version: 0.0.2
 Summary: isupermath
 Author: Iffiisyed
 Author-email: iffiisyed@gmail.com
-Keywords: arithmetic,supermath,mathematics,python tutorial,iffiisyed
+Keywords: csv,read_csv,readfile,iffiisyed
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: pandas
 
-A package to perform basic maths
+A package to read csv file and make it dataframe
```

