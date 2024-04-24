# Comparing `tmp/prefsampling-0.1.8.tar.gz` & `tmp/prefsampling-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefsampling-0.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "prefsampling-0.1.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `prefsampling-0.1.8.tar` & `prefsampling-0.1.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    35149 2024-02-21 13:59:46.647173 prefsampling-0.1.8/LICENSE.md
--rw-r--r--   0        0        0     4929 2024-02-21 13:59:46.647173 prefsampling-0.1.8/README.md
--rw-r--r--   0        0        0      101 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/__init__.py
--rw-r--r--   0        0        0      890 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/approval/__init__.py
--rw-r--r--   0        0        0     2244 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/approval/euclidean.py
--rw-r--r--   0        0        0     2270 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/approval/identity.py
--rw-r--r--   0        0        0     2995 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/approval/impartial.py
--rw-r--r--   0        0        0     3577 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/approval/noise.py
--rw-r--r--   0        0        0     1840 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/approval/partylist.py
--rw-r--r--   0        0        0     6020 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/approval/resampling.py
--rw-r--r--   0        0        0     1974 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/approval/truncated_ordinal.py
--rw-r--r--   0        0        0      379 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/core/__init__.py
--rw-r--r--   0        0        0     5592 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/core/composition.py
--rw-r--r--   0        0        0     3298 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/core/euclidean.py
--rw-r--r--   0        0        0     3323 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/core/filters.py
--rw-r--r--   0        0        0     1840 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/core/urn.py
--rw-r--r--   0        0        0     2512 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/inputvalidators.py
--rw-r--r--   0        0        0     1292 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/ordinal/__init__.py
--rw-r--r--   0        0        0     2045 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/ordinal/didi.py
--rw-r--r--   0        0        0     2288 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/ordinal/euclidean.py
--rw-r--r--   0        0        0     6248 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/ordinal/groupseparable.py
--rw-r--r--   0        0        0      724 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/ordinal/identity.py
--rw-r--r--   0        0        0     3890 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/ordinal/impartial.py
--rw-r--r--   0        0        0     7198 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/ordinal/mallows.py
--rw-r--r--   0        0        0     2177 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/ordinal/plackettluce.py
--rw-r--r--   0        0        0     9459 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/ordinal/singlecrossing.py
--rw-r--r--   0        0        0     6021 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/ordinal/singlepeaked.py
--rw-r--r--   0        0        0     1548 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/ordinal/urn.py
--rw-r--r--   0        0        0      438 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/tree/__init__.py
--rw-r--r--   0        0        0      901 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/tree/balanced.py
--rw-r--r--   0        0        0      827 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/tree/caterpillar.py
--rw-r--r--   0        0        0     7013 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/tree/node.py
--rw-r--r--   0        0        0    16099 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/tree/schroeder.py
--rw-r--r--   0        0        0      498 2024-02-21 13:59:46.735173 prefsampling-0.1.8/prefsampling/utils.py
--rw-r--r--   0        0        0     1248 2024-02-21 13:59:46.735173 prefsampling-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     6218 1970-01-01 00:00:00.000000 prefsampling-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-21 16:56:54.956849 prefsampling-0.1.9/LICENSE.md
+-rw-r--r--   0        0        0     4929 2024-02-21 16:56:54.956849 prefsampling-0.1.9/README.md
+-rw-r--r--   0        0        0      747 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/__init__.py
+-rw-r--r--   0        0        0      890 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/approval/__init__.py
+-rw-r--r--   0        0        0     2244 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/approval/euclidean.py
+-rw-r--r--   0        0        0     2270 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/approval/identity.py
+-rw-r--r--   0        0        0     2995 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/approval/impartial.py
+-rw-r--r--   0        0        0     3778 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/approval/noise.py
+-rw-r--r--   0        0        0     1840 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/approval/partylist.py
+-rw-r--r--   0        0        0     6020 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/approval/resampling.py
+-rw-r--r--   0        0        0     1974 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/approval/truncated_ordinal.py
+-rw-r--r--   0        0        0      379 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/core/__init__.py
+-rw-r--r--   0        0        0     5592 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/core/composition.py
+-rw-r--r--   0        0        0     3487 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/core/euclidean.py
+-rw-r--r--   0        0        0     3323 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/core/filters.py
+-rw-r--r--   0        0        0     1840 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/core/urn.py
+-rw-r--r--   0        0        0     2512 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/inputvalidators.py
+-rw-r--r--   0        0        0     1292 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/ordinal/__init__.py
+-rw-r--r--   0        0        0     2045 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/ordinal/didi.py
+-rw-r--r--   0        0        0     2288 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/ordinal/euclidean.py
+-rw-r--r--   0        0        0     6515 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/ordinal/groupseparable.py
+-rw-r--r--   0        0        0      724 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/ordinal/identity.py
+-rw-r--r--   0        0        0     3890 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/ordinal/impartial.py
+-rw-r--r--   0        0        0     7198 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/ordinal/mallows.py
+-rw-r--r--   0        0        0     2177 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/ordinal/plackettluce.py
+-rw-r--r--   0        0        0     9459 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/ordinal/singlecrossing.py
+-rw-r--r--   0        0        0     6021 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/ordinal/singlepeaked.py
+-rw-r--r--   0        0        0     1548 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/ordinal/urn.py
+-rw-r--r--   0        0        0      438 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/tree/__init__.py
+-rw-r--r--   0        0        0      901 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/tree/balanced.py
+-rw-r--r--   0        0        0      827 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/tree/caterpillar.py
+-rw-r--r--   0        0        0     7013 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/tree/node.py
+-rw-r--r--   0        0        0    16099 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/tree/schroeder.py
+-rw-r--r--   0        0        0      498 2024-02-21 16:56:55.040850 prefsampling-0.1.9/prefsampling/utils.py
+-rw-r--r--   0        0        0     1248 2024-02-21 16:56:55.040850 prefsampling-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6218 1970-01-01 00:00:00.000000 prefsampling-0.1.9/PKG-INFO
```

### Comparing `prefsampling-0.1.8/LICENSE.md` & `prefsampling-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/README.md` & `prefsampling-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/approval/__init__.py` & `prefsampling-0.1.9/prefsampling/approval/__init__.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/approval/euclidean.py` & `prefsampling-0.1.9/prefsampling/approval/euclidean.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/approval/identity.py` & `prefsampling-0.1.9/prefsampling/approval/identity.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/approval/impartial.py` & `prefsampling-0.1.9/prefsampling/approval/impartial.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/approval/noise.py` & `prefsampling-0.1.9/prefsampling/approval/noise.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 
 
 class NoiseType(Enum):
     """
     Constants representing the different types of noise that can be applied to the noise sampler.
     """
 
-    HAMMING = 1
+    HAMMING = "Hamming noise"
     """
     Hamming noise.
     """
 
-    JACCARD = 2
+    JACCARD = "Jaccard noise"
     """
     Jaccard noise.
     """
 
-    ZELINKA = 3
+    ZELINKA = "Zelinka noise"
     """
     Zelinka noise.
     """
 
-    BUNKE_SHEARER = 4
+    BUNKE_SHEARER = "Bunke-Shearer noise"
     """
     Bunke-Shearer noise.
     """
 
 
 @validate_num_voters_candidates
 def noise(
@@ -89,14 +89,18 @@
 
     A = {i for i in range(k)}
     B = set(range(num_candidates)) - A
 
     choices = []
     probabilities = []
 
+    if isinstance(noise_type, Enum):
+        noise_type = NoiseType(noise_type.value)
+    else:
+        noise_type = NoiseType(noise_type)
     # Prepare buckets
     for x in range(len(A) + 1):
         num_options_in = comb(len(A), x)
         for y in range(len(B) + 1):
             num_options_out = comb(len(B), y)
 
             if noise_type == NoiseType.HAMMING:
```

### Comparing `prefsampling-0.1.8/prefsampling/approval/partylist.py` & `prefsampling-0.1.9/prefsampling/approval/partylist.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/approval/resampling.py` & `prefsampling-0.1.9/prefsampling/approval/resampling.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/approval/truncated_ordinal.py` & `prefsampling-0.1.9/prefsampling/approval/truncated_ordinal.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/core/composition.py` & `prefsampling-0.1.9/prefsampling/core/composition.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/core/euclidean.py` & `prefsampling-0.1.9/prefsampling/core/euclidean.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 
 
 class EuclideanSpace(Enum):
     """
     Constants used to represent Euclidean spaces
     """
 
-    UNIFORM = 1
+    UNIFORM = "Uniform Space"
     """
     Uniform space
     """
-    GAUSSIAN = 2
+    GAUSSIAN = "Gaussian Space"
     """
     Gaussian space
     """
-    SPHERE = 3
+    SPHERE = "Spherical Space"
     """
-    Spheric space
+    Spherical space
     """
-    BALL = 4
+    BALL = "Ball Space"
     """
-    Ball space
+    Ball-shaped space
     """
 
 
 @validate_num_voters_candidates
 def election_positions(
     num_voters: int,
     num_candidates: int,
@@ -56,14 +56,18 @@
         The numpy generator to use for randomness.
 
     Returns
     -------
     (np.ndarray, np.ndarray)
         The position of the voters and of the candidates respectively.
     """
+    if isinstance(space, Enum):
+        space = EuclideanSpace(space.value)
+    else:
+        space = EuclideanSpace(space)
     if space == EuclideanSpace.UNIFORM:
         voters = rng.random((num_voters, dimension))
         candidates = rng.random((num_candidates, dimension))
     elif space == EuclideanSpace.GAUSSIAN:
         voters = rng.normal(loc=0.5, scale=0.15, size=(num_voters, dimension))
         candidates = rng.normal(loc=0.5, scale=0.15, size=(num_candidates, dimension))
     elif space == EuclideanSpace.SPHERE:
```

### Comparing `prefsampling-0.1.8/prefsampling/core/filters.py` & `prefsampling-0.1.9/prefsampling/core/filters.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/core/urn.py` & `prefsampling-0.1.9/prefsampling/core/urn.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/inputvalidators.py` & `prefsampling-0.1.9/prefsampling/inputvalidators.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/ordinal/__init__.py` & `prefsampling-0.1.9/prefsampling/ordinal/__init__.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/ordinal/didi.py` & `prefsampling-0.1.9/prefsampling/ordinal/didi.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/ordinal/euclidean.py` & `prefsampling-0.1.9/prefsampling/ordinal/euclidean.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/ordinal/groupseparable.py` & `prefsampling-0.1.9/prefsampling/ordinal/groupseparable.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import math
 from enum import Enum
 from itertools import chain
 
 import numpy as np
 
 from prefsampling.tree.schroeder import (
     schroeder_tree,
@@ -19,35 +18,35 @@
 
 class TreeSampler(Enum):
     """
     Constants use to represent different samplers for trees that can be used for group separable
     preferences.
     """
 
-    SCHROEDER = 1
+    SCHROEDER = "Scröder Tree by Alsonso, Rémy, Schott"
     """
     Random Schröder trees sampled following Alonso, Rémy, Schott (1997)
     """
 
-    SCHROEDER_UNIFORM = 2
+    SCHROEDER_UNIFORM = "Scröder Tree by brute-force"
     """
     Random Schröder sampled uniformly via complete enumeration algorithm
     """
 
-    SCHROEDER_LESCANNE = 3
+    SCHROEDER_LESCANNE = "Scröder Tree by Lescanne"
     """
     Random Schröder trees sampled following Lescanne (2022)
     """
 
-    CATERPILLAR = 4
+    CATERPILLAR = "Caterpillar Tree"
     """
     Caterpillar trees
     """
 
-    BALANCED = 5
+    BALANCED = "Balanced Tree"
     """
     Balanced trees
     """
 
 
 @validate_num_voters_candidates
 def group_separable(
@@ -93,14 +92,18 @@
     -------
         np.ndarray
             Ordinal votes.
     """
 
     rng = np.random.default_rng(seed)
 
+    if isinstance(tree_sampler, Enum):
+        tree_sampler = TreeSampler(tree_sampler.value)
+    else:
+        tree_sampler = TreeSampler(tree_sampler)
     if tree_sampler in (
         TreeSampler.SCHROEDER,
         TreeSampler.SCHROEDER_UNIFORM,
         TreeSampler.SCHROEDER_LESCANNE,
     ):
         buckets = np.zeros(num_candidates - 1)
         for r in range(1, num_candidates):
```

### Comparing `prefsampling-0.1.8/prefsampling/ordinal/identity.py` & `prefsampling-0.1.9/prefsampling/ordinal/identity.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/ordinal/impartial.py` & `prefsampling-0.1.9/prefsampling/ordinal/impartial.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/ordinal/mallows.py` & `prefsampling-0.1.9/prefsampling/ordinal/mallows.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/ordinal/plackettluce.py` & `prefsampling-0.1.9/prefsampling/ordinal/plackettluce.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/ordinal/singlecrossing.py` & `prefsampling-0.1.9/prefsampling/ordinal/singlecrossing.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/ordinal/singlepeaked.py` & `prefsampling-0.1.9/prefsampling/ordinal/singlepeaked.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/ordinal/urn.py` & `prefsampling-0.1.9/prefsampling/ordinal/urn.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/tree/balanced.py` & `prefsampling-0.1.9/prefsampling/tree/balanced.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/tree/caterpillar.py` & `prefsampling-0.1.9/prefsampling/tree/caterpillar.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/tree/node.py` & `prefsampling-0.1.9/prefsampling/tree/node.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/prefsampling/tree/schroeder.py` & `prefsampling-0.1.9/prefsampling/tree/schroeder.py`

 * *Files identical despite different names*

### Comparing `prefsampling-0.1.8/pyproject.toml` & `prefsampling-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "prefsampling"
-version = "0.1.8"
+version = "0.1.9"
 description = "Algorithms to sample preferences of all kinds."
 authors = [
   { name = "Simon Rey", email = "reysimon@orange.fr" },
   { name = "Stanisław Szufa", email = "s.szufa@gmail.com" },
 ]
 license = { file = "LICENSE.md" }
 readme = "README.md"
```

### Comparing `prefsampling-0.1.8/PKG-INFO` & `prefsampling-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefsampling
-Version: 0.1.8
+Version: 0.1.9
 Summary: Algorithms to sample preferences of all kinds.
 Author-email: Simon Rey <reysimon@orange.fr>, Stanisław Szufa <s.szufa@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

