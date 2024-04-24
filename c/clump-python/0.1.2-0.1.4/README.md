# Comparing `tmp/clump-python-0.1.2.tar.gz` & `tmp/clump-python-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clump-python-0.1.2.tar", last modified: Wed Apr 24 14:47:03 2024, max compression
+gzip compressed data, was "clump-python-0.1.4.tar", last modified: Wed Apr 24 15:05:07 2024, max compression
```

## Comparing `clump-python-0.1.2.tar` & `clump-python-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 14:47:03.169736 clump-python-0.1.2/
--rw-rw-r--   0 utku      (1000) utku      (1000)    35149 2022-11-01 09:30:38.000000 clump-python-0.1.2/LICENSE
--rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 14:47:03.169736 clump-python-0.1.2/PKG-INFO
--rw-rw-r--   0 utku      (1000) utku      (1000)     7677 2024-04-23 16:13:16.000000 clump-python-0.1.2/README.md
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 14:47:03.169736 clump-python-0.1.2/clump/
--rw-rw-r--   0 utku      (1000) utku      (1000)     8703 2024-04-23 16:33:08.000000 clump-python-0.1.2/clump/ExtractSurface.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     9256 2024-04-23 15:06:12.000000 clump-python-0.1.2/clump/GenerateClump_Euclidean_3D.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     8730 2024-04-23 15:39:48.000000 clump-python-0.1.2/clump/GenerateClump_Favier.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     8158 2024-04-23 15:39:58.000000 clump-python-0.1.2/clump/GenerateClump_Ferellec_McDowell.py
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.1.2/clump/__init__.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 14:47:03.169736 clump-python-0.1.2/clump/utils/
--rw-rw-r--   0 utku      (1000) utku      (1000)    15528 2024-04-23 12:24:18.000000 clump-python-0.1.2/clump/utils/MyRobustCrust.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     2620 2024-04-23 14:28:16.000000 clump-python-0.1.2/clump/utils/ParticlePlotter.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     1995 2024-04-23 16:32:00.000000 clump-python-0.1.2/clump/utils/PatchNormals.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     9442 2024-04-23 16:28:34.000000 clump-python-0.1.2/clump/utils/RigidBodyParameters.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     3308 2024-04-23 16:32:44.000000 clump-python-0.1.2/clump/utils/STL_ReaderWriter.py
--rw-rw-r--   0 utku      (1000) utku      (1000)     1260 2024-04-23 16:32:48.000000 clump-python-0.1.2/clump/utils/VTK_Writer.py
--rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.1.2/clump/utils/__init__.py
-drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 14:47:03.169736 clump-python-0.1.2/clump_python.egg-info/
--rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 14:47:03.000000 clump-python-0.1.2/clump_python.egg-info/PKG-INFO
--rw-rw-r--   0 utku      (1000) utku      (1000)      559 2024-04-24 14:47:03.000000 clump-python-0.1.2/clump_python.egg-info/SOURCES.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)        1 2024-04-24 14:47:03.000000 clump-python-0.1.2/clump_python.egg-info/dependency_links.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)       49 2024-04-24 14:47:03.000000 clump-python-0.1.2/clump_python.egg-info/requires.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)        6 2024-04-24 14:47:03.000000 clump-python-0.1.2/clump_python.egg-info/top_level.txt
--rw-rw-r--   0 utku      (1000) utku      (1000)       38 2024-04-24 14:47:03.169736 clump-python-0.1.2/setup.cfg
--rw-rw-r--   0 utku      (1000) utku      (1000)      820 2024-04-24 14:46:36.000000 clump-python-0.1.2/setup.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:05:07.059607 clump-python-0.1.4/
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:05:07.059607 clump-python-0.1.4/CLUMP/
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8695 2024-04-24 15:03:18.000000 clump-python-0.1.4/CLUMP/ExtractSurface.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     9244 2024-04-24 15:03:18.000000 clump-python-0.1.4/CLUMP/GenerateClump_Euclidean_3D.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8714 2024-04-24 15:03:18.000000 clump-python-0.1.4/CLUMP/GenerateClump_Favier.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     8138 2024-04-24 15:03:18.000000 clump-python-0.1.4/CLUMP/GenerateClump_Ferellec_McDowell.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)      241 2024-04-24 14:39:02.000000 clump-python-0.1.4/CLUMP/__init__.py
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:05:07.059607 clump-python-0.1.4/CLUMP/utils/
+-rw-rw-r--   0 utku      (1000) utku      (1000)    15528 2024-04-23 12:24:18.000000 clump-python-0.1.4/CLUMP/utils/MyRobustCrust.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     2620 2024-04-23 14:28:16.000000 clump-python-0.1.4/CLUMP/utils/ParticlePlotter.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1995 2024-04-23 16:32:00.000000 clump-python-0.1.4/CLUMP/utils/PatchNormals.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     9442 2024-04-23 16:28:34.000000 clump-python-0.1.4/CLUMP/utils/RigidBodyParameters.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     3308 2024-04-23 16:32:44.000000 clump-python-0.1.4/CLUMP/utils/STL_ReaderWriter.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)     1260 2024-04-23 16:32:48.000000 clump-python-0.1.4/CLUMP/utils/VTK_Writer.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)        0 2024-04-17 12:23:12.000000 clump-python-0.1.4/CLUMP/utils/__init__.py
+-rw-rw-r--   0 utku      (1000) utku      (1000)    35149 2022-11-01 09:30:38.000000 clump-python-0.1.4/LICENSE
+-rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 15:05:07.059607 clump-python-0.1.4/PKG-INFO
+-rw-rw-r--   0 utku      (1000) utku      (1000)     7674 2024-04-24 15:03:18.000000 clump-python-0.1.4/README.md
+drwxrwxr-x   0 utku      (1000) utku      (1000)        0 2024-04-24 15:05:07.059607 clump-python-0.1.4/clump_python.egg-info/
+-rw-r--r--   0 utku      (1000) utku      (1000)      723 2024-04-24 15:05:07.000000 clump-python-0.1.4/clump_python.egg-info/PKG-INFO
+-rw-rw-r--   0 utku      (1000) utku      (1000)      559 2024-04-24 15:05:07.000000 clump-python-0.1.4/clump_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)        1 2024-04-24 15:05:07.000000 clump-python-0.1.4/clump_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)       49 2024-04-24 15:05:07.000000 clump-python-0.1.4/clump_python.egg-info/requires.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)        6 2024-04-24 15:05:07.000000 clump-python-0.1.4/clump_python.egg-info/top_level.txt
+-rw-rw-r--   0 utku      (1000) utku      (1000)       38 2024-04-24 15:05:07.059607 clump-python-0.1.4/setup.cfg
+-rw-rw-r--   0 utku      (1000) utku      (1000)      820 2024-04-24 15:04:50.000000 clump-python-0.1.4/setup.py
```

### Comparing `clump-python-0.1.2/LICENSE` & `clump-python-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.2/PKG-INFO` & `clump-python-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clump-python
-Version: 0.1.2
+Version: 0.1.4
 Summary: This Python library provides tools for creating and examining clumps using techniques: the Euclidean Distance Transform, Favier, and Ferellec-McDowell. It allows for the efficient generation of clumps and the extraction of their surfaces.
 Home-page: https://github.com/vsangelidakis/CLUMP
 Author: Utku Canbolat, Vasileios Angelidakis
 Author-email: utku.canbolat@fau.de
 License: GPL-3.0-only
 Keywords: Clump,Clump Generation,Euclidean Distance Transform,Favier,Ferellec-McDowell,Surface Extraction
 License-File: LICENSE
```

### Comparing `clump-python-0.1.2/README.md` & `clump-python-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -78,23 +78,24 @@
 [mesh, clump]=GenerateClump_Ferellec_McDowell( stlFile, dmin, rmin, rstep, pmax, seed, output );
 
 % Generate clumps using the approach proposed in this code, involving the Euclidean transform of 3D images
 [mesh, clump]=GenerateClump_Euclidean_3D( stlFile, N, rMin, div, overlap, output );
 ```
 
 Python implementation of CLUMP:
+
 ```Python
-from functions.GenerateClump_Ferellec_McDowell import GenerateClump_Ferellec_McDowell
-from functions.GenerateClump_Euclidean_3D import GenerateClump_Euclidean_3D
+from CLUMP.GenerateClump_Ferellec_McDowell import GenerateClump_Ferellec_McDowell
+from CLUMP.GenerateClump_Euclidean_3D import GenerateClump_Euclidean_3D
 
 # Generate clumps using the approach of Ferellec and McDowell (2010)
-mesh,clump=GenerateClump_Ferellec_McDowell(inputGeom, dmin, rmin, rstep, pmax, seed, output, outputVTK, visualise)
+mesh, clump = GenerateClump_Ferellec_McDowell(inputGeom, dmin, rmin, rstep, pmax, seed, output, outputVTK, visualise)
 
 # Generate clumps using the approach proposed in this code, involving the Euclidean transform of 3D images
-mesh,clump = GenerateClump_Euclidean_3D(inputGeom, N, rMin, div, overlap, output, outputVTK, visualise)
+mesh, clump = GenerateClump_Euclidean_3D(inputGeom, N, rMin, div, overlap, output, outputVTK, visualise)
 ```
 
 New users are advised to start from running the available examples in the [examples](examples) folder, to get familiarised with the syntax and functionalities of CLUMP.
 
 ## Credits
 The MATLAB and Python implementations of CLUMP use different sets of external dependencies.
```

#### html2text {}

```diff
@@ -35,48 +35,47 @@
 house functions addpath(genpath('lib')); % Load external functions
 (dependencies) addpath(genpath('classes')); % Load object-oriented architecture
 % Generate clumps using the approach of Ferellec and McDowell (2010) [mesh,
 clump]=GenerateClump_Ferellec_McDowell( stlFile, dmin, rmin, rstep, pmax, seed,
 output ); % Generate clumps using the approach proposed in this code, involving
 the Euclidean transform of 3D images [mesh, clump]=GenerateClump_Euclidean_3D
 ( stlFile, N, rMin, div, overlap, output ); ``` Python implementation of CLUMP:
-```Python from functions.GenerateClump_Ferellec_McDowell import
-GenerateClump_Ferellec_McDowell from functions.GenerateClump_Euclidean_3D
-import GenerateClump_Euclidean_3D # Generate clumps using the approach of
-Ferellec and McDowell (2010) mesh,clump=GenerateClump_Ferellec_McDowell
-(inputGeom, dmin, rmin, rstep, pmax, seed, output, outputVTK, visualise) #
-Generate clumps using the approach proposed in this code, involving the
-Euclidean transform of 3D images mesh,clump = GenerateClump_Euclidean_3D
-(inputGeom, N, rMin, div, overlap, output, outputVTK, visualise) ``` New users
-are advised to start from running the available examples in the [examples]
-(examples) folder, to get familiarised with the syntax and functionalities of
-CLUMP. ## Credits The MATLAB and Python implementations of CLUMP use different
-sets of external dependencies. - CLUMP_MATLAB uses several external functions
-available within the Matlab FEX community. We want to acknowledge the following
-contributions: - Qianqian Fang - [Iso2Mesh](https://uk.mathworks.com/
-matlabcentral/fileexchange/68258-iso2mesh) - Luigi Giaccari - [Surface
-Reconstruction From Scattered Points Cloud](https://www.mathworks.com/
-matlabcentral/fileexchange/63730-surface-reconstruction-from-scattered-points-
-cloud) - Pau MicÃ³ - [stlTools](https://uk.mathworks.com/matlabcentral/
-fileexchange/51200-stltools) - Anton Semechko - [Rigid body parameters of
-closed surface meshes](https://uk.mathworks.com/matlabcentral/fileexchange/
-48913-rigid-body-parameters-of-closed-surface-meshes) These external
-dependencies are added within the source code of CLUMP, to provide an out-of-
-the-box implementation. The licensing terms of each external dependency can be
-found inside the [lib](lib/) folder. - CLUMP_Python uses alternative
-dependencies that carry out the same operations as their MATLAB counterparts.
-Some of the dependencies have also been translated from MATLAB to Python. -
-[matplotlib](https://matplotlib.org/) - [numpy](https://numpy.org/) - [numpy-
-stl](https://numpy-stl.readthedocs.io/en/latest/) - [os](https://
-docs.python.org/3/library/os.html) - [pyvista](https://docs.pyvista.org/
-version/stable/) - [scipy](https://scipy.org/) - [time](https://
-docs.python.org/3/library/time.html) - [trimesh](https://trimesh.org/) ## BYOS
-(Bring Your Own Scripts)! If you enjoy using CLUMP, you are welcome to request
-the implementation of new features or even better contribute and share your
-implementations of new or existing clump-generation techniques. CLUMP was
+```Python from CLUMP.GenerateClump_Ferellec_McDowell import
+GenerateClump_Ferellec_McDowell from CLUMP.GenerateClump_Euclidean_3D import
+GenerateClump_Euclidean_3D # Generate clumps using the approach of Ferellec and
+McDowell (2010) mesh, clump = GenerateClump_Ferellec_McDowell(inputGeom, dmin,
+rmin, rstep, pmax, seed, output, outputVTK, visualise) # Generate clumps using
+the approach proposed in this code, involving the Euclidean transform of 3D
+images mesh, clump = GenerateClump_Euclidean_3D(inputGeom, N, rMin, div,
+overlap, output, outputVTK, visualise) ``` New users are advised to start from
+running the available examples in the [examples](examples) folder, to get
+familiarised with the syntax and functionalities of CLUMP. ## Credits The
+MATLAB and Python implementations of CLUMP use different sets of external
+dependencies. - CLUMP_MATLAB uses several external functions available within
+the Matlab FEX community. We want to acknowledge the following contributions: -
+Qianqian Fang - [Iso2Mesh](https://uk.mathworks.com/matlabcentral/fileexchange/
+68258-iso2mesh) - Luigi Giaccari - [Surface Reconstruction From Scattered
+Points Cloud](https://www.mathworks.com/matlabcentral/fileexchange/63730-
+surface-reconstruction-from-scattered-points-cloud) - Pau MicÃ³ - [stlTools]
+(https://uk.mathworks.com/matlabcentral/fileexchange/51200-stltools) - Anton
+Semechko - [Rigid body parameters of closed surface meshes](https://
+uk.mathworks.com/matlabcentral/fileexchange/48913-rigid-body-parameters-of-
+closed-surface-meshes) These external dependencies are added within the source
+code of CLUMP, to provide an out-of-the-box implementation. The licensing terms
+of each external dependency can be found inside the [lib](lib/) folder. -
+CLUMP_Python uses alternative dependencies that carry out the same operations
+as their MATLAB counterparts. Some of the dependencies have also been
+translated from MATLAB to Python. - [matplotlib](https://matplotlib.org/) -
+[numpy](https://numpy.org/) - [numpy-stl](https://numpy-stl.readthedocs.io/en/
+latest/) - [os](https://docs.python.org/3/library/os.html) - [pyvista](https://
+docs.pyvista.org/version/stable/) - [scipy](https://scipy.org/) - [time](https:
+//docs.python.org/3/library/time.html) - [trimesh](https://trimesh.org/) ##
+BYOS (Bring Your Own Scripts)! If you enjoy using CLUMP, you are welcome to
+request the implementation of new features or even better contribute and share
+your implementations of new or existing clump-generation techniques. CLUMP was
 created out of our intent to provide the DEM community with a means of easy
 comparison between different particle generation methods, by collecting them in
 one place and we share this tool hoping that members of the community will find
 it useful. So, feel free to expand the code, propose improvements and report
 issues. ## Acknowledging CLUMP Angelidakis, V., Nadimi, S., Otsubo, M. and
 Utili, S., 2021. CLUMP: A Code Library to generate Universal Multi-sphere
 Particles. SoftwareX 15, p.100735. [Download BibTeX entry](https://github.com/
```

### Comparing `clump-python-0.1.2/clump/ExtractSurface.py` & `clump-python-0.1.4/CLUMP/ExtractSurface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from scipy.spatial import ConvexHull
-from functions.utils.MyRobustCrust import MyRobustCrust
-from functions.utils.ParticlePlotter import mesh_plotter_trimesh
+from CLUMP.utils.MyRobustCrust import MyRobustCrust
+from CLUMP.utils.ParticlePlotter import mesh_plotter_trimesh
 
 #import matplotlib.pyplot as plt
 #from mpl_toolkits.mplot3d.art3d import Poly3DCollection
 
 """
 Tesselation of the surface of a clump into a surface mesh
 2021 © V. Angelidakis, S. Nadimi, M. Otsubo, S. Utili.
```

### Comparing `clump-python-0.1.2/clump/GenerateClump_Euclidean_3D.py` & `clump-python-0.1.4/CLUMP/GenerateClump_Euclidean_3D.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import trimesh
 from scipy.ndimage import distance_transform_edt
-from functions.utils.ParticlePlotter import clump_plotter_pyvista
+from CLUMP.utils.ParticlePlotter import clump_plotter_pyvista
 from scipy.io import loadmat
-from functions.utils import RigidBodyParameters
-from functions.utils.VTK_Writer import clump_to_VTK
+from CLUMP.utils import RigidBodyParameters
+from CLUMP.utils.VTK_Writer import clump_to_VTK
 
 """
 Clump generator using the Euclidean map for voxelated, 3D particles 
 2021 © V. Angelidakis, S. Nadimi, M. Otsubo, S. Utili.
 
 2021 MATLAB implementation by V. Angelidakis <v.angelidakis@qub.ac>
 2024 Translated from MATLAB to Python by U.A. Canbolat <utku.canbolat@fau.de>
```

### Comparing `clump-python-0.1.2/clump/GenerateClump_Favier.py` & `clump-python-0.1.4/CLUMP/GenerateClump_Favier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
-import functions.utils.RigidBodyParameters as RigidBodyParameters
-import functions.utils.STL_ReaderWriter as STL_ReaderWriter
-from functions.utils.ParticlePlotter import clump_plotter_pyvista
-from functions.utils.VTK_Writer import clump_to_VTK
+import CLUMP.utils.RigidBodyParameters as RigidBodyParameters
+import CLUMP.utils.STL_ReaderWriter as STL_ReaderWriter
+from CLUMP.utils.ParticlePlotter import clump_plotter_pyvista
+from CLUMP.utils.VTK_Writer import clump_to_VTK
 
 """
 Implementation of the clump-generation concept proposed by Favier et al. (1999) [1]
 2021 © V. Angelidakis, S. Nadimi, M. Otsubo, S. Utili.
 
 2021 MATLAB implementation by V. Angelidakis <v.angelidakis@qub.ac>
 2024 Translated from MATLAB to Python by U.A. Canbolat <utku.canbolat@fau.de>
```

### Comparing `clump-python-0.1.2/clump/GenerateClump_Ferellec_McDowell.py` & `clump-python-0.1.4/CLUMP/GenerateClump_Ferellec_McDowell.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
-import functions.utils.PatchNormals as PatchNormals
-import functions.utils.RigidBodyParameters as RigidBodyParameters
-import functions.utils.STL_ReaderWriter as STL_ReaderWriter
-from functions.utils.ParticlePlotter import clump_plotter_pyvista
-from functions.utils.VTK_Writer import clump_to_VTK
+import CLUMP.utils.PatchNormals as PatchNormals
+import CLUMP.utils.RigidBodyParameters as RigidBodyParameters
+import CLUMP.utils.STL_ReaderWriter as STL_ReaderWriter
+from CLUMP.utils.ParticlePlotter import clump_plotter_pyvista
+from CLUMP.utils.VTK_Writer import clump_to_VTK
 import trimesh
 
 """
 Implementation of the clump-generation concept proposed by Ferellec and McDowell (2010) [1]
 2021 © V. Angelidakis, S. Nadimi, M. Otsubo, S. Utili.
 
 2021 MATLAB implementation by V. Angelidakis <v.angelidakis@qub.ac>
```

### Comparing `clump-python-0.1.2/clump/utils/MyRobustCrust.py` & `clump-python-0.1.4/CLUMP/utils/MyRobustCrust.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.2/clump/utils/ParticlePlotter.py` & `clump-python-0.1.4/CLUMP/utils/ParticlePlotter.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.2/clump/utils/PatchNormals.py` & `clump-python-0.1.4/CLUMP/utils/PatchNormals.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.2/clump/utils/RigidBodyParameters.py` & `clump-python-0.1.4/CLUMP/utils/RigidBodyParameters.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.2/clump/utils/STL_ReaderWriter.py` & `clump-python-0.1.4/CLUMP/utils/STL_ReaderWriter.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.2/clump/utils/VTK_Writer.py` & `clump-python-0.1.4/CLUMP/utils/VTK_Writer.py`

 * *Files identical despite different names*

### Comparing `clump-python-0.1.2/clump_python.egg-info/PKG-INFO` & `clump-python-0.1.4/clump_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clump-python
-Version: 0.1.2
+Version: 0.1.4
 Summary: This Python library provides tools for creating and examining clumps using techniques: the Euclidean Distance Transform, Favier, and Ferellec-McDowell. It allows for the efficient generation of clumps and the extraction of their surfaces.
 Home-page: https://github.com/vsangelidakis/CLUMP
 Author: Utku Canbolat, Vasileios Angelidakis
 Author-email: utku.canbolat@fau.de
 License: GPL-3.0-only
 Keywords: Clump,Clump Generation,Euclidean Distance Transform,Favier,Ferellec-McDowell,Surface Extraction
 License-File: LICENSE
```

### Comparing `clump-python-0.1.2/setup.py` & `clump-python-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="clump-python",
-    version="0.1.2",
+    version="0.1.4",
     packages=find_packages(),
     install_requires=[
         'matplotlib',
         'numpy',
         'numpy-stl',
         'pyvista',
         'scipy',
```

