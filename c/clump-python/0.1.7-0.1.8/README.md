# Comparing `tmp/clump-python-0.1.7.tar.gz` & `tmp/clump-python-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clump-python-0.1.7.tar", last modified: Wed Apr 24 15:31:26 2024, max compression
+gzip compressed data, was "clump-python-0.1.8.tar", last modified: Wed Apr 24 15:40:43 2024, max compression
```

## Comparing `clump-python-0.1.7.tar` & `clump-python-0.1.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:31:26.578618 clump-python-0.1.7/
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:31:26.574617 clump-python-0.1.7/CLUMP/
--rw-rw-r--   0 utku      (1000) utku      (1000)     8695 2024-04-24 15:03:18.000000 clump-python-0.1.7/CLUMP/ExtractSurface.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     9244 2024-04-24 15:03:18.000000 clump-python-0.1.7/CLUMP/GenerateClump_Euclidean_3D.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     8714 2024-04-24 15:03:18.000000 clump-python-0.1.7/CLUMP/GenerateClump_Favier.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     8138 2024-04-24 15:03:18.000000 clump-python-0.1.7/CLUMP/GenerateClump_Ferellec_McDowell.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      241 2024-04-24 14:39:02.000000 clump-python-0.1.7/CLUMP/__init__.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:31:26.578618 clump-python-0.1.7/CLUMP/examples/
--rw-rw-r--   0 utku      (1000) utku      (1000)      797 2024-04-24 15:24:47.000000 clump-python-0.1.7/CLUMP/examples/Example_Euclidean_3D.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      922 2024-04-24 15:24:47.000000 clump-python-0.1.7/CLUMP/examples/Example_Euclidean_3D_Extended.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      700 2024-04-24 15:24:47.000000 clump-python-0.1.7/CLUMP/examples/Example_ExtractSurface.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      695 2024-04-24 15:24:47.000000 clump-python-0.1.7/CLUMP/examples/Example_Favier_automatic_generation.py
--rw-rw-r--   0 utku      (1000) utku      (1000)      736 2024-04-24 15:24:47.000000 clump-python-0.1.7/CLUMP/examples/Example_Ferellec_McDowell.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:31:26.578618 clump-python-0.1.7/CLUMP/examples/ParticleGeometries/
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.1.7/CLUMP/examples/ParticleGeometries/__init__.py
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.1.7/CLUMP/examples/__init__.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:31:26.578618 clump-python-0.1.7/CLUMP/utils/
--rw-rw-r--   0 utku      (1000) utku      (1000)    15528 2024-04-23 12:24:18.000000 clump-python-0.1.7/CLUMP/utils/MyRobustCrust.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     2620 2024-04-23 14:28:16.000000 clump-python-0.1.7/CLUMP/utils/ParticlePlotter.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     1995 2024-04-23 16:32:00.000000 clump-python-0.1.7/CLUMP/utils/PatchNormals.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     9442 2024-04-23 16:28:34.000000 clump-python-0.1.7/CLUMP/utils/RigidBodyParameters.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     3308 2024-04-23 16:32:44.000000 clump-python-0.1.7/CLUMP/utils/STL_ReaderWriter.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     1260 2024-04-23 16:32:48.000000 clump-python-0.1.7/CLUMP/utils/VTK_Writer.py
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.1.7/CLUMP/utils/__init__.py
--rw-rw-r--   0 utku      (1000) utku      (1000)    35149 2022-11-01 09:30:38.000000 clump-python-0.1.7/LICENSE
--rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 15:31:26.578618 clump-python-0.1.7/PKG-INFO
--rw-rw-r--   0 utku      (1000) utku      (1000)     7680 2024-04-24 15:24:47.000000 clump-python-0.1.7/README.md
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:31:26.578618 clump-python-0.1.7/clump_python.egg-info/
--rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 15:31:26.000000 clump-python-0.1.7/clump_python.egg-info/PKG-INFO
--rw-rw-r--   0 utku      (1000) utku      (1000)      858 2024-04-24 15:31:26.000000 clump-python-0.1.7/clump_python.egg-info/SOURCES.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)        1 2024-04-24 15:31:26.000000 clump-python-0.1.7/clump_python.egg-info/dependency_links.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)       49 2024-04-24 15:31:26.000000 clump-python-0.1.7/clump_python.egg-info/requires.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)        6 2024-04-24 15:31:26.000000 clump-python-0.1.7/clump_python.egg-info/top_level.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)       38 2024-04-24 15:31:26.578618 clump-python-0.1.7/setup.cfg
--rw-rw-r--   0 utku      (1000) utku      (1000)      820 2024-04-24 15:31:02.000000 clump-python-0.1.7/setup.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:40:43.666505 clump-python-0.1.8/
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:40:43.666505 clump-python-0.1.8/CLUMP/
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8695 2024-04-24 15:03:18.000000 clump-python-0.1.8/CLUMP/ExtractSurface.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     9244 2024-04-24 15:03:18.000000 clump-python-0.1.8/CLUMP/GenerateClump_Euclidean_3D.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8714 2024-04-24 15:03:18.000000 clump-python-0.1.8/CLUMP/GenerateClump_Favier.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8138 2024-04-24 15:03:18.000000 clump-python-0.1.8/CLUMP/GenerateClump_Ferellec_McDowell.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      241 2024-04-24 14:39:02.000000 clump-python-0.1.8/CLUMP/__init__.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:40:43.666505 clump-python-0.1.8/CLUMP/examples/
+-rw-rw-r--   0 utku      (1000) utku      (1000)      770 2024-04-24 15:37:50.000000 clump-python-0.1.8/CLUMP/examples/Example_Euclidean_3D.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      895 2024-04-24 15:37:50.000000 clump-python-0.1.8/CLUMP/examples/Example_Euclidean_3D_Extended.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      687 2024-04-24 15:38:15.000000 clump-python-0.1.8/CLUMP/examples/Example_ExtractSurface.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      674 2024-04-24 15:37:50.000000 clump-python-0.1.8/CLUMP/examples/Example_Favier_automatic_generation.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      704 2024-04-24 15:37:26.000000 clump-python-0.1.8/CLUMP/examples/Example_Ferellec_McDowell.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:40:43.666505 clump-python-0.1.8/CLUMP/examples/ParticleGeometries/
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.1.8/CLUMP/examples/ParticleGeometries/__init__.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-24 15:10:19.000000 clump-python-0.1.8/CLUMP/examples/__init__.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:40:43.666505 clump-python-0.1.8/CLUMP/utils/
+-rw-rw-r--   0 utku      (1000) utku      (1000)    15528 2024-04-23 12:24:18.000000 clump-python-0.1.8/CLUMP/utils/MyRobustCrust.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     2620 2024-04-23 14:28:16.000000 clump-python-0.1.8/CLUMP/utils/ParticlePlotter.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1995 2024-04-23 16:32:00.000000 clump-python-0.1.8/CLUMP/utils/PatchNormals.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     9442 2024-04-23 16:28:34.000000 clump-python-0.1.8/CLUMP/utils/RigidBodyParameters.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     3308 2024-04-23 16:32:44.000000 clump-python-0.1.8/CLUMP/utils/STL_ReaderWriter.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1260 2024-04-23 16:32:48.000000 clump-python-0.1.8/CLUMP/utils/VTK_Writer.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.1.8/CLUMP/utils/__init__.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)    35149 2022-11-01 09:30:38.000000 clump-python-0.1.8/LICENSE
+-rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 15:40:43.666505 clump-python-0.1.8/PKG-INFO
+-rw-rw-r--   0 utku      (1000) utku      (1000)     7680 2024-04-24 15:24:47.000000 clump-python-0.1.8/README.md
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:40:43.666505 clump-python-0.1.8/clump_python.egg-info/
+-rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 15:40:43.000000 clump-python-0.1.8/clump_python.egg-info/PKG-INFO
+-rw-rw-r--   0 utku      (1000) utku      (1000)      858 2024-04-24 15:40:43.000000 clump-python-0.1.8/clump_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)        1 2024-04-24 15:40:43.000000 clump-python-0.1.8/clump_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)       49 2024-04-24 15:40:43.000000 clump-python-0.1.8/clump_python.egg-info/requires.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)        6 2024-04-24 15:40:43.000000 clump-python-0.1.8/clump_python.egg-info/top_level.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)       38 2024-04-24 15:40:43.666505 clump-python-0.1.8/setup.cfg
+-rw-rw-r--   0 utku      (1000) utku      (1000)      820 2024-04-24 15:38:49.000000 clump-python-0.1.8/setup.py
```

### Comparing `clump-python-0.1.7/CLUMP/ExtractSurface.py` & `clump-python-0.1.8/CLUMP/ExtractSurface.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.7/CLUMP/GenerateClump_Euclidean_3D.py` & `clump-python-0.1.8/CLUMP/GenerateClump_Euclidean_3D.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.7/CLUMP/GenerateClump_Favier.py` & `clump-python-0.1.8/CLUMP/GenerateClump_Favier.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.7/CLUMP/GenerateClump_Ferellec_McDowell.py` & `clump-python-0.1.8/CLUMP/GenerateClump_Ferellec_McDowell.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.7/CLUMP/examples/Example_Euclidean_3D.py` & `clump-python-0.1.8/CLUMP/examples/Example_Euclidean_3D.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 2021 © V. Angelidakis, S. Nadimi, M. Otsubo, S. Utili.
 
 # 2021 MATLAB implementation by V. Angelidakis <v.angelidakis@qub.ac>
 # 2024 Translated from MATLAB to Python by U.A. Canbolat <utku.canbolat@fau.de>
 
 import sys
 
-from CLUMP.GenerateClump_Euclidean_3D import GenerateClump_Euclidean_3D
+from CLUMP import GenerateClump_Euclidean_3D
 import sys
 sys.path.append('../../')
 
 # Load particle shape from stl file
 inputGeom = 'ParticleGeometries/Hexahedron.stl'
 N = 21
 rMin = 0
```

### Comparing `clump-python-0.1.7/CLUMP/examples/Example_Euclidean_3D_Extended.py` & `clump-python-0.1.8/CLUMP/examples/Example_Euclidean_3D_Extended.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 2021 © V. Angelidakis, S. Nadimi, M. Otsubo, S. Utili.
 
 # 2021 MATLAB implementation by V. Angelidakis <v.angelidakis@qub.ac>
 # 2024 Translated from MATLAB to Python by U.A. Canbolat <utku.canbolat@fau.de>
 
 import sys
 
-from CLUMP.GenerateClump_Euclidean_3D import GenerateClump_Euclidean_3D
+from CLUMP import GenerateClump_Euclidean_3D
 import sys
 sys.path.append('../../')
 
 # Load particle shape from stl file
 inputGeom = 'ParticleGeometries/Human_femur.stl'
 N = 200
 rMin = 0
```

### Comparing `clump-python-0.1.7/CLUMP/examples/Example_ExtractSurface.py` & `clump-python-0.1.8/CLUMP/examples/Example_ExtractSurface.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 # 2021 MATLAB implementation by V. Angelidakis <v.angelidakis@qub.ac>
 # 2024 Translated from MATLAB to Python by U.A. Canbolat <utku.canbolat@fau.de>
 
 import sys
 
 import numpy as np
-from CLUMP.ExtractSurface import ExtractSurface
+from CLUMP import ExtractSurface
 from CLUMP.utils.STL_ReaderWriter import write_stl
 
 clump = np.array([[1, 0, 0, 1.1],
                   [2, 1, 0, 1.1],
                   [3, 0, 0, 1.2],
                   [1, 0, 1, 1.2]])
 
 N_sphere = 200
 N_circle = 100
 visualise = True
 
 faces, vertices = ExtractSurface(clump, N_sphere, N_circle, visualise)
 
-write_stl('Particle_surface.stl',vertices,faces)
+write_stl('Particle_surface.stl', vertices, faces)
```

### Comparing `clump-python-0.1.7/CLUMP/examples/Example_Favier_automatic_generation.py` & `clump-python-0.1.8/CLUMP/examples/Example_Favier_automatic_generation.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 2021 © V. Angelidakis, S. Nadimi, M. Otsubo, S. Utili.
 
 # 2021 MATLAB implementation by V. Angelidakis <v.angelidakis@qub.ac>
 # 2024 Translated from MATLAB to Python by U.A. Canbolat <utku.canbolat@fau.de>
 
 import sys
 
-from CLUMP.GenerateClump_Favier import GenerateClump_Favier
+from CLUMP import GenerateClump_Favier
 import sys
 sys.path.append('../../')
 
 inputGeom = 'ParticleGeometries/Ellipsoid_R_2.0_1.0_1.0.stl'
 N = 10
 chooseDistance = 'min'
 output = 'FA_Ellipsoid_2.0_1.0_1.0.txt'
```

### Comparing `clump-python-0.1.7/CLUMP/examples/Example_Ferellec_McDowell.py` & `clump-python-0.1.8/CLUMP/examples/Example_Ferellec_McDowell.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 2021 © V. Angelidakis, S. Nadimi, M. Otsubo, S. Utili.
 
 # 2021 MATLAB implementation by V. Angelidakis <v.angelidakis@qub.ac>
 # 2024 Translated from MATLAB to Python by U.A. Canbolat <utku.canbolat@fau.de>
 
 import sys
 
-from CLUMP.GenerateClump_Ferellec_McDowell import GenerateClump_Ferellec_McDowell
+from CLUMP import GenerateClump_Ferellec_McDowell
 import sys
 sys.path.append('../../')
 
 inputGeom = 'ParticleGeometries/Torus.stl'
 dmin = 0.1
 rmin = 0.01
 rstep = 0.01
```

### Comparing `clump-python-0.1.7/CLUMP/utils/MyRobustCrust.py` & `clump-python-0.1.8/CLUMP/utils/MyRobustCrust.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.7/CLUMP/utils/ParticlePlotter.py` & `clump-python-0.1.8/CLUMP/utils/ParticlePlotter.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.7/CLUMP/utils/PatchNormals.py` & `clump-python-0.1.8/CLUMP/utils/PatchNormals.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.7/CLUMP/utils/RigidBodyParameters.py` & `clump-python-0.1.8/CLUMP/utils/RigidBodyParameters.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.7/CLUMP/utils/STL_ReaderWriter.py` & `clump-python-0.1.8/CLUMP/utils/STL_ReaderWriter.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.7/CLUMP/utils/VTK_Writer.py` & `clump-python-0.1.8/CLUMP/utils/VTK_Writer.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.7/LICENSE` & `clump-python-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.7/PKG-INFO` & `clump-python-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clump-python
-Version: 0.1.7
+Version: 0.1.8
 Summary: This Python library provides tools for creating and examining clumps using techniques: the Euclidean Distance Transform, Favier, and Ferellec-McDowell. It allows for the efficient generation of clumps and the extraction of their surfaces.
 Home-page: https://github.com/vsangelidakis/CLUMP
 Author: Utku Canbolat, Vasileios Angelidakis
 Author-email: utku.canbolat@fau.de
 License: GPL-3.0-only
 Keywords: Clump,Clump Generation,Euclidean Distance Transform,Favier,Ferellec-McDowell,Surface Extraction
 License-File: LICENSE
```

### Comparing `clump-python-0.1.7/README.md` & `clump-python-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.7/clump_python.egg-info/PKG-INFO` & `clump-python-0.1.8/clump_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clump-python
-Version: 0.1.7
+Version: 0.1.8
 Summary: This Python library provides tools for creating and examining clumps using techniques: the Euclidean Distance Transform, Favier, and Ferellec-McDowell. It allows for the efficient generation of clumps and the extraction of their surfaces.
 Home-page: https://github.com/vsangelidakis/CLUMP
 Author: Utku Canbolat, Vasileios Angelidakis
 Author-email: utku.canbolat@fau.de
 License: GPL-3.0-only
 Keywords: Clump,Clump Generation,Euclidean Distance Transform,Favier,Ferellec-McDowell,Surface Extraction
 License-File: LICENSE
```

### Comparing `clump-python-0.1.7/clump_python.egg-info/SOURCES.txt` & `clump-python-0.1.8/clump_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.7/setup.py` & `clump-python-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="clump-python",
-    version="0.1.7",
+    version="0.1.8",
     packages=find_packages(),
     install_requires=[
         'matplotlib',
         'numpy',
         'numpy-stl',
         'pyvista',
         'scipy',
```

