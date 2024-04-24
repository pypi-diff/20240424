# Comparing `tmp/boxcounting-1.0.0.2.tar.gz` & `tmp/boxcounting-1.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boxcounting-1.0.0.2.tar", last modified: Wed Nov 29 04:22:20 2023, max compression
+gzip compressed data, was "boxcounting-1.0.0.3.tar", last modified: Wed Apr 24 08:00:22 2024, max compression
```

## Comparing `boxcounting-1.0.0.2.tar` & `boxcounting-1.0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-11-29 04:22:20.083353 boxcounting-1.0.0.2/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1078 2023-11-27 10:47:38.000000 boxcounting-1.0.0.2/LICENSE
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      657 2023-11-29 04:22:20.083353 boxcounting-1.0.0.2/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      218 2023-11-28 10:30:20.000000 boxcounting-1.0.0.2/README.md
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-11-29 04:22:20.083353 boxcounting-1.0.0.2/boxcounting/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1024 2023-11-28 09:57:51.000000 boxcounting-1.0.0.2/boxcounting/1D_random_cantor.bin
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)   360000 2023-11-28 10:05:24.000000 boxcounting-1.0.0.2/boxcounting/2D_apollonian_gasket.bin
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    32768 2023-11-27 13:29:44.000000 boxcounting-1.0.0.2/boxcounting/3D_random_cantor.bin
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       34 2023-11-29 04:15:54.000000 boxcounting-1.0.0.2/boxcounting/__init__.py
--rwxrwxrwx   0 abhishek  (1000) abhishek  (1000)     5299 2023-11-28 09:47:54.000000 boxcounting-1.0.0.2/boxcounting/boxcounting.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2695 2023-11-28 10:46:43.000000 boxcounting-1.0.0.2/boxcounting/runTests.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-11-29 04:22:20.083353 boxcounting-1.0.0.2/boxcounting.egg-info/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      657 2023-11-29 04:22:20.000000 boxcounting-1.0.0.2/boxcounting.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      344 2023-11-29 04:22:20.000000 boxcounting-1.0.0.2/boxcounting.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-11-29 04:22:20.000000 boxcounting-1.0.0.2/boxcounting.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       12 2023-11-29 04:22:20.000000 boxcounting-1.0.0.2/boxcounting.egg-info/top_level.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       38 2023-11-29 04:22:20.083353 boxcounting-1.0.0.2/setup.cfg
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      753 2023-11-29 04:22:16.000000 boxcounting-1.0.0.2/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-04-24 08:00:22.805280 boxcounting-1.0.0.3/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1078 2023-11-27 10:47:38.000000 boxcounting-1.0.0.3/LICENSE
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      657 2024-04-24 08:00:22.805280 boxcounting-1.0.0.3/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      218 2023-11-28 10:30:20.000000 boxcounting-1.0.0.3/README.md
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-04-24 08:00:22.805280 boxcounting-1.0.0.3/boxcounting/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1024 2023-11-28 09:57:51.000000 boxcounting-1.0.0.3/boxcounting/1D_random_cantor.bin
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)   360000 2023-11-28 10:05:24.000000 boxcounting-1.0.0.3/boxcounting/2D_apollonian_gasket.bin
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    32768 2023-11-27 13:29:44.000000 boxcounting-1.0.0.3/boxcounting/3D_random_cantor.bin
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       34 2023-11-29 04:15:54.000000 boxcounting-1.0.0.3/boxcounting/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5291 2024-04-24 07:48:18.000000 boxcounting-1.0.0.3/boxcounting/boxcounting.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2697 2024-04-24 07:57:35.000000 boxcounting-1.0.0.3/boxcounting/runTests.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2024-04-24 08:00:22.805280 boxcounting-1.0.0.3/boxcounting.egg-info/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      657 2024-04-24 08:00:22.000000 boxcounting-1.0.0.3/boxcounting.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      344 2024-04-24 08:00:22.000000 boxcounting-1.0.0.3/boxcounting.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2024-04-24 08:00:22.000000 boxcounting-1.0.0.3/boxcounting.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       12 2024-04-24 08:00:22.000000 boxcounting-1.0.0.3/boxcounting.egg-info/top_level.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       38 2024-04-24 08:00:22.805280 boxcounting-1.0.0.3/setup.cfg
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      753 2024-04-24 08:00:19.000000 boxcounting-1.0.0.3/setup.py
```

### Comparing `boxcounting-1.0.0.2/LICENSE` & `boxcounting-1.0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `boxcounting-1.0.0.2/PKG-INFO` & `boxcounting-1.0.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxcounting
-Version: 1.0.0.2
+Version: 1.0.0.3
 Summary: A python port of the MATLAB boxcount to calculate the     fractal (box-counting) dimension of 1D, 2D or 3D data
 Home-page: https://github.com/Phoenixfire1081/fractaldimension
 Author: Abhishek Harikrishnan
 Author-email: abhishek.harikrishnan@fu-berlin.de
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `boxcounting-1.0.0.2/boxcounting/boxcounting.py` & `boxcounting-1.0.0.3/boxcounting/boxcounting.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,10 +183,10 @@
 			xlen, ylen, zlen = np.shape(self.paddedData)
 			n = self.computeFast3(xlen, ylen, zlen, self.paddedData, self.p, self.width, reverse_range, n, r)
 			
 		else:
 			print('Exceeded 3 dimensions. Not implemented.')
 			raise NotImplementedError
 		
-		df = - np.gradient(np.log(n)) / np.gradient(np.log(r))
+		df = - np.diff(np.log(n)) / np.diff(np.log(r))
 		
 		return n, r, df
```

### Comparing `boxcounting-1.0.0.2/boxcounting/runTests.py` & `boxcounting-1.0.0.3/boxcounting/runTests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import array
 import numpy as np
-from box_count import boxCount
+from boxcounting import boxCount
 import unittest
 
 #---------------------------------------------------------------------#
 
 # Author: Abhishek Harikrishnan
 # Email: abhishek.harikrishnan@fu-berlin.de
-# Last updated: 28-11-2023
+# Last updated: 24-04-2024
 # Tests to ensure correct working of boxCount python module
 
 #---------------------------------------------------------------------#
 
 class TestBoxCount(unittest.TestCase):
 	
 	'''
```

### Comparing `boxcounting-1.0.0.2/boxcounting.egg-info/PKG-INFO` & `boxcounting-1.0.0.3/boxcounting.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxcounting
-Version: 1.0.0.2
+Version: 1.0.0.3
 Summary: A python port of the MATLAB boxcount to calculate the     fractal (box-counting) dimension of 1D, 2D or 3D data
 Home-page: https://github.com/Phoenixfire1081/fractaldimension
 Author: Abhishek Harikrishnan
 Author-email: abhishek.harikrishnan@fu-berlin.de
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `boxcounting-1.0.0.2/setup.py` & `boxcounting-1.0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
   
 with open("README.md", "r") as fh: 
     description = fh.read() 
   
 setuptools.setup( 
     name="boxcounting", 
-    version="1.0.0.2", 
+    version="1.0.0.3", 
     author="Abhishek Harikrishnan", 
     author_email="abhishek.harikrishnan@fu-berlin.de", 
     packages=["boxcounting"], 
     package_dir={'boxcounting': 'boxcounting'},
     package_data={'boxcounting': ['*.bin', 'runTests.py']},
     description="A python port of the MATLAB boxcount to calculate the \
     fractal (box-counting) dimension of 1D, 2D or 3D data",
```

