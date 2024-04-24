# Comparing `tmp/imt_ikarus-1.0.2.tar.gz` & `tmp/imt_ikarus-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imt_ikarus-1.0.2.tar", last modified: Wed Apr 24 11:20:23 2024, max compression
+gzip compressed data, was "imt_ikarus-1.1.2.tar", last modified: Wed Apr 24 11:20:56 2024, max compression
```

## Comparing `imt_ikarus-1.0.2.tar` & `imt_ikarus-1.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:23.772284 imt_ikarus-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-24 11:20:23.772284 imt_ikarus-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-24 11:20:16.000000 imt_ikarus-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-24 11:20:16.000000 imt_ikarus-1.0.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-24 11:20:23.772284 imt_ikarus-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:23.764284 imt_ikarus-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:23.764284 imt_ikarus-1.0.2/src/ikarus/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 11:20:16.000000 imt_ikarus-1.0.2/src/ikarus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-24 11:20:16.000000 imt_ikarus-1.0.2/src/ikarus/_src.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:23.764284 imt_ikarus-1.0.2/src/ikarus/baselines/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-24 11:20:16.000000 imt_ikarus-1.0.2/src/ikarus/baselines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-04-24 11:20:16.000000 imt_ikarus-1.0.2/src/ikarus/baselines/qmt_baselines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:23.768284 imt_ikarus-1.0.2/src/ikarus/baselines/riann/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 11:20:16.000000 imt_ikarus-1.0.2/src/ikarus/baselines/riann/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1471345 2024-04-24 11:20:16.000000 imt_ikarus-1.0.2/src/ikarus/baselines/riann/riann.onnx
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-24 11:20:16.000000 imt_ikarus-1.0.2/src/ikarus/baselines/riann/riann.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:23.768284 imt_ikarus-1.0.2/src/ikarus/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-24 11:20:16.000000 imt_ikarus-1.0.2/src/ikarus/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-24 11:20:16.000000 imt_ikarus-1.0.2/src/ikarus/benchmark/_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:23.768284 imt_ikarus-1.0.2/src/ikarus/benchmark/xmls/
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-24 11:20:16.000000 imt_ikarus-1.0.2/src/ikarus/benchmark/xmls/arm.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-24 11:20:16.000000 imt_ikarus-1.0.2/src/ikarus/benchmark/xmls/gait.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-24 11:20:16.000000 imt_ikarus-1.0.2/src/ikarus/dataverse_github.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-24 11:20:16.000000 imt_ikarus-1.0.2/src/ikarus/test_dataverse_github.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-24 11:20:16.000000 imt_ikarus-1.0.2/src/ikarus/test_src.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-24 11:20:16.000000 imt_ikarus-1.0.2/src/ikarus/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-04-24 11:20:16.000000 imt_ikarus-1.0.2/src/ikarus/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:23.768284 imt_ikarus-1.0.2/src/imt_ikarus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-24 11:20:23.000000 imt_ikarus-1.0.2/src/imt_ikarus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-24 11:20:23.000000 imt_ikarus-1.0.2/src/imt_ikarus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:20:23.000000 imt_ikarus-1.0.2/src/imt_ikarus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 11:20:23.000000 imt_ikarus-1.0.2/src/imt_ikarus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 11:20:23.000000 imt_ikarus-1.0.2/src/imt_ikarus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:56.270224 imt_ikarus-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-24 11:20:56.270224 imt_ikarus-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-24 11:20:56.270224 imt_ikarus-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:56.262224 imt_ikarus-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:56.266224 imt_ikarus-1.1.2/src/ikarus/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/_src.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:56.266224 imt_ikarus-1.1.2/src/ikarus/baselines/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/baselines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/baselines/qmt_baselines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:56.266224 imt_ikarus-1.1.2/src/ikarus/baselines/riann/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/baselines/riann/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1471345 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/baselines/riann/riann.onnx
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/baselines/riann/riann.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:56.270224 imt_ikarus-1.1.2/src/ikarus/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/benchmark/_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:56.270224 imt_ikarus-1.1.2/src/ikarus/benchmark/xmls/
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/benchmark/xmls/arm.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/benchmark/xmls/gait.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/dataverse_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/test_dataverse_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/test_src.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:56.270224 imt_ikarus-1.1.2/src/imt_ikarus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-24 11:20:56.000000 imt_ikarus-1.1.2/src/imt_ikarus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-24 11:20:56.000000 imt_ikarus-1.1.2/src/imt_ikarus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:20:56.000000 imt_ikarus-1.1.2/src/imt_ikarus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-24 11:20:56.000000 imt_ikarus-1.1.2/src/imt_ikarus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 11:20:56.000000 imt_ikarus-1.1.2/src/imt_ikarus.egg-info/top_level.txt
```

### Comparing `imt_ikarus-1.0.2/PKG-INFO` & `imt_ikarus-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imt-ikarus
-Version: 1.0.2
+Version: 1.1.2
 Summary: IKArus - Inertial and Optical Data of Kinematic ChAin Motion
 Author-email: Simon Bachhuber <simon.bachhuber@fau.de>
 Project-URL: Homepage, https://github.com/SimiPixel/ikarus
 Project-URL: Issues, https://github.com/SimiPixel/ikarus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,15 @@
 Requires-Dist: qmt
 Requires-Dist: scipy
 Requires-Dist: dm-tree
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: imt-tree-utils
 Provides-Extra: benchmark
+Requires-Dist: imt-ring; extra == "benchmark"
 Provides-Extra: baselines
 Requires-Dist: onnxruntime; extra == "baselines"
 
 # `IKArus` <ins>I</ins>nertial and Optical Data of <ins>K</ins>inematic Ch<ins>A</ins>in Motion
 
 This repository hosts the `Ikarus` dataset.
 It contains *real-world* IMU and OMC data from kinematic chain motion.
```

### Comparing `imt_ikarus-1.0.2/pyproject.toml` & `imt_ikarus-1.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "imt-ikarus"
-version = "1.0.2"
+version = "1.1.2"
 authors = [
   { name="Simon Bachhuber", email="simon.bachhuber@fau.de" },
 ]
 description = "IKArus - Inertial and Optical Data of Kinematic ChAin Motion"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -24,14 +24,15 @@
     "requests",
     "pandas",
     "imt-tree-utils",
 ]
 
 [project.optional-dependencies]
 benchmark = [
+    "imt-ring",
 ]
 baselines = [
     "onnxruntime",
 ]
 
 [project.urls]
 Homepage = "https://github.com/SimiPixel/ikarus"
```

### Comparing `imt_ikarus-1.0.2/readme.md` & `imt_ikarus-1.1.2/readme.md`

 * *Files identical despite different names*

### Comparing `imt_ikarus-1.0.2/src/ikarus/_src.py` & `imt_ikarus-1.1.2/src/ikarus/_src.py`

 * *Files identical despite different names*

### Comparing `imt_ikarus-1.0.2/src/ikarus/baselines/qmt_baselines.py` & `imt_ikarus-1.1.2/src/ikarus/baselines/qmt_baselines.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from typing import Optional
 
 import jax
 import numpy as np
 import qmt
 from ring import maths
-from ring import sim2real
-from ring import utils
-from ring.algorithms import sensors
 from ring.ml import base as ml_base
 
 from .riann import RIANN
 
 
 def _riann_predict(gyr, acc, params: dict):
     fs = 1 / params["Ts"]
@@ -28,24 +25,29 @@
 
 
 class AttitudeBaseline(ml_base.AbstractFilterUnbatched):
     def __init__(self, method: str) -> None:
         """ """
         self._name, self._method = _attitude_methods[method]
 
-    def _predict_2d(self, X, sys):
-        quats = dict()
-        for name, imu_data in X.items():
-            quats[name] = self._method(
-                gyr=imu_data["gyr"], acc=imu_data["acc"], params=dict(Ts=float(sys.dt))
+    def _apply_unbatched(self, X, params, state, y, lam):
+
+        T, N, F = X.shape
+        assert F == 10 or F == 7
+        dt = float(X[0, 0, -1])
+
+        quats = np.zeros((T, N, 4))
+        for i in range(N):
+            quats[:, i] = self._method(
+                gyr=X[:, i, 3:6], acc=X[:, i, :3], params=dict(Ts=dt)
             )
 
         # NOTE CONVENTION !!
-        quats = {name: qmt.qinv(quats[name]) for name in quats}
-        return quats
+        quats = qmt.qinv(quats)
+        return quats, state
 
 
 class TwoSeg1D(ml_base.AbstractFilterUnbatched):
     def __init__(
         self,
         method: str,
         seg: str,
@@ -112,71 +114,51 @@
             None,
             estSettings=dict(constraint=self.method),
         )[0]
 
         # NOTE CONVENTION !!
         quats = {name: qmt.qinv(quats[name]) for name in quats}
 
-        quats = _maybe_lowpassfilter_quats(quats, self.lpf_glo)
+        # quats = _maybe_lowpassfilter_quats(quats, self.lpf_glo)
 
         yhat = dict()
 
         # tibia to femur
         yhat[second] = maths.quat_mul(quats[first], maths.quat_inv(quats[second]))
         # add it such that it gets low-pass-filtered for `lpf_rel` too
         yhat[first] = quats[first]
-        yhat = _maybe_lowpassfilter_quats(yhat, self.lpf_rel)
+        # yhat = _maybe_lowpassfilter_quats(yhat, self.lpf_rel)
 
         return yhat
 
 
 class VQF_9D(ml_base.AbstractFilterUnbatched):
     def __init__(
         self,
         name: str,
-        Ts: float = 0.01,
-        lpf_glo: Optional[float] = None,
-        lpf_rel: Optional[float] = None,
     ):
-        """Use 9D VQF on kinematic chain.
-
-        Args:
-            name (str): Name of filter
-            chain (list[str]): Name of segments that make up chain.
-        """
         self._name = name
-        self.Ts = Ts
-        self.lpf_glo, self.lpf_rel = lpf_glo, lpf_rel
 
-    def _predict_2d(self, X, sys, y: dict | None):
-        quats = dict()
-        for name, imu_data in X.items():
-            quats[name] = qmt.oriEstVQF(
-                imu_data["gyr"],
-                imu_data["acc"],
-                imu_data["mag"],
-                params=dict(Ts=self.Ts),
+    def _apply_unbatched(self, X, params, state, y, lam):
+
+        assert lam is not None
+        T, N, F = X.shape
+        assert F == 13 or F == 10
+        dt = float(X[0, 0, -1])
+
+        quats = np.zeros((T, N, 4))
+        for i in range(N):
+            quats[:, i] = qmt.oriEstVQF(
+                gyr=X[:, i, 3:6], acc=X[:, i, :3], mag=X[:, i, 6:9], params=dict(Ts=dt)
             )
 
         # NOTE CONVENTION !!
-        quats = {name: qmt.qinv(quats[name]) for name in quats}
-
-        quats = _maybe_lowpassfilter_quats(quats, self.lpf_glo)
-        # self.transfer_ground_truth_heading(sys, y, quats)
-        quats = utils.dict_to_nested(quats, "quat")
-
-        xs = sim2real.xs_from_raw(sys, quats, qinv=False)
-        yhat = sensors.rel_pose(sys, xs)
-        yhat = utils.dict_union(yhat, sensors.root_full(sys, xs, sys))
-
-        yhat = _maybe_lowpassfilter_quats(yhat, self.lpf_rel)
-        self.transfer_ground_truth_heading(sys, y, yhat)
-        return yhat
+        quats = qmt.qinv(quats)
 
+        _quats = quats.copy()
+        for i, p in enumerate(lam):
+            if p == -1:
+                continue
+            q1, q2 = quats[:, p], quats[:, i]
+            _quats[:, i] = qmt.qmult(q1, qmt.qinv(q2))
 
-def _maybe_lowpassfilter_quats(quats: dict, cutoff_freq: float | None):
-    if cutoff_freq is None:
-        return quats
-    return {
-        name: maths.quat_lowpassfilter(quats[name], cutoff_freq, filtfilt=True)
-        for name in quats
-    }
+        return _quats, state
```

### Comparing `imt_ikarus-1.0.2/src/ikarus/baselines/riann/riann.onnx` & `imt_ikarus-1.1.2/src/ikarus/baselines/riann/riann.onnx`

 * *Files identical despite different names*

### Comparing `imt_ikarus-1.0.2/src/ikarus/baselines/riann/riann.py` & `imt_ikarus-1.1.2/src/ikarus/baselines/riann/riann.py`

 * *Files identical despite different names*

### Comparing `imt_ikarus-1.0.2/src/ikarus/benchmark/_benchmark.py` & `imt_ikarus-1.1.2/src/ikarus/benchmark/_benchmark.py`

 * *Files identical despite different names*

### Comparing `imt_ikarus-1.0.2/src/ikarus/benchmark/xmls/arm.xml` & `imt_ikarus-1.1.2/src/ikarus/benchmark/xmls/arm.xml`

 * *Files 0% similar despite different names*

#### Comparing `imt_ikarus-1.0.2/src/ikarus/benchmark/xmls/arm.xml` & `imt_ikarus-1.1.2/src/ikarus/benchmark/xmls/arm.xml`

```diff
@@ -10,48 +10,48 @@
       <geom type="box" mass="1" pos="0.1 0 0" dim="0.2 0.05 0.05" color="dustin_exp_blue"/>
       <geom type="box" mass="0.1" pos="0.03 -0.05 0" dim="0.01 0.1 0.01" color="dustin_exp_white"/>
       <geom type="box" mass="0.1" pos="0.17 0.05 0" dim="0.01 0.1 0.01" color="dustin_exp_white"/>
       <body name="imu1" joint="frozen" pos="0.1 0.0 0.035" pos_min="0.05 -0.05 -0.05" pos_max="0.15 0.05 0.05">
         <omc name="seg1" pos_marker="2" pos=".1 0 .015"/>
         <geom type="box" mass="0.1" dim="0.05 0.03 0.02" color="dustin_exp_orange"/>
       </body>
-      <body name="seg5" joint="spherical" pos="0.2 0 0" pos_min="0.15 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="5 5 5">
-        <omc name="seg5" pos_marker="2" pos="0 0 -.02"/>
+      <body name="seg2" joint="spherical" pos="0.2 0 0" pos_min="0.15 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="5 5 5">
+        <omc name="seg2" pos_marker="2" pos="0 0 -.02"/>
         <geom type="box" mass="1" pos="0.1 0 0" dim="0.2 0.05 0.05" color="dustin_exp_white"/>
         <geom type="box" mass="0.1" pos="0.03 -0.05 0" dim="0.01 0.1 0.01" color="dustin_exp_white"/>
         <geom type="box" mass="0.1" pos="0.17 -0.05 0" dim="0.01 0.1 0.01" color="dustin_exp_white"/>
-        <body name="imu5" joint="frozen" pos="0.1 0.0 0.035" pos_min="0.05 -0.05 -0.05" pos_max="0.15 0.05 0.05">
-          <omc name="seg5" pos_marker="2" pos=".1 0 .015"/>
+        <body name="imu2" joint="frozen" pos="0.1 0.0 0.035" pos_min="0.05 -0.05 -0.05" pos_max="0.15 0.05 0.05">
+          <omc name="seg2" pos_marker="2" pos=".1 0 .015"/>
           <geom type="box" mass="0.1" dim="0.05 0.03 0.02" color="dustin_exp_orange"/>
         </body>
-        <body name="seg2" joint="rx" pos="0.2 0 0" pos_min="0 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3">
-          <omc name="seg2" pos_marker="1" pos="0 0 -.02"/>
+        <body name="seg3" joint="rx" pos="0.2 0 0" pos_min="0 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3">
+          <omc name="seg3" pos_marker="1" pos="0 0 -.02"/>
           <geom type="box" mass="1" pos="0.1 0 0" dim="0.2 0.05 0.05" color="dustin_exp_blue"/>
           <geom type="box" mass="0.1" pos="0.05 0.05 0" dim="0.01 0.1 0.01" color="black"/>
           <geom type="box" mass="0.1" pos="0.15 -0.05 0" dim="0.01 0.1 0.01" color="black"/>
-          <body name="imu2" joint="frozen" pos="0.1 0.0 0.035" pos_min="0.05 -0.05 -0.05" pos_max="0.15 0.05 0.05">
-            <omc name="seg2" pos_marker="1" pos=".1 0 .015"/>
+          <body name="imu3" joint="frozen" pos="0.1 0.0 0.035" pos_min="0.05 -0.05 -0.05" pos_max="0.15 0.05 0.05">
+            <omc name="seg3" pos_marker="1" pos=".1 0 .015"/>
             <geom type="box" mass="0.1" dim="0.05 0.03 0.02" color="dustin_exp_orange"/>
           </body>
-          <body name="seg3" joint="ry" pos="0.2 0 0" pos_min="0 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3">
-            <omc name="seg3" pos_marker="2" pos="0 0 -.02"/>
+          <body name="seg4" joint="ry" pos="0.2 0 0" pos_min="0 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3">
+            <omc name="seg4" pos_marker="2" pos="0 0 -.02"/>
             <geom type="box" mass="1" pos="0.1 0 0" dim="0.2 0.05 0.05" color="dustin_exp_white"/>
             <geom type="box" mass="0.1" pos="0.1 0.05 0" dim="0.01 0.1 0.01" color="black"/>
             <geom type="box" mass="0.1" pos="0.15 -0.05 0" dim="0.01 0.1 0.01" color="black"/>
-            <body name="imu3" joint="frozen" pos="0.1 0.0 0.035" pos_min="0.05 -0.05 -0.05" pos_max="0.15 0.05 0.05">
-              <omc name="seg3" pos_marker="2" pos=".1 0 .015"/>
+            <body name="imu4" joint="frozen" pos="0.1 0.0 0.035" pos_min="0.05 -0.05 -0.05" pos_max="0.15 0.05 0.05">
+              <omc name="seg4" pos_marker="2" pos=".1 0 .015"/>
               <geom type="box" mass="0.1" dim="0.05 0.03 0.02" color="dustin_exp_orange"/>
             </body>
-            <body name="seg4" joint="rz" pos="0.2 0 0" pos_min="0 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3">
-              <omc name="seg4" pos_marker="4" pos="0 0 -.02"/>
+            <body name="seg5" joint="rz" pos="0.2 0 0" pos_min="0 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3">
+              <omc name="seg5" pos_marker="4" pos="0 0 -.02"/>
               <geom type="box" mass="1" pos="0.1 0 0" dim="0.2 0.05 0.05" color="dustin_exp_white"/>
               <geom type="box" mass="0.1" pos="0.03 -0.05 0" dim="0.01 0.1 0.01" color="black"/>
               <geom type="box" mass="0.1" pos="0.17 -0.05 0" dim="0.01 0.1 0.01" color="black"/>
-              <body name="imu4" joint="frozen" pos="0.1 0.0 0.035" pos_min="0.05 -0.05 -0.05" pos_max="0.15 0.05 0.05">
-                <omc name="seg4" pos_marker="4" pos=".1 0 .015"/>
+              <body name="imu5" joint="frozen" pos="0.1 0.0 0.035" pos_min="0.05 -0.05 -0.05" pos_max="0.15 0.05 0.05">
+                <omc name="seg5" pos_marker="4" pos=".1 0 .015"/>
                 <geom type="box" mass="0.1" dim="0.05 0.03 0.02" color="dustin_exp_orange"/>
               </body>
             </body>
           </body>
         </body>
       </body>
     </body>
```

### Comparing `imt_ikarus-1.0.2/src/ikarus/benchmark/xmls/gait.xml` & `imt_ikarus-1.1.2/src/ikarus/benchmark/xmls/gait.xml`

 * *Files 0% similar despite different names*

#### Comparing `imt_ikarus-1.0.2/src/ikarus/benchmark/xmls/gait.xml` & `imt_ikarus-1.1.2/src/ikarus/benchmark/xmls/gait.xml`

```diff
@@ -1,47 +1,47 @@
 <?xml version="1.0" encoding="utf-8"?>
 <x_xy model="gait">
   <options gravity="0 0 9.81" dt="0.01"/>
   <defaults>
     <geom edge_color="black" color="1 0.8 0.7 1"/>
   </defaults>
   <worldbody>
-    <body name="seg4" joint="free" euler="0 -90 0" damping="5 5 5 25 25 25">
-      <omc name="seg4" pos_marker="4" pos="0 0 -.02"/>
+    <body name="seg5" joint="free" euler="0 -90 0" damping="5 5 5 25 25 25">
+      <omc name="seg5" pos_marker="4" pos="0 0 -.02"/>
       <geom type="box" mass="1" pos="0.1 0 0" dim="0.2 0.05 0.05"/>
-      <body name="imu4" joint="frozen" pos="0.1 0.0 0.035" pos_min="0.05 -0.05 -0.05" pos_max="0.15 0.05 0.05">
-        <omc name="seg4" pos_marker="4" pos=".1 0 .015"/>
+      <body name="imu5" joint="frozen" pos="0.1 0.0 0.035" pos_min="0.05 -0.05 -0.05" pos_max="0.15 0.05 0.05">
+        <omc name="seg5" pos_marker="4" pos=".1 0 .015"/>
         <geom type="box" mass="0.1" dim="0.05 0.03 0.02" color="green"/>
       </body>
       <body name="seg1" joint="ry" pos="0.2 0 0" pos_min="0.15 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3">
         <omc name="seg1" pos_marker="2" pos="0 0 -.02"/>
         <geom type="box" mass="1" pos="0.1 0 0" dim="0.2 0.05 0.05"/>
         <body name="imu1" joint="frozen" pos="0.1 0.0 0.035" pos_min="0.05 -0.05 -0.05" pos_max="0.15 0.05 0.05">
           <omc name="seg1" pos_marker="2" pos=".1 0 .015"/>
           <geom type="box" mass="0.1" dim="0.05 0.03 0.02" color="orange"/>
         </body>
-        <body name="seg5" joint="saddle" pos="0.2 0 0" pos_min="0.15 -0.05 -0.05" pos_max="0.35 0.05 0.05" euler="0 0 90" damping="3 3">
-          <omc name="seg5" pos_marker="2" pos="0 0 -.02"/>
+        <body name="seg2" joint="saddle" pos="0.2 0 0" pos_min="0.15 -0.05 -0.05" pos_max="0.35 0.05 0.05" euler="0 0 90" damping="3 3">
+          <omc name="seg2" pos_marker="2" pos="0 0 -.02"/>
           <geom type="box" mass="1" pos="0.1 0 0" dim="0.2 0.05 0.05"/>
-          <body name="imu5" joint="frozen" pos="0.1 0.0 0.035" pos_min="0.05 -0.05 -0.05" pos_max="0.15 0.05 0.05">
-            <omc name="seg5" pos_marker="2" pos=".1 0 .015"/>
+          <body name="imu2" joint="frozen" pos="0.1 0.0 0.035" pos_min="0.05 -0.05 -0.05" pos_max="0.15 0.05 0.05">
+            <omc name="seg2" pos_marker="2" pos=".1 0 .015"/>
             <geom type="box" mass="0.1" dim="0.05 0.03 0.02" color="orange"/>
           </body>
-          <body name="seg2" joint="saddle" pos="0.2 0 0" pos_min="0.15 -0.05 -0.05" pos_max="0.35 0.05 0.05" euler="0 0 90" damping="3 3">
-            <omc name="seg2" pos_marker="1" pos="0 0 -.02"/>
+          <body name="seg3" joint="saddle" pos="0.2 0 0" pos_min="0.15 -0.05 -0.05" pos_max="0.35 0.05 0.05" euler="0 0 90" damping="3 3">
+            <omc name="seg3" pos_marker="1" pos="0 0 -.02"/>
             <geom type="box" mass="1" pos="0.1 0 0" dim="0.2 0.05 0.05"/>
-            <body name="imu2" joint="frozen" pos="0.1 0.0 0.035" pos_min="0.05 -0.05 -0.05" pos_max="0.15 0.05 0.05">
-              <omc name="seg2" pos_marker="1" pos=".1 0 .015"/>
+            <body name="imu3" joint="frozen" pos="0.1 0.0 0.035" pos_min="0.05 -0.05 -0.05" pos_max="0.15 0.05 0.05">
+              <omc name="seg3" pos_marker="1" pos=".1 0 .015"/>
               <geom type="box" mass="0.1" dim="0.05 0.03 0.02" color="orange"/>
             </body>
-            <body name="seg3" joint="ry" pos="0.2 0 0" pos_min="0.15 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3">
-              <omc name="seg3" pos_marker="2" pos="0 0 -.02"/>
+            <body name="seg4" joint="ry" pos="0.2 0 0" pos_min="0.15 -0.05 -0.05" pos_max="0.35 0.05 0.05" damping="3">
+              <omc name="seg4" pos_marker="2" pos="0 0 -.02"/>
               <geom type="box" mass="1" pos="0.1 0 0" dim="0.2 0.05 0.05"/>
-              <body name="imu3" joint="frozen" pos="0.1 0.0 0.035" pos_min="0.05 -0.05 -0.05" pos_max="0.15 0.05 0.05">
-                <omc name="seg3" pos_marker="2" pos=".1 0 .015"/>
+              <body name="imu4" joint="frozen" pos="0.1 0.0 0.035" pos_min="0.05 -0.05 -0.05" pos_max="0.15 0.05 0.05">
+                <omc name="seg4" pos_marker="2" pos=".1 0 .015"/>
                 <geom type="box" mass="0.1" dim="0.05 0.03 0.02" color="blue"/>
               </body>
             </body>
           </body>
         </body>
       </body>
     </body>
```

### Comparing `imt_ikarus-1.0.2/src/ikarus/dataverse_github.py` & `imt_ikarus-1.1.2/src/ikarus/dataverse_github.py`

 * *Files identical despite different names*

### Comparing `imt_ikarus-1.0.2/src/ikarus/test_src.py` & `imt_ikarus-1.1.2/src/ikarus/test_src.py`

 * *Files identical despite different names*

### Comparing `imt_ikarus-1.0.2/src/ikarus/test_utils.py` & `imt_ikarus-1.1.2/src/ikarus/test_utils.py`

 * *Files identical despite different names*

### Comparing `imt_ikarus-1.0.2/src/ikarus/utils.py` & `imt_ikarus-1.1.2/src/ikarus/utils.py`

 * *Files identical despite different names*

### Comparing `imt_ikarus-1.0.2/src/imt_ikarus.egg-info/PKG-INFO` & `imt_ikarus-1.1.2/src/imt_ikarus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imt-ikarus
-Version: 1.0.2
+Version: 1.1.2
 Summary: IKArus - Inertial and Optical Data of Kinematic ChAin Motion
 Author-email: Simon Bachhuber <simon.bachhuber@fau.de>
 Project-URL: Homepage, https://github.com/SimiPixel/ikarus
 Project-URL: Issues, https://github.com/SimiPixel/ikarus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,15 @@
 Requires-Dist: qmt
 Requires-Dist: scipy
 Requires-Dist: dm-tree
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: imt-tree-utils
 Provides-Extra: benchmark
+Requires-Dist: imt-ring; extra == "benchmark"
 Provides-Extra: baselines
 Requires-Dist: onnxruntime; extra == "baselines"
 
 # `IKArus` <ins>I</ins>nertial and Optical Data of <ins>K</ins>inematic Ch<ins>A</ins>in Motion
 
 This repository hosts the `Ikarus` dataset.
 It contains *real-world* IMU and OMC data from kinematic chain motion.
```

### Comparing `imt_ikarus-1.0.2/src/imt_ikarus.egg-info/SOURCES.txt` & `imt_ikarus-1.1.2/src/imt_ikarus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

