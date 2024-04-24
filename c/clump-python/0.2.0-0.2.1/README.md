# Comparing `tmp/clump-python-0.2.0.tar.gz` & `tmp/clump-python-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clump-python-0.2.0.tar", last modified: Wed Apr 24 16:38:40 2024, max compression
+gzip compressed data, was "clump-python-0.2.1.tar", last modified: Wed Apr 24 17:40:39 2024, max compression
```

## Comparing `clump-python-0.2.0.tar` & `clump-python-0.2.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 16:38:40.924496 clump-python-0.2.0/
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 16:38:40.912495 clump-python-0.2.0/CLUMP/
--rw-rw-r--   0 utku      (1000) utku      (1000)     8695 2024-04-24 15:03:18.000000 clump-python-0.2.0/CLUMP/ExtractSurface.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     9244 2024-04-24 15:03:18.000000 clump-python-0.2.0/CLUMP/GenerateClump_Euclidean_3D.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     8714 2024-04-24 15:03:18.000000 clump-python-0.2.0/CLUMP/GenerateClump_Favier.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     8138 2024-04-24 15:03:18.000000 clump-python-0.2.0/CLUMP/GenerateClump_Ferellec_McDowell.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      241 2024-04-24 14:39:02.000000 clump-python-0.2.0/CLUMP/__init__.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 16:38:40.912495 clump-python-0.2.0/CLUMP/examples/
--rw-rw-r--   0 utku      (1000) utku      (1000)      770 2024-04-24 15:37:50.000000 clump-python-0.2.0/CLUMP/examples/Example_Euclidean_3D.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      895 2024-04-24 15:37:50.000000 clump-python-0.2.0/CLUMP/examples/Example_Euclidean_3D_Extended.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      687 2024-04-24 15:38:15.000000 clump-python-0.2.0/CLUMP/examples/Example_ExtractSurface.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      674 2024-04-24 15:37:50.000000 clump-python-0.2.0/CLUMP/examples/Example_Favier_automatic_generation.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      704 2024-04-24 15:37:26.000000 clump-python-0.2.0/CLUMP/examples/Example_Ferellec_McDowell.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 16:38:40.920495 clump-python-0.2.0/CLUMP/examples/ParticleGeometries/
--rw-rw-r--   0 utku      (1000) utku      (1000)     8351 2024-04-17 12:23:12.000000 clump-python-0.2.0/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat
--rw-rw-r--   0 utku      (1000) utku      (1000)     4280 2024-04-17 12:23:12.000000 clump-python-0.2.0/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat
--rw-rw-r--   0 utku      (1000) utku      (1000)  1024084 2022-11-01 09:30:38.000000 clump-python-0.2.0/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)   153684 2024-04-17 12:23:12.000000 clump-python-0.2.0/CLUMP/examples/ParticleGeometries/Hexahedron.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)  2670559 2024-04-17 12:23:12.000000 clump-python-0.2.0/CLUMP/examples/ParticleGeometries/Human_femur.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)   102484 2024-04-17 12:23:12.000000 clump-python-0.2.0/CLUMP/examples/ParticleGeometries/Octahedron.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)  2880084 2024-04-23 14:41:30.000000 clump-python-0.2.0/CLUMP/examples/ParticleGeometries/Torus.stl
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.2.0/CLUMP/examples/ParticleGeometries/__init__.py
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.2.0/CLUMP/examples/__init__.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 16:38:40.920495 clump-python-0.2.0/CLUMP/utils/
--rw-rw-r--   0 utku      (1000) utku      (1000)    15528 2024-04-23 12:24:18.000000 clump-python-0.2.0/CLUMP/utils/MyRobustCrust.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     2620 2024-04-23 14:28:16.000000 clump-python-0.2.0/CLUMP/utils/ParticlePlotter.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     1995 2024-04-23 16:32:00.000000 clump-python-0.2.0/CLUMP/utils/PatchNormals.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     9442 2024-04-23 16:28:34.000000 clump-python-0.2.0/CLUMP/utils/RigidBodyParameters.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     3308 2024-04-23 16:32:44.000000 clump-python-0.2.0/CLUMP/utils/STL_ReaderWriter.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     1260 2024-04-23 16:32:48.000000 clump-python-0.2.0/CLUMP/utils/VTK_Writer.py
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.2.0/CLUMP/utils/__init__.py
--rw-rw-r--   0 utku      (1000) utku      (1000)    35149 2022-11-01 09:30:38.000000 clump-python-0.2.0/LICENSE
--rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 16:38:40.924496 clump-python-0.2.0/PKG-INFO
--rw-rw-r--   0 utku      (1000) utku      (1000)     7680 2024-04-24 15:24:47.000000 clump-python-0.2.0/README.md
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 16:38:40.920495 clump-python-0.2.0/clump_python.egg-info/
--rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 16:38:40.000000 clump-python-0.2.0/clump_python.egg-info/PKG-INFO
--rw-rw-r--   0 utku      (1000) utku      (1000)     1220 2024-04-24 16:38:40.000000 clump-python-0.2.0/clump_python.egg-info/SOURCES.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)        1 2024-04-24 16:38:40.000000 clump-python-0.2.0/clump_python.egg-info/dependency_links.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)       49 2024-04-24 16:38:40.000000 clump-python-0.2.0/clump_python.egg-info/requires.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)        6 2024-04-24 16:38:40.000000 clump-python-0.2.0/clump_python.egg-info/top_level.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)       38 2024-04-24 16:38:40.924496 clump-python-0.2.0/setup.cfg
--rw-rw-r--   0 utku      (1000) utku      (1000)     1023 2024-04-24 16:36:58.000000 clump-python-0.2.0/setup.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 17:40:39.084329 clump-python-0.2.1/
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 17:40:39.076329 clump-python-0.2.1/CLUMP/
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8695 2024-04-24 15:03:18.000000 clump-python-0.2.1/CLUMP/ExtractSurface.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     9244 2024-04-24 15:03:18.000000 clump-python-0.2.1/CLUMP/GenerateClump_Euclidean_3D.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8714 2024-04-24 15:03:18.000000 clump-python-0.2.1/CLUMP/GenerateClump_Favier.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8138 2024-04-24 15:03:18.000000 clump-python-0.2.1/CLUMP/GenerateClump_Ferellec_McDowell.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      241 2024-04-24 14:39:02.000000 clump-python-0.2.1/CLUMP/__init__.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 17:40:39.076329 clump-python-0.2.1/CLUMP/examples/
+-rw-rw-r--   0 utku      (1000) utku      (1000)      812 2024-04-24 17:36:11.000000 clump-python-0.2.1/CLUMP/examples/Example_Euclidean_3D.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      937 2024-04-24 17:36:11.000000 clump-python-0.2.1/CLUMP/examples/Example_Euclidean_3D_Extended.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      675 2024-04-24 17:36:11.000000 clump-python-0.2.1/CLUMP/examples/Example_ExtractSurface.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      713 2024-04-24 17:36:11.000000 clump-python-0.2.1/CLUMP/examples/Example_Favier_automatic_generation.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      743 2024-04-24 17:36:11.000000 clump-python-0.2.1/CLUMP/examples/Example_Ferellec_McDowell.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 17:40:39.084329 clump-python-0.2.1/CLUMP/examples/ParticleGeometries/
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8351 2024-04-17 12:23:12.000000 clump-python-0.2.1/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat
+-rw-rw-r--   0 utku      (1000) utku      (1000)     4280 2024-04-17 12:23:12.000000 clump-python-0.2.1/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat
+-rw-rw-r--   0 utku      (1000) utku      (1000)  1024084 2022-11-01 09:30:38.000000 clump-python-0.2.1/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)   153684 2024-04-17 12:23:12.000000 clump-python-0.2.1/CLUMP/examples/ParticleGeometries/Hexahedron.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)  2670559 2024-04-17 12:23:12.000000 clump-python-0.2.1/CLUMP/examples/ParticleGeometries/Human_femur.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)   102484 2024-04-17 12:23:12.000000 clump-python-0.2.1/CLUMP/examples/ParticleGeometries/Octahedron.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)  2880084 2024-04-23 14:41:30.000000 clump-python-0.2.1/CLUMP/examples/ParticleGeometries/Torus.stl
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.2.1/CLUMP/examples/ParticleGeometries/__init__.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.2.1/CLUMP/examples/__init__.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 17:40:39.084329 clump-python-0.2.1/CLUMP/utils/
+-rw-rw-r--   0 utku      (1000) utku      (1000)    15528 2024-04-23 12:24:18.000000 clump-python-0.2.1/CLUMP/utils/MyRobustCrust.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     2620 2024-04-23 14:28:16.000000 clump-python-0.2.1/CLUMP/utils/ParticlePlotter.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1995 2024-04-23 16:32:00.000000 clump-python-0.2.1/CLUMP/utils/PatchNormals.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     9442 2024-04-23 16:28:34.000000 clump-python-0.2.1/CLUMP/utils/RigidBodyParameters.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     3308 2024-04-23 16:32:44.000000 clump-python-0.2.1/CLUMP/utils/STL_ReaderWriter.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1260 2024-04-23 16:32:48.000000 clump-python-0.2.1/CLUMP/utils/VTK_Writer.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.2.1/CLUMP/utils/__init__.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)    35149 2022-11-01 09:30:38.000000 clump-python-0.2.1/LICENSE
+-rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 17:40:39.084329 clump-python-0.2.1/PKG-INFO
+-rw-rw-r--   0 utku      (1000) utku      (1000)     7680 2024-04-24 15:24:47.000000 clump-python-0.2.1/README.md
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 17:40:39.084329 clump-python-0.2.1/clump_python.egg-info/
+-rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 17:40:39.000000 clump-python-0.2.1/clump_python.egg-info/PKG-INFO
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1220 2024-04-24 17:40:39.000000 clump-python-0.2.1/clump_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)        1 2024-04-24 17:40:39.000000 clump-python-0.2.1/clump_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)       49 2024-04-24 17:40:39.000000 clump-python-0.2.1/clump_python.egg-info/requires.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)        6 2024-04-24 17:40:39.000000 clump-python-0.2.1/clump_python.egg-info/top_level.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)       38 2024-04-24 17:40:39.084329 clump-python-0.2.1/setup.cfg
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1023 2024-04-24 17:39:37.000000 clump-python-0.2.1/setup.py
```

### Comparing `clump-python-0.2.0/CLUMP/ExtractSurface.py` & `clump-python-0.2.1/CLUMP/ExtractSurface.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.0/CLUMP/GenerateClump_Euclidean_3D.py` & `clump-python-0.2.1/CLUMP/GenerateClump_Euclidean_3D.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.0/CLUMP/GenerateClump_Favier.py` & `clump-python-0.2.1/CLUMP/GenerateClump_Favier.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.0/CLUMP/GenerateClump_Ferellec_McDowell.py` & `clump-python-0.2.1/CLUMP/GenerateClump_Ferellec_McDowell.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.0/CLUMP/examples/Example_Euclidean_3D.py` & `clump-python-0.2.1/CLUMP/examples/Example_Euclidean_3D.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Script to run GenerateClump_Euclidean_3D
 # 2021 © V. Angelidakis, S. Nadimi, M. Otsubo, S. Utili.
 
 # 2021 MATLAB implementation by V. Angelidakis <v.angelidakis@qub.ac>
 # 2024 Translated from MATLAB to Python by U.A. Canbolat <utku.canbolat@fau.de>
 
-import sys
 
 from CLUMP import GenerateClump_Euclidean_3D
 import sys
+import os
 sys.path.append('../../')
 
 # Load particle shape from stl file
-inputGeom = 'ParticleGeometries/Hexahedron.stl'
+inputGeom = os.path.join(os.path.dirname(__file__), 'ParticleGeometries/Hexahedron.stl')
 N = 21
 rMin = 0
 div = 102
 overlap = 0.6
 output = 'EU_Hexahedron.txt'
 outputVTK = 'EU_Hexahedron.vtk'
 visualise = True
 
-mesh,clump = GenerateClump_Euclidean_3D(inputGeom=inputGeom, N=N, rMin=rMin, div=div, overlap=overlap, output=output, outputVTK=outputVTK, visualise=visualise)
+mesh, clump = GenerateClump_Euclidean_3D(inputGeom=inputGeom, N=N, rMin=rMin, div=div, overlap=overlap, output=output, outputVTK=outputVTK, visualise=visualise)
 
-print('Total number of spheres: '+ str(clump.numSpheres))
+print('Total number of spheres: ' + str(clump.numSpheres))
```

### Comparing `clump-python-0.2.0/CLUMP/examples/Example_Euclidean_3D_Extended.py` & `clump-python-0.2.1/CLUMP/examples/Example_Euclidean_3D_Extended.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Script to run GenerateClump_Euclidean_3D (Extended Euclidean method)
 # 2021 © V. Angelidakis, S. Nadimi, M. Otsubo, S. Utili.
 
 # 2021 MATLAB implementation by V. Angelidakis <v.angelidakis@qub.ac>
 # 2024 Translated from MATLAB to Python by U.A. Canbolat <utku.canbolat@fau.de>
 
-import sys
 
 from CLUMP import GenerateClump_Euclidean_3D
 import sys
+import os
 sys.path.append('../../')
 
 # Load particle shape from stl file
-inputGeom = 'ParticleGeometries/Human_femur.stl'
+inputGeom = os.path.join(os.path.dirname(__file__), 'ParticleGeometries/Human_femur.stl')
 N = 200
 rMin = 0
 div = 102
 overlap = 0.0
 output = 'EU_Human_femur.txt'
 outputVTK = 'EU_Human_femur.vtk'
 visualise = True
-rMax_ratio = 0.3 # Parameter to trigger the Extended Euclidean method
+rMax_ratio = 0.3  # Parameter to trigger the Extended Euclidean method
 
 mesh,clump = GenerateClump_Euclidean_3D(inputGeom=inputGeom, N=N, rMin=rMin, div=div, overlap=overlap, output=output, outputVTK=outputVTK, visualise=visualise, rMax_ratio=rMax_ratio)
 
-print('Total number of spheres: '+ str(clump.numSpheres))
+print('Total number of spheres: ' + str(clump.numSpheres))
```

### Comparing `clump-python-0.2.0/CLUMP/examples/Example_ExtractSurface.py` & `clump-python-0.2.1/CLUMP/examples/Example_ExtractSurface.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # Script to demonstrate the ExtractSurface function
 # 2021 © V. Angelidakis, S. Nadimi, M. Otsubo, S. Utili.
 
 # 2021 MATLAB implementation by V. Angelidakis <v.angelidakis@qub.ac>
 # 2024 Translated from MATLAB to Python by U.A. Canbolat <utku.canbolat@fau.de>
 
-import sys
-
 import numpy as np
 from CLUMP import ExtractSurface
 from CLUMP.utils.STL_ReaderWriter import write_stl
 
 clump = np.array([[1, 0, 0, 1.1],
                   [2, 1, 0, 1.1],
                   [3, 0, 0, 1.2],
```

### Comparing `clump-python-0.2.0/CLUMP/examples/Example_Favier_automatic_generation.py` & `clump-python-0.2.1/CLUMP/examples/Example_Favier_automatic_generation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # Script to run GenerateClump_Favier
 # 2021 © V. Angelidakis, S. Nadimi, M. Otsubo, S. Utili.
 
 # 2021 MATLAB implementation by V. Angelidakis <v.angelidakis@qub.ac>
 # 2024 Translated from MATLAB to Python by U.A. Canbolat <utku.canbolat@fau.de>
 
-import sys
-
 from CLUMP import GenerateClump_Favier
 import sys
+import os
 sys.path.append('../../')
 
-inputGeom = 'ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl'
+inputGeom = os.path.join(os.path.dirname(__file__), 'ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl')
 N = 10
 chooseDistance = 'min'
 output = 'FA_Ellipsoid_2.0_1.0_1.0.txt'
 outputVTK = 'FA_Ellipsoid_2.0_1.0_1.0.vtk'
 visualise = True
 
 mesh,clump=GenerateClump_Favier(inputGeom=inputGeom, N=N, chooseDistance=chooseDistance, output=output, outputVTK=outputVTK, visualise=visualise)
```

### Comparing `clump-python-0.2.0/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat` & `clump-python-0.2.1/CLUMP/examples/ParticleGeometries/Binary_3D_Cube.mat`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.0/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat` & `clump-python-0.2.1/CLUMP/examples/ParticleGeometries/Binary_3D_Cuboid.mat`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.0/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl` & `clump-python-0.2.1/CLUMP/examples/ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.0/CLUMP/examples/ParticleGeometries/Hexahedron.stl` & `clump-python-0.2.1/CLUMP/examples/ParticleGeometries/Hexahedron.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.0/CLUMP/examples/ParticleGeometries/Human_femur.stl` & `clump-python-0.2.1/CLUMP/examples/ParticleGeometries/Human_femur.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.0/CLUMP/examples/ParticleGeometries/Octahedron.stl` & `clump-python-0.2.1/CLUMP/examples/ParticleGeometries/Octahedron.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.0/CLUMP/examples/ParticleGeometries/Torus.stl` & `clump-python-0.2.1/CLUMP/examples/ParticleGeometries/Torus.stl`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.0/CLUMP/utils/MyRobustCrust.py` & `clump-python-0.2.1/CLUMP/utils/MyRobustCrust.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.0/CLUMP/utils/ParticlePlotter.py` & `clump-python-0.2.1/CLUMP/utils/ParticlePlotter.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.0/CLUMP/utils/PatchNormals.py` & `clump-python-0.2.1/CLUMP/utils/PatchNormals.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.0/CLUMP/utils/RigidBodyParameters.py` & `clump-python-0.2.1/CLUMP/utils/RigidBodyParameters.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.0/CLUMP/utils/STL_ReaderWriter.py` & `clump-python-0.2.1/CLUMP/utils/STL_ReaderWriter.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.0/CLUMP/utils/VTK_Writer.py` & `clump-python-0.2.1/CLUMP/utils/VTK_Writer.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.0/LICENSE` & `clump-python-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.0/PKG-INFO` & `clump-python-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clump-python
-Version: 0.2.0
+Version: 0.2.1
 Summary: This Python library provides tools for creating and examining clumps using techniques: the Euclidean Distance Transform, Favier, and Ferellec-McDowell. It allows for the efficient generation of clumps and the extraction of their surfaces.
 Home-page: https://github.com/vsangelidakis/CLUMP
 Author: Utku Canbolat, Vasileios Angelidakis
 Author-email: utku.canbolat@fau.de
 License: GPL-3.0-only
 Keywords: Clump,Clump Generation,Euclidean Distance Transform,Favier,Ferellec-McDowell,Surface Extraction
 License-File: LICENSE
```

### Comparing `clump-python-0.2.0/README.md` & `clump-python-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.0/clump_python.egg-info/PKG-INFO` & `clump-python-0.2.1/clump_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clump-python
-Version: 0.2.0
+Version: 0.2.1
 Summary: This Python library provides tools for creating and examining clumps using techniques: the Euclidean Distance Transform, Favier, and Ferellec-McDowell. It allows for the efficient generation of clumps and the extraction of their surfaces.
 Home-page: https://github.com/vsangelidakis/CLUMP
 Author: Utku Canbolat, Vasileios Angelidakis
 Author-email: utku.canbolat@fau.de
 License: GPL-3.0-only
 Keywords: Clump,Clump Generation,Euclidean Distance Transform,Favier,Ferellec-McDowell,Surface Extraction
 License-File: LICENSE
```

### Comparing `clump-python-0.2.0/clump_python.egg-info/SOURCES.txt` & `clump-python-0.2.1/clump_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clump-python-0.2.0/setup.py` & `clump-python-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="clump-python",
-    version="0.2.0",
+    version="0.2.1",
     packages=find_packages(),
     install_requires=[
         'matplotlib',
         'numpy',
         'numpy-stl',
         'pyvista',
         'scipy',
```

