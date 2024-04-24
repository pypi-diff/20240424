# Comparing `tmp/mysqllibran-0.0.2.tar.gz` & `tmp/mysqllibran-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysqllibran-0.0.2.tar", last modified: Tue Apr 23 19:55:00 2024, max compression
+gzip compressed data, was "mysqllibran-0.0.3.tar", last modified: Tue Apr 23 20:18:41 2024, max compression
```

## Comparing `mysqllibran-0.0.2.tar` & `mysqllibran-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 hikinari  (1000) hikinari  (1000)        0 2024-04-23 19:55:00.490242 mysqllibran-0.0.2/
-drwxr-xr-x   0 hikinari  (1000) hikinari  (1000)        0 2024-04-23 19:55:00.489242 mysqllibran-0.0.2/MyLib/
--rw-r--r--   0 hikinari  (1000) hikinari  (1000)       19 2024-04-23 19:29:00.000000 mysqllibran-0.0.2/MyLib/__init__.py
--rw-r--r--   0 hikinari  (1000) hikinari  (1000)       74 2024-04-23 19:49:06.000000 mysqllibran-0.0.2/MyLib/narek.py
--rw-r--r--   0 hikinari  (1000) hikinari  (1000)      554 2024-04-23 19:55:00.490242 mysqllibran-0.0.2/PKG-INFO
--rw-r--r--   0 hikinari  (1000) hikinari  (1000)        6 2024-04-23 19:31:54.000000 mysqllibran-0.0.2/README.md
-drwxr-xr-x   0 hikinari  (1000) hikinari  (1000)        0 2024-04-23 19:55:00.490242 mysqllibran-0.0.2/mysqlLibRan.egg-info/
--rw-r--r--   0 hikinari  (1000) hikinari  (1000)      554 2024-04-23 19:55:00.000000 mysqllibran-0.0.2/mysqlLibRan.egg-info/PKG-INFO
--rw-r--r--   0 hikinari  (1000) hikinari  (1000)      235 2024-04-23 19:55:00.000000 mysqllibran-0.0.2/mysqlLibRan.egg-info/SOURCES.txt
--rw-r--r--   0 hikinari  (1000) hikinari  (1000)        1 2024-04-23 19:55:00.000000 mysqllibran-0.0.2/mysqlLibRan.egg-info/dependency_links.txt
--rw-r--r--   0 hikinari  (1000) hikinari  (1000)       17 2024-04-23 19:55:00.000000 mysqllibran-0.0.2/mysqlLibRan.egg-info/requires.txt
--rw-r--r--   0 hikinari  (1000) hikinari  (1000)        6 2024-04-23 19:55:00.000000 mysqllibran-0.0.2/mysqlLibRan.egg-info/top_level.txt
--rw-r--r--   0 hikinari  (1000) hikinari  (1000)       38 2024-04-23 19:55:00.490242 mysqllibran-0.0.2/setup.cfg
--rw-r--r--   0 hikinari  (1000) hikinari  (1000)      831 2024-04-23 19:49:06.000000 mysqllibran-0.0.2/setup.py
+drwxr-xr-x   0 hikinari  (1000) hikinari  (1000)        0 2024-04-23 20:18:41.606385 mysqllibran-0.0.3/
+drwxr-xr-x   0 hikinari  (1000) hikinari  (1000)        0 2024-04-23 20:18:41.605385 mysqllibran-0.0.3/MyLib/
+-rw-r--r--   0 hikinari  (1000) hikinari  (1000)       19 2024-04-23 19:29:00.000000 mysqllibran-0.0.3/MyLib/__init__.py
+-rw-r--r--   0 hikinari  (1000) hikinari  (1000)     9011 2024-04-23 20:17:34.000000 mysqllibran-0.0.3/MyLib/narek.py
+-rw-r--r--   0 hikinari  (1000) hikinari  (1000)      554 2024-04-23 20:18:41.606385 mysqllibran-0.0.3/PKG-INFO
+-rw-r--r--   0 hikinari  (1000) hikinari  (1000)        6 2024-04-23 19:31:54.000000 mysqllibran-0.0.3/README.md
+drwxr-xr-x   0 hikinari  (1000) hikinari  (1000)        0 2024-04-23 20:18:41.606385 mysqllibran-0.0.3/mysqlLibRan.egg-info/
+-rw-r--r--   0 hikinari  (1000) hikinari  (1000)      554 2024-04-23 20:18:41.000000 mysqllibran-0.0.3/mysqlLibRan.egg-info/PKG-INFO
+-rw-r--r--   0 hikinari  (1000) hikinari  (1000)      235 2024-04-23 20:18:41.000000 mysqllibran-0.0.3/mysqlLibRan.egg-info/SOURCES.txt
+-rw-r--r--   0 hikinari  (1000) hikinari  (1000)        1 2024-04-23 20:18:41.000000 mysqllibran-0.0.3/mysqlLibRan.egg-info/dependency_links.txt
+-rw-r--r--   0 hikinari  (1000) hikinari  (1000)       17 2024-04-23 20:18:41.000000 mysqllibran-0.0.3/mysqlLibRan.egg-info/requires.txt
+-rw-r--r--   0 hikinari  (1000) hikinari  (1000)        6 2024-04-23 20:18:41.000000 mysqllibran-0.0.3/mysqlLibRan.egg-info/top_level.txt
+-rw-r--r--   0 hikinari  (1000) hikinari  (1000)       38 2024-04-23 20:18:41.606385 mysqllibran-0.0.3/setup.cfg
+-rw-r--r--   0 hikinari  (1000) hikinari  (1000)      831 2024-04-23 20:18:10.000000 mysqllibran-0.0.3/setup.py
```

### Comparing `mysqllibran-0.0.2/PKG-INFO` & `mysqllibran-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlLibRan
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is the simplest module for quick work with files.
 Home-page: https://github.com/Narek24IS/my_lib
 Author: Narek24IS
 Author-email: narekd192@gmail.com
 Project-URL: GitHub, https://github.com/Narek24IS/my_lib
 Keywords: files speedfiles
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `mysqllibran-0.0.2/mysqlLibRan.egg-info/PKG-INFO` & `mysqllibran-0.0.3/mysqlLibRan.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlLibRan
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is the simplest module for quick work with files.
 Home-page: https://github.com/Narek24IS/my_lib
 Author: Narek24IS
 Author-email: narekd192@gmail.com
 Project-URL: GitHub, https://github.com/Narek24IS/my_lib
 Keywords: files speedfiles
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `mysqllibran-0.0.2/setup.py` & `mysqllibran-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='mysqlLibRan',
-    version='0.0.2',
+    version='0.0.3',
     author='Narek24IS',
     author_email='narekd192@gmail.com',
     description='This is the simplest module for quick work with files.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/Narek24IS/my_lib',
     packages=find_packages(),
```

