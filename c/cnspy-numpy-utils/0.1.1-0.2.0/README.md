# Comparing `tmp/cnspy_numpy_utils-0.1.1.tar.gz` & `tmp/cnspy_numpy_utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jungr/workspace/CNS/VIO_Evaluation_Framework/py3_pkgs/cnspy_eco_system_test/pkgs/a_numpy_utils/dist/tmp8e4bfthx/cnspy_num", last modified: Sat Mar 20 14:23:02 2021, max compression
+gzip compressed data, was "cnspy_numpy_utils-0.2.0.tar", last modified: Wed Apr 24 12:16:10 2024, max compression
```

## Comparing `cnspy_numpy_utils-0.1.1.tar` & `cnspy_numpy_utils-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:23:02.484698 cnspy_numpy_utils-0.1.1/
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     2153 2021-03-20 14:23:02.484698 cnspy_numpy_utils-0.1.1/PKG-INFO
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     1192 2021-03-20 14:21:27.000000 cnspy_numpy_utils-0.1.1/README.md
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:23:02.484698 cnspy_numpy_utils-0.1.1/cnspy_numpy_utils/
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 12:20:48.000000 cnspy_numpy_utils-0.1.1/cnspy_numpy_utils/__init__.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     2186 2021-03-20 12:20:48.000000 cnspy_numpy_utils-0.1.1/cnspy_numpy_utils/accumulated_distance.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     2143 2021-03-20 12:20:48.000000 cnspy_numpy_utils-0.1.1/cnspy_numpy_utils/matrix_conversions.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     2337 2021-03-20 12:20:48.000000 cnspy_numpy_utils-0.1.1/cnspy_numpy_utils/numpy_statistics.py
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:23:02.484698 cnspy_numpy_utils-0.1.1/cnspy_numpy_utils.egg-info/
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     2153 2021-03-20 14:23:02.000000 cnspy_numpy_utils-0.1.1/cnspy_numpy_utils.egg-info/PKG-INFO
--rw-rw-r--   0 jungr     (1000) jungr     (1000)      453 2021-03-20 14:23:02.000000 cnspy_numpy_utils-0.1.1/cnspy_numpy_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)        1 2021-03-20 14:23:02.000000 cnspy_numpy_utils-0.1.1/cnspy_numpy_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)        6 2021-03-20 14:23:02.000000 cnspy_numpy_utils-0.1.1/cnspy_numpy_utils.egg-info/requires.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)       23 2021-03-20 14:23:02.000000 cnspy_numpy_utils-0.1.1/cnspy_numpy_utils.egg-info/top_level.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)       38 2021-03-20 14:23:02.484698 cnspy_numpy_utils-0.1.1/setup.cfg
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     1246 2021-03-20 14:21:27.000000 cnspy_numpy_utils-0.1.1/setup.py
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:23:02.484698 cnspy_numpy_utils-0.1.1/test/
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 12:20:48.000000 cnspy_numpy_utils-0.1.1/test/__init__.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     1638 2021-03-20 12:20:48.000000 cnspy_numpy_utils-0.1.1/test/test_MatrixConversion.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     2122 2021-03-20 12:20:48.000000 cnspy_numpy_utils-0.1.1/test/test_accumulated_distance.py
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:16:10.121165 cnspy_numpy_utils-0.2.0/
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)    35149 2022-05-30 14:10:28.000000 cnspy_numpy_utils-0.2.0/LICENCE
+-rw-r--r--   0 jungr     (1000) jungr     (1000)     1983 2024-04-24 12:16:10.121165 cnspy_numpy_utils-0.2.0/PKG-INFO
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     1315 2022-05-30 14:10:28.000000 cnspy_numpy_utils-0.2.0/README.md
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:16:10.117165 cnspy_numpy_utils-0.2.0/cnspy_numpy_utils/
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2022-05-30 14:10:28.000000 cnspy_numpy_utils-0.2.0/cnspy_numpy_utils/__init__.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)     2186 2022-05-30 14:10:28.000000 cnspy_numpy_utils-0.2.0/cnspy_numpy_utils/accumulated_distance.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)     2507 2024-04-24 11:41:49.000000 cnspy_numpy_utils-0.2.0/cnspy_numpy_utils/matrix_conversions.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)     3072 2024-04-24 11:41:49.000000 cnspy_numpy_utils-0.2.0/cnspy_numpy_utils/numpy_statistics.py
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:16:10.121165 cnspy_numpy_utils-0.2.0/cnspy_numpy_utils.egg-info/
+-rw-r--r--   0 jungr     (1000) jungr     (1000)     1983 2024-04-24 12:16:10.000000 cnspy_numpy_utils-0.2.0/cnspy_numpy_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)      491 2024-04-24 12:16:10.000000 cnspy_numpy_utils-0.2.0/cnspy_numpy_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)        1 2024-04-24 12:16:10.000000 cnspy_numpy_utils-0.2.0/cnspy_numpy_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)        6 2024-04-24 12:16:10.000000 cnspy_numpy_utils-0.2.0/cnspy_numpy_utils.egg-info/requires.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)       23 2024-04-24 12:16:10.000000 cnspy_numpy_utils-0.2.0/cnspy_numpy_utils.egg-info/top_level.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)       38 2024-04-24 12:16:10.121165 cnspy_numpy_utils-0.2.0/setup.cfg
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     1246 2022-05-30 14:10:28.000000 cnspy_numpy_utils-0.2.0/setup.py
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:16:10.121165 cnspy_numpy_utils-0.2.0/test/
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2022-05-30 14:10:28.000000 cnspy_numpy_utils-0.2.0/test/__init__.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     1638 2022-05-30 14:10:28.000000 cnspy_numpy_utils-0.2.0/test/test_MatrixConversion.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     2122 2022-05-30 14:10:28.000000 cnspy_numpy_utils-0.2.0/test/test_accumulated_distance.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     1444 2024-04-24 11:41:49.000000 cnspy_numpy_utils-0.2.0/test/test_numpy_statistics.py
```

### Comparing `cnspy_numpy_utils-0.1.1/PKG-INFO` & `cnspy_numpy_utils-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 Metadata-Version: 2.1
 Name: cnspy_numpy_utils
-Version: 0.1.1
+Version: 0.2.0
 Summary: Some utility functions for numpy data types
 Home-page: https://github.com/aau-cns/cnspy_numpy_utils/
 Author: Roland Jung
 Author-email: roland.jung@aau.at
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/aau-cns/cnspy_numpy_utils/issues
-Description: # cnspy_numpy_utils Package
-        
-        A package holding useful scripts based on the numpy package, that cannot be associated to any other (dangling code, that is used in different places). 
-        
-        Most important functions:
-        1. [tri_vec_to_mat(tri_vec, n=None)](./cnspy_numpy_utils/matrix_conversions.py)
-        1. [mat_to_tri_vec(P)](./cnspy_numpy_utils/matrix_conversions.py)
-        1. [accumulated_distance(p_vec)](./cnspy_numpy_utils/accumulated_distance.py)
-        1. [total_distance(p_vec)](./cnspy_numpy_utils/accumulated_distance.py)
-        1. [numpy_statistics(vNumpy](./cnspy_numpy_utils/numpy_statistics.py)
-        1. [print_statistics(metrics](./cnspy_numpy_utils/numpy_statistics.py)
-        
-        ## Installation
-        
-        Install the current code base from GitHub and pip install a link to that cloned copy
-        ```
-        git clone https://github.com/aau-cns/cnspy_numpy_utils.git
-        cd cnspy_numpy_utils
-        pip install -e .
-        ```
-        
-        
-        ## Dependencies
-        
-        It is part of the [cnspy eco-system](hhttps://github.com/aau-cns/cnspy_eco_system_test) of the [cns-github](https://github.com/aau-cns) group.  
-        
-        * [numpy]()
-        
-        
-        
-        ## License
-        
-        Software License Agreement (GNU GPLv3  License), refer to the LICENSE file.
-        
-        *Sharing is caring!* - [Roland Jung](https://github.com/jungr-ait)  
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENCE
+Requires-Dist: numpy
+
+# cnspy_numpy_utils Package
+
+A package holding useful scripts based on the numpy package, that cannot be associated to any other (dangling code, that is used in different places). 
+
+Most important functions:
+1. [tri_vec_to_mat(tri_vec, n=None)](./cnspy_numpy_utils/matrix_conversions.py)
+1. [mat_to_tri_vec(P)](./cnspy_numpy_utils/matrix_conversions.py)
+1. [accumulated_distance(p_vec)](./cnspy_numpy_utils/accumulated_distance.py)
+1. [total_distance(p_vec)](./cnspy_numpy_utils/accumulated_distance.py)
+1. [numpy_statistics(vNumpy](./cnspy_numpy_utils/numpy_statistics.py)
+1. [print_statistics(metrics](./cnspy_numpy_utils/numpy_statistics.py)
+
+## Installation
+
+Install the current code base from GitHub and pip install a link to that cloned copy
+```
+git clone https://github.com/aau-cns/cnspy_numpy_utils.git
+cd cnspy_numpy_utils
+pip install -e .
+```
+or the [official package](https://pypi.org/project/cnspy-numpy-utils/) via
+```commandline
+pip install cnspy-numpy-utils
+```
+
+## Dependencies
+
+It is part of the [cnspy eco-system](hhttps://github.com/aau-cns/cnspy_eco_system_test) of the [cns-github](https://github.com/aau-cns) group.  
+
+* [numpy]()
+
+
+
+## License
+
+Software License Agreement (GNU GPLv3  License), refer to the LICENSE file.
+
+*Sharing is caring!* - [Roland Jung](https://github.com/jungr-ait)  
+
```

### Comparing `cnspy_numpy_utils-0.1.1/README.md` & `cnspy_numpy_utils-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,18 @@
 
 Install the current code base from GitHub and pip install a link to that cloned copy
 ```
 git clone https://github.com/aau-cns/cnspy_numpy_utils.git
 cd cnspy_numpy_utils
 pip install -e .
 ```
-
+or the [official package](https://pypi.org/project/cnspy-numpy-utils/) via
+```commandline
+pip install cnspy-numpy-utils
+```
 
 ## Dependencies
 
 It is part of the [cnspy eco-system](hhttps://github.com/aau-cns/cnspy_eco_system_test) of the [cns-github](https://github.com/aau-cns) group.  
 
 * [numpy]()
```

### Comparing `cnspy_numpy_utils-0.1.1/cnspy_numpy_utils/accumulated_distance.py` & `cnspy_numpy_utils-0.2.0/cnspy_numpy_utils/accumulated_distance.py`

 * *Files identical despite different names*

### Comparing `cnspy_numpy_utils-0.1.1/cnspy_numpy_utils/matrix_conversions.py` & `cnspy_numpy_utils-0.2.0/cnspy_numpy_utils/matrix_conversions.py`

 * *Files 18% similar despite different names*

```diff
@@ -53,17 +53,21 @@
 
 
 def mat_to_tri_vec(P):
     """"
     converts an upper triangular matrix of a symmetric matrix into a vector.
 
     Example:
+    >> import numpy as np
+    >> from cnspy_numpy_utils.matrix_conversions import *
     >> M = np.array([[11, 12, 13], [21, 22, 23], [31, 32, 33]])
     >> v = mat_to_tri_vec(P=M) # [11 12 13 22 23 33]
-
+    >> M2 = np.array([[11, 12, 13, 14, 15 ,16], [21, 22, 23, 24, 25, 26], [31, 32, 33, 34, 35, 36], [41,42,43,44,45,46], [51,52,53,54,55,56], [61,62,63,64,65,66]])
+    >> v2 = mat_to_tri_vec(P=M2) # [11 12 13 14 15 16 22 23 24 25 26 33 34 35 36 44 45 46 55 56 66]
+    >> print(v2)
 
     Input:
     P -- numpy.ndarray, square matrix [NxN]
 
     Output:
     tri_vec -- numpy.ndarray, vector [1xM],
     """
```

### Comparing `cnspy_numpy_utils-0.1.1/cnspy_numpy_utils/numpy_statistics.py` & `cnspy_numpy_utils-0.2.0/cnspy_numpy_utils/numpy_statistics.py`

 * *Files 27% similar despite different names*

```diff
@@ -22,38 +22,49 @@
 import numpy as np
 
 
 def numpy_statistics(vNumpy, prefix=''):
     if prefix:
         metrics = {
             prefix + '.pairs': len(vNumpy),
-            prefix + '.rmse': np.sqrt(np.dot(vNumpy, vNumpy) / len(vNumpy)),
-            prefix + '.mean': np.mean(vNumpy),
+            prefix + '.rmse': np.sqrt(np.square(vNumpy).mean(axis=0)),
+            prefix + '.mean': np.mean(vNumpy, axis=1),
             prefix + '.median': np.median(vNumpy),
             prefix + '.std': np.std(vNumpy),
             prefix + '.var': np.square(np.std(vNumpy)),
             prefix + '.min': np.min(vNumpy),
             prefix + '.max': np.max(vNumpy)
         }
     else:
         metrics = {
             'pairs': len(vNumpy),
-            'rmse': np.sqrt(np.dot(vNumpy, vNumpy) / len(vNumpy)),
-            'mean': np.mean(vNumpy),
-            'median': np.median(vNumpy),
-            'std': np.std(vNumpy),
-            'var': np.square(np.std(vNumpy)),
-            'min': np.min(vNumpy),
-            'max': np.max(vNumpy)
+            'rmse': np.sqrt(np.square(vNumpy).mean(axis=0)),
+            'mean': np.mean(vNumpy, axis=0),
+            'median': np.median(vNumpy, axis=0),
+            'std': np.std(vNumpy, axis=0),
+            'var': np.square(np.std(vNumpy, axis=0)),
+            'min': np.min(vNumpy, axis=0),
+            'max': np.max(vNumpy, axis=0)
         }
     return metrics
 
 
-def print_statistics(metrics, desc='error'):
-    print("samples   %d" % (metrics['pairs']))
-    print("%s.rmse   %f m" % (str(desc), metrics['rmse']))
-    print("%s.mean   %f m" % (str(desc), metrics['mean']))
-    print("%s.median %f m" % (str(desc), metrics['median']))
-    print("%s.std    %f m" % (str(desc), metrics['std']))
-    print("%s.var    %f m" % (str(desc), metrics['var']))
-    print("%s.min    %f m" % (str(desc), metrics['min']))
-    print("%s.max    %f m" % (str(desc), metrics['max']))
+def print_statistics(metrics, desc='error', file=None):
+    if file:
+        print("samples   %d" % (metrics['pairs']), file=file)
+        print("%s.rmse   %s" % (str(desc), str(metrics['rmse'])), file=file)
+        print("%s.mean   %s" % (str(desc), str(metrics['mean'])), file=file)
+        print("%s.median %s" % (str(desc), str(metrics['median'])), file=file)
+        print("%s.std    %s" % (str(desc), str(metrics['std'])), file=file)
+        print("%s.var    %s" % (str(desc), str(metrics['var'])), file=file)
+        print("%s.min    %s" % (str(desc), str(metrics['min'])), file=file)
+        print("%s.max    %s" % (str(desc), str(metrics['max'])), file=file)
+    else:
+        print("samples   %d" % (metrics['pairs']))
+        print("%s.rmse   %s" % (str(desc), str(metrics['rmse'])))
+        print("%s.mean   %s" % (str(desc), str(metrics['mean'])))
+        print("%s.median %s" % (str(desc), str(metrics['median'])))
+        print("%s.std    %s" % (str(desc), str(metrics['std'])))
+        print("%s.var    %s" % (str(desc), str(metrics['var'])))
+        print("%s.min    %s" % (str(desc), str(metrics['min'])))
+        print("%s.max    %s" % (str(desc), str(metrics['max'])))
+str()
```

### Comparing `cnspy_numpy_utils-0.1.1/cnspy_numpy_utils.egg-info/PKG-INFO` & `cnspy_numpy_utils-0.2.0/cnspy_numpy_utils.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 Metadata-Version: 2.1
-Name: cnspy-numpy-utils
-Version: 0.1.1
+Name: cnspy_numpy_utils
+Version: 0.2.0
 Summary: Some utility functions for numpy data types
 Home-page: https://github.com/aau-cns/cnspy_numpy_utils/
 Author: Roland Jung
 Author-email: roland.jung@aau.at
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/aau-cns/cnspy_numpy_utils/issues
-Description: # cnspy_numpy_utils Package
-        
-        A package holding useful scripts based on the numpy package, that cannot be associated to any other (dangling code, that is used in different places). 
-        
-        Most important functions:
-        1. [tri_vec_to_mat(tri_vec, n=None)](./cnspy_numpy_utils/matrix_conversions.py)
-        1. [mat_to_tri_vec(P)](./cnspy_numpy_utils/matrix_conversions.py)
-        1. [accumulated_distance(p_vec)](./cnspy_numpy_utils/accumulated_distance.py)
-        1. [total_distance(p_vec)](./cnspy_numpy_utils/accumulated_distance.py)
-        1. [numpy_statistics(vNumpy](./cnspy_numpy_utils/numpy_statistics.py)
-        1. [print_statistics(metrics](./cnspy_numpy_utils/numpy_statistics.py)
-        
-        ## Installation
-        
-        Install the current code base from GitHub and pip install a link to that cloned copy
-        ```
-        git clone https://github.com/aau-cns/cnspy_numpy_utils.git
-        cd cnspy_numpy_utils
-        pip install -e .
-        ```
-        
-        
-        ## Dependencies
-        
-        It is part of the [cnspy eco-system](hhttps://github.com/aau-cns/cnspy_eco_system_test) of the [cns-github](https://github.com/aau-cns) group.  
-        
-        * [numpy]()
-        
-        
-        
-        ## License
-        
-        Software License Agreement (GNU GPLv3  License), refer to the LICENSE file.
-        
-        *Sharing is caring!* - [Roland Jung](https://github.com/jungr-ait)  
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENCE
+Requires-Dist: numpy
+
+# cnspy_numpy_utils Package
+
+A package holding useful scripts based on the numpy package, that cannot be associated to any other (dangling code, that is used in different places). 
+
+Most important functions:
+1. [tri_vec_to_mat(tri_vec, n=None)](./cnspy_numpy_utils/matrix_conversions.py)
+1. [mat_to_tri_vec(P)](./cnspy_numpy_utils/matrix_conversions.py)
+1. [accumulated_distance(p_vec)](./cnspy_numpy_utils/accumulated_distance.py)
+1. [total_distance(p_vec)](./cnspy_numpy_utils/accumulated_distance.py)
+1. [numpy_statistics(vNumpy](./cnspy_numpy_utils/numpy_statistics.py)
+1. [print_statistics(metrics](./cnspy_numpy_utils/numpy_statistics.py)
+
+## Installation
+
+Install the current code base from GitHub and pip install a link to that cloned copy
+```
+git clone https://github.com/aau-cns/cnspy_numpy_utils.git
+cd cnspy_numpy_utils
+pip install -e .
+```
+or the [official package](https://pypi.org/project/cnspy-numpy-utils/) via
+```commandline
+pip install cnspy-numpy-utils
+```
+
+## Dependencies
+
+It is part of the [cnspy eco-system](hhttps://github.com/aau-cns/cnspy_eco_system_test) of the [cns-github](https://github.com/aau-cns) group.  
+
+* [numpy]()
+
+
+
+## License
+
+Software License Agreement (GNU GPLv3  License), refer to the LICENSE file.
+
+*Sharing is caring!* - [Roland Jung](https://github.com/jungr-ait)  
+
```

### Comparing `cnspy_numpy_utils-0.1.1/setup.py` & `cnspy_numpy_utils-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `cnspy_numpy_utils-0.1.1/test/test_MatrixConversion.py` & `cnspy_numpy_utils-0.2.0/test/test_MatrixConversion.py`

 * *Files identical despite different names*

### Comparing `cnspy_numpy_utils-0.1.1/test/test_accumulated_distance.py` & `cnspy_numpy_utils-0.2.0/test/test_accumulated_distance.py`

 * *Files identical despite different names*

