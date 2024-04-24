# Comparing `tmp/tolvera-0.1.0rc5.tar.gz` & `tmp/tolvera-0.1.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tolvera-0.1.0rc5.tar", max compression
+gzip compressed data, was "tolvera-0.1.0rc6.tar", max compression
```

## Comparing `tolvera-0.1.0rc5.tar` & `tolvera-0.1.0rc6.tar`

### file list

```diff
@@ -1,35 +1,46 @@
--rw-r--r--   0        0        0    34523 2023-11-23 15:54:16.427339 tolvera-0.1.0rc5/LICENSE
--rw-r--r--   0        0        0     7283 2024-02-20 11:05:46.343736 tolvera-0.1.0rc5/README.md
--rw-r--r--   0        0        0     1351 2024-02-24 13:28:03.992985 tolvera-0.1.0rc5/pyproject.toml
--rw-r--r--   0        0        0      239 2024-01-29 12:02:44.581497 tolvera-0.1.0rc5/src/tolvera/__init__.py
--rw-r--r--   0        0        0     1415 2023-12-21 14:09:56.095758 tolvera-0.1.0rc5/src/tolvera/__main__.py
--rw-r--r--   0        0        0     7427 2024-02-04 07:31:20.624889 tolvera-0.1.0rc5/src/tolvera/context.py
--rw-r--r--   0        0        0     6021 2024-01-31 15:04:30.100714 tolvera-0.1.0rc5/src/tolvera/cv.py
--rw-r--r--   0        0        0    34367 2024-02-21 17:12:04.366669 tolvera-0.1.0rc5/src/tolvera/iml.py
--rw-r--r--   0        0        0     9311 2024-01-29 14:38:36.090975 tolvera-0.1.0rc5/src/tolvera/mp.py
--rw-r--r--   0        0        0    17634 2023-12-21 18:27:34.390753 tolvera-0.1.0rc5/src/tolvera/npndarray_dict.py
--rw-r--r--   0        0        0      109 2023-12-14 12:21:58.843464 tolvera-0.1.0rc5/src/tolvera/osc/__init__.py
--rw-r--r--   0        0        0    16592 2023-12-14 12:47:13.058565 tolvera-0.1.0rc5/src/tolvera/osc/maxmsp.py
--rw-r--r--   0        0        0     2172 2023-12-14 12:47:18.249669 tolvera-0.1.0rc5/src/tolvera/osc/osc.py
--rw-r--r--   0        0        0    18113 2024-02-22 10:32:21.735357 tolvera-0.1.0rc5/src/tolvera/osc/oscmap.py
--rw-r--r--   0        0        0    21320 2024-02-22 10:43:23.946423 tolvera-0.1.0rc5/src/tolvera/osc/pd.py
--rw-r--r--   0        0        0     8050 2024-01-27 21:40:29.377144 tolvera-0.1.0rc5/src/tolvera/osc/update.py
--rw-r--r--   0        0        0    16314 2024-01-31 15:05:03.399943 tolvera-0.1.0rc5/src/tolvera/particles.py
--rw-r--r--   0        0        0     8746 2023-12-21 14:09:56.095961 tolvera-0.1.0rc5/src/tolvera/patches.py
--rw-r--r--   0        0        0    20406 2024-01-31 15:08:25.335482 tolvera-0.1.0rc5/src/tolvera/pixels.py
--rw-r--r--   0        0        0    11293 2023-12-21 18:24:43.829290 tolvera-0.1.0rc5/src/tolvera/sketchbook.py
--rw-r--r--   0        0        0     1603 2024-01-30 20:44:49.707521 tolvera-0.1.0rc5/src/tolvera/species.py
--rw-r--r--   0        0        0    15351 2024-01-28 19:20:04.820030 tolvera-0.1.0rc5/src/tolvera/state.py
--rw-r--r--   0        0        0     2753 2023-12-22 00:55:57.401473 tolvera-0.1.0rc5/src/tolvera/taichi_.py
--rw-r--r--   0        0        0     7019 2024-01-29 12:15:55.136773 tolvera-0.1.0rc5/src/tolvera/tolvera_.py
--rw-r--r--   0        0        0    13382 2024-02-23 19:07:07.895869 tolvera-0.1.0rc5/src/tolvera/utils.py
--rw-r--r--   0        0        0     1351 2024-01-17 17:49:01.254572 tolvera-0.1.0rc5/src/tolvera/vera/__init__.py
--rw-r--r--   0        0        0     1410 2024-01-28 15:19:14.309793 tolvera-0.1.0rc5/src/tolvera/vera/attractors.py
--rw-r--r--   0        0        0     5123 2024-02-20 18:01:18.205322 tolvera-0.1.0rc5/src/tolvera/vera/flock.py
--rw-r--r--   0        0        0     8236 2024-01-29 14:18:58.869204 tolvera-0.1.0rc5/src/tolvera/vera/forces.py
--rw-r--r--   0        0        0     2558 2024-01-18 21:45:30.996549 tolvera-0.1.0rc5/src/tolvera/vera/nca.py
--rw-r--r--   0        0        0     2445 2024-01-23 08:44:55.671162 tolvera-0.1.0rc5/src/tolvera/vera/particle_life.py
--rw-r--r--   0        0        0     4139 2023-12-14 11:51:35.601296 tolvera-0.1.0rc5/src/tolvera/vera/reaction_diffusion.py
--rw-r--r--   0        0        0     8254 2024-01-31 15:06:17.521952 tolvera-0.1.0rc5/src/tolvera/vera/slime.py
--rw-r--r--   0        0        0     5944 2024-01-18 19:24:08.637792 tolvera-0.1.0rc5/src/tolvera/vera/swarmalators.py
--rw-r--r--   0        0        0     8393 1970-01-01 00:00:00.000000 tolvera-0.1.0rc5/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-11-23 15:54:16.427339 tolvera-0.1.0rc6/LICENSE
+-rw-r--r--   0        0        0     7283 2024-03-12 14:02:15.429456 tolvera-0.1.0rc6/README.md
+-rw-r--r--   0        0        0     1356 2024-04-24 07:10:42.289125 tolvera-0.1.0rc6/pyproject.toml
+-rw-r--r--   0        0        0      257 2024-04-05 15:10:24.578539 tolvera-0.1.0rc6/src/tolvera/__init__.py
+-rw-r--r--   0        0        0     1415 2024-03-12 14:02:15.430630 tolvera-0.1.0rc6/src/tolvera/__main__.py
+-rw-r--r--   0        0        0     7859 2024-04-06 16:34:13.230063 tolvera-0.1.0rc6/src/tolvera/context.py
+-rw-r--r--   0        0        0     5841 2024-03-12 14:02:15.431092 tolvera-0.1.0rc6/src/tolvera/cv.py
+-rw-r--r--   0        0        0    34367 2024-03-12 14:02:15.431395 tolvera-0.1.0rc6/src/tolvera/iml.py
+-rw-r--r--   0        0        0      111 2024-03-16 12:45:28.778553 tolvera-0.1.0rc6/src/tolvera/mp/__init__.py
+-rw-r--r--   0        0        0     3543 2024-03-16 14:14:12.562796 tolvera-0.1.0rc6/src/tolvera/mp/face.py
+-rw-r--r--   0        0        0     6515 2024-03-16 15:10:11.518026 tolvera-0.1.0rc6/src/tolvera/mp/face_mesh.py
+-rw-r--r--   0        0        0    35788 2024-03-16 14:19:01.531491 tolvera-0.1.0rc6/src/tolvera/mp/face_mesh_connections.py
+-rw-r--r--   0        0        0     9488 2024-03-16 14:03:33.168705 tolvera-0.1.0rc6/src/tolvera/mp/hands.py
+-rw-r--r--   0        0        0     5051 2024-03-16 12:44:02.945408 tolvera-0.1.0rc6/src/tolvera/mp/pose.py
+-rw-r--r--   0        0        0    17634 2024-03-12 14:02:15.432183 tolvera-0.1.0rc6/src/tolvera/npndarray_dict.py
+-rw-r--r--   0        0        0      109 2024-03-12 14:02:15.432380 tolvera-0.1.0rc6/src/tolvera/osc/__init__.py
+-rw-r--r--   0        0        0    16592 2024-03-12 14:02:15.432591 tolvera-0.1.0rc6/src/tolvera/osc/maxmsp.py
+-rw-r--r--   0        0        0     2172 2024-03-12 14:02:15.432747 tolvera-0.1.0rc6/src/tolvera/osc/osc.py
+-rw-r--r--   0        0        0    18115 2024-03-12 14:02:15.432951 tolvera-0.1.0rc6/src/tolvera/osc/oscmap.py
+-rw-r--r--   0        0        0    21320 2024-03-12 14:02:15.433176 tolvera-0.1.0rc6/src/tolvera/osc/pd.py
+-rw-r--r--   0        0        0     8050 2024-03-12 14:02:15.433346 tolvera-0.1.0rc6/src/tolvera/osc/update.py
+-rw-r--r--   0        0        0    18350 2024-04-05 19:33:09.067969 tolvera-0.1.0rc6/src/tolvera/particles.py
+-rw-r--r--   0        0        0     8746 2024-03-12 14:02:15.433864 tolvera-0.1.0rc6/src/tolvera/patches.py
+-rw-r--r--   0        0        0    20397 2024-03-13 09:04:51.448910 tolvera-0.1.0rc6/src/tolvera/pixels.py
+-rw-r--r--   0        0        0     8299 2024-04-14 18:45:30.236884 tolvera-0.1.0rc6/src/tolvera/sf/__init__.py
+-rw-r--r--   0        0        0    11293 2024-03-12 14:02:15.434348 tolvera-0.1.0rc6/src/tolvera/sketchbook.py
+-rw-r--r--   0        0        0     1603 2024-03-12 14:02:15.434519 tolvera-0.1.0rc6/src/tolvera/species.py
+-rw-r--r--   0        0        0    15351 2024-03-12 14:02:15.434756 tolvera-0.1.0rc6/src/tolvera/state.py
+-rw-r--r--   0        0        0     2753 2024-03-12 14:02:15.434914 tolvera-0.1.0rc6/src/tolvera/taichi_.py
+-rw-r--r--   0        0        0     7364 2024-03-16 14:25:42.689663 tolvera-0.1.0rc6/src/tolvera/tolvera_.py
+-rw-r--r--   0        0        0    13382 2024-03-12 14:02:15.435388 tolvera-0.1.0rc6/src/tolvera/utils.py
+-rw-r--r--   0        0        0     1641 2024-04-06 20:24:19.369051 tolvera-0.1.0rc6/src/tolvera/vera/__init__.py
+-rw-r--r--   0        0        0     1410 2024-01-28 15:19:14.309793 tolvera-0.1.0rc6/src/tolvera/vera/attractors.py
+-rw-r--r--   0        0        0     1250 2024-04-06 17:13:45.518822 tolvera-0.1.0rc6/src/tolvera/vera/diffline.py
+-rw-r--r--   0        0        0     5117 2024-04-05 19:16:35.354112 tolvera-0.1.0rc6/src/tolvera/vera/flock.py
+-rw-r--r--   0        0        0     6658 2024-03-20 11:17:12.058891 tolvera-0.1.0rc6/src/tolvera/vera/flock2.py
+-rw-r--r--   0        0        0     4933 2024-03-19 11:20:46.646127 tolvera-0.1.0rc6/src/tolvera/vera/flock_shiffman.py
+-rw-r--r--   0        0        0     9569 2024-04-06 20:21:36.901912 tolvera-0.1.0rc6/src/tolvera/vera/forces.py
+-rw-r--r--   0        0        0     1436 2024-04-06 19:11:18.568109 tolvera-0.1.0rc6/src/tolvera/vera/geom.py
+-rw-r--r--   0        0        0     2558 2024-01-18 21:45:30.996549 tolvera-0.1.0rc6/src/tolvera/vera/nca.py
+-rw-r--r--   0        0        0     2618 2024-04-05 18:26:46.699886 tolvera-0.1.0rc6/src/tolvera/vera/particle_life.py
+-rw-r--r--   0        0        0     4145 2024-04-10 08:39:25.013654 tolvera-0.1.0rc6/src/tolvera/vera/reaction_diffusion.py
+-rw-r--r--   0        0        0     8254 2024-03-12 14:02:15.437046 tolvera-0.1.0rc6/src/tolvera/vera/slime.py
+-rw-r--r--   0        0        0     5944 2024-03-12 14:02:15.437195 tolvera-0.1.0rc6/src/tolvera/vera/swarmalators.py
+-rw-r--r--   0        0        0     2761 2024-03-21 11:59:27.308477 tolvera-0.1.0rc6/src/tolvera/vera/viscek.py
+-rw-r--r--   0        0        0     8398 1970-01-01 00:00:00.000000 tolvera-0.1.0rc6/PKG-INFO
```

### Comparing `tolvera-0.1.0rc5/LICENSE` & `tolvera-0.1.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc5/README.md` & `tolvera-0.1.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc5/pyproject.toml` & `tolvera-0.1.0rc6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "tolvera"
 packages = [{ include = "tolvera", from = "src"}]
-version = "0.1.0-rc5"
+version = "0.1.0-rc6"
 description = "Tölvera is a library for exploring music interaction with artificial life and self-organising systems."
 authors = ["Jack Armitage <jack.armitage@me.com>"]
 readme = "README.md"
 license = "AGPL-3.0"
 repository = "https://github.com/Intelligent-Instruments-Lab/tolvera"
 documentation = "https://intelligent-instruments-lab.github.io/tolvera/"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
-taichi = "^1.6.0"
+taichi = "^1.7.0"
 jsons = "^1.6.3"
 opencv-python = "^4.8.1.78"
-torch = "^2.1.1"
 iipyper = "^0.1.0b1"
 anguilla-iml = "^0.1.0b4"
 sardine = "^0.0.0b3"
 mediapipe = "^0.10.9"
+signalflow = "^0.4.8"
 
 [tool.poetry.group.dev.dependencies]
 mkdocs = "^1.5.3"
 mkdocs-video = "^1.5.0"
 mkdocstrings = {extras = ["python"], version = "^0.23.0"}
 mkdocs-gen-files = "^0.5.0"
 mkdocs-include-markdown-plugin = "^6.0.4"
```

### Comparing `tolvera-0.1.0rc5/src/tolvera/__main__.py` & `tolvera-0.1.0rc6/src/tolvera/__main__.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc5/src/tolvera/context.py` & `tolvera-0.1.0rc6/src/tolvera/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 from sys import exit
 
 from iipyper.state import _lock
 
 from .taichi_ import Taichi
 from .cv import CV
-from .mp import MPHands
+from .mp import *
 from .iml import IMLDict
 from .osc.osc import OSC
 from .patches import *
 from .pixels import *
 from .utils import *
 from .state import StateDict
 
@@ -97,32 +97,42 @@
             iml (bool): Enable IML. Default: False.
             cv (bool): Enable CV. Default: False.
             see also kwargs for Taichi, OSC, IMLDict, and CV.
         """
         self.name = "Tölvera Context"
         self.name_clean = clean_name(self.name)
         print(f"[{self.name}] Initializing context...")
-        self.i = 0
         self.x = kwargs.get("x", 1920)
         self.y = kwargs.get("y", 1080)
         self.ti = Taichi(self, **kwargs)
+        self.i = ti.field(ti.i32, ())
         self.show = self.ti.show
         self.canvas = Pixels(self, **kwargs)
         self.s = StateDict(self)
         self.osc = kwargs.get("osc", False)
         self.iml = kwargs.get("iml", False)
         self.cv = kwargs.get("cv", False)
         self.hands = kwargs.get("hands", False)
+        self.pose = kwargs.get("pose", False)
+        self.face = kwargs.get("face", False)
+        self.face_mesh = kwargs.get("face_mesh", False)
         if self.osc:
             self.osc = OSC(self, **kwargs)
         if self.iml:
             self.iml = IMLDict(self)
         if self.cv:
             self.cv = CV(self, **kwargs)
-            self.hands = MPHands(self, **kwargs)
+            if self.hands:
+                self.hands = MPHands(self, **kwargs)
+            if self.pose:
+                self.pose = MPPose(self, **kwargs)
+            if self.face:
+                self.face = MPFace(self, **kwargs)
+            if self.face_mesh:
+                self.face_mesh = MPFaceMesh(self, **kwargs)
         self._cleanup_fns = []
         self.tolveras = {}
         print(f"[{self.name}] Context initialisation complete.")
 
     def run(self, f=None, **kwargs):
         """
         Run Tölvera with given render function and keyword arguments.
@@ -135,25 +145,28 @@
         """
         if f is not None:
             print(f"[{self.name}] Running with render function {f.__name__}...")
         else:
             print(f"[{self.name}] Running with no render function...")
         while self.ti.window.running:
             with _lock:
-                [t.p() for t in self.tolveras.values()]
-                if f is not None:
-                    self.canvas = f(**kwargs)
-                if self.osc is not False:
-                    self.osc.map()
-                if self.iml is not False:
-                    self.iml()
-                if self.cv is not False:
-                    self.cv()
-                self.ti.show(self.canvas)
-                self.i += 1
+                self.step(f, **kwargs)
+    
+    def step(self, f, **kwargs):
+        [t.p() for t in self.tolveras.values()]
+        if f is not None:
+            self.canvas = f(**kwargs)
+        if self.osc is not False:
+            self.osc.map()
+        if self.iml is not False:
+            self.iml()
+        if self.cv is not False:
+            self.cv()
+        self.ti.show(self.canvas)
+        self.i[None] += 1
 
     def stop(self):
         """
         Run cleanup functions and exit.
         """
         print(f"\n[{self.name}] Stopping {self.name}...")
         for f in self._cleanup_fns:
```

### Comparing `tolvera-0.1.0rc5/src/tolvera/cv.py` & `tolvera-0.1.0rc6/src/tolvera/cv.py`

 * *Files 5% similar despite different names*

```diff
@@ -144,27 +144,23 @@
             _i, _j = self.y - j, self.x - i
             p = img[_i, _j] / 255
             self.px.px.rgba[i, j] = [p, p, p, 1]
 
     def process(self):
         self.i += 1
         if self.i % self.camera_substeps == 0:
-            # prev = self.cc_frame
             frame = self.camera_read()
-            # self.cv_to_px(self.diff.astype(np.float32))
             # thresh = self.threshold(frame)
             # contours = self.find_contours(thresh)
             # polygons = self.approx_poly_dp(contours)
             # img      = self.draw_contours(contours)
             # img      = self.gaussian_blur(img)
             # img      = self.resize(img, dsize=(int(1920/4), int(1080/4)))
             # self.cv_to_px(self.camera_frame)
-            # diff = self.abs_diff(self.cc_frame, prev)
             self.cv_to_px(frame)
-            # self.px.invert()
 
     def cleanup(self):
         self.camera_capture.release()
 
     def __call__(self, *args, **kwargs):
         self.process()
         return self.px
```

### Comparing `tolvera-0.1.0rc5/src/tolvera/iml.py` & `tolvera-0.1.0rc6/src/tolvera/iml.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc5/src/tolvera/mp.py` & `tolvera-0.1.0rc6/src/tolvera/mp/hands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import mediapipe as mp
 import taichi as ti
 import numpy as np
 import enum
 
-from .osc.update import Updater
+from ..osc.update import Updater
 
 class HandLandmark(enum.IntEnum):
   """The 21 hand landmarks."""
   WRIST = 0
   THUMB_CMC = 1
   THUMB_MCP = 2
   THUMB_IP = 3
@@ -47,45 +47,46 @@
     b: ti.i32
 
 @ti.data_oriented
 class MPHands:
     def __init__(self, context, **kwargs) -> None:
         self.ctx = context
         self.kwargs = kwargs
+        self.n_conns = len(HAND_CONNECTIONS)
 
         self.config = {
             'static_image_mode': kwargs.get('static_mode', False),
             'max_num_hands': kwargs.get('max_hands', 2),
             'model_complexity': kwargs.get('model_complexity', 1),
             'min_detection_confidence': kwargs.get('detection_con', .5),
             'min_tracking_confidence': kwargs.get('min_track_con', .5),
         }
         self.mpHands = mp.solutions.hands
         self.hands = self.mpHands.Hands(**self.config)
         self.setup_connections()
         
         self.hands_np = {
-            'pxnorm':np.zeros((self.config['max_num_hands'], 21, 3), np.float32),
-            'px':np.zeros((self.config['max_num_hands'], 21, 2), np.float32),
+            'pxnorm':np.zeros((self.config['max_num_hands'], self.n_conns, 3), np.float32),
+            'px':np.zeros((self.config['max_num_hands'], self.n_conns, 2), np.float32),
         }
         self.ctx.s.hands = {
             'state': {
                 'pxnorm': (ti.math.vec3, 0.0, 1.0),
                 'px': (ti.math.vec2, 0.0, 1.0),
                 # 'metres': (ti.math.vec3, 0.0, 1.0), # multi_hand_world_landmarks
             },
-            'shape': (self.config['max_num_hands'], 21)
+            'shape': (self.config['max_num_hands'], self.n_conns)
         }
         self.handed = ti.field(ti.i32, shape=(self.config['max_num_hands'])) # 0=l, 1=r
         self.handed.fill(-1)
 
         if self.ctx.iml:
             self.ctx.iml.hands = {
                 'type': 'vec2vec',
-                'size': ((21,2), 1),
+                'size': ((self.n_conns,2), 1),
             }
 
         self.updater = Updater(self.detect, kwargs.get('hands_detect_rate', 10))
     
     def setup_connections(self):
         self.palm_conns = HandConnection.field(shape=(len(HAND_PALM_CONNECTIONS)))
         self.thumb_conns = HandConnection.field(shape=(len(HAND_THUMB_CONNECTIONS)))
@@ -245,14 +246,17 @@
     def recognize(self, id):
         # get all pairs that match id
         # iml.index.metric(iml.embed_input([input]), iml.embed_input(pairs))
         pass
 
     def landmark_name_from_index(self, index):
         return HandLandmark(index).name
+    
+    def landmark_index_from_name(self, name):
+        return HandLandmark[name].value
 
     @ti.kernel
     def get_landmark(self, hand: ti.i32, landmark: ti.i32) -> ti.math.vec2:
         return self.ctx.s.hands[hand, landmark].px
 
     def __call__(self, frame):
         self.updater(frame)
```

### Comparing `tolvera-0.1.0rc5/src/tolvera/npndarray_dict.py` & `tolvera-0.1.0rc6/src/tolvera/npndarray_dict.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc5/src/tolvera/osc/maxmsp.py` & `tolvera-0.1.0rc6/src/tolvera/osc/maxmsp.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc5/src/tolvera/osc/osc.py` & `tolvera-0.1.0rc6/src/tolvera/osc/osc.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc5/src/tolvera/osc/oscmap.py` & `tolvera-0.1.0rc6/src/tolvera/osc/oscmap.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
                 client=self.client_name,
             )
         else:
             f["sender"] = OSCSend(
                 self.osc,
                 f["address"],
                 f=func,
-                count=kwargs["count"],
+                # count=kwargs["count"],
                 client=self.client_name,
             )
         f["type"] = "args"
         self.dict["send"][f["name"]] = f
         if self.export is not None:
             self.export_dict()
```

### Comparing `tolvera-0.1.0rc5/src/tolvera/osc/pd.py` & `tolvera-0.1.0rc6/src/tolvera/osc/pd.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc5/src/tolvera/osc/update.py` & `tolvera-0.1.0rc6/src/tolvera/osc/update.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc5/src/tolvera/particles.py` & `tolvera-0.1.0rc6/src/tolvera/particles.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 such as updating the particles, and getting and setting particle properties.
 """
 
 import taichi as ti
 
 from .species import Species
 from .state import State
-
+from .utils import CONSTS
 
 @ti.dataclass
 class Particle:
     """Particle data structure and methods."""
     species: ti.i32
     active: ti.f32
     pos: ti.math.vec2
     vel: ti.math.vec2
+    ppos: ti.math.vec2
+    pvel: ti.math.vec2
     mass: ti.f32
     size: ti.f32
     speed: ti.f32
 
     @ti.func
     def dist(self, other):
         """Distance between two particles.
@@ -163,14 +165,23 @@
         self.substep = self.tv.substep
         self.field = Particle.field(shape=(self.n))
         # TODO: These should be possible with State
         # self.pos = State(self.tv, {
         #     'x': (0., self.tv.x),
         #     'y': (0., self.tv.y),
         # }, shape=(self.n,), osc=('get'), name='particles_pos')
+        self.C = CONSTS({"COLL_RAD": (ti.f32, 10.0)})
+        self.tv.s.collisions_p = {
+            'state': {
+                'collision': (ti.i32, 0, 1),
+                'dpos': (ti.math.vec2, 0., 1.),
+                'dvel': (ti.math.vec2, 0., 1.),
+            },
+            'shape': self.n,
+        }
         self.tmp_pos = ti.Vector.field(2, ti.f32, shape=(self.n))
         self.tmp_vel = ti.Vector.field(2, ti.f32, shape=(self.n))
         self.tmp_pos_species = ti.Vector.field(2, ti.f32, shape=(self.p_per_s))
         self.tmp_vel_species = ti.Vector.field(2, ti.f32, shape=(self.p_per_s))
         self.tmp_vel_stats = ti.Vector.field(1, ti.f32, shape=(7))
         self.active_indexes = ti.field(ti.i32, shape=(self.n))
         self.active_count = ti.field(ti.i32, shape=())
@@ -221,30 +232,23 @@
                 size=size,
                 speed=speed,
             )
 
     @ti.kernel
     def update(self):
         """Update the particle system."""
-        # TODO: collisions
+        j = 0
         for i in range(self.n):
-            if self.field[i] == 0.0:
-                continue
+            if self.field[i] == 0.0: continue
             self.toroidal_wrap(i)
             self.limit_speed(i)
-
-    @ti.kernel
-    def update_active(self):
-        """Update the active particles."""
-        j = 0
-        for i in range(self.n):
-            p = self.field[i]
-            if p.active > 0.0:
-                self.active_indexes[j] = i
-                j += 1
+            self.detect_collisions(i, self.C.COLL_RAD)
+            self.update_prev(i)
+            self.active_indexes[j] = i
+            j += 1
         self.active_count[None] = j
 
     @ti.func
     def toroidal_wrap(self, i: ti.i32):
         """Toroidal wrap a particle.
 
         Args:
@@ -273,76 +277,120 @@
         sp = (
             s.speed * self.tv.species_consts.MAX_SPEED
             + self.tv.species_consts.MIN_SPEED
         )
         if p.vel.norm() > s.speed:
             self.field[i].vel = p.vel.normalized() * sp * self._speed[None]
 
+    @ti.func
+    def detect_collisions(self, i: ti.i32, radius: ti.f32):
+        """Detect collisions between particles.
+
+        TODO: Merge deltas into @ti.dataclass, or reimplement Particle.field as tv.s?
+        TODO: Multiple collision states? Collided, Colliding, etc.
+        TODO: Detect collisions between external objects.
+
+        Args:
+            i (ti.i32): Particle index.
+            radius (ti.f32): Collision radius.
+        """
+        for j in range(self.n):
+            p1, p2 = self.tv.p.field[i], self.tv.p.field[j]
+            if p2.active == 0: continue
+            dist = p1.pos - p2.pos
+            if dist.norm() < radius:
+                pdist = p1.ppos - p2.ppos
+                dpos = ti.abs(pdist - dist)
+                dvel = ti.abs((p1.pvel - p2.pvel) - (p1.vel - p2.vel))
+                self.tv.s.collisions_p[i].dpos = dpos
+                self.tv.s.collisions_p[i].dvel = dvel
+                if pdist.norm() > radius:
+                    self.tv.s.collisions_p[i].collision = 1
+                else:
+                    self.tv.s.collisions_p[i].collision = 0
+
+    @ti.func
+    def update_prev(self, i: ti.i32):
+        """Update the previous position and velocity of a particle.
+
+        Args:
+            i (ti.i32): Particle index.
+        """
+        self.field[i].ppos = self.field[i].pos
+        self.field[i].pvel = self.field[i].vel
+
     @ti.kernel
     def activity_decay(self):
         """Decay the activity of the particles."""
         for i in range(self.active_count[None]):
             idx = self.active_indexes[i]
             self.field[idx].active *= self.field[i].decay
 
     def process(self):
         """Process the particle system."""
         for i in range(self.substep):
-            self.update_active()
             self.update()
 
     @ti.kernel
-    def set_active(self, a: ti.i32):
-        """Set the active particles.
+    def set_total_active(self, total: ti.i32):
+        """Set the total number of active particles.
 
         Args:
-            a (ti.i32): Amount of active particles.
+            total (ti.i32): Total active particles.
         """
         for i in range(self.field.shape[0]):
-            if i > a:
+            if i >= total:
                 self.field[i].active = 0
             else:
                 self.field[i].active = 1
 
     @ti.kernel
-    def set_species_active(self, i: ti.i32, a: ti.i32):
-        """Set the active particles of a species.
+    def set_total_active_amount(self, total: ti.i32, amount: ti.f32):
+        """Set the total number of active particles.
+
+        Args:
+            total (ti.i32): Total active particles.
+            amount (ti.f32): Amount of activity.
+        """
+        for i in range(self.field.shape[0]):
+            if i >= total:
+                self.field[i].active = 0
+            else:
+                self.field[i].active = amount
+
+    @ti.kernel
+    def set_species_total_active(self, i: ti.i32, total: ti.i32):
+        """Set the total number of active particles for a species.
 
         Args:
             i (ti.i32): Species index.
-            a (ti.i32): Amount of active particles.
+            total (ti.i32): Total active particles.
         """
         for j in range(self.field.shape[0]):
             if self.field[j].species == i:
-                if j > a:
+                if j >= total:
                     self.field[j].active = 0
                 else:
                     self.field[j].active = 1
-
-    @ti.kernel
-    def set_active_amount(self, a: ti.f32):
-        """Set particle activity amount.
-
-        Args:
-            a (ti.i32): Amount of activity.
-        """
-        for i in range(self.field.shape[0]):
-            self.field[i].active = a
     
     @ti.kernel
-    def set_species_active_amount(self, i: ti.i32, a: ti.f32):
+    def set_species_total_active_amount(self, i: ti.i32, total: ti.i32, amount: ti.f32):
         """Set particle activity amount of a species.
 
         Args:
             i (ti.i32): Species index.
-            a (ti.i32): Amount of activity.
+            total: (ti.i32): Total number of active particles.
+            amount (ti.i32): Amount of activity.
         """
         for j in range(self.field.shape[0]):
             if self.field[j].species == i:
-                self.field[j].active = a
+                if j >= total:
+                    self.field[j].active = 0
+                else:
+                    self.field[j].active = amount
 
     def set_pos(self, i, x, y):
         self.field[i].pos = [x, y]
 
     def set_vel(self, i, x, y):
         self.field[i].vel = [x, y]
```

### Comparing `tolvera-0.1.0rc5/src/tolvera/patches.py` & `tolvera-0.1.0rc6/src/tolvera/patches.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc5/src/tolvera/pixels.py` & `tolvera-0.1.0rc6/src/tolvera/pixels.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     def diffuse(self, evaporate: ti.f32):
         """Diffuse pixels.
         
         Args:
             evaporate (float): Evaporation rate.
         """
         for i, j in ti.ndrange(self.x, self.y):
-            d = ti.Vector([0.0, 0.0, 0.0, 0.0]) 
+            d = ti.Vector([0.0, 0.0, 0.0, 0.0])
             for di in ti.static(range(-1, 2)):
                 for dj in ti.static(range(-1, 2)):
                     dx = (i + di) % self.x
                     dy = (j + dj) % self.y
                     d += self.px.rgba[dx, dy]
             d *= 0.99 / 9.0
             self.px.rgba[i, j] = d
@@ -380,21 +380,21 @@
                 n -= 1
         return n
 
     @ti.kernel
     def flip_x(self):
         """Flip image in x-axis."""
         for i, j in ti.ndrange(self.x, self.y):
-            self.px.rgba_inv[i, j] = self.px.rgba[self.x - 1 - i, j]
+            self.px.rgba[i, j] = self.px.rgba[self.x - 1 - i, j]
 
     @ti.kernel
     def flip_y(self):
         """Flip image in y-axis."""
         for i, j in ti.ndrange(self.x, self.y):
-            self.px.rgba_inv[i, j] = self.px.rgba[i, self.y - 1 - j]
+            self.px.rgba[i, j] = self.px.rgba[i, self.y - 1 - j]
 
     @ti.kernel
     def invert(self):
         """Invert image."""
         for i, j in ti.ndrange(self.x, self.y):
             self.px.rgba[i, j] = 1.0 - self.px.rgba[i, j]
```

### Comparing `tolvera-0.1.0rc5/src/tolvera/sketchbook.py` & `tolvera-0.1.0rc6/src/tolvera/sketchbook.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc5/src/tolvera/species.py` & `tolvera-0.1.0rc6/src/tolvera/species.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc5/src/tolvera/state.py` & `tolvera-0.1.0rc6/src/tolvera/state.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc5/src/tolvera/taichi_.py` & `tolvera-0.1.0rc6/src/tolvera/taichi_.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc5/src/tolvera/tolvera_.py` & `tolvera-0.1.0rc6/src/tolvera/tolvera_.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,17 @@
         self.osc = context.osc
         self.s = context.s
         self.iml = context.iml
         self.render = context.render
         self.cleanup = context.cleanup
         self.cv = context.cv
         self.hands = context.hands
+        self.pose = context.pose
+        self.face = context.face
+        self.face_mesh = context.face_mesh
 
     def setup(self, **kwargs):
         """
         Setup Tölvera with given keyword arguments.
         This can be called multiple throughout the lifetime of a Tölvera instance.
 
         Args:
@@ -154,15 +157,22 @@
         self._species = Species(self, **kwargs)
         self.p = Particles(self, **kwargs)
         self.speed(self._speed)
         self.v = Vera(self, **kwargs)
         if self.osc is not False:
             self.add_to_osc_map()
         if self.cv is not False:
-            self.hands.px = self.px
+            if self.hands:
+                self.hands.px = self.px
+            if self.pose:
+                self.pose.px = self.px
+            if self.face:
+                self.face.px = self.px
+            if self.face_mesh:
+                self.face_mesh.px = self.px
         self.ctx.add(self)
         print(f"[{self.name}] Setup complete.")
 
     def randomise(self):
         """
         Randomise particles, species, and Vera.
         """
```

### Comparing `tolvera-0.1.0rc5/src/tolvera/utils.py` & `tolvera-0.1.0rc6/src/tolvera/utils.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc5/src/tolvera/vera/__init__.py` & `tolvera-0.1.0rc6/src/tolvera/vera/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """The Vera module provides a wrapper for all available forces and behaviours."""
 
 from . import forces
+from . import geom
 from .flock import Flock
+from .flock2 import Flock2
 from .reaction_diffusion import ReactionDiffusion
 from .slime import Slime
 from .particle_life import ParticleLife
 from .swarmalators import Swarmalators
 
 class Vera:
     """The Vera class provides a wrapper for all available forces and behaviours,
@@ -15,23 +17,30 @@
         
         Args:
             tolvera (Tolvera): A Tolvera instance.
             **kwargs: Keyword arguments passed to the Vera.
         """
         self.tv = tolvera
         self.add_forces_to_self()
+        # self.add_geom_to_self()
         self.flock = Flock(tolvera, **kwargs)
+        self.flock2 = Flock2(tolvera, **kwargs)
         self.slime = Slime(tolvera, **kwargs)
         self.rd = ReactionDiffusion(tolvera, **kwargs)
         self.plife = ParticleLife(tolvera, **kwargs)
         self.swarm = Swarmalators(tolvera, **kwargs)
 
     def add_forces_to_self(self):
         """Add all forces to the Vera instance."""
-        for force in forces.__all__:
-            setattr(self, force, getattr(forces, force))
+        for f in forces.__all__:
+            setattr(self, f, getattr(forces, f))
+    
+    def add_geom_to_self(self):
+        """Add all geom functions to the Vera instance."""
+        for g in geom.__all__:
+            setattr(self, g, getattr(geom, g))
 
     def randomise(self):
         """Randomise all forces and behaviours."""
         self.flock.randomise()
         self.slime.randomise()
         self.rd.randomise()
```

### Comparing `tolvera-0.1.0rc5/src/tolvera/vera/attractors.py` & `tolvera-0.1.0rc6/src/tolvera/vera/attractors.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc5/src/tolvera/vera/flock.py` & `tolvera-0.1.0rc6/src/tolvera/vera/flock.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             "randomise": True,
         }
         self.tv.s.flock_p = {
             "state": {
                 "separate": (ti.math.vec2, 0.0, 1.0),
                 "align": (ti.math.vec2, 0.0, 1.0),
                 "cohere": (ti.math.vec2, 0.0, 1.0),
-                "nearby": (ti.i32, 0, self.tv.p.n - 1),
+                "nearby": (ti.i32, 0.0, self.tv.p.n - 1),
             },
             "shape": self.tv.pn,
             "osc": ("get"),
             "randomise": False,
         }
         self.tv.s.flock_dist = {
             "state": {
@@ -113,16 +113,16 @@
             if nearby > 0:
                 separate = (
                     separate / nearby * p1.active * ti.math.max(species.separate, 0.2)
                 )
                 align = align / nearby * p1.active * species.align
                 cohere = (cohere / nearby - p1.pos) * p1.active * species.cohere
                 vel = (separate + align + cohere).normalized()
-                particles[i].vel += vel * weight
-                particles[i].pos += particles[i].vel * p1.speed * p1.active * weight
+                particles[i].vel += vel * weight * p1.speed * p1.active 
+                particles[i].pos += particles[i].vel
             self.tv.s.flock_p[i] = self.tv.s.flock_p.struct(
                 separate, align, cohere, nearby
             )
 
     def __call__(self, particles, weight: ti.f32 = 1.0):
         """Call the Flock behaviour.
```

### Comparing `tolvera-0.1.0rc5/src/tolvera/vera/forces.py` & `tolvera-0.1.0rc6/src/tolvera/vera/forces.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     "_attract_species",
     "attract_particle",
     "repel",
     "repel_species",
     "gravitate",
     "gravitate_species",
     "noise",
+    "centripetal",
+    "centripetal_particle",
 ]
 
 
 @ti.kernel
 def move(particles: ti.template()):
     """Move the particles.
 
@@ -283,7 +285,46 @@
     """
     for i in range(particles.field.shape[0]):
         p = particles.field[i]
         if p.active == 0:
             continue
         particles.field[i].vel += (ti.Vector([ti.random() - 0.5, ti.random() - 0.5]) * weight)
         particles.field[i].pos += p.vel * p.speed * p.active
+
+@ti.kernel
+def centripetal(particles: ti.template(), centre: ti.math.vec2, direction: ti.i32, weight: ti.f32):
+    """Apply a centripetal force to the particles.
+
+    Args:
+        particles (ti.template): Particles.
+        centre (ti.math.vec2): Centripetal centre.
+        direction (ti.i32): Centripetal direction.
+        weight (ti.f32): Centripetal weight.
+    """
+    for i in range(particles.field.shape[0]):
+        p = particles.field[i]
+        if p.active == 0:
+            continue
+        particles.field[i].vel += centripetal_particle(p, centre, direction, weight)
+
+@ti.func
+def centripetal_particle(p: ti.template(), centre: ti.math.vec2, direction: ti.i32, weight: ti.f32) -> ti.math.vec2:
+    """Apply a centripetal force to a particle.
+
+    Args:
+        p (Particle): Individual particle.
+        centre (ti.math.vec2): Centripetal centre.
+        direction (ti.i32): Centripetal direction.
+        weight (ti.f32): Centripetal weight.
+
+    Returns:
+        ti.math.vec2: Centripetal velocity.
+    """
+    r = p.pos - centre
+    if direction == 0:
+        r = -r
+    v_perp = ti.Vector([-r[1], r[0]])
+    norm = v_perp.norm() + 1e-5
+    v_perp_normalized = v_perp / norm
+    speed = p.vel.norm()
+    new_vel = v_perp_normalized * speed * weight
+    return new_vel
```

### Comparing `tolvera-0.1.0rc5/src/tolvera/vera/nca.py` & `tolvera-0.1.0rc6/src/tolvera/vera/nca.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc5/src/tolvera/vera/particle_life.py` & `tolvera-0.1.0rc6/src/tolvera/vera/particle_life.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,16 +58,18 @@
                 dx = p1.pos[0] - p2.pos[0]
                 dy = p1.pos[1] - p2.pos[1]
                 d = ti.sqrt(dx*dx + dy*dy)
                 if 0. < d and d < s.radius:
                     F = s.attract/d
                     fx += F*dx
                     fy += F*dy
-            particles[i].vel = (particles[i].vel + ti.Vector([fx, fy])) * self.CONSTS.V * weight
-            particles[i].pos += (particles[i].vel * p1.speed * p1.active * weight)
+            # particles[i].vel = (particles[i].vel + ti.Vector([fx, fy])) * self.CONSTS.V * weight
+            # particles[i].pos += (particles[i].vel * p1.speed * p1.active * weight)
+            particles[i].vel = (particles[i].vel + ti.Vector([fx, fy])) * self.CONSTS.V * weight * p1.speed * p1.active
+            particles[i].pos += particles[i].vel
     def __call__(self, particles, weight: ti.f32 = 1.0):
         """Call the Particle Life model.
 
         Args:
             particles (Particles): The particles to step.
         """
         self.step(particles.field, weight)
```

### Comparing `tolvera-0.1.0rc5/src/tolvera/vera/reaction_diffusion.py` & `tolvera-0.1.0rc6/src/tolvera/vera/reaction_diffusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,13 +110,13 @@
                     a = (value - c0.w) / (c1.w - c0.w)
                     color = ti.math.mix(c0.xyz, c1.xyz, a)
             self.field.px.rgba[i, j] = [color.x, color.y, color.z, 1.0]
 
     def process(self):
         # for _ in range(self.substep[None]):
         for _ in range(self.tv.s.rd.field[0].substep):
-            self.compute(self.tv.ctx.i % 2)
+            self.compute(self.tv.ctx.i[None] % 2)
 
     def __call__(self):
         self.process()
         self.render()
         return self.field.px
```

### Comparing `tolvera-0.1.0rc5/src/tolvera/vera/slime.py` & `tolvera-0.1.0rc6/src/tolvera/vera/slime.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc5/src/tolvera/vera/swarmalators.py` & `tolvera-0.1.0rc6/src/tolvera/vera/swarmalators.py`

 * *Files identical despite different names*

### Comparing `tolvera-0.1.0rc5/PKG-INFO` & `tolvera-0.1.0rc6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tolvera
-Version: 0.1.0rc5
+Version: 0.1.0rc6
 Summary: Tölvera is a library for exploring music interaction with artificial life and self-organising systems.
 Home-page: https://github.com/Intelligent-Instruments-Lab/tolvera
 License: AGPL-3.0
 Author: Jack Armitage
 Author-email: jack.armitage@me.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -13,16 +13,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anguilla-iml (>=0.1.0b4,<0.2.0)
 Requires-Dist: iipyper (>=0.1.0b1,<0.2.0)
 Requires-Dist: jsons (>=1.6.3,<2.0.0)
 Requires-Dist: mediapipe (>=0.10.9,<0.11.0)
 Requires-Dist: opencv-python (>=4.8.1.78,<5.0.0.0)
 Requires-Dist: sardine (>=0.0.0b3,<0.0.1)
-Requires-Dist: taichi (>=1.6.0,<2.0.0)
-Requires-Dist: torch (>=2.1.1,<3.0.0)
+Requires-Dist: signalflow (>=0.4.8,<0.5.0)
+Requires-Dist: taichi (>=1.7.0,<2.0.0)
 Project-URL: Documentation, https://intelligent-instruments-lab.github.io/tolvera/
 Project-URL: Repository, https://github.com/Intelligent-Instruments-Lab/tolvera
 Description-Content-Type: text/markdown
 
 # Tölvera
 
 [Tölvera](https://tolvera.is) is a library for exploring musical performance with artificial life (ALife) and self-organising systems. The word is an Icelandic [kenning](https://en.wikipedia.org/wiki/Kenning):
```

