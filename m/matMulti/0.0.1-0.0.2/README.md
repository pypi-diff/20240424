# Comparing `tmp/matMulti-0.0.1.tar.gz` & `tmp/matMulti-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matMulti-0.0.1.tar", last modified: Wed Apr 24 18:48:07 2024, max compression
+gzip compressed data, was "matMulti-0.0.2.tar", last modified: Wed Apr 24 19:24:26 2024, max compression
```

## Comparing `matMulti-0.0.1.tar` & `matMulti-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 sajal     (1000) sajal     (1000)        0 2024-04-24 18:48:07.049335 matMulti-0.0.1/
--rw-rw-r--   0 sajal     (1000) sajal     (1000)     1153 2024-04-24 18:33:02.000000 matMulti-0.0.1/LICENSE.txt
--rw-rw-r--   0 sajal     (1000) sajal     (1000)       44 2024-04-24 18:32:29.000000 matMulti-0.0.1/MANIFEST.in
--rw-rw-r--   0 sajal     (1000) sajal     (1000)     1246 2024-04-24 18:48:07.049335 matMulti-0.0.1/PKG-INFO
--rw-rw-r--   0 sajal     (1000) sajal     (1000)      627 2024-04-24 18:30:44.000000 matMulti-0.0.1/README.txt
-drwxrwxr-x   0 sajal     (1000) sajal     (1000)        0 2024-04-24 18:48:07.049335 matMulti-0.0.1/matMulti.egg-info/
--rw-rw-r--   0 sajal     (1000) sajal     (1000)     1246 2024-04-24 18:48:06.000000 matMulti-0.0.1/matMulti.egg-info/PKG-INFO
--rw-rw-r--   0 sajal     (1000) sajal     (1000)      171 2024-04-24 18:48:06.000000 matMulti-0.0.1/matMulti.egg-info/SOURCES.txt
--rw-rw-r--   0 sajal     (1000) sajal     (1000)        1 2024-04-24 18:48:06.000000 matMulti-0.0.1/matMulti.egg-info/dependency_links.txt
--rw-rw-r--   0 sajal     (1000) sajal     (1000)        1 2024-04-24 18:48:06.000000 matMulti-0.0.1/matMulti.egg-info/top_level.txt
--rw-rw-r--   0 sajal     (1000) sajal     (1000)       38 2024-04-24 18:48:07.049335 matMulti-0.0.1/setup.cfg
--rw-rw-r--   0 sajal     (1000) sajal     (1000)      778 2024-04-24 18:46:09.000000 matMulti-0.0.1/setup.py
+drwxrwxr-x   0 sajal     (1000) sajal     (1000)        0 2024-04-24 19:24:26.792286 matMulti-0.0.2/
+-rw-rw-r--   0 sajal     (1000) sajal     (1000)     1153 2024-04-24 18:33:02.000000 matMulti-0.0.2/LICENSE.txt
+-rw-rw-r--   0 sajal     (1000) sajal     (1000)       44 2024-04-24 18:32:29.000000 matMulti-0.0.2/MANIFEST.in
+-rw-rw-r--   0 sajal     (1000) sajal     (1000)     1247 2024-04-24 19:24:26.792286 matMulti-0.0.2/PKG-INFO
+-rw-rw-r--   0 sajal     (1000) sajal     (1000)      628 2024-04-24 19:19:26.000000 matMulti-0.0.2/README.txt
+drwxrwxr-x   0 sajal     (1000) sajal     (1000)        0 2024-04-24 19:24:26.792286 matMulti-0.0.2/matMulti.egg-info/
+-rw-rw-r--   0 sajal     (1000) sajal     (1000)     1247 2024-04-24 19:24:26.000000 matMulti-0.0.2/matMulti.egg-info/PKG-INFO
+-rw-rw-r--   0 sajal     (1000) sajal     (1000)      171 2024-04-24 19:24:26.000000 matMulti-0.0.2/matMulti.egg-info/SOURCES.txt
+-rw-rw-r--   0 sajal     (1000) sajal     (1000)        1 2024-04-24 19:24:26.000000 matMulti-0.0.2/matMulti.egg-info/dependency_links.txt
+-rw-rw-r--   0 sajal     (1000) sajal     (1000)        1 2024-04-24 19:24:26.000000 matMulti-0.0.2/matMulti.egg-info/top_level.txt
+-rw-rw-r--   0 sajal     (1000) sajal     (1000)       38 2024-04-24 19:24:26.792286 matMulti-0.0.2/setup.cfg
+-rw-rw-r--   0 sajal     (1000) sajal     (1000)      778 2024-04-24 19:23:11.000000 matMulti-0.0.2/setup.py
```

### Comparing `matMulti-0.0.1/LICENSE.txt` & `matMulti-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `matMulti-0.0.1/PKG-INFO` & `matMulti-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matMulti
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to multiply two matrix of any dimensions
 Home-page: https://github.com/SajalDasShovon/Own-Simple-Python-Package
 Author: Sajal Das Shovon
 Author-email: shovon030cse.kuet@gmail.com
 License: MIT
 Keywords: matrixMultiplier
 Platform: UNKNOWN
@@ -22,21 +22,21 @@
 This package provides a simple and efficient way to multiply two matrices of any dimensions. 
 Whether you're dealing with small matrices or large ones, this package offers a reliable 
 solution to perform matrix multiplication with ease.
 
 1. Installation:
 
 ```
-pip install pymatrix
+pip install matMulti
 ```
 
 2. Generate multiplication result:
 
 ```
-from pymatrix import product
+from matMulti import product 
 ```
 
 
 Features
 --Supports matrix multiplication of any dimensions.
 --Efficient algorithm implementation for fast computation.
 --Works with Python 3.
```

### Comparing `matMulti-0.0.1/README.txt` & `matMulti-0.0.2/README.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 This package provides a simple and efficient way to multiply two matrices of any dimensions. 
 Whether you're dealing with small matrices or large ones, this package offers a reliable 
 solution to perform matrix multiplication with ease.
 
 1. Installation:
 
 ```
-pip install pymatrix
+pip install matMulti
 ```
 
 2. Generate multiplication result:
 
 ```
-from pymatrix import product
+from matMulti import product 
 ```
 
 
 Features
 --Supports matrix multiplication of any dimensions.
 --Efficient algorithm implementation for fast computation.
 --Works with Python 3.
```

### Comparing `matMulti-0.0.1/matMulti.egg-info/PKG-INFO` & `matMulti-0.0.2/matMulti.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matMulti
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to multiply two matrix of any dimensions
 Home-page: https://github.com/SajalDasShovon/Own-Simple-Python-Package
 Author: Sajal Das Shovon
 Author-email: shovon030cse.kuet@gmail.com
 License: MIT
 Keywords: matrixMultiplier
 Platform: UNKNOWN
@@ -22,21 +22,21 @@
 This package provides a simple and efficient way to multiply two matrices of any dimensions. 
 Whether you're dealing with small matrices or large ones, this package offers a reliable 
 solution to perform matrix multiplication with ease.
 
 1. Installation:
 
 ```
-pip install pymatrix
+pip install matMulti
 ```
 
 2. Generate multiplication result:
 
 ```
-from pymatrix import product
+from matMulti import product 
 ```
 
 
 Features
 --Supports matrix multiplication of any dimensions.
 --Efficient algorithm implementation for fast computation.
 --Works with Python 3.
```

### Comparing `matMulti-0.0.1/setup.py` & `matMulti-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   'Operating System :: OS Independent',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='matMulti',
-  version='0.0.1',
+  version='0.0.2',
   description='A package to multiply two matrix of any dimensions',
   long_description=open('README.txt').read(),
   long_description_content_type='text/plain',
   url='https://github.com/SajalDasShovon/Own-Simple-Python-Package',  
   author='Sajal Das Shovon',
   author_email='shovon030cse.kuet@gmail.com',
   license='MIT',
```

