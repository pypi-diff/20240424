# Comparing `tmp/gleweather-0.1.2.tar.gz` & `tmp/gleweather-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gleweather-0.1.2.tar", last modified: Tue Apr 23 23:32:09 2024, max compression
+gzip compressed data, was "gleweather-0.1.3.tar", last modified: Wed Apr 24 00:37:43 2024, max compression
```

## Comparing `gleweather-0.1.2.tar` & `gleweather-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-23 23:32:09.811016 gleweather-0.1.2/
--rw-r--r--   0 pohie      (501) staff       (20)     1211 2024-04-23 21:50:15.000000 gleweather-0.1.2/LICENSE.txt
--rw-r--r--   0 pohie      (501) staff       (20)      684 2024-04-23 23:32:09.810687 gleweather-0.1.2/PKG-INFO
-drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-23 23:32:09.809506 gleweather-0.1.2/gleweather/
--rw-r--r--   0 pohie      (501) staff       (20)      930 2024-04-23 23:30:50.000000 gleweather-0.1.2/gleweather/__init__.py
-drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-23 23:32:09.810416 gleweather-0.1.2/gleweather.egg-info/
--rw-r--r--   0 pohie      (501) staff       (20)      684 2024-04-23 23:32:09.000000 gleweather-0.1.2/gleweather.egg-info/PKG-INFO
--rw-r--r--   0 pohie      (501) staff       (20)      212 2024-04-23 23:32:09.000000 gleweather-0.1.2/gleweather.egg-info/SOURCES.txt
--rw-r--r--   0 pohie      (501) staff       (20)        1 2024-04-23 23:32:09.000000 gleweather-0.1.2/gleweather.egg-info/dependency_links.txt
--rw-r--r--   0 pohie      (501) staff       (20)       13 2024-04-23 23:32:09.000000 gleweather-0.1.2/gleweather.egg-info/requires.txt
--rw-r--r--   0 pohie      (501) staff       (20)       11 2024-04-23 23:32:09.000000 gleweather-0.1.2/gleweather.egg-info/top_level.txt
--rw-r--r--   0 pohie      (501) staff       (20)       38 2024-04-23 23:32:09.811098 gleweather-0.1.2/setup.cfg
--rw-r--r--   0 pohie      (501) staff       (20)      782 2024-04-23 23:32:05.000000 gleweather-0.1.2/setup.py
+drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-24 00:37:43.292075 gleweather-0.1.3/
+-rw-r--r--   0 pohie      (501) staff       (20)     1211 2024-04-23 21:50:15.000000 gleweather-0.1.3/LICENSE.txt
+-rw-r--r--   0 pohie      (501) staff       (20)      762 2024-04-24 00:37:43.291877 gleweather-0.1.3/PKG-INFO
+drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-24 00:37:43.291032 gleweather-0.1.3/gleweather/
+-rw-r--r--   0 pohie      (501) staff       (20)      930 2024-04-23 23:30:50.000000 gleweather-0.1.3/gleweather/__init__.py
+drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-24 00:37:43.291649 gleweather-0.1.3/gleweather.egg-info/
+-rw-r--r--   0 pohie      (501) staff       (20)      762 2024-04-24 00:37:43.000000 gleweather-0.1.3/gleweather.egg-info/PKG-INFO
+-rw-r--r--   0 pohie      (501) staff       (20)      212 2024-04-24 00:37:43.000000 gleweather-0.1.3/gleweather.egg-info/SOURCES.txt
+-rw-r--r--   0 pohie      (501) staff       (20)        1 2024-04-24 00:37:43.000000 gleweather-0.1.3/gleweather.egg-info/dependency_links.txt
+-rw-r--r--   0 pohie      (501) staff       (20)       13 2024-04-24 00:37:43.000000 gleweather-0.1.3/gleweather.egg-info/requires.txt
+-rw-r--r--   0 pohie      (501) staff       (20)       11 2024-04-24 00:37:43.000000 gleweather-0.1.3/gleweather.egg-info/top_level.txt
+-rw-r--r--   0 pohie      (501) staff       (20)       38 2024-04-24 00:37:43.292122 gleweather-0.1.3/setup.cfg
+-rw-r--r--   0 pohie      (501) staff       (20)      883 2024-04-24 00:37:40.000000 gleweather-0.1.3/setup.py
```

### Comparing `gleweather-0.1.2/LICENSE.txt` & `gleweather-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gleweather-0.1.2/PKG-INFO` & `gleweather-0.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: gleweather
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python package aiming to allow you to use google's weather service with automatic city detection without having to search for hours to learn how to do it.
 Home-page: https://github.com/Pohie/gleweather-py.git
 Author: Abbott Broughton
 Author-email: abbottbroughton@icloud.com
 License: The Unlicense
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE.txt
 Requires-Dist: requests
 Requires-Dist: bs4
+
+You can use gleweather.weather() to get the weather where you currently are.
```

### Comparing `gleweather-0.1.2/gleweather/__init__.py` & `gleweather-0.1.3/gleweather/__init__.py`

 * *Files identical despite different names*

### Comparing `gleweather-0.1.2/gleweather.egg-info/PKG-INFO` & `gleweather-0.1.3/gleweather.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: gleweather
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python package aiming to allow you to use google's weather service with automatic city detection without having to search for hours to learn how to do it.
 Home-page: https://github.com/Pohie/gleweather-py.git
 Author: Abbott Broughton
 Author-email: abbottbroughton@icloud.com
 License: The Unlicense
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE.txt
 Requires-Dist: requests
 Requires-Dist: bs4
+
+You can use gleweather.weather() to get the weather where you currently are.
```

### Comparing `gleweather-0.1.2/setup.py` & `gleweather-0.1.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup
 
 setup(
     name='gleweather',
-    version='0.1.2',
+    version='0.1.3',
     description="A python package aiming to allow you to use google's weather service with automatic city detection "
                 "without having to search for hours to learn how to do it.",
     url='https://github.com/Pohie/gleweather-py.git',
     author='Abbott Broughton',
     author_email='abbottbroughton@icloud.com',
     license='The Unlicense',
     packages=['gleweather'],
     install_requires=['requests', 'bs4'],
+    long_description='You can use gleweather.weather() to get the weather where you currently are.',
 
     classifiers=[
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
```

