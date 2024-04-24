# Comparing `tmp/clump-python-0.1.8.tar.gz` & `tmp/clump-python-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clump-python-0.1.8.tar", last modified: Wed Apr 24 15:40:43 2024, max compression
+gzip compressed data, was "clump-python-0.1.9.tar", last modified: Wed Apr 24 16:33:25 2024, max compression
```

## Comparing `clump-python-0.1.8.tar` & `clump-python-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,42 @@
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:40:43.666505 clump-python-0.1.8/
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:40:43.666505 clump-python-0.1.8/CLUMP/
--rw-rw-r--   0 utku      (1000) utku      (1000)     8695 2024-04-24 15:03:18.000000 clump-python-0.1.8/CLUMP/ExtractSurface.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     9244 2024-04-24 15:03:18.000000 clump-python-0.1.8/CLUMP/GenerateClump_Euclidean_3D.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     8714 2024-04-24 15:03:18.000000 clump-python-0.1.8/CLUMP/GenerateClump_Favier.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     8138 2024-04-24 15:03:18.000000 clump-python-0.1.8/CLUMP/GenerateClump_Ferellec_McDowell.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      241 2024-04-24 14:39:02.000000 clump-python-0.1.8/CLUMP/__init__.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:40:43.666505 clump-python-0.1.8/CLUMP/examples/
--rw-rw-r--   0 utku      (1000) utku      (1000)      770 2024-04-24 15:37:50.000000 clump-python-0.1.8/CLUMP/examples/Example_Euclidean_3D.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      895 2024-04-24 15:37:50.000000 clump-python-0.1.8/CLUMP/examples/Example_Euclidean_3D_Extended.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      687 2024-04-24 15:38:15.000000 clump-python-0.1.8/CLUMP/examples/Example_ExtractSurface.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      674 2024-04-24 15:37:50.000000 clump-python-0.1.8/CLUMP/examples/Example_Favier_automatic_generation.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      704 2024-04-24 15:37:26.000000 clump-python-0.1.8/CLUMP/examples/Example_Ferellec_McDowell.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:40:43.666505 clump-python-0.1.8/CLUMP/examples/ParticleGeometries/
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.1.8/CLUMP/examples/ParticleGeometries/__init__.py
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.1.8/CLUMP/examples/__init__.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:40:43.666505 clump-python-0.1.8/CLUMP/utils/
--rw-rw-r--   0 utku      (1000) utku      (1000)    15528 2024-04-23 12:24:18.000000 clump-python-0.1.8/CLUMP/utils/MyRobustCrust.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     2620 2024-04-23 14:28:16.000000 clump-python-0.1.8/CLUMP/utils/ParticlePlotter.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     1995 2024-04-23 16:32:00.000000 clump-python-0.1.8/CLUMP/utils/PatchNormals.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     9442 2024-04-23 16:28:34.000000 clump-python-0.1.8/CLUMP/utils/RigidBodyParameters.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     3308 2024-04-23 16:32:44.000000 clump-python-0.1.8/CLUMP/utils/STL_ReaderWriter.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     1260 2024-04-23 16:32:48.000000 clump-python-0.1.8/CLUMP/utils/VTK_Writer.py
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.1.8/CLUMP/utils/__init__.py
--rw-rw-r--   0 utku      (1000) utku      (1000)    35149 2022-11-01 09:30:38.000000 clump-python-0.1.8/LICENSE
--rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 15:40:43.666505 clump-python-0.1.8/PKG-INFO
--rw-rw-r--   0 utku      (1000) utku      (1000)     7680 2024-04-24 15:24:47.000000 clump-python-0.1.8/README.md
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:40:43.666505 clump-python-0.1.8/clump_python.egg-info/
--rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 15:40:43.000000 clump-python-0.1.8/clump_python.egg-info/PKG-INFO
--rw-rw-r--   0 utku      (1000) utku      (1000)      858 2024-04-24 15:40:43.000000 clump-python-0.1.8/clump_python.egg-info/SOURCES.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)        1 2024-04-24 15:40:43.000000 clump-python-0.1.8/clump_python.egg-info/dependency_links.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)       49 2024-04-24 15:40:43.000000 clump-python-0.1.8/clump_python.egg-info/requires.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)        6 2024-04-24 15:40:43.000000 clump-python-0.1.8/clump_python.egg-info/top_level.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)       38 2024-04-24 15:40:43.666505 clump-python-0.1.8/setup.cfg
--rw-rw-r--   0 utku      (1000) utku      (1000)      820 2024-04-24 15:38:49.000000 clump-python-0.1.8/setup.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 16:33:25.482167 clump-python-0.1.9/
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 16:33:25.470167 clump-python-0.1.9/CLUMP/
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8695 2024-04-24 15:03:18.000000 clump-python-0.1.9/CLUMP/ExtractSurface.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     9244 2024-04-24 15:03:18.000000 clump-python-0.1.9/CLUMP/GenerateClump_Euclidean_3D.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8714 2024-04-24 15:03:18.000000 clump-python-0.1.9/CLUMP/GenerateClump_Favier.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8138 2024-04-24 15:03:18.000000 clump-python-0.1.9/CLUMP/GenerateClump_Ferellec_McDowell.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      241 2024-04-24 14:39:02.000000 clump-python-0.1.9/CLUMP/__init__.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 16:33:25.474167 clump-python-0.1.9/CLUMP/examples/
+-rw-rw-r--   0 utku      (1000) utku      (1000)      770 2024-04-24 15:37:50.000000 clump-python-0.1.9/CLUMP/examples/Example_Euclidean_3D.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      895 2024-04-24 15:37:50.000000 clump-python-0.1.9/CLUMP/examples/Example_Euclidean_3D_Extended.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      687 2024-04-24 15:38:15.000000 clump-python-0.1.9/CLUMP/examples/Example_ExtractSurface.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      674 2024-04-24 15:37:50.000000 clump-python-0.1.9/CLUMP/examples/Example_Favier_automatic_generation.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      704 2024-04-24 15:37:26.000000 clump-python-0.1.9/CLUMP/examples/Example_Ferellec_McDowell.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 16:33:25.478167 clump-python-0.1.9/CLUMP/examples/ParticleGeometries/
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8351 2024-04-17 12:23:12.000000 clump-python-0.1.9/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat
+-rw-rw-r--   0 utku      (1000) utku      (1000)     4280 2024-04-17 12:23:12.000000 clump-python-0.1.9/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat
+-rw-rw-r--   0 utku      (1000) utku      (1000)  1024084 2022-11-01 09:30:38.000000 clump-python-0.1.9/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)   153684 2024-04-17 12:23:12.000000 clump-python-0.1.9/CLUMP/examples/ParticleGeometries/Hexahedron.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)  2670559 2024-04-17 12:23:12.000000 clump-python-0.1.9/CLUMP/examples/ParticleGeometries/Human_femur.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)   102484 2024-04-17 12:23:12.000000 clump-python-0.1.9/CLUMP/examples/ParticleGeometries/Octahedron.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)  2880084 2024-04-23 14:41:30.000000 clump-python-0.1.9/CLUMP/examples/ParticleGeometries/Torus.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.1.9/CLUMP/examples/ParticleGeometries/__init__.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.1.9/CLUMP/examples/__init__.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 16:33:25.482167 clump-python-0.1.9/CLUMP/utils/
+-rw-rw-r--   0 utku      (1000) utku      (1000)    15528 2024-04-23 12:24:18.000000 clump-python-0.1.9/CLUMP/utils/MyRobustCrust.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     2620 2024-04-23 14:28:16.000000 clump-python-0.1.9/CLUMP/utils/ParticlePlotter.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1995 2024-04-23 16:32:00.000000 clump-python-0.1.9/CLUMP/utils/PatchNormals.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     9442 2024-04-23 16:28:34.000000 clump-python-0.1.9/CLUMP/utils/RigidBodyParameters.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     3308 2024-04-23 16:32:44.000000 clump-python-0.1.9/CLUMP/utils/STL_ReaderWriter.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1260 2024-04-23 16:32:48.000000 clump-python-0.1.9/CLUMP/utils/VTK_Writer.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.1.9/CLUMP/utils/__init__.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)    35149 2022-11-01 09:30:38.000000 clump-python-0.1.9/LICENSE
+-rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 16:33:25.482167 clump-python-0.1.9/PKG-INFO
+-rw-rw-r--   0 utku      (1000) utku      (1000)     7680 2024-04-24 15:24:47.000000 clump-python-0.1.9/README.md
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 16:33:25.482167 clump-python-0.1.9/clump_python.egg-info/
+-rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 16:33:25.000000 clump-python-0.1.9/clump_python.egg-info/PKG-INFO
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1220 2024-04-24 16:33:25.000000 clump-python-0.1.9/clump_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)        1 2024-04-24 16:33:25.000000 clump-python-0.1.9/clump_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)       49 2024-04-24 16:33:25.000000 clump-python-0.1.9/clump_python.egg-info/requires.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)        6 2024-04-24 16:33:25.000000 clump-python-0.1.9/clump_python.egg-info/top_level.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)       38 2024-04-24 16:33:25.482167 clump-python-0.1.9/setup.cfg
+-rw-rw-r--   0 utku      (1000) utku      (1000)      947 2024-04-24 16:33:11.000000 clump-python-0.1.9/setup.py
```

### Comparing `clump-python-0.1.8/CLUMP/ExtractSurface.py` & `clump-python-0.1.9/CLUMP/ExtractSurface.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.8/CLUMP/GenerateClump_Euclidean_3D.py` & `clump-python-0.1.9/CLUMP/GenerateClump_Euclidean_3D.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.8/CLUMP/GenerateClump_Favier.py` & `clump-python-0.1.9/CLUMP/GenerateClump_Favier.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.8/CLUMP/GenerateClump_Ferellec_McDowell.py` & `clump-python-0.1.9/CLUMP/GenerateClump_Ferellec_McDowell.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.8/CLUMP/examples/Example_Euclidean_3D.py` & `clump-python-0.1.9/CLUMP/examples/Example_Euclidean_3D.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.8/CLUMP/examples/Example_Euclidean_3D_Extended.py` & `clump-python-0.1.9/CLUMP/examples/Example_Euclidean_3D_Extended.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.8/CLUMP/examples/Example_ExtractSurface.py` & `clump-python-0.1.9/CLUMP/examples/Example_ExtractSurface.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.8/CLUMP/examples/Example_Favier_automatic_generation.py` & `clump-python-0.1.9/CLUMP/examples/Example_Favier_automatic_generation.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.8/CLUMP/examples/Example_Ferellec_McDowell.py` & `clump-python-0.1.9/CLUMP/examples/Example_Ferellec_McDowell.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.8/CLUMP/utils/MyRobustCrust.py` & `clump-python-0.1.9/CLUMP/utils/MyRobustCrust.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.8/CLUMP/utils/ParticlePlotter.py` & `clump-python-0.1.9/CLUMP/utils/ParticlePlotter.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.8/CLUMP/utils/PatchNormals.py` & `clump-python-0.1.9/CLUMP/utils/PatchNormals.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.8/CLUMP/utils/RigidBodyParameters.py` & `clump-python-0.1.9/CLUMP/utils/RigidBodyParameters.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.8/CLUMP/utils/STL_ReaderWriter.py` & `clump-python-0.1.9/CLUMP/utils/STL_ReaderWriter.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.8/CLUMP/utils/VTK_Writer.py` & `clump-python-0.1.9/CLUMP/utils/VTK_Writer.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.8/LICENSE` & `clump-python-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.8/PKG-INFO` & `clump-python-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clump-python
-Version: 0.1.8
+Version: 0.1.9
 Summary: This Python library provides tools for creating and examining clumps using techniques: the Euclidean Distance Transform, Favier, and Ferellec-McDowell. It allows for the efficient generation of clumps and the extraction of their surfaces.
 Home-page: https://github.com/vsangelidakis/CLUMP
 Author: Utku Canbolat, Vasileios Angelidakis
 Author-email: utku.canbolat@fau.de
 License: GPL-3.0-only
 Keywords: Clump,Clump Generation,Euclidean Distance Transform,Favier,Ferellec-McDowell,Surface Extraction
 License-File: LICENSE
```

### Comparing `clump-python-0.1.8/README.md` & `clump-python-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.8/clump_python.egg-info/PKG-INFO` & `clump-python-0.1.9/clump_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clump-python
-Version: 0.1.8
+Version: 0.1.9
 Summary: This Python library provides tools for creating and examining clumps using techniques: the Euclidean Distance Transform, Favier, and Ferellec-McDowell. It allows for the efficient generation of clumps and the extraction of their surfaces.
 Home-page: https://github.com/vsangelidakis/CLUMP
 Author: Utku Canbolat, Vasileios Angelidakis
 Author-email: utku.canbolat@fau.de
 License: GPL-3.0-only
 Keywords: Clump,Clump Generation,Euclidean Distance Transform,Favier,Ferellec-McDowell,Surface Extraction
 License-File: LICENSE
```

### Comparing `clump-python-0.1.8/clump_python.egg-info/SOURCES.txt` & `clump-python-0.1.9/clump_python.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 CLUMP/__init__.py
 CLUMP/examples/Example_Euclidean_3D.py
 CLUMP/examples/Example_Euclidean_3D_Extended.py
 CLUMP/examples/Example_ExtractSurface.py
 CLUMP/examples/Example_Favier_automatic_generation.py
 CLUMP/examples/Example_Ferellec_McDowell.py
 CLUMP/examples/__init__.py
+CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat
+CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat
+CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl
+CLUMP/examples/ParticleGeometries/Hexahedron.stl
+CLUMP/examples/ParticleGeometries/Human_femur.stl
+CLUMP/examples/ParticleGeometries/Octahedron.stl
+CLUMP/examples/ParticleGeometries/Torus.stl
 CLUMP/examples/ParticleGeometries/__init__.py
 CLUMP/utils/MyRobustCrust.py
 CLUMP/utils/ParticlePlotter.py
 CLUMP/utils/PatchNormals.py
 CLUMP/utils/RigidBodyParameters.py
 CLUMP/utils/STL_ReaderWriter.py
 CLUMP/utils/VTK_Writer.py
```

