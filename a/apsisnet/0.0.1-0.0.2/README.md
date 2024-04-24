# Comparing `tmp/apsisnet-0.0.1.tar.gz` & `tmp/apsisnet-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apsisnet-0.0.1.tar", last modified: Mon Apr  1 10:32:16 2024, max compression
+gzip compressed data, was "apsisnet-0.0.2.tar", last modified: Wed Apr 24 19:42:27 2024, max compression
```

## Comparing `apsisnet-0.0.1.tar` & `apsisnet-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2024-04-01 10:32:16.131483 apsisnet-0.0.1/
--rw-rw-r--   0 ansary    (1000) ansary    (1000)        0 2024-04-01 00:36:05.000000 apsisnet-0.0.1/CHANGELOG.txt
--rw-rw-r--   0 ansary    (1000) ansary    (1000)       25 2023-04-15 06:54:42.000000 apsisnet-0.0.1/MANIFEST.in
--rw-r--r--   0 ansary    (1000) ansary    (1000)     3718 2024-04-01 10:32:16.131483 apsisnet-0.0.1/PKG-INFO
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     2942 2024-04-01 10:29:41.000000 apsisnet-0.0.1/README.md
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2024-04-01 10:32:16.131483 apsisnet-0.0.1/apsisnet/
--rw-rw-r--   0 ansary    (1000) ansary    (1000)      103 2024-04-01 00:44:16.000000 apsisnet-0.0.1/apsisnet/__init__.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     6128 2024-04-01 01:32:42.000000 apsisnet-0.0.1/apsisnet/apsisnet.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)      386 2024-04-01 00:33:07.000000 apsisnet-0.0.1/apsisnet/modules.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     4648 2024-04-01 00:45:40.000000 apsisnet-0.0.1/apsisnet/utils.py
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2024-04-01 10:32:16.131483 apsisnet-0.0.1/apsisnet.egg-info/
--rw-r--r--   0 ansary    (1000) ansary    (1000)     3718 2024-04-01 10:32:16.000000 apsisnet-0.0.1/apsisnet.egg-info/PKG-INFO
--rw-rw-r--   0 ansary    (1000) ansary    (1000)      305 2024-04-01 10:32:16.000000 apsisnet-0.0.1/apsisnet.egg-info/SOURCES.txt
--rw-rw-r--   0 ansary    (1000) ansary    (1000)        1 2024-04-01 10:32:16.000000 apsisnet-0.0.1/apsisnet.egg-info/dependency_links.txt
--rw-rw-r--   0 ansary    (1000) ansary    (1000)       95 2024-04-01 10:32:16.000000 apsisnet-0.0.1/apsisnet.egg-info/requires.txt
--rw-rw-r--   0 ansary    (1000) ansary    (1000)        9 2024-04-01 10:32:16.000000 apsisnet-0.0.1/apsisnet.egg-info/top_level.txt
--rw-rw-r--   0 ansary    (1000) ansary    (1000)       38 2024-04-01 10:32:16.131483 apsisnet-0.0.1/setup.cfg
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     1271 2024-04-01 00:53:19.000000 apsisnet-0.0.1/setup.py
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2024-04-01 10:32:16.131483 apsisnet-0.0.1/useage/
--rw-rw-r--   0 ansary    (1000) ansary    (1000)      784 2024-04-01 10:30:36.000000 apsisnet-0.0.1/useage/setup_check.py
+drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2024-04-24 19:42:27.004866 apsisnet-0.0.2/
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)       61 2024-04-24 19:40:39.000000 apsisnet-0.0.2/CHANGELOG.txt
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)       25 2023-04-15 06:54:42.000000 apsisnet-0.0.2/MANIFEST.in
+-rw-r--r--   0 ansary    (1000) ansary    (1000)     3788 2024-04-24 19:42:27.004866 apsisnet-0.0.2/PKG-INFO
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     2942 2024-04-01 10:29:41.000000 apsisnet-0.0.2/README.md
+drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2024-04-24 19:42:27.004866 apsisnet-0.0.2/apsisnet/
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)      103 2024-04-01 00:44:16.000000 apsisnet-0.0.2/apsisnet/__init__.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     6128 2024-04-01 01:32:42.000000 apsisnet-0.0.2/apsisnet/apsisnet.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)      386 2024-04-01 00:33:07.000000 apsisnet-0.0.2/apsisnet/modules.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     4648 2024-04-01 00:45:40.000000 apsisnet-0.0.2/apsisnet/utils.py
+drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2024-04-24 19:42:27.004866 apsisnet-0.0.2/apsisnet.egg-info/
+-rw-r--r--   0 ansary    (1000) ansary    (1000)     3788 2024-04-24 19:42:26.000000 apsisnet-0.0.2/apsisnet.egg-info/PKG-INFO
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)      305 2024-04-24 19:42:27.000000 apsisnet-0.0.2/apsisnet.egg-info/SOURCES.txt
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)        1 2024-04-24 19:42:26.000000 apsisnet-0.0.2/apsisnet.egg-info/dependency_links.txt
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)      103 2024-04-24 19:42:26.000000 apsisnet-0.0.2/apsisnet.egg-info/requires.txt
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)        9 2024-04-24 19:42:26.000000 apsisnet-0.0.2/apsisnet.egg-info/top_level.txt
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)       38 2024-04-24 19:42:27.004866 apsisnet-0.0.2/setup.cfg
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     1279 2024-04-24 19:40:49.000000 apsisnet-0.0.2/setup.py
+drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2024-04-24 19:42:27.004866 apsisnet-0.0.2/useage/
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)      784 2024-04-01 10:30:36.000000 apsisnet-0.0.2/useage/setup_check.py
```

### Comparing `apsisnet-0.0.1/PKG-INFO` & `apsisnet-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apsisnet
-Version: 0.0.1
+Version: 0.0.2
 Summary: Bangla Languge Recognizer Toolkit
 Home-page: https://github.com/mnansary/apsisnet.git
 Author: Nazmuddoha Ansary
 Author-email: nazmuddoha.ansary@apsissolutions.com
 License: MIT
 Keywords: ocr,scene ocr,apsisnet
 Classifier: Development Status :: 3 - Alpha
@@ -17,15 +17,15 @@
 Requires-Dist: matplotlib
 Requires-Dist: opencv-python
 Requires-Dist: pandas
 Requires-Dist: tqdm
 Requires-Dist: termcolor
 Requires-Dist: gdown
 Requires-Dist: bnunicodenormalizer
-Requires-Dist: onnxruntime-gpu
+Requires-Dist: onnxruntime-gpu==1.16.0
 
 # apsis-net
 ![](/useage/apsis.png) 
 
 Apsis-net is a Bengali language ocr system for Printed Documents developed at [Apsis Solutions limited](https://apsissolutions.com/)
 
 The full system is focused on bengali text recognition only 
@@ -146,7 +146,10 @@
 # License
 Contents of this repository are restricted to non-commercial research purposes only under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/). 
 
 <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a>
 
 
 
+25-04-2024
+----------------
+* changed onnxruntime-gpu version
```

### Comparing `apsisnet-0.0.1/README.md` & `apsisnet-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `apsisnet-0.0.1/apsisnet/apsisnet.py` & `apsisnet-0.0.2/apsisnet/apsisnet.py`

 * *Files identical despite different names*

### Comparing `apsisnet-0.0.1/apsisnet/utils.py` & `apsisnet-0.0.2/apsisnet/utils.py`

 * *Files identical despite different names*

### Comparing `apsisnet-0.0.1/apsisnet.egg-info/PKG-INFO` & `apsisnet-0.0.2/apsisnet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apsisnet
-Version: 0.0.1
+Version: 0.0.2
 Summary: Bangla Languge Recognizer Toolkit
 Home-page: https://github.com/mnansary/apsisnet.git
 Author: Nazmuddoha Ansary
 Author-email: nazmuddoha.ansary@apsissolutions.com
 License: MIT
 Keywords: ocr,scene ocr,apsisnet
 Classifier: Development Status :: 3 - Alpha
@@ -17,15 +17,15 @@
 Requires-Dist: matplotlib
 Requires-Dist: opencv-python
 Requires-Dist: pandas
 Requires-Dist: tqdm
 Requires-Dist: termcolor
 Requires-Dist: gdown
 Requires-Dist: bnunicodenormalizer
-Requires-Dist: onnxruntime-gpu
+Requires-Dist: onnxruntime-gpu==1.16.0
 
 # apsis-net
 ![](/useage/apsis.png) 
 
 Apsis-net is a Bengali language ocr system for Printed Documents developed at [Apsis Solutions limited](https://apsissolutions.com/)
 
 The full system is focused on bengali text recognition only 
@@ -146,7 +146,10 @@
 # License
 Contents of this repository are restricted to non-commercial research purposes only under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/). 
 
 <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a>
 
 
 
+25-04-2024
+----------------
+* changed onnxruntime-gpu version
```

### Comparing `apsisnet-0.0.1/setup.py` & `apsisnet-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   'Operating System :: POSIX :: Linux',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='apsisnet',
-  version='0.0.1',
+  version='0.0.2',
   description='Bangla Languge Recognizer Toolkit',
   long_description=open('README.md',encoding='utf-8').read() + '\n\n' + open('CHANGELOG.txt',encoding='utf-8').read(),
   long_description_content_type='text/markdown',
   url='https://github.com/mnansary/apsisnet.git',  
   author='Nazmuddoha Ansary',
   author_email='nazmuddoha.ansary@apsissolutions.com',
   license='MIT', 
@@ -30,9 +30,9 @@
                     "matplotlib", 
                     "opencv-python",
                     "pandas",
                     "tqdm",
                     "termcolor",
                     "gdown",
                     "bnunicodenormalizer",
-                    "onnxruntime-gpu"]
+                    "onnxruntime-gpu==1.16.0"]
 )
```

### Comparing `apsisnet-0.0.1/useage/setup_check.py` & `apsisnet-0.0.2/useage/setup_check.py`

 * *Files identical despite different names*

