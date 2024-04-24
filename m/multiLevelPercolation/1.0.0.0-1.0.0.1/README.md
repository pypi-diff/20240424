# Comparing `tmp/multiLevelPercolation-1.0.0.0.tar.gz` & `tmp/multiLevelPercolation-1.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiLevelPercolation-1.0.0.0.tar", last modified: Wed Apr 24 11:45:54 2024, max compression
+gzip compressed data, was "multiLevelPercolation-1.0.0.1.tar", last modified: Wed Apr 24 11:46:55 2024, max compression
```

## Comparing `multiLevelPercolation-1.0.0.0.tar` & `multiLevelPercolation-1.0.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-04-24 11:45:54.384762 multiLevelPercolation-1.0.0.0/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1078 2024-04-22 12:11:26.000000 multiLevelPercolation-1.0.0.0/LICENSE
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      645 2024-04-24 11:45:54.384762 multiLevelPercolation-1.0.0.0/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      213 2024-04-22 12:12:25.000000 multiLevelPercolation-1.0.0.0/README.md
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-04-24 11:45:54.380762 multiLevelPercolation-1.0.0.0/multiLevelPercolation/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       57 2024-04-24 11:45:49.000000 multiLevelPercolation-1.0.0.0/multiLevelPercolation/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17112 2024-04-24 11:36:42.000000 multiLevelPercolation-1.0.0.0/multiLevelPercolation/multiLevelPercolation.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)  4000000 2024-04-22 09:38:09.000000 multiLevelPercolation-1.0.0.0/multiLevelPercolation/testData.bin
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-04-24 11:45:54.384762 multiLevelPercolation-1.0.0.0/multiLevelPercolation.egg-info/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      645 2024-04-24 11:45:54.000000 multiLevelPercolation-1.0.0.0/multiLevelPercolation.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      322 2024-04-24 11:45:54.000000 multiLevelPercolation-1.0.0.0/multiLevelPercolation.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2024-04-24 11:45:54.000000 multiLevelPercolation-1.0.0.0/multiLevelPercolation.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       22 2024-04-24 11:45:54.000000 multiLevelPercolation-1.0.0.0/multiLevelPercolation.egg-info/top_level.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       38 2024-04-24 11:45:54.384762 multiLevelPercolation-1.0.0.0/setup.cfg
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      769 2024-04-24 11:45:40.000000 multiLevelPercolation-1.0.0.0/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-04-24 11:46:55.161169 multiLevelPercolation-1.0.0.1/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1078 2024-04-22 12:11:26.000000 multiLevelPercolation-1.0.0.1/LICENSE
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      628 2024-04-24 11:46:55.161169 multiLevelPercolation-1.0.0.1/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      196 2024-04-24 11:46:37.000000 multiLevelPercolation-1.0.0.1/README.md
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-04-24 11:46:55.157169 multiLevelPercolation-1.0.0.1/multiLevelPercolation/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       57 2024-04-24 11:45:49.000000 multiLevelPercolation-1.0.0.1/multiLevelPercolation/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17112 2024-04-24 11:36:42.000000 multiLevelPercolation-1.0.0.1/multiLevelPercolation/multiLevelPercolation.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)  4000000 2024-04-22 09:38:09.000000 multiLevelPercolation-1.0.0.1/multiLevelPercolation/testData.bin
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-04-24 11:46:55.161169 multiLevelPercolation-1.0.0.1/multiLevelPercolation.egg-info/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      628 2024-04-24 11:46:55.000000 multiLevelPercolation-1.0.0.1/multiLevelPercolation.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      322 2024-04-24 11:46:55.000000 multiLevelPercolation-1.0.0.1/multiLevelPercolation.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2024-04-24 11:46:55.000000 multiLevelPercolation-1.0.0.1/multiLevelPercolation.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       22 2024-04-24 11:46:55.000000 multiLevelPercolation-1.0.0.1/multiLevelPercolation.egg-info/top_level.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       38 2024-04-24 11:46:55.161169 multiLevelPercolation-1.0.0.1/setup.cfg
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      769 2024-04-24 11:46:46.000000 multiLevelPercolation-1.0.0.1/setup.py
```

### Comparing `multiLevelPercolation-1.0.0.0/LICENSE` & `multiLevelPercolation-1.0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `multiLevelPercolation-1.0.0.0/multiLevelPercolation/multiLevelPercolation.py` & `multiLevelPercolation-1.0.0.1/multiLevelPercolation/multiLevelPercolation.py`

 * *Files identical despite different names*

### Comparing `multiLevelPercolation-1.0.0.0/multiLevelPercolation/testData.bin` & `multiLevelPercolation-1.0.0.1/multiLevelPercolation/testData.bin`

 * *Files identical despite different names*

### Comparing `multiLevelPercolation-1.0.0.0/setup.py` & `multiLevelPercolation-1.0.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
   
 with open("README.md", "r") as fh: 
     description = fh.read() 
   
 setuptools.setup( 
     name="multiLevelPercolation", 
-    version="1.0.0.0", 
+    version="1.0.0.1", 
     author="Abhishek Harikrishnan", 
     author_email="abhishek.harikrishnan@fu-berlin.de", 
     packages=["multiLevelPercolation"], 
     package_dir={'multiLevelPercolation': 'multiLevelPercolation'},
     package_data={'multiLevelPercolation': ['*.bin']},
     description="Identifying individual unique thresholds for structures educed from scalar fields", 
     long_description=description,
```

