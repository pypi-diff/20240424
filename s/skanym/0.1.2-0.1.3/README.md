# Comparing `tmp/skanym-0.1.2.tar.gz` & `tmp/skanym-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skanym-0.1.2.tar", last modified: Wed Apr 17 12:40:41 2024, max compression
+gzip compressed data, was "skanym-0.1.3.tar", last modified: Wed Apr 24 07:42:03 2024, max compression
```

## Comparing `skanym-0.1.2.tar` & `skanym-0.1.3.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 12:40:41.617611 skanym-0.1.2/
--rw-rw-rw-   0        0        0     1090 2023-11-07 12:29:13.000000 skanym-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2425 2024-04-17 12:40:41.614109 skanym-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-11-21 09:04:08.000000 skanym-0.1.2/README.md
--rw-rw-rw-   0        0        0     1077 2024-04-17 12:40:21.000000 skanym-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 12:40:41.618623 skanym-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-17 12:40:41.278147 skanym-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-17 12:40:41.313391 skanym-0.1.2/src/skanym/
--rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.2/src/skanym/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:40:41.347782 skanym-0.1.2/src/skanym/animators/
--rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.2/src/skanym/animators/__init__.py
--rw-rw-rw-   0        0        0     2315 2024-04-16 12:41:55.000000 skanym-0.1.2/src/skanym/animators/baseAnimator.py
--rw-rw-rw-   0        0        0    10365 2024-04-10 13:40:13.000000 skanym-0.1.2/src/skanym/animators/baseFkAnimator.py
--rw-rw-rw-   0        0        0     2019 2024-04-10 13:40:13.000000 skanym-0.1.2/src/skanym/animators/globalFkAnimator.py
--rw-rw-rw-   0        0        0     1391 2024-04-10 13:40:13.000000 skanym-0.1.2/src/skanym/animators/localFkAnimator.py
--rw-rw-rw-   0        0        0     9332 2024-04-16 13:47:14.000000 skanym-0.1.2/src/skanym/animators/pcaAnimator.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:40:41.363408 skanym-0.1.2/src/skanym/loaders/
--rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.2/src/skanym/loaders/__init__.py
--rw-rw-rw-   0        0        0    10732 2024-04-17 12:40:12.000000 skanym-0.1.2/src/skanym/loaders/fbxLoader.py
--rw-rw-rw-   0        0        0     7899 2024-04-08 11:54:24.000000 skanym-0.1.2/src/skanym/loaders/glbLoader.py
--rw-rw-rw-   0        0        0      655 2024-04-08 11:54:24.000000 skanym-0.1.2/src/skanym/loaders/iFileLoader.py
--rw-rw-rw-   0        0        0      423 2024-04-08 11:54:24.000000 skanym-0.1.2/src/skanym/loaders/objectLoader.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:40:41.367933 skanym-0.1.2/src/skanym/structures/
--rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.2/src/skanym/structures/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:40:41.394984 skanym-0.1.2/src/skanym/structures/animation/
--rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.2/src/skanym/structures/animation/__init__.py
--rw-rw-rw-   0        0        0     1644 2024-04-10 13:40:13.000000 skanym-0.1.2/src/skanym/structures/animation/animation.py
--rw-rw-rw-   0        0        0      547 2024-04-08 11:54:24.000000 skanym-0.1.2/src/skanym/structures/animation/animationCurve.py
--rw-rw-rw-   0        0        0     2041 2024-04-08 11:54:24.000000 skanym-0.1.2/src/skanym/structures/animation/iCurve.py
--rw-rw-rw-   0        0        0      890 2024-04-08 11:54:24.000000 skanym-0.1.2/src/skanym/structures/animation/key.py
--rw-rw-rw-   0        0        0     1146 2024-04-10 13:40:13.000000 skanym-0.1.2/src/skanym/structures/animation/positionCurve.py
--rw-rw-rw-   0        0        0     1208 2024-04-10 13:40:13.000000 skanym-0.1.2/src/skanym/structures/animation/quaternionCurve.py
--rw-rw-rw-   0        0        0      784 2024-04-08 11:54:24.000000 skanym-0.1.2/src/skanym/structures/animation/scalarCurve.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:40:41.405639 skanym-0.1.2/src/skanym/structures/character/
--rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.2/src/skanym/structures/character/__init__.py
--rw-rw-rw-   0        0        0     5439 2024-04-10 13:40:13.000000 skanym-0.1.2/src/skanym/structures/character/joint.py
--rw-rw-rw-   0        0        0     4233 2024-04-10 13:40:13.000000 skanym-0.1.2/src/skanym/structures/character/skeleton.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:40:41.423273 skanym-0.1.2/src/skanym/structures/data/
--rw-rw-rw-   0        0        0        0 2024-04-10 13:40:13.000000 skanym-0.1.2/src/skanym/structures/data/__init__.py
--rw-rw-rw-   0        0        0      771 2024-04-10 13:40:13.000000 skanym-0.1.2/src/skanym/structures/data/iTransform.py
--rw-rw-rw-   0        0        0     1305 2024-04-10 13:40:13.000000 skanym-0.1.2/src/skanym/structures/data/transform.py
--rw-rw-rw-   0        0        0     1179 2024-04-10 13:40:13.000000 skanym-0.1.2/src/skanym/structures/data/transformMatrix.py
--rw-rw-rw-   0        0        0     2305 2024-04-10 13:40:13.000000 skanym-0.1.2/src/skanym/structures/data/vectorizedArray.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:40:41.428937 skanym-0.1.2/src/skanym/utils/
--rw-rw-rw-   0        0        0        0 2024-03-20 13:33:29.000000 skanym-0.1.2/src/skanym/utils/__init__.py
--rw-rw-rw-   0        0        0    10909 2024-04-09 13:24:52.000000 skanym-0.1.2/src/skanym/utils/conversion.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:40:41.604028 skanym-0.1.2/src/skanym/utils/fbx_bindings/
--rw-rw-rw-   0        0        0     3075 2023-11-07 11:28:47.000000 skanym-0.1.2/src/skanym/utils/fbx_bindings/FbxCommon.py
--rw-rw-rw-   0        0        0        0 2024-03-19 18:17:16.000000 skanym-0.1.2/src/skanym/utils/fbx_bindings/__init__.py
--rw-rw-rw-   0        0        0  9286144 2023-11-07 11:28:47.000000 skanym-0.1.2/src/skanym/utils/fbx_bindings/fbx.pyd
--rw-rw-rw-   0        0        0   105472 2023-11-07 11:28:47.000000 skanym-0.1.2/src/skanym/utils/fbx_bindings/sip.pyd
-drwxrwxrwx   0        0        0        0 2024-04-17 12:40:41.610546 skanym-0.1.2/src/skanym.egg-info/
--rw-rw-rw-   0        0        0     2425 2024-04-17 12:40:41.000000 skanym-0.1.2/src/skanym.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1581 2024-04-17 12:40:41.000000 skanym-0.1.2/src/skanym.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 12:40:41.000000 skanym-0.1.2/src/skanym.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2024-04-17 12:40:41.000000 skanym-0.1.2/src/skanym.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-17 12:40:41.000000 skanym-0.1.2/src/skanym.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 07:42:03.997569 skanym-0.1.3/
+-rw-rw-rw-   0        0        0     1090 2023-11-07 12:29:13.000000 skanym-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2425 2024-04-24 07:42:03.994773 skanym-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-11-21 09:04:08.000000 skanym-0.1.3/README.md
+-rw-rw-rw-   0        0        0     1077 2024-04-24 07:35:26.000000 skanym-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-24 07:42:03.998090 skanym-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 07:42:03.638601 skanym-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 07:42:03.659516 skanym-0.1.3/src/skanym/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.3/src/skanym/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 07:42:03.697534 skanym-0.1.3/src/skanym/animators/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.3/src/skanym/animators/__init__.py
+-rw-rw-rw-   0        0        0     2315 2024-04-16 12:41:55.000000 skanym-0.1.3/src/skanym/animators/baseAnimator.py
+-rw-rw-rw-   0        0        0    10365 2024-04-10 13:40:13.000000 skanym-0.1.3/src/skanym/animators/baseFkAnimator.py
+-rw-rw-rw-   0        0        0     2019 2024-04-10 13:40:13.000000 skanym-0.1.3/src/skanym/animators/globalFkAnimator.py
+-rw-rw-rw-   0        0        0     1391 2024-04-10 13:40:13.000000 skanym-0.1.3/src/skanym/animators/localFkAnimator.py
+-rw-rw-rw-   0        0        0     9332 2024-04-16 13:47:14.000000 skanym-0.1.3/src/skanym/animators/pcaAnimator.py
+drwxrwxrwx   0        0        0        0 2024-04-24 07:42:03.719795 skanym-0.1.3/src/skanym/loaders/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.3/src/skanym/loaders/__init__.py
+-rw-rw-rw-   0        0        0    10937 2024-04-24 06:58:40.000000 skanym-0.1.3/src/skanym/loaders/assimpLoader.py
+-rw-rw-rw-   0        0        0    11891 2024-04-24 06:58:44.000000 skanym-0.1.3/src/skanym/loaders/fbxLoader.py
+-rw-rw-rw-   0        0        0     7899 2024-04-08 11:54:24.000000 skanym-0.1.3/src/skanym/loaders/glbLoader.py
+-rw-rw-rw-   0        0        0      655 2024-04-08 11:54:24.000000 skanym-0.1.3/src/skanym/loaders/iFileLoader.py
+-rw-rw-rw-   0        0        0      423 2024-04-08 11:54:24.000000 skanym-0.1.3/src/skanym/loaders/objectLoader.py
+drwxrwxrwx   0        0        0        0 2024-04-24 07:42:03.725563 skanym-0.1.3/src/skanym/structures/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.3/src/skanym/structures/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 07:42:03.755900 skanym-0.1.3/src/skanym/structures/animation/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.3/src/skanym/structures/animation/__init__.py
+-rw-rw-rw-   0        0        0     1644 2024-04-10 13:40:13.000000 skanym-0.1.3/src/skanym/structures/animation/animation.py
+-rw-rw-rw-   0        0        0      547 2024-04-08 11:54:24.000000 skanym-0.1.3/src/skanym/structures/animation/animationCurve.py
+-rw-rw-rw-   0        0        0     2041 2024-04-08 11:54:24.000000 skanym-0.1.3/src/skanym/structures/animation/iCurve.py
+-rw-rw-rw-   0        0        0      890 2024-04-08 11:54:24.000000 skanym-0.1.3/src/skanym/structures/animation/key.py
+-rw-rw-rw-   0        0        0     1146 2024-04-10 13:40:13.000000 skanym-0.1.3/src/skanym/structures/animation/positionCurve.py
+-rw-rw-rw-   0        0        0     1208 2024-04-10 13:40:13.000000 skanym-0.1.3/src/skanym/structures/animation/quaternionCurve.py
+-rw-rw-rw-   0        0        0      784 2024-04-08 11:54:24.000000 skanym-0.1.3/src/skanym/structures/animation/scalarCurve.py
+drwxrwxrwx   0        0        0        0 2024-04-24 07:42:03.766801 skanym-0.1.3/src/skanym/structures/character/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.3/src/skanym/structures/character/__init__.py
+-rw-rw-rw-   0        0        0     5546 2024-04-22 11:10:23.000000 skanym-0.1.3/src/skanym/structures/character/joint.py
+-rw-rw-rw-   0        0        0     4233 2024-04-10 13:40:13.000000 skanym-0.1.3/src/skanym/structures/character/skeleton.py
+drwxrwxrwx   0        0        0        0 2024-04-24 07:42:03.784575 skanym-0.1.3/src/skanym/structures/data/
+-rw-rw-rw-   0        0        0        0 2024-04-10 13:40:13.000000 skanym-0.1.3/src/skanym/structures/data/__init__.py
+-rw-rw-rw-   0        0        0      771 2024-04-10 13:40:13.000000 skanym-0.1.3/src/skanym/structures/data/iTransform.py
+-rw-rw-rw-   0        0        0     1305 2024-04-10 13:40:13.000000 skanym-0.1.3/src/skanym/structures/data/transform.py
+-rw-rw-rw-   0        0        0     1179 2024-04-10 13:40:13.000000 skanym-0.1.3/src/skanym/structures/data/transformMatrix.py
+-rw-rw-rw-   0        0        0     2305 2024-04-10 13:40:13.000000 skanym-0.1.3/src/skanym/structures/data/vectorizedArray.py
+drwxrwxrwx   0        0        0        0 2024-04-24 07:42:03.791723 skanym-0.1.3/src/skanym/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-20 13:33:29.000000 skanym-0.1.3/src/skanym/utils/__init__.py
+-rw-rw-rw-   0        0        0    10909 2024-04-09 13:24:52.000000 skanym-0.1.3/src/skanym/utils/conversion.py
+drwxrwxrwx   0        0        0        0 2024-04-24 07:42:03.983699 skanym-0.1.3/src/skanym/utils/fbx_bindings/
+-rw-rw-rw-   0        0        0     3075 2023-11-07 11:28:47.000000 skanym-0.1.3/src/skanym/utils/fbx_bindings/FbxCommon.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 18:17:16.000000 skanym-0.1.3/src/skanym/utils/fbx_bindings/__init__.py
+-rw-rw-rw-   0        0        0  9286144 2023-11-07 11:28:47.000000 skanym-0.1.3/src/skanym/utils/fbx_bindings/fbx.pyd
+-rw-rw-rw-   0        0        0   105472 2023-11-07 11:28:47.000000 skanym-0.1.3/src/skanym/utils/fbx_bindings/sip.pyd
+drwxrwxrwx   0        0        0        0 2024-04-24 07:42:03.991523 skanym-0.1.3/src/skanym.egg-info/
+-rw-rw-rw-   0        0        0     2425 2024-04-24 07:42:03.000000 skanym-0.1.3/src/skanym.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1616 2024-04-24 07:42:03.000000 skanym-0.1.3/src/skanym.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 07:42:03.000000 skanym-0.1.3/src/skanym.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2024-04-24 07:42:03.000000 skanym-0.1.3/src/skanym.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 07:42:03.000000 skanym-0.1.3/src/skanym.egg-info/top_level.txt
```

### Comparing `skanym-0.1.2/LICENSE.txt` & `skanym-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `skanym-0.1.2/PKG-INFO` & `skanym-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skanym
-Version: 0.1.2
+Version: 0.1.3
 Summary: Standalone package for skeletal animation
 Author-email: Dimitri Kohler <dimitri.kohler@he-arc.ch>
 License: MIT License
         
         Copyright (c) 2022 Dimitri Kohler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `skanym-0.1.2/pyproject.toml` & `skanym-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "skanym"
-version = "0.1.2"
+version = "0.1.3"
 description = "Standalone package for skeletal animation"
 readme = "README.md"
 requires-python = "==3.10.*"
 license = {file = "LICENSE.txt"} 
 authors = [
     {name = "Dimitri Kohler", email = "dimitri.kohler@he-arc.ch"},
 ]
```

### Comparing `skanym-0.1.2/src/skanym/animators/baseAnimator.py` & `skanym-0.1.3/src/skanym/animators/baseAnimator.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.2/src/skanym/animators/baseFkAnimator.py` & `skanym-0.1.3/src/skanym/animators/baseFkAnimator.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.2/src/skanym/animators/globalFkAnimator.py` & `skanym-0.1.3/src/skanym/animators/globalFkAnimator.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.2/src/skanym/animators/localFkAnimator.py` & `skanym-0.1.3/src/skanym/animators/localFkAnimator.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.2/src/skanym/animators/pcaAnimator.py` & `skanym-0.1.3/src/skanym/animators/pcaAnimator.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.2/src/skanym/loaders/fbxLoader.py` & `skanym-0.1.3/src/skanym/loaders/fbxLoader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import sys
 import warnings
 from typing import List
 from pathlib import Path
 
 import numpy as np
+import quaternion
+np.set_printoptions(precision=3, suppress=True)
 
 from skanym.loaders.iFileLoader import IFileLoader
 from skanym.structures.character.skeleton import Skeleton
 from skanym.structures.character.joint import Joint
 from skanym.structures.animation.animation import Animation
 from skanym.structures.animation.animationCurve import AnimationCurve
 from skanym.structures.animation.positionCurve import PositionCurve
 from skanym.structures.animation.quaternionCurve import QuaternionCurve
 from skanym.structures.animation.key import Key
 from skanym.structures.data.transform import Transform
+from skanym.utils import conversion
+from skanym.animators.globalFkAnimator import GlobalFkAnimator
 
 
 class FbxLoader(IFileLoader):
     def __init__(self, path: Path):
         super().__init__(path)
         try:
             import fbx
@@ -57,20 +61,30 @@
 
             rotation = skeleton_node.PreRotation.Get()
 
             v = self._fbx.FbxVector4(rotation)
 
             m = self._fbx.FbxAMatrix()
             m.SetR(v)
+            m_bis = np.ndarray((4,4))
+            for i in range(4):
+                for j in range(4):
+                    m_bis[i,j] = m.Get(i,j)
+            q_bis = conversion.rotationMatrixToQuaternion(m_bis[:3,:3])[0]    
+            q_bis = quaternion.as_float_array(q_bis)  
             q = m.GetQ()
-            orient = np.quaternion(q.GetAt(3), q.GetAt(0), q.GetAt(1), q.GetAt(2))
+
+            q = np.quaternion(q.GetAt(3), q.GetAt(0), q.GetAt(1), q.GetAt(2))           
+
+            # print(np.abs(quaternion.as_float_array(q)) - np.abs(q_bis))
+
             # if orient.w < 0:
             #     print(f"NEGATIVE QUATERNION for {joint_name} in {fbx_file_path.split('/')[-1]}, {orient}")
 
-            joint = Joint(name=joint_name, local_bind_transform=Transform(pos, orient))
+            joint = Joint(name=joint_name, local_bind_transform=Transform(pos, q))
 
             children = []
             for i in range(skeleton_node.GetChildCount()):
                 child_node = skeleton_node.GetChild(i)
                 children.append(child_node.GetName())
 
             joint_hierarchy.append((joint, children))
@@ -249,16 +263,24 @@
                     rX_curve.KeyGetValue(key_id),
                     rY_curve.KeyGetValue(key_id),
                     rZ_curve.KeyGetValue(key_id),
                 )
 
                 m = self._fbx.FbxAMatrix()
                 m.SetR(v)
+                m_bis = np.ndarray((4,4))
+                for i in range(4):
+                    for j in range(4):
+                        m_bis[i,j] = m.Get(i,j)
+                q_bis = conversion.rotationMatrixToQuaternion(m_bis[:3,:3])[0]
+                q_bis = quaternion.as_float_array(q_bis)
                 q = m.GetQ()
                 q = np.array([q.GetAt(3), q.GetAt(0), q.GetAt(1), q.GetAt(2)])
+                
+                # print(np.abs(q) - np.abs(q_bis))
 
                 # if q.w < 0:
                 #     print(f"NEGATIVE QUATERNION for {skeleton_node.GetName()} in {fbx_file_path.split('/')[-1]} at time {key_time}, {q}")
 
                 if "*" in key_time:
                     # Keys whose time is marked with "*" are not used in the animation.
                     # They are probably used to improve interpolation quality in between keyframes.
@@ -276,16 +298,19 @@
             key.time /= duration
 
         translation_curve = PositionCurve(translation_keys)
         rotation_curve = QuaternionCurve(rotation_keys)
         return translation_curve, rotation_curve, duration
 
 if __name__ == "__main__":
-    fbx = FbxLoader(Path("C:\dev\MotionMachine\skanym\src\skanym\examples\input\walk.fbx"))
-    skeleton = fbx.load_skeleton()
-    for joint in skeleton.as_joint_list()[0:3]:
-        print(type(joint.local_bind_transform.position))
-
-    animation = fbx.load_animation()
-    for curve in animation.position_curves[0:3]:
-        for key in curve.curve.keys[0:3]:
-            print(type(key.value))
+    np.set_printoptions(precision=6, suppress=True)    
+    np.set_printoptions(formatter={'float': lambda x: "{: 0.6f}".format(x)})
+    file_path = "C:/dev/MotionMachine/3D Animation DB/synthetic-animation-data/animations/run_kh0_sp0_as30.fbx"
+    fbx = FbxLoader(Path(file_path))
+    s = fbx.load_skeleton()
+    a = fbx.load_animation()
+    for anim_curve in a.rotation_curves:
+        print(s.get_joint_by_id(anim_curve.id).name)   
+        for key in anim_curve.curve.keys[0:3]:
+            # if a value is close to 0, set it to 0
+            key.value = np.where(np.abs(key.value) < 1e-3, 0, key.value)
+            print(key.value)
```

### Comparing `skanym-0.1.2/src/skanym/loaders/glbLoader.py` & `skanym-0.1.3/src/skanym/loaders/glbLoader.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.2/src/skanym/loaders/iFileLoader.py` & `skanym-0.1.3/src/skanym/loaders/iFileLoader.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.2/src/skanym/structures/animation/animation.py` & `skanym-0.1.3/src/skanym/structures/animation/animation.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.2/src/skanym/structures/animation/animationCurve.py` & `skanym-0.1.3/src/skanym/structures/animation/animationCurve.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.2/src/skanym/structures/animation/iCurve.py` & `skanym-0.1.3/src/skanym/structures/animation/iCurve.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.2/src/skanym/structures/animation/key.py` & `skanym-0.1.3/src/skanym/structures/animation/key.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.2/src/skanym/structures/animation/positionCurve.py` & `skanym-0.1.3/src/skanym/structures/animation/positionCurve.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.2/src/skanym/structures/animation/quaternionCurve.py` & `skanym-0.1.3/src/skanym/structures/animation/quaternionCurve.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.2/src/skanym/structures/animation/scalarCurve.py` & `skanym-0.1.3/src/skanym/structures/animation/scalarCurve.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.2/src/skanym/structures/character/joint.py` & `skanym-0.1.3/src/skanym/structures/character/joint.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,28 +22,31 @@
         Parent of the joint.
     children : (Joint) list
         List of children joints.
     local_bind_transform : Transform
         Initial transform of the joint in the parent's local coordinate system.
     """
 
-    def __init__(self, name="new joint", parent=None, children = None, local_bind_transform: ITransform=Transform()):
+    def __init__(self, name="new joint", parent=None, children = None, local_bind_transform: ITransform=None):
         """**Default constructor for the Joint class.**
 
         Parameters
         ----------
         name : str, optional
             Name of the joint, by default "new joint".
         local_bind_transform : Transform, optional
             Initial transform relative to the parent, by default identity transform.
         """
         self.name = name
         self.parent: Joint = None
         self.children: List[Joint] = []
-        self.local_bind_transform = local_bind_transform
+        if local_bind_transform is None:
+            self.local_bind_transform = Transform()
+        else:
+            self.local_bind_transform = local_bind_transform
 
 
     def add_child(self, joint: 'Joint'):
         """Makes the given joint a child of the current joint.
 
         Note
         ----
```

### Comparing `skanym-0.1.2/src/skanym/structures/character/skeleton.py` & `skanym-0.1.3/src/skanym/structures/character/skeleton.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.2/src/skanym/structures/data/iTransform.py` & `skanym-0.1.3/src/skanym/structures/data/iTransform.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.2/src/skanym/structures/data/transform.py` & `skanym-0.1.3/src/skanym/structures/data/transform.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.2/src/skanym/structures/data/transformMatrix.py` & `skanym-0.1.3/src/skanym/structures/data/transformMatrix.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.2/src/skanym/structures/data/vectorizedArray.py` & `skanym-0.1.3/src/skanym/structures/data/vectorizedArray.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.2/src/skanym/utils/conversion.py` & `skanym-0.1.3/src/skanym/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.2/src/skanym/utils/fbx_bindings/FbxCommon.py` & `skanym-0.1.3/src/skanym/utils/fbx_bindings/FbxCommon.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.2/src/skanym.egg-info/PKG-INFO` & `skanym-0.1.3/src/skanym.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skanym
-Version: 0.1.2
+Version: 0.1.3
 Summary: Standalone package for skeletal animation
 Author-email: Dimitri Kohler <dimitri.kohler@he-arc.ch>
 License: MIT License
         
         Copyright (c) 2022 Dimitri Kohler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `skanym-0.1.2/src/skanym.egg-info/SOURCES.txt` & `skanym-0.1.3/src/skanym.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/skanym/animators/__init__.py
 src/skanym/animators/baseAnimator.py
 src/skanym/animators/baseFkAnimator.py
 src/skanym/animators/globalFkAnimator.py
 src/skanym/animators/localFkAnimator.py
 src/skanym/animators/pcaAnimator.py
 src/skanym/loaders/__init__.py
+src/skanym/loaders/assimpLoader.py
 src/skanym/loaders/fbxLoader.py
 src/skanym/loaders/glbLoader.py
 src/skanym/loaders/iFileLoader.py
 src/skanym/loaders/objectLoader.py
 src/skanym/structures/__init__.py
 src/skanym/structures/animation/__init__.py
 src/skanym/structures/animation/animation.py
```

