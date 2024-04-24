# Comparing `tmp/clump-python-0.2.2.tar.gz` & `tmp/clump-python-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clump-python-0.2.2.tar", last modified: Wed Apr 24 17:44:58 2024, max compression
+gzip compressed data, was "clump-python-0.2.3.tar", last modified: Wed Apr 24 17:53:49 2024, max compression
```

## Comparing `clump-python-0.2.2.tar` & `clump-python-0.2.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 17:44:58.565743 clump-python-0.2.2/
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 17:44:58.557743 clump-python-0.2.2/CLUMP/
--rw-rw-r--   0 utku      (1000) utku      (1000)     8695 2024-04-24 15:03:18.000000 clump-python-0.2.2/CLUMP/ExtractSurface.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     9244 2024-04-24 15:03:18.000000 clump-python-0.2.2/CLUMP/GenerateClump_Euclidean_3D.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     8714 2024-04-24 15:03:18.000000 clump-python-0.2.2/CLUMP/GenerateClump_Favier.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     8138 2024-04-24 15:03:18.000000 clump-python-0.2.2/CLUMP/GenerateClump_Ferellec_McDowell.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      241 2024-04-24 14:39:02.000000 clump-python-0.2.2/CLUMP/__init__.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 17:44:58.557743 clump-python-0.2.2/CLUMP/examples/
--rw-rw-r--   0 utku      (1000) utku      (1000)      812 2024-04-24 17:36:11.000000 clump-python-0.2.2/CLUMP/examples/Example_Euclidean_3D.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      937 2024-04-24 17:36:11.000000 clump-python-0.2.2/CLUMP/examples/Example_Euclidean_3D_Extended.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      675 2024-04-24 17:36:11.000000 clump-python-0.2.2/CLUMP/examples/Example_ExtractSurface.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      713 2024-04-24 17:36:11.000000 clump-python-0.2.2/CLUMP/examples/Example_Favier_automatic_generation.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      743 2024-04-24 17:36:11.000000 clump-python-0.2.2/CLUMP/examples/Example_Ferellec_McDowell.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 17:44:58.565743 clump-python-0.2.2/CLUMP/examples/ParticleGeometries/
--rw-rw-r--   0 utku      (1000) utku      (1000)     8351 2024-04-17 12:23:12.000000 clump-python-0.2.2/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat
--rw-rw-r--   0 utku      (1000) utku      (1000)     4280 2024-04-17 12:23:12.000000 clump-python-0.2.2/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat
--rw-rw-r--   0 utku      (1000) utku      (1000)  1024084 2022-11-01 09:30:38.000000 clump-python-0.2.2/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)   153684 2024-04-17 12:23:12.000000 clump-python-0.2.2/CLUMP/examples/ParticleGeometries/Hexahedron.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)  2670559 2024-04-17 12:23:12.000000 clump-python-0.2.2/CLUMP/examples/ParticleGeometries/Human_femur.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)   102484 2024-04-17 12:23:12.000000 clump-python-0.2.2/CLUMP/examples/ParticleGeometries/Octahedron.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)  2880084 2024-04-23 14:41:30.000000 clump-python-0.2.2/CLUMP/examples/ParticleGeometries/Torus.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.2.2/CLUMP/examples/ParticleGeometries/__init__.py
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.2.2/CLUMP/examples/__init__.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 17:44:58.565743 clump-python-0.2.2/CLUMP/utils/
--rw-rw-r--   0 utku      (1000) utku      (1000)    15528 2024-04-23 12:24:18.000000 clump-python-0.2.2/CLUMP/utils/MyRobustCrust.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     2620 2024-04-23 14:28:16.000000 clump-python-0.2.2/CLUMP/utils/ParticlePlotter.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     1995 2024-04-23 16:32:00.000000 clump-python-0.2.2/CLUMP/utils/PatchNormals.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     9442 2024-04-23 16:28:34.000000 clump-python-0.2.2/CLUMP/utils/RigidBodyParameters.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     3308 2024-04-23 16:32:44.000000 clump-python-0.2.2/CLUMP/utils/STL_ReaderWriter.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     1260 2024-04-23 16:32:48.000000 clump-python-0.2.2/CLUMP/utils/VTK_Writer.py
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.2.2/CLUMP/utils/__init__.py
--rw-rw-r--   0 utku      (1000) utku      (1000)    35149 2022-11-01 09:30:38.000000 clump-python-0.2.2/LICENSE
--rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 17:44:58.565743 clump-python-0.2.2/PKG-INFO
--rw-rw-r--   0 utku      (1000) utku      (1000)     7680 2024-04-24 15:24:47.000000 clump-python-0.2.2/README.md
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 17:44:58.565743 clump-python-0.2.2/clump_python.egg-info/
--rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 17:44:58.000000 clump-python-0.2.2/clump_python.egg-info/PKG-INFO
--rw-rw-r--   0 utku      (1000) utku      (1000)     1220 2024-04-24 17:44:58.000000 clump-python-0.2.2/clump_python.egg-info/SOURCES.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)        1 2024-04-24 17:44:58.000000 clump-python-0.2.2/clump_python.egg-info/dependency_links.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)       49 2024-04-24 17:44:58.000000 clump-python-0.2.2/clump_python.egg-info/requires.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)        6 2024-04-24 17:44:58.000000 clump-python-0.2.2/clump_python.egg-info/top_level.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)       38 2024-04-24 17:44:58.565743 clump-python-0.2.2/setup.cfg
--rw-rw-r--   0 utku      (1000) utku      (1000)     1023 2024-04-24 17:43:55.000000 clump-python-0.2.2/setup.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 17:53:49.476702 clump-python-0.2.3/
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 17:53:49.464702 clump-python-0.2.3/CLUMP/
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8695 2024-04-24 15:03:18.000000 clump-python-0.2.3/CLUMP/ExtractSurface.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     9244 2024-04-24 15:03:18.000000 clump-python-0.2.3/CLUMP/GenerateClump_Euclidean_3D.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8714 2024-04-24 15:03:18.000000 clump-python-0.2.3/CLUMP/GenerateClump_Favier.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8138 2024-04-24 15:03:18.000000 clump-python-0.2.3/CLUMP/GenerateClump_Ferellec_McDowell.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      241 2024-04-24 14:39:02.000000 clump-python-0.2.3/CLUMP/__init__.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 17:53:49.464702 clump-python-0.2.3/CLUMP/examples/
+-rw-rw-r--   0 utku      (1000) utku      (1000)      812 2024-04-24 17:36:11.000000 clump-python-0.2.3/CLUMP/examples/Example_Euclidean_3D.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      937 2024-04-24 17:36:11.000000 clump-python-0.2.3/CLUMP/examples/Example_Euclidean_3D_Extended.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      675 2024-04-24 17:36:11.000000 clump-python-0.2.3/CLUMP/examples/Example_ExtractSurface.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      713 2024-04-24 17:36:11.000000 clump-python-0.2.3/CLUMP/examples/Example_Favier_automatic_generation.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      743 2024-04-24 17:36:11.000000 clump-python-0.2.3/CLUMP/examples/Example_Ferellec_McDowell.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 17:53:49.472702 clump-python-0.2.3/CLUMP/examples/ParticleGeometries/
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8351 2024-04-17 12:23:12.000000 clump-python-0.2.3/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat
+-rw-rw-r--   0 utku      (1000) utku      (1000)     4280 2024-04-17 12:23:12.000000 clump-python-0.2.3/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat
+-rw-rw-r--   0 utku      (1000) utku      (1000)  1024084 2022-11-01 09:30:38.000000 clump-python-0.2.3/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)   153684 2024-04-17 12:23:12.000000 clump-python-0.2.3/CLUMP/examples/ParticleGeometries/Hexahedron.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)  2670559 2024-04-17 12:23:12.000000 clump-python-0.2.3/CLUMP/examples/ParticleGeometries/Human_femur.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)   102484 2024-04-17 12:23:12.000000 clump-python-0.2.3/CLUMP/examples/ParticleGeometries/Octahedron.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)  2880084 2024-04-23 14:41:30.000000 clump-python-0.2.3/CLUMP/examples/ParticleGeometries/Torus.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.2.3/CLUMP/examples/ParticleGeometries/__init__.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.2.3/CLUMP/examples/__init__.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 17:53:49.476702 clump-python-0.2.3/CLUMP/utils/
+-rw-rw-r--   0 utku      (1000) utku      (1000)    15528 2024-04-23 12:24:18.000000 clump-python-0.2.3/CLUMP/utils/MyRobustCrust.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     2620 2024-04-23 14:28:16.000000 clump-python-0.2.3/CLUMP/utils/ParticlePlotter.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1995 2024-04-23 16:32:00.000000 clump-python-0.2.3/CLUMP/utils/PatchNormals.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     9442 2024-04-23 16:28:34.000000 clump-python-0.2.3/CLUMP/utils/RigidBodyParameters.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     3308 2024-04-23 16:32:44.000000 clump-python-0.2.3/CLUMP/utils/STL_ReaderWriter.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1260 2024-04-23 16:32:48.000000 clump-python-0.2.3/CLUMP/utils/VTK_Writer.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.2.3/CLUMP/utils/__init__.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)    35149 2022-11-01 09:30:38.000000 clump-python-0.2.3/LICENSE
+-rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 17:53:49.476702 clump-python-0.2.3/PKG-INFO
+-rw-rw-r--   0 utku      (1000) utku      (1000)     7680 2024-04-24 15:24:47.000000 clump-python-0.2.3/README.md
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 17:53:49.476702 clump-python-0.2.3/clump_python.egg-info/
+-rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 17:53:49.000000 clump-python-0.2.3/clump_python.egg-info/PKG-INFO
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1220 2024-04-24 17:53:49.000000 clump-python-0.2.3/clump_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)        1 2024-04-24 17:53:49.000000 clump-python-0.2.3/clump_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)       49 2024-04-24 17:53:49.000000 clump-python-0.2.3/clump_python.egg-info/requires.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)        6 2024-04-24 17:53:49.000000 clump-python-0.2.3/clump_python.egg-info/top_level.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)       38 2024-04-24 17:53:49.476702 clump-python-0.2.3/setup.cfg
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1023 2024-04-24 17:52:55.000000 clump-python-0.2.3/setup.py
```

### Comparing `clump-python-0.2.2/CLUMP/ExtractSurface.py` & `clump-python-0.2.3/CLUMP/ExtractSurface.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/CLUMP/GenerateClump_Euclidean_3D.py` & `clump-python-0.2.3/CLUMP/GenerateClump_Euclidean_3D.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/CLUMP/GenerateClump_Favier.py` & `clump-python-0.2.3/CLUMP/GenerateClump_Favier.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/CLUMP/GenerateClump_Ferellec_McDowell.py` & `clump-python-0.2.3/CLUMP/GenerateClump_Ferellec_McDowell.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/CLUMP/examples/Example_Euclidean_3D.py` & `clump-python-0.2.3/CLUMP/examples/Example_Euclidean_3D.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/CLUMP/examples/Example_Euclidean_3D_Extended.py` & `clump-python-0.2.3/CLUMP/examples/Example_Euclidean_3D_Extended.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/CLUMP/examples/Example_ExtractSurface.py` & `clump-python-0.2.3/CLUMP/examples/Example_ExtractSurface.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/CLUMP/examples/Example_Favier_automatic_generation.py` & `clump-python-0.2.3/CLUMP/examples/Example_Favier_automatic_generation.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/CLUMP/examples/Example_Ferellec_McDowell.py` & `clump-python-0.2.3/CLUMP/examples/Example_Ferellec_McDowell.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat` & `clump-python-0.2.3/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat` & `clump-python-0.2.3/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl` & `clump-python-0.2.3/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/CLUMP/examples/ParticleGeometries/Hexahedron.stl` & `clump-python-0.2.3/CLUMP/examples/ParticleGeometries/Hexahedron.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/CLUMP/examples/ParticleGeometries/Human_femur.stl` & `clump-python-0.2.3/CLUMP/examples/ParticleGeometries/Human_femur.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/CLUMP/examples/ParticleGeometries/Octahedron.stl` & `clump-python-0.2.3/CLUMP/examples/ParticleGeometries/Octahedron.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/CLUMP/examples/ParticleGeometries/Torus.stl` & `clump-python-0.2.3/CLUMP/examples/ParticleGeometries/Torus.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/CLUMP/utils/MyRobustCrust.py` & `clump-python-0.2.3/CLUMP/utils/MyRobustCrust.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/CLUMP/utils/ParticlePlotter.py` & `clump-python-0.2.3/CLUMP/utils/ParticlePlotter.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/CLUMP/utils/PatchNormals.py` & `clump-python-0.2.3/CLUMP/utils/PatchNormals.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/CLUMP/utils/RigidBodyParameters.py` & `clump-python-0.2.3/CLUMP/utils/RigidBodyParameters.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/CLUMP/utils/STL_ReaderWriter.py` & `clump-python-0.2.3/CLUMP/utils/STL_ReaderWriter.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/CLUMP/utils/VTK_Writer.py` & `clump-python-0.2.3/CLUMP/utils/VTK_Writer.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/LICENSE` & `clump-python-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/PKG-INFO` & `clump-python-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clump-python
-Version: 0.2.2
+Version: 0.2.3
 Summary: This Python library provides tools for creating and examining clumps using techniques: the Euclidean Distance Transform, Favier, and Ferellec-McDowell. It allows for the efficient generation of clumps and the extraction of their surfaces.
 Home-page: https://github.com/vsangelidakis/CLUMP
 Author: Utku Canbolat, Vasileios Angelidakis
 Author-email: utku.canbolat@fau.de
 License: GPL-3.0-only
 Keywords: Clump,Clump Generation,Euclidean Distance Transform,Favier,Ferellec-McDowell,Surface Extraction
 License-File: LICENSE
```

### Comparing `clump-python-0.2.2/README.md` & `clump-python-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/clump_python.egg-info/PKG-INFO` & `clump-python-0.2.3/clump_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clump-python
-Version: 0.2.2
+Version: 0.2.3
 Summary: This Python library provides tools for creating and examining clumps using techniques: the Euclidean Distance Transform, Favier, and Ferellec-McDowell. It allows for the efficient generation of clumps and the extraction of their surfaces.
 Home-page: https://github.com/vsangelidakis/CLUMP
 Author: Utku Canbolat, Vasileios Angelidakis
 Author-email: utku.canbolat@fau.de
 License: GPL-3.0-only
 Keywords: Clump,Clump Generation,Euclidean Distance Transform,Favier,Ferellec-McDowell,Surface Extraction
 License-File: LICENSE
```

### Comparing `clump-python-0.2.2/clump_python.egg-info/SOURCES.txt` & `clump-python-0.2.3/clump_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.2/setup.py` & `clump-python-0.2.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="clump-python",
-    version="0.2.2",
+    version="0.2.3",
     packages=find_packages(),
     install_requires=[
         'matplotlib',
         'numpy',
         'numpy-stl',
         'pyvista',
         'scipy',
```

