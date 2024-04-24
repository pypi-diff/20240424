# Comparing `tmp/clump-python-0.1.tar.gz` & `tmp/clump-python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clump-python-0.1.tar", last modified: Wed Apr 24 12:07:56 2024, max compression
+gzip compressed data, was "clump-python-0.1.1.tar", last modified: Wed Apr 24 12:38:57 2024, max compression
```

## Comparing `clump-python-0.1.tar` & `clump-python-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 12:07:56.579815 clump-python-0.1/
--rw-rw-r--   0 utku      (1000) utku      (1000)    35149 2022-11-01 09:30:38.000000 clump-python-0.1/LICENSE
--rw-r--r--   0 utku      (1000) utku      (1000)      721 2024-04-24 12:07:56.579815 clump-python-0.1/PKG-INFO
--rw-rw-r--   0 utku      (1000) utku      (1000)     7677 2024-04-23 16:13:16.000000 clump-python-0.1/README.md
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 12:07:56.579815 clump-python-0.1/clump_python.egg-info/
--rw-r--r--   0 utku      (1000) utku      (1000)      721 2024-04-24 12:07:56.000000 clump-python-0.1/clump_python.egg-info/PKG-INFO
--rw-rw-r--   0 utku      (1000) utku      (1000)      607 2024-04-24 12:07:56.000000 clump-python-0.1/clump_python.egg-info/SOURCES.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)        1 2024-04-24 12:07:56.000000 clump-python-0.1/clump_python.egg-info/dependency_links.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)       49 2024-04-24 12:07:56.000000 clump-python-0.1/clump_python.egg-info/requires.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)       10 2024-04-24 12:07:56.000000 clump-python-0.1/clump_python.egg-info/top_level.txt
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 12:07:56.579815 clump-python-0.1/functions/
--rw-rw-r--   0 utku      (1000) utku      (1000)     8703 2024-04-23 16:33:08.000000 clump-python-0.1/functions/ExtractSurface.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     9256 2024-04-23 15:06:12.000000 clump-python-0.1/functions/GenerateClump_Euclidean_3D.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     8730 2024-04-23 15:39:48.000000 clump-python-0.1/functions/GenerateClump_Favier.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     8158 2024-04-23 15:39:58.000000 clump-python-0.1/functions/GenerateClump_Ferellec_McDowell.py
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.1/functions/__init__.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 12:07:56.579815 clump-python-0.1/functions/utils/
--rw-rw-r--   0 utku      (1000) utku      (1000)    15528 2024-04-23 12:24:18.000000 clump-python-0.1/functions/utils/MyRobustCrust.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     2620 2024-04-23 14:28:16.000000 clump-python-0.1/functions/utils/ParticlePlotter.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     1995 2024-04-23 16:32:00.000000 clump-python-0.1/functions/utils/PatchNormals.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     9442 2024-04-23 16:28:34.000000 clump-python-0.1/functions/utils/RigidBodyParameters.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     3308 2024-04-23 16:32:44.000000 clump-python-0.1/functions/utils/STL_ReaderWriter.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     1260 2024-04-23 16:32:48.000000 clump-python-0.1/functions/utils/VTK_Writer.py
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.1/functions/utils/__init__.py
--rw-rw-r--   0 utku      (1000) utku      (1000)       38 2024-04-24 12:07:56.579815 clump-python-0.1/setup.cfg
--rw-rw-r--   0 utku      (1000) utku      (1000)      818 2024-04-24 11:27:12.000000 clump-python-0.1/setup.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 12:38:57.130817 clump-python-0.1.1/
+-rw-rw-r--   0 utku      (1000) utku      (1000)    35149 2022-11-01 09:30:38.000000 clump-python-0.1.1/LICENSE
+-rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 12:38:57.130817 clump-python-0.1.1/PKG-INFO
+-rw-rw-r--   0 utku      (1000) utku      (1000)     7677 2024-04-23 16:13:16.000000 clump-python-0.1.1/README.md
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 12:38:57.130817 clump-python-0.1.1/clump/
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8703 2024-04-23 16:33:08.000000 clump-python-0.1.1/clump/ExtractSurface.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     9256 2024-04-23 15:06:12.000000 clump-python-0.1.1/clump/GenerateClump_Euclidean_3D.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8730 2024-04-23 15:39:48.000000 clump-python-0.1.1/clump/GenerateClump_Favier.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8158 2024-04-23 15:39:58.000000 clump-python-0.1.1/clump/GenerateClump_Ferellec_McDowell.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.1.1/clump/__init__.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 12:38:57.130817 clump-python-0.1.1/clump/utils/
+-rw-rw-r--   0 utku      (1000) utku      (1000)    15528 2024-04-23 12:24:18.000000 clump-python-0.1.1/clump/utils/MyRobustCrust.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     2620 2024-04-23 14:28:16.000000 clump-python-0.1.1/clump/utils/ParticlePlotter.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1995 2024-04-23 16:32:00.000000 clump-python-0.1.1/clump/utils/PatchNormals.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     9442 2024-04-23 16:28:34.000000 clump-python-0.1.1/clump/utils/RigidBodyParameters.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     3308 2024-04-23 16:32:44.000000 clump-python-0.1.1/clump/utils/STL_ReaderWriter.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1260 2024-04-23 16:32:48.000000 clump-python-0.1.1/clump/utils/VTK_Writer.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.1.1/clump/utils/__init__.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 12:38:57.130817 clump-python-0.1.1/clump_python.egg-info/
+-rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 12:38:57.000000 clump-python-0.1.1/clump_python.egg-info/PKG-INFO
+-rw-rw-r--   0 utku      (1000) utku      (1000)      559 2024-04-24 12:38:57.000000 clump-python-0.1.1/clump_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)        1 2024-04-24 12:38:57.000000 clump-python-0.1.1/clump_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)       49 2024-04-24 12:38:57.000000 clump-python-0.1.1/clump_python.egg-info/requires.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)        6 2024-04-24 12:38:57.000000 clump-python-0.1.1/clump_python.egg-info/top_level.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)       38 2024-04-24 12:38:57.130817 clump-python-0.1.1/setup.cfg
+-rw-rw-r--   0 utku      (1000) utku      (1000)      820 2024-04-24 12:38:43.000000 clump-python-0.1.1/setup.py
```

### Comparing `clump-python-0.1/LICENSE` & `clump-python-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clump-python-0.1/PKG-INFO` & `clump-python-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clump-python
-Version: 0.1
+Version: 0.1.1
 Summary: This Python library provides tools for creating and examining clumps using techniques: the Euclidean Distance Transform, Favier, and Ferellec-McDowell. It allows for the efficient generation of clumps and the extraction of their surfaces.
 Home-page: https://github.com/vsangelidakis/CLUMP
 Author: Utku Canbolat, Vasileios Angelidakis
 Author-email: utku.canbolat@fau.de
 License: GPL-3.0-only
 Keywords: Clump,Clump Generation,Euclidean Distance Transform,Favier,Ferellec-McDowell,Surface Extraction
 License-File: LICENSE
```

### Comparing `clump-python-0.1/README.md` & `clump-python-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `clump-python-0.1/clump_python.egg-info/PKG-INFO` & `clump-python-0.1.1/clump_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clump-python
-Version: 0.1
+Version: 0.1.1
 Summary: This Python library provides tools for creating and examining clumps using techniques: the Euclidean Distance Transform, Favier, and Ferellec-McDowell. It allows for the efficient generation of clumps and the extraction of their surfaces.
 Home-page: https://github.com/vsangelidakis/CLUMP
 Author: Utku Canbolat, Vasileios Angelidakis
 Author-email: utku.canbolat@fau.de
 License: GPL-3.0-only
 Keywords: Clump,Clump Generation,Euclidean Distance Transform,Favier,Ferellec-McDowell,Surface Extraction
 License-File: LICENSE
```

### Comparing `clump-python-0.1/functions/ExtractSurface.py` & `clump-python-0.1.1/clump/ExtractSurface.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1/functions/GenerateClump_Euclidean_3D.py` & `clump-python-0.1.1/clump/GenerateClump_Euclidean_3D.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1/functions/GenerateClump_Favier.py` & `clump-python-0.1.1/clump/GenerateClump_Favier.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1/functions/GenerateClump_Ferellec_McDowell.py` & `clump-python-0.1.1/clump/GenerateClump_Ferellec_McDowell.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1/functions/utils/MyRobustCrust.py` & `clump-python-0.1.1/clump/utils/MyRobustCrust.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1/functions/utils/ParticlePlotter.py` & `clump-python-0.1.1/clump/utils/ParticlePlotter.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1/functions/utils/PatchNormals.py` & `clump-python-0.1.1/clump/utils/PatchNormals.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1/functions/utils/RigidBodyParameters.py` & `clump-python-0.1.1/clump/utils/RigidBodyParameters.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1/functions/utils/STL_ReaderWriter.py` & `clump-python-0.1.1/clump/utils/STL_ReaderWriter.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1/functions/utils/VTK_Writer.py` & `clump-python-0.1.1/clump/utils/VTK_Writer.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1/setup.py` & `clump-python-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="clump-python",
-    version="0.1",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=[
         'matplotlib',
         'numpy',
         'numpy-stl',
         'pyvista',
         'scipy',
```

