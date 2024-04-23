# Comparing `tmp/ehdg_pupil_detector-3.5.0.tar.gz` & `tmp/ehdg_pupil_detector-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdg_pupil_detector-3.5.0.tar", last modified: Tue Apr 23 03:55:04 2024, max compression
+gzip compressed data, was "ehdg_pupil_detector-3.5.1.tar", last modified: Tue Apr 23 04:25:35 2024, max compression
```

## Comparing `ehdg_pupil_detector-3.5.0.tar` & `ehdg_pupil_detector-3.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 03:55:04.500054 ehdg_pupil_detector-3.5.0/
--rw-rw-rw-   0        0        0    11558 2023-11-05 22:14:35.000000 ehdg_pupil_detector-3.5.0/LICENSE
--rw-rw-rw-   0        0        0     4075 2024-04-23 03:55:04.498060 ehdg_pupil_detector-3.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     3261 2023-11-22 04:05:27.000000 ehdg_pupil_detector-3.5.0/README.md
--rw-rw-rw-   0        0        0     1162 2024-04-23 03:37:05.000000 ehdg_pupil_detector-3.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-23 03:55:04.500054 ehdg_pupil_detector-3.5.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-23 03:55:04.468594 ehdg_pupil_detector-3.5.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-23 03:55:04.476543 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector/
--rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector/__init__.py
--rw-rw-rw-   0        0        0    25943 2024-04-23 03:36:38.000000 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector/ehdg_pupil_detector.py
--rw-rw-rw-   0        0        0      312 2024-04-22 23:25:41.000000 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector/opm_detector_config.json
--rw-rw-rw-   0        0        0    24813 2024-04-23 03:52:15.000000 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector/opmtrack.py
--rw-rw-rw-   0        0        0      200 2024-04-17 02:41:31.000000 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector/opmtrack_plot.json
-drwxrwxrwx   0        0        0        0 2024-04-23 03:55:04.497063 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector.egg-info/
--rw-rw-rw-   0        0        0     4075 2024-04-23 03:55:04.000000 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      527 2024-04-23 03:55:04.000000 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 03:55:04.000000 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-23 03:55:04.000000 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      105 2024-04-23 03:55:04.000000 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-23 03:55:04.000000 ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 04:25:35.490976 ehdg_pupil_detector-3.5.1/
+-rw-rw-rw-   0        0        0    11558 2023-11-05 22:14:35.000000 ehdg_pupil_detector-3.5.1/LICENSE
+-rw-rw-rw-   0        0        0     4075 2024-04-23 04:25:35.489979 ehdg_pupil_detector-3.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3261 2023-11-22 04:05:27.000000 ehdg_pupil_detector-3.5.1/README.md
+-rw-rw-rw-   0        0        0     1162 2024-04-23 04:23:07.000000 ehdg_pupil_detector-3.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 04:25:35.490976 ehdg_pupil_detector-3.5.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-23 04:25:35.460016 ehdg_pupil_detector-3.5.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-23 04:25:35.467525 ehdg_pupil_detector-3.5.1/src/ehdg_pupil_detector/
+-rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_pupil_detector-3.5.1/src/ehdg_pupil_detector/__init__.py
+-rw-rw-rw-   0        0        0    25943 2024-04-23 03:36:38.000000 ehdg_pupil_detector-3.5.1/src/ehdg_pupil_detector/ehdg_pupil_detector.py
+-rw-rw-rw-   0        0        0      312 2024-04-22 23:25:41.000000 ehdg_pupil_detector-3.5.1/src/ehdg_pupil_detector/opm_detector_config.json
+-rw-rw-rw-   0        0        0    24813 2024-04-23 04:19:56.000000 ehdg_pupil_detector-3.5.1/src/ehdg_pupil_detector/opmtrack.py
+-rw-rw-rw-   0        0        0      200 2024-04-17 02:41:31.000000 ehdg_pupil_detector-3.5.1/src/ehdg_pupil_detector/opmtrack_plot.json
+drwxrwxrwx   0        0        0        0 2024-04-23 04:25:35.488981 ehdg_pupil_detector-3.5.1/src/ehdg_pupil_detector.egg-info/
+-rw-rw-rw-   0        0        0     4075 2024-04-23 04:25:35.000000 ehdg_pupil_detector-3.5.1/src/ehdg_pupil_detector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      527 2024-04-23 04:25:35.000000 ehdg_pupil_detector-3.5.1/src/ehdg_pupil_detector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 04:25:35.000000 ehdg_pupil_detector-3.5.1/src/ehdg_pupil_detector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-23 04:25:35.000000 ehdg_pupil_detector-3.5.1/src/ehdg_pupil_detector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      105 2024-04-23 04:25:35.000000 ehdg_pupil_detector-3.5.1/src/ehdg_pupil_detector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-23 04:25:35.000000 ehdg_pupil_detector-3.5.1/src/ehdg_pupil_detector.egg-info/top_level.txt
```

### Comparing `ehdg_pupil_detector-3.5.0/LICENSE` & `ehdg_pupil_detector-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.5.0/PKG-INFO` & `ehdg_pupil_detector-3.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_pupil_detector
-Version: 3.5.0
+Version: 3.5.1
 Summary: Python Library for Pupil Detector of Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/ehdg_pupil_detector
 Project-URL: Bug Tracker, https://github.com/jtur044/ehdg_pupil_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ehdg_pupil_detector-3.5.0/README.md` & `ehdg_pupil_detector-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.5.0/pyproject.toml` & `ehdg_pupil_detector-3.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ehdg_pupil_detector"
-version = "3.5.0"
+version = "3.5.1"
 authors = [
   { name="Zaw Lin Tun", email="zawlintun1511@gmail.com" },
 ]
 description = "Python Library for Pupil Detector of Eye Health Diagnostic Group"
 readme = "README.md"
 dependencies = ["setuptools>=61.0", "opencv-python>=4.8.1.78", "scipy>=1.11.3", "numpy>=1.26.1", "commentjson", "ehdg_tools>=4.2.2", "numpy"]
 requires-python = ">=3.9"
```

### Comparing `ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector/ehdg_pupil_detector.py` & `ehdg_pupil_detector-3.5.1/src/ehdg_pupil_detector/ehdg_pupil_detector.py`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector/opmtrack.py` & `ehdg_pupil_detector-3.5.1/src/ehdg_pupil_detector/opmtrack.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                rrt_lower_limit=0, rrt_upper_limit=255,
                gaussian_blur=True, binary_fill=True,
                direction_input=None, min_max_circle=True,
                min_circle_color="green", max_circle_color="orange",
                pupil_circle_color="red"):
     out_csv_dir = os.path.join(out_folder, "result.csv")
     out_video_dir = os.path.join(out_folder, "result.mp4")
-    log_dir = os.path.join(out_folder, "result.txt")
+    log_dir = os.path.join(out_folder, "result.log")
     pupil_circle_color_tuple = string_to_bgr_tuple(pupil_circle_color)
     min_circle_color_tuple = string_to_bgr_tuple(min_circle_color)
     max_circle_color_tuple = string_to_bgr_tuple(max_circle_color)
 
     detector = ehdg_pupil_detector.Detector(reflection_removal=reflection_removal,
                                             reflection_removal_lower_limit=rrt_lower_limit,
                                             reflection_removal_upper_limit=rrt_upper_limit,
```

### Comparing `ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector.egg-info/PKG-INFO` & `ehdg_pupil_detector-3.5.1/src/ehdg_pupil_detector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_pupil_detector
-Version: 3.5.0
+Version: 3.5.1
 Summary: Python Library for Pupil Detector of Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/ehdg_pupil_detector
 Project-URL: Bug Tracker, https://github.com/jtur044/ehdg_pupil_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ehdg_pupil_detector-3.5.0/src/ehdg_pupil_detector.egg-info/SOURCES.txt` & `ehdg_pupil_detector-3.5.1/src/ehdg_pupil_detector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

