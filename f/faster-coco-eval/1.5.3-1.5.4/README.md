# Comparing `tmp/faster_coco_eval-1.5.3.tar.gz` & `tmp/faster_coco_eval-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faster_coco_eval-1.5.3.tar", last modified: Mon Apr 22 12:28:45 2024, max compression
+gzip compressed data, was "faster_coco_eval-1.5.4.tar", last modified: Wed Apr 24 11:14:24 2024, max compression
```

## Comparing `faster_coco_eval-1.5.3.tar` & `faster_coco_eval-1.5.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:28:45.062947 faster_coco_eval-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-22 12:28:45.062947 faster_coco_eval-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:28:45.054947 faster_coco_eval-1.5.3/csrc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:28:45.058947 faster_coco_eval-1.5.3/csrc/faster_eval_api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:28:45.058947 faster_coco_eval-1.5.3/csrc/faster_eval_api/coco_eval/
--rw-r--r--   0 runner    (1001) docker     (127)    25273 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/csrc/faster_eval_api/coco_eval/cocoeval.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/csrc/faster_eval_api/coco_eval/cocoeval.h
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/csrc/faster_eval_api/faster_eval_api.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:28:45.054947 faster_coco_eval-1.5.3/csrc/mask/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:28:45.058947 faster_coco_eval-1.5.3/csrc/mask/common/
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/csrc/mask/common/maskApi.c
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/csrc/mask/common/maskApi.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:28:45.058947 faster_coco_eval-1.5.3/csrc/mask/pycocotools/
--rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/csrc/mask/pycocotools/_mask.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:28:45.058947 faster_coco_eval-1.5.3/faster_coco_eval/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/faster_coco_eval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:28:45.058947 faster_coco_eval-1.5.3/faster_coco_eval/core/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/faster_coco_eval/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17218 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/faster_coco_eval/core/coco.py
--rw-r--r--   0 runner    (1001) docker     (127)    22816 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/faster_coco_eval/core/cocoeval.py
--rw-r--r--   0 runner    (1001) docker     (127)    13521 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/faster_coco_eval/core/faster_eval_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/faster_coco_eval/core/mask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:28:45.062947 faster_coco_eval-1.5.3/faster_coco_eval/extra/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/faster_coco_eval/extra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/faster_coco_eval/extra/curves.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/faster_coco_eval/extra/display.py
--rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/faster_coco_eval/extra/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/faster_coco_eval/extra/extra.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/faster_coco_eval/extra/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/faster_coco_eval/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:28:45.062947 faster_coco_eval-1.5.3/faster_coco_eval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-22 12:28:45.000000 faster_coco_eval-1.5.3/faster_coco_eval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-22 12:28:45.000000 faster_coco_eval-1.5.3/faster_coco_eval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 12:28:45.000000 faster_coco_eval-1.5.3/faster_coco_eval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-22 12:28:45.000000 faster_coco_eval-1.5.3/faster_coco_eval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 12:28:45.000000 faster_coco_eval-1.5.3/faster_coco_eval.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:28:45.062947 faster_coco_eval-1.5.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/requirements/extra.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 12:28:45.062947 faster_coco_eval-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-22 12:28:38.000000 faster_coco_eval-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:14:24.749281 faster_coco_eval-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-24 11:14:24.749281 faster_coco_eval-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:14:24.745281 faster_coco_eval-1.5.4/csrc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:14:24.745281 faster_coco_eval-1.5.4/csrc/faster_eval_api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:14:24.745281 faster_coco_eval-1.5.4/csrc/faster_eval_api/coco_eval/
+-rw-r--r--   0 runner    (1001) docker     (127)    25273 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/csrc/faster_eval_api/coco_eval/cocoeval.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/csrc/faster_eval_api/coco_eval/cocoeval.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/csrc/faster_eval_api/faster_eval_api.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:14:24.745281 faster_coco_eval-1.5.4/csrc/mask/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:14:24.745281 faster_coco_eval-1.5.4/csrc/mask/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/csrc/mask/common/maskApi.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/csrc/mask/common/maskApi.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:14:24.745281 faster_coco_eval-1.5.4/csrc/mask/pycocotools/
+-rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/csrc/mask/pycocotools/_mask.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:14:24.749281 faster_coco_eval-1.5.4/faster_coco_eval/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/faster_coco_eval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:14:24.749281 faster_coco_eval-1.5.4/faster_coco_eval/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/faster_coco_eval/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17218 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/faster_coco_eval/core/coco.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22816 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/faster_coco_eval/core/cocoeval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13497 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/faster_coco_eval/core/faster_eval_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/faster_coco_eval/core/mask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:14:24.749281 faster_coco_eval-1.5.4/faster_coco_eval/extra/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/faster_coco_eval/extra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/faster_coco_eval/extra/curves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/faster_coco_eval/extra/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12285 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/faster_coco_eval/extra/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/faster_coco_eval/extra/extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/faster_coco_eval/extra/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/faster_coco_eval/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:14:24.749281 faster_coco_eval-1.5.4/faster_coco_eval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-24 11:14:24.000000 faster_coco_eval-1.5.4/faster_coco_eval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-24 11:14:24.000000 faster_coco_eval-1.5.4/faster_coco_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:14:24.000000 faster_coco_eval-1.5.4/faster_coco_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 11:14:24.000000 faster_coco_eval-1.5.4/faster_coco_eval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 11:14:24.000000 faster_coco_eval-1.5.4/faster_coco_eval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:14:24.749281 faster_coco_eval-1.5.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/requirements/extra.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/requirements/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 11:14:24.749281 faster_coco_eval-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-24 11:14:19.000000 faster_coco_eval-1.5.4/setup.py
```

### Comparing `faster_coco_eval-1.5.3/LICENSE` & `faster_coco_eval-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.3/PKG-INFO` & `faster_coco_eval-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster-coco-eval
-Version: 1.5.3
+Version: 1.5.4
 Summary: Faster interpretation of the original COCOEval
 Home-page: https://github.com/MiXaiLL76/faster_coco_eval
 Author: MiXaiLL76
 Author-email: mike.milos@yandex.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `faster_coco_eval-1.5.3/README.md` & `faster_coco_eval-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.3/csrc/faster_eval_api/coco_eval/cocoeval.cpp` & `faster_coco_eval-1.5.4/csrc/faster_eval_api/coco_eval/cocoeval.cpp`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.3/csrc/faster_eval_api/coco_eval/cocoeval.h` & `faster_coco_eval-1.5.4/csrc/faster_eval_api/coco_eval/cocoeval.h`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.3/csrc/faster_eval_api/faster_eval_api.cpp` & `faster_coco_eval-1.5.4/csrc/faster_eval_api/faster_eval_api.cpp`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.3/csrc/mask/common/maskApi.c` & `faster_coco_eval-1.5.4/csrc/mask/common/maskApi.c`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.3/csrc/mask/common/maskApi.h` & `faster_coco_eval-1.5.4/csrc/mask/common/maskApi.h`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.3/csrc/mask/pycocotools/_mask.pyx` & `faster_coco_eval-1.5.4/csrc/mask/pycocotools/_mask.pyx`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.3/faster_coco_eval/core/coco.py` & `faster_coco_eval-1.5.4/faster_coco_eval/core/coco.py`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.3/faster_coco_eval/core/cocoeval.py` & `faster_coco_eval-1.5.4/faster_coco_eval/core/cocoeval.py`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.3/faster_coco_eval/core/faster_eval_api.py` & `faster_coco_eval-1.5.4/faster_coco_eval/core/faster_eval_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,36 +330,34 @@
 
         if self.matched:
             self.all_stats = np.append(self.all_stats, self.compute_mIoU())
             self.all_stats = np.append(self.all_stats, self.compute_mAUC())
 
     @property
     def stats_as_dict(self):
-        iouType = self.params.iouType
-        assert (
-            iouType == "segm" or iouType == "bbox"
-        ), "iouType={} not supported".format(iouType)
-
         labels = [
             "AP_all",
             "AP_50",
             "AP_75",
             "AP_small",
             "AP_medium",
             "AP_large",
             "AR_all",
             "AR_second",
             "AR_third",
             "AR_small",
             "AR_medium",
             "AR_large",
-            "AR_50",
-            "AR_75",
         ]
 
+        if self.params.iouType in ["segm", "bbox"]:
+            labels += ["AR_50", "AR_75"]
+        else:
+            labels = [label for label in labels if "small" not in label]
+
         if self.matched:
             labels += [
                 "mIoU",
                 "mAUC_" + str(int(self.params.iouThrs[0] * 100)),
             ]
 
         maxDets = self.params.maxDets
```

### Comparing `faster_coco_eval-1.5.3/faster_coco_eval/core/mask.py` & `faster_coco_eval-1.5.4/faster_coco_eval/core/mask.py`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.3/faster_coco_eval/extra/curves.py` & `faster_coco_eval-1.5.4/faster_coco_eval/extra/curves.py`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.3/faster_coco_eval/extra/display.py` & `faster_coco_eval-1.5.4/faster_coco_eval/extra/display.py`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.3/faster_coco_eval/extra/draw.py` & `faster_coco_eval-1.5.4/faster_coco_eval/extra/draw.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,20 @@
         ready_bones = {i: True for i in range(xyz.shape[0])}
         for p1, p2 in skeleton:
             if ready_bones.get(p1 - 1, False) and ready_bones.get(
                 p2 - 1, False
             ):
                 all_x += [xyz[int(p1 - 1), 0], xyz[int(p2 - 1), 0], None]
                 all_y += [xyz[int(p1 - 1), 1], xyz[int(p2 - 1), 1], None]
+
+        if ann.get("bbox"):
+            x1, y1, w, h = ann.get("bbox")
+            all_x += [x1, x1 + w, x1 + w, x1, x1, None]
+            all_y += [y1, y1, y1 + h, y1 + h, y1, None]
+
     else:
         raise ValueError()
 
     return go.Scatter(
         x=all_x,
         y=all_y,
         name="",
@@ -214,17 +220,18 @@
         binary_format="jpg",
         aspect="auto",
         labels=dict(animation_frame="shown picture"),
     )
 
     legends = {}
     for poly in polygons:
-        if legends.get(poly.legendgroup) is None:
-            poly.showlegend = True
-            legends[poly.legendgroup] = True
+        if poly is not None:
+            if legends.get(poly.legendgroup) is None:
+                poly.showlegend = True
+                legends[poly.legendgroup] = True
 
         fig.add_trace(poly)
 
     layout = {
         "title": "image_id={}<br>image_fn={}".format(image_id, image_fn),
         "autosize": True,
         "height": 700,
```

### Comparing `faster_coco_eval-1.5.3/faster_coco_eval/extra/extra.py` & `faster_coco_eval-1.5.4/faster_coco_eval/extra/extra.py`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.3/faster_coco_eval/extra/utils.py` & `faster_coco_eval-1.5.4/faster_coco_eval/extra/utils.py`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.3/faster_coco_eval.egg-info/PKG-INFO` & `faster_coco_eval-1.5.4/faster_coco_eval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster-coco-eval
-Version: 1.5.3
+Version: 1.5.4
 Summary: Faster interpretation of the original COCOEval
 Home-page: https://github.com/MiXaiLL76/faster_coco_eval
 Author: MiXaiLL76
 Author-email: mike.milos@yandex.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `faster_coco_eval-1.5.3/faster_coco_eval.egg-info/SOURCES.txt` & `faster_coco_eval-1.5.4/faster_coco_eval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `faster_coco_eval-1.5.3/setup.py` & `faster_coco_eval-1.5.4/setup.py`

 * *Files identical despite different names*

