# Comparing `tmp/gleweather-0.1.0.tar.gz` & `tmp/gleweather-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gleweather-0.1.0.tar", last modified: Tue Apr 23 23:07:02 2024, max compression
+gzip compressed data, was "gleweather-0.1.1.tar", last modified: Tue Apr 23 23:10:36 2024, max compression
```

## Comparing `gleweather-0.1.0.tar` & `gleweather-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-23 23:07:02.681117 gleweather-0.1.0/
--rw-r--r--   0 pohie      (501) staff       (20)     1211 2024-04-23 21:50:15.000000 gleweather-0.1.0/LICENSE.txt
--rw-r--r--   0 pohie      (501) staff       (20)      684 2024-04-23 23:07:02.680873 gleweather-0.1.0/PKG-INFO
-drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-23 23:07:02.679752 gleweather-0.1.0/gleweather/
--rw-r--r--   0 pohie      (501) staff       (20)        0 2024-04-23 21:51:39.000000 gleweather-0.1.0/gleweather/__init__.py
--rw-r--r--   0 pohie      (501) staff       (20)     1066 2024-04-23 22:13:45.000000 gleweather-0.1.0/gleweather/gleweather.py
-drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-23 23:07:02.680618 gleweather-0.1.0/gleweather.egg-info/
--rw-r--r--   0 pohie      (501) staff       (20)      684 2024-04-23 23:07:02.000000 gleweather-0.1.0/gleweather.egg-info/PKG-INFO
--rw-r--r--   0 pohie      (501) staff       (20)      237 2024-04-23 23:07:02.000000 gleweather-0.1.0/gleweather.egg-info/SOURCES.txt
--rw-r--r--   0 pohie      (501) staff       (20)        1 2024-04-23 23:07:02.000000 gleweather-0.1.0/gleweather.egg-info/dependency_links.txt
--rw-r--r--   0 pohie      (501) staff       (20)       13 2024-04-23 23:07:02.000000 gleweather-0.1.0/gleweather.egg-info/requires.txt
--rw-r--r--   0 pohie      (501) staff       (20)       11 2024-04-23 23:07:02.000000 gleweather-0.1.0/gleweather.egg-info/top_level.txt
--rw-r--r--   0 pohie      (501) staff       (20)       38 2024-04-23 23:07:02.681165 gleweather-0.1.0/setup.cfg
--rw-r--r--   0 pohie      (501) staff       (20)      782 2024-04-23 22:27:47.000000 gleweather-0.1.0/setup.py
+drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-23 23:10:36.946364 gleweather-0.1.1/
+-rw-r--r--   0 pohie      (501) staff       (20)     1211 2024-04-23 21:50:15.000000 gleweather-0.1.1/LICENSE.txt
+-rw-r--r--   0 pohie      (501) staff       (20)      684 2024-04-23 23:10:36.946143 gleweather-0.1.1/PKG-INFO
+drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-23 23:10:36.945207 gleweather-0.1.1/gleweather/
+-rw-r--r--   0 pohie      (501) staff       (20)     1066 2024-04-23 23:10:12.000000 gleweather-0.1.1/gleweather/__init__.py
+-rw-r--r--   0 pohie      (501) staff       (20)     1066 2024-04-23 22:13:45.000000 gleweather-0.1.1/gleweather/gleweather.py
+drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-23 23:10:36.945906 gleweather-0.1.1/gleweather.egg-info/
+-rw-r--r--   0 pohie      (501) staff       (20)      684 2024-04-23 23:10:36.000000 gleweather-0.1.1/gleweather.egg-info/PKG-INFO
+-rw-r--r--   0 pohie      (501) staff       (20)      237 2024-04-23 23:10:36.000000 gleweather-0.1.1/gleweather.egg-info/SOURCES.txt
+-rw-r--r--   0 pohie      (501) staff       (20)        1 2024-04-23 23:10:36.000000 gleweather-0.1.1/gleweather.egg-info/dependency_links.txt
+-rw-r--r--   0 pohie      (501) staff       (20)       13 2024-04-23 23:10:36.000000 gleweather-0.1.1/gleweather.egg-info/requires.txt
+-rw-r--r--   0 pohie      (501) staff       (20)       11 2024-04-23 23:10:36.000000 gleweather-0.1.1/gleweather.egg-info/top_level.txt
+-rw-r--r--   0 pohie      (501) staff       (20)       38 2024-04-23 23:10:36.946412 gleweather-0.1.1/setup.cfg
+-rw-r--r--   0 pohie      (501) staff       (20)      782 2024-04-23 23:10:31.000000 gleweather-0.1.1/setup.py
```

### Comparing `gleweather-0.1.0/LICENSE.txt` & `gleweather-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gleweather-0.1.0/PKG-INFO` & `gleweather-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gleweather
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python package aiming to allow you to use google's weather service with automatic city detection without having to search for hours to learn how to do it.
 Home-page: https://github.com/Pohie/gleweather-py.git
 Author: Abbott Broughton
 Author-email: abbottbroughton@icloud.com
 License: The Unlicense
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gleweather-0.1.0/gleweather/gleweather.py` & `gleweather-0.1.1/gleweather/__init__.py`

 * *Files identical despite different names*

### Comparing `gleweather-0.1.0/gleweather.egg-info/PKG-INFO` & `gleweather-0.1.1/gleweather.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gleweather
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python package aiming to allow you to use google's weather service with automatic city detection without having to search for hours to learn how to do it.
 Home-page: https://github.com/Pohie/gleweather-py.git
 Author: Abbott Broughton
 Author-email: abbottbroughton@icloud.com
 License: The Unlicense
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gleweather-0.1.0/setup.py` & `gleweather-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='gleweather',
-    version='0.1.0',
+    version='0.1.1',
     description="A python package aiming to allow you to use google's weather service with automatic city detection "
                 "without having to search for hours to learn how to do it.",
     url='https://github.com/Pohie/gleweather-py.git',
     author='Abbott Broughton',
     author_email='abbottbroughton@icloud.com',
     license='The Unlicense',
     packages=['gleweather'],
```

