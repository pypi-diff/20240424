# Comparing `tmp/clump-python-0.1.5.tar.gz` & `tmp/clump-python-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clump-python-0.1.5.tar", last modified: Wed Apr 24 15:13:23 2024, max compression
+gzip compressed data, was "clump-python-0.1.6.tar", last modified: Wed Apr 24 15:20:25 2024, max compression
```

## Comparing `clump-python-0.1.5.tar` & `clump-python-0.1.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:13:23.483405 clump-python-0.1.5/
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:13:23.479405 clump-python-0.1.5/CLUMP/
--rw-rw-r--   0 utku      (1000) utku      (1000)     8695 2024-04-24 15:03:18.000000 clump-python-0.1.5/CLUMP/ExtractSurface.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     9244 2024-04-24 15:03:18.000000 clump-python-0.1.5/CLUMP/GenerateClump_Euclidean_3D.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     8714 2024-04-24 15:03:18.000000 clump-python-0.1.5/CLUMP/GenerateClump_Favier.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     8138 2024-04-24 15:03:18.000000 clump-python-0.1.5/CLUMP/GenerateClump_Ferellec_McDowell.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      241 2024-04-24 14:39:02.000000 clump-python-0.1.5/CLUMP/__init__.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:13:23.479405 clump-python-0.1.5/CLUMP/utils/
--rw-rw-r--   0 utku      (1000) utku      (1000)    15528 2024-04-23 12:24:18.000000 clump-python-0.1.5/CLUMP/utils/MyRobustCrust.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     2620 2024-04-23 14:28:16.000000 clump-python-0.1.5/CLUMP/utils/ParticlePlotter.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     1995 2024-04-23 16:32:00.000000 clump-python-0.1.5/CLUMP/utils/PatchNormals.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     9442 2024-04-23 16:28:34.000000 clump-python-0.1.5/CLUMP/utils/RigidBodyParameters.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     3308 2024-04-23 16:32:44.000000 clump-python-0.1.5/CLUMP/utils/STL_ReaderWriter.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     1260 2024-04-23 16:32:48.000000 clump-python-0.1.5/CLUMP/utils/VTK_Writer.py
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.1.5/CLUMP/utils/__init__.py
--rw-rw-r--   0 utku      (1000) utku      (1000)    35149 2022-11-01 09:30:38.000000 clump-python-0.1.5/LICENSE
--rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 15:13:23.483405 clump-python-0.1.5/PKG-INFO
--rw-rw-r--   0 utku      (1000) utku      (1000)     7674 2024-04-24 15:03:18.000000 clump-python-0.1.5/README.md
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:13:23.479405 clump-python-0.1.5/clump_python.egg-info/
--rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 15:13:23.000000 clump-python-0.1.5/clump_python.egg-info/PKG-INFO
--rw-rw-r--   0 utku      (1000) utku      (1000)      816 2024-04-24 15:13:23.000000 clump-python-0.1.5/clump_python.egg-info/SOURCES.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)        1 2024-04-24 15:13:23.000000 clump-python-0.1.5/clump_python.egg-info/dependency_links.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)       49 2024-04-24 15:13:23.000000 clump-python-0.1.5/clump_python.egg-info/requires.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)       15 2024-04-24 15:13:23.000000 clump-python-0.1.5/clump_python.egg-info/top_level.txt
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:13:23.479405 clump-python-0.1.5/examples/
--rw-rw-r--   0 utku      (1000) utku      (1000)      862 2024-04-24 15:03:18.000000 clump-python-0.1.5/examples/Example_Euclidean_3D.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      987 2024-04-24 15:03:18.000000 clump-python-0.1.5/examples/Example_Euclidean_3D_Extended.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      768 2024-04-24 15:03:18.000000 clump-python-0.1.5/examples/Example_ExtractSurface.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      760 2024-04-24 15:03:18.000000 clump-python-0.1.5/examples/Example_Favier_automatic_generation.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      801 2024-04-24 15:03:18.000000 clump-python-0.1.5/examples/Example_Ferellec_McDowell.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:13:23.479405 clump-python-0.1.5/examples/ParticleGeometries/
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.1.5/examples/ParticleGeometries/__init__.py
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.1.5/examples/__init__.py
--rw-rw-r--   0 utku      (1000) utku      (1000)       38 2024-04-24 15:13:23.483405 clump-python-0.1.5/setup.cfg
--rw-rw-r--   0 utku      (1000) utku      (1000)      820 2024-04-24 15:13:09.000000 clump-python-0.1.5/setup.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:20:25.778009 clump-python-0.1.6/
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:20:25.778009 clump-python-0.1.6/CLUMP/
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8695 2024-04-24 15:03:18.000000 clump-python-0.1.6/CLUMP/ExtractSurface.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     9244 2024-04-24 15:03:18.000000 clump-python-0.1.6/CLUMP/GenerateClump_Euclidean_3D.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8714 2024-04-24 15:03:18.000000 clump-python-0.1.6/CLUMP/GenerateClump_Favier.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8138 2024-04-24 15:03:18.000000 clump-python-0.1.6/CLUMP/GenerateClump_Ferellec_McDowell.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      241 2024-04-24 14:39:02.000000 clump-python-0.1.6/CLUMP/__init__.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:20:25.778009 clump-python-0.1.6/CLUMP/examples/
+-rw-rw-r--   0 utku      (1000) utku      (1000)      862 2024-04-24 15:03:18.000000 clump-python-0.1.6/CLUMP/examples/Example_Euclidean_3D.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      987 2024-04-24 15:03:18.000000 clump-python-0.1.6/CLUMP/examples/Example_Euclidean_3D_Extended.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      768 2024-04-24 15:03:18.000000 clump-python-0.1.6/CLUMP/examples/Example_ExtractSurface.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      760 2024-04-24 15:03:18.000000 clump-python-0.1.6/CLUMP/examples/Example_Favier_automatic_generation.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      801 2024-04-24 15:03:18.000000 clump-python-0.1.6/CLUMP/examples/Example_Ferellec_McDowell.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:20:25.778009 clump-python-0.1.6/CLUMP/examples/ParticleGeometries/
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.1.6/CLUMP/examples/ParticleGeometries/__init__.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.1.6/CLUMP/examples/__init__.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:20:25.778009 clump-python-0.1.6/CLUMP/utils/
+-rw-rw-r--   0 utku      (1000) utku      (1000)    15528 2024-04-23 12:24:18.000000 clump-python-0.1.6/CLUMP/utils/MyRobustCrust.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     2620 2024-04-23 14:28:16.000000 clump-python-0.1.6/CLUMP/utils/ParticlePlotter.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1995 2024-04-23 16:32:00.000000 clump-python-0.1.6/CLUMP/utils/PatchNormals.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     9442 2024-04-23 16:28:34.000000 clump-python-0.1.6/CLUMP/utils/RigidBodyParameters.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     3308 2024-04-23 16:32:44.000000 clump-python-0.1.6/CLUMP/utils/STL_ReaderWriter.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1260 2024-04-23 16:32:48.000000 clump-python-0.1.6/CLUMP/utils/VTK_Writer.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.1.6/CLUMP/utils/__init__.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)    35149 2022-11-01 09:30:38.000000 clump-python-0.1.6/LICENSE
+-rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 15:20:25.778009 clump-python-0.1.6/PKG-INFO
+-rw-rw-r--   0 utku      (1000) utku      (1000)     7674 2024-04-24 15:03:18.000000 clump-python-0.1.6/README.md
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:20:25.778009 clump-python-0.1.6/clump_python.egg-info/
+-rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 15:20:25.000000 clump-python-0.1.6/clump_python.egg-info/PKG-INFO
+-rw-rw-r--   0 utku      (1000) utku      (1000)      858 2024-04-24 15:20:25.000000 clump-python-0.1.6/clump_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)        1 2024-04-24 15:20:25.000000 clump-python-0.1.6/clump_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)       49 2024-04-24 15:20:25.000000 clump-python-0.1.6/clump_python.egg-info/requires.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)        6 2024-04-24 15:20:25.000000 clump-python-0.1.6/clump_python.egg-info/top_level.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)       38 2024-04-24 15:20:25.778009 clump-python-0.1.6/setup.cfg
+-rw-rw-r--   0 utku      (1000) utku      (1000)      820 2024-04-24 15:20:06.000000 clump-python-0.1.6/setup.py
```

### Comparing `clump-python-0.1.5/CLUMP/ExtractSurface.py` & `clump-python-0.1.6/CLUMP/ExtractSurface.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.5/CLUMP/GenerateClump_Euclidean_3D.py` & `clump-python-0.1.6/CLUMP/GenerateClump_Euclidean_3D.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.5/CLUMP/GenerateClump_Favier.py` & `clump-python-0.1.6/CLUMP/GenerateClump_Favier.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.5/CLUMP/GenerateClump_Ferellec_McDowell.py` & `clump-python-0.1.6/CLUMP/GenerateClump_Ferellec_McDowell.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.5/CLUMP/utils/MyRobustCrust.py` & `clump-python-0.1.6/CLUMP/utils/MyRobustCrust.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.5/CLUMP/utils/ParticlePlotter.py` & `clump-python-0.1.6/CLUMP/utils/ParticlePlotter.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.5/CLUMP/utils/PatchNormals.py` & `clump-python-0.1.6/CLUMP/utils/PatchNormals.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.5/CLUMP/utils/RigidBodyParameters.py` & `clump-python-0.1.6/CLUMP/utils/RigidBodyParameters.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.5/CLUMP/utils/STL_ReaderWriter.py` & `clump-python-0.1.6/CLUMP/utils/STL_ReaderWriter.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.5/CLUMP/utils/VTK_Writer.py` & `clump-python-0.1.6/CLUMP/utils/VTK_Writer.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.5/LICENSE` & `clump-python-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.5/PKG-INFO` & `clump-python-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clump-python
-Version: 0.1.5
+Version: 0.1.6
 Summary: This Python library provides tools for creating and examining clumps using techniques: the Euclidean Distance Transform, Favier, and Ferellec-McDowell. It allows for the efficient generation of clumps and the extraction of their surfaces.
 Home-page: https://github.com/vsangelidakis/CLUMP
 Author: Utku Canbolat, Vasileios Angelidakis
 Author-email: utku.canbolat@fau.de
 License: GPL-3.0-only
 Keywords: Clump,Clump Generation,Euclidean Distance Transform,Favier,Ferellec-McDowell,Surface Extraction
 License-File: LICENSE
```

### Comparing `clump-python-0.1.5/README.md` & `clump-python-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.5/clump_python.egg-info/PKG-INFO` & `clump-python-0.1.6/clump_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clump-python
-Version: 0.1.5
+Version: 0.1.6
 Summary: This Python library provides tools for creating and examining clumps using techniques: the Euclidean Distance Transform, Favier, and Ferellec-McDowell. It allows for the efficient generation of clumps and the extraction of their surfaces.
 Home-page: https://github.com/vsangelidakis/CLUMP
 Author: Utku Canbolat, Vasileios Angelidakis
 Author-email: utku.canbolat@fau.de
 License: GPL-3.0-only
 Keywords: Clump,Clump Generation,Euclidean Distance Transform,Favier,Ferellec-McDowell,Surface Extraction
 License-File: LICENSE
```

### Comparing `clump-python-0.1.5/clump_python.egg-info/SOURCES.txt` & `clump-python-0.1.6/clump_python.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 README.md
 setup.py
 CLUMP/ExtractSurface.py
 CLUMP/GenerateClump_Euclidean_3D.py
 CLUMP/GenerateClump_Favier.py
 CLUMP/GenerateClump_Ferellec_McDowell.py
 CLUMP/__init__.py
+CLUMP/examples/Example_Euclidean_3D.py
+CLUMP/examples/Example_Euclidean_3D_Extended.py
+CLUMP/examples/Example_ExtractSurface.py
+CLUMP/examples/Example_Favier_automatic_generation.py
+CLUMP/examples/Example_Ferellec_McDowell.py
+CLUMP/examples/__init__.py
+CLUMP/examples/ParticleGeometries/__init__.py
 CLUMP/utils/MyRobustCrust.py
 CLUMP/utils/ParticlePlotter.py
 CLUMP/utils/PatchNormals.py
 CLUMP/utils/RigidBodyParameters.py
 CLUMP/utils/STL_ReaderWriter.py
 CLUMP/utils/VTK_Writer.py
 CLUMP/utils/__init__.py
 clump_python.egg-info/PKG-INFO
 clump_python.egg-info/SOURCES.txt
 clump_python.egg-info/dependency_links.txt
 clump_python.egg-info/requires.txt
-clump_python.egg-info/top_level.txt
-examples/Example_Euclidean_3D.py
-examples/Example_Euclidean_3D_Extended.py
-examples/Example_ExtractSurface.py
-examples/Example_Favier_automatic_generation.py
-examples/Example_Ferellec_McDowell.py
-examples/__init__.py
-examples/ParticleGeometries/__init__.py
+clump_python.egg-info/top_level.txt
```

### Comparing `clump-python-0.1.5/examples/Example_Euclidean_3D.py` & `clump-python-0.1.6/CLUMP/examples/Example_Euclidean_3D.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.5/examples/Example_Euclidean_3D_Extended.py` & `clump-python-0.1.6/CLUMP/examples/Example_Euclidean_3D_Extended.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.5/examples/Example_ExtractSurface.py` & `clump-python-0.1.6/CLUMP/examples/Example_ExtractSurface.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.5/examples/Example_Favier_automatic_generation.py` & `clump-python-0.1.6/CLUMP/examples/Example_Favier_automatic_generation.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.5/examples/Example_Ferellec_McDowell.py` & `clump-python-0.1.6/CLUMP/examples/Example_Ferellec_McDowell.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.5/setup.py` & `clump-python-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="clump-python",
-    version="0.1.5",
+    version="0.1.6",
     packages=find_packages(),
     install_requires=[
         'matplotlib',
         'numpy',
         'numpy-stl',
         'pyvista',
         'scipy',
```
