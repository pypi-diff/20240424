# Comparing `tmp/imap_box_up-0.0.3.tar.gz` & `tmp/imap_box_up-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imap_box_up-0.0.3.tar", last modified: Fri Apr 12 09:18:45 2024, max compression
+gzip compressed data, was "imap_box_up-0.0.4.tar", last modified: Wed Apr 24 11:36:58 2024, max compression
```

## Comparing `imap_box_up-0.0.3.tar` & `imap_box_up-0.0.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:18:45.708883 imap_box_up-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-04-12 09:18:45.708883 imap_box_up-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:18:45.704883 imap_box_up-0.0.3/imap/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/editor.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/global_var.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:18:45.704883 imap_box_up-0.0.3/imap/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/lib/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    30241 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/lib/convertor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/lib/convex_hull.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/lib/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/lib/odr_spiral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:18:45.708883 imap_box_up-0.0.3/imap/lib/opendrive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/lib/opendrive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/lib/opendrive/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/lib/opendrive/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/lib/opendrive/junction.py
--rw-r--r--   0 runner    (1001) docker     (127)    15637 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/lib/opendrive/lanes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/lib/opendrive/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     8140 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/lib/opendrive/plan_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/lib/opendrive/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/lib/opendrive/road.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/lib/opendrive/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/lib/opendrive/user_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/lib/polynoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/lib/proj_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/lib/proto_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/lib/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/imap/map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:18:45.708883 imap_box_up-0.0.3/imap_box_up.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-04-12 09:18:45.000000 imap_box_up-0.0.3/imap_box_up.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-12 09:18:45.000000 imap_box_up-0.0.3/imap_box_up.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:18:45.000000 imap_box_up-0.0.3/imap_box_up.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 09:18:45.000000 imap_box_up-0.0.3/imap_box_up.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 09:18:45.000000 imap_box_up-0.0.3/imap_box_up.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-12 09:18:45.000000 imap_box_up-0.0.3/imap_box_up.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 09:18:45.708883 imap_box_up-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-12 09:18:06.000000 imap_box_up-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:36:58.930940 imap_box_up-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-04-24 11:36:58.930940 imap_box_up-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:36:58.922939 imap_box_up-0.0.4/imap/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/global_var.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:36:58.926939 imap_box_up-0.0.4/imap/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32951 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/convertor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/convex_hull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/odr_spiral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:36:58.926939 imap_box_up-0.0.4/imap/lib/opendrive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/opendrive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/opendrive/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/opendrive/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/opendrive/junction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15637 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/opendrive/lanes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/opendrive/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8140 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/opendrive/plan_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/opendrive/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/opendrive/road.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/opendrive/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/opendrive/user_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/polynoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/proj_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/proto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/lib/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/imap/map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:36:58.926939 imap_box_up-0.0.4/imap_box_up.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-04-24 11:36:58.000000 imap_box_up-0.0.4/imap_box_up.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-24 11:36:58.000000 imap_box_up-0.0.4/imap_box_up.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:36:58.000000 imap_box_up-0.0.4/imap_box_up.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 11:36:58.000000 imap_box_up-0.0.4/imap_box_up.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-24 11:36:58.000000 imap_box_up-0.0.4/imap_box_up.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 11:36:58.000000 imap_box_up-0.0.4/imap_box_up.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 11:36:58.930940 imap_box_up-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-24 11:36:15.000000 imap_box_up-0.0.4/setup.py
```

### Comparing `imap_box_up-0.0.3/LICENSE` & `imap_box_up-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.3/PKG-INFO` & `imap_box_up-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imap_box_up
-Version: 0.0.3
+Version: 0.0.4
 Summary: High-resolution map visualization and conversion tool, opendrive hdmap convert to appollo base map!
 Home-page: https://github.com/porterpan/imap_box_up
 Author: porter
 Author-email: porter.pan@outlook.com
 Project-URL: Bug Tracker, https://github.com/porterpan/imap_box_up/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -19,37 +19,34 @@
 Requires-Dist: concave-hull<=0.0.7
 Requires-Dist: scipy<=1.13.0
 
 # imap_box_up
 
 [![Documentation Status](https://readthedocs.org/projects/imap/badge/?version=latest)](https://imap.readthedocs.io/en/latest/?badge=latest)
 
-**[imap_box_up](https://imap.readthedocs.io/en/latest/)** is a tool for visualize and convert format of the hd-map. This project was inspired by Apollo, modified by [imap](https://github.com/daohu527/imap), the imap tool is very useful. 
+**[imap_box_up](https://imap.readthedocs.io/en/latest/)** is a tool for visualize and convert format of the hd-map. This project was inspired by Apollo, modified by [imap](https://github.com/daohu527/imap/releases/tag/v0.1.7), the imap tool is very useful. 
 
 The name of **imap_box_up** , Just to modified from imap_box
 
 The modified tool is named **imap_box_up** just to distinguish it from **imap_box**
 
 imap_box_up source code: [https://github.com/porterpan/imap_box_up](https://github.com/porterpan/imap_box_up)
 
 **Note:**
 
-The project is Modify on project of [https://github.com/daohu527/imap](https://github.com/daohu527/imap)
+- the map road lane attribution should have curb, if not have curb, task will random selection shouler, stop, walking to create apoolo map.
 
-> I found that imap_box had the problem of inaccurate junction drawing, which could not meet the needs of my project. Therefore, I modified imap_box based on it to adapt to appollo hdmap code. 
-
-## now(fix junction bug)
-
-![valid junction](https://img2.imgtp.com/2024/04/12/aHEcAl7a.png)
+- The project is Modify on project of [https://github.com/daohu527/imap](https://github.com/daohu527/imap)
 
+> I found that imap_box had the problem of inaccurate junction drawing, which could not meet the needs of my project. Therefore, I modified imap_box based on it to adapt to appollo hdmap code. 
 
-## the old tool bug
 
-![invalid junction](https://img2.imgtp.com/2024/04/12/hOWOvqyr.jpg)
+## fix junction bug
 
+![valid junction](https://img2.imgtp.com/2024/04/12/aHEcAl7a.png)
 
 **Supported features**:
 1. Visualize the hd-map, supported formats: Apollo, OpenDrive.
 2. Find lane by id
 3. Convert format: Opendrive to Apollo format.
 
 | os      | support                 | remark |
```

### Comparing `imap_box_up-0.0.3/README.md` & `imap_box_up-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 # imap_box_up
 
 [![Documentation Status](https://readthedocs.org/projects/imap/badge/?version=latest)](https://imap.readthedocs.io/en/latest/?badge=latest)
 
-**[imap_box_up](https://imap.readthedocs.io/en/latest/)** is a tool for visualize and convert format of the hd-map. This project was inspired by Apollo, modified by [imap](https://github.com/daohu527/imap), the imap tool is very useful. 
+**[imap_box_up](https://imap.readthedocs.io/en/latest/)** is a tool for visualize and convert format of the hd-map. This project was inspired by Apollo, modified by [imap](https://github.com/daohu527/imap/releases/tag/v0.1.7), the imap tool is very useful. 
 
 The name of **imap_box_up** , Just to modified from imap_box
 
 The modified tool is named **imap_box_up** just to distinguish it from **imap_box**
 
 imap_box_up source code: [https://github.com/porterpan/imap_box_up](https://github.com/porterpan/imap_box_up)
 
 **Note:**
 
-The project is Modify on project of [https://github.com/daohu527/imap](https://github.com/daohu527/imap)
+- the map road lane attribution should have curb, if not have curb, task will random selection shouler, stop, walking to create apoolo map.
 
-> I found that imap_box had the problem of inaccurate junction drawing, which could not meet the needs of my project. Therefore, I modified imap_box based on it to adapt to appollo hdmap code. 
-
-## now(fix junction bug)
-
-![valid junction](https://img2.imgtp.com/2024/04/12/aHEcAl7a.png)
+- The project is Modify on project of [https://github.com/daohu527/imap](https://github.com/daohu527/imap)
 
+> I found that imap_box had the problem of inaccurate junction drawing, which could not meet the needs of my project. Therefore, I modified imap_box based on it to adapt to appollo hdmap code. 
 
-## the old tool bug
 
-![invalid junction](https://img2.imgtp.com/2024/04/12/hOWOvqyr.jpg)
+## fix junction bug
 
+![valid junction](https://img2.imgtp.com/2024/04/12/aHEcAl7a.png)
 
 **Supported features**:
 1. Visualize the hd-map, supported formats: Apollo, OpenDrive.
 2. Find lane by id
 3. Convert format: Opendrive to Apollo format.
 
 | os      | support                 | remark |
```

### Comparing `imap_box_up-0.0.3/imap/editor.py` & `imap_box_up-0.0.4/imap/editor.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.3/imap/global_var.py` & `imap_box_up-0.0.4/imap/global_var.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.3/imap/lib/common.py` & `imap_box_up-0.0.4/imap/lib/common.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.3/imap/lib/convertor.py` & `imap_box_up-0.0.4/imap/lib/convertor.py`

 * *Files 6% similar despite different names*

```diff
@@ -616,42 +616,94 @@
           link_name = self.xodr_map.roads[junction_connecting_lane.connecting_road].link
           # print("junction_id: ", junction_id)
           # print("pre: {} sub: {}".format(link_name.predecessor.contact_point, link_name.successor.contact_point))          
           incomRoadID = junction_connecting_lane.connecting_road #incoming_road
           left_boundary_points = []
           right_boundary_points = []  
           
+          have_right_curb = False           
+          for lanesectionright in lanesection_.right:
+              for roadmark in lanesectionright.road_marks:
+                if roadmark.roadmark_type == "curb":
+                  have_right_curb = True
+
           for lanesectionright in lanesection_.right: # -            
-            if  lanesectionright.lane_type != "driving" and lanesectionright.lane_type != "shoulder": 
+            if have_right_curb==True:
+              record_right = False
+              for roadmark in lanesectionright.road_marks:
+                if roadmark.roadmark_type == "curb":
+                  record_right = True
+              if record_right == True:   
+                if incomRoadID in right_incomroadlist:
+                  break
+                right_incomroadlist.append(incomRoadID) 
+                # if len(lanesection_.right)>0 and len(lanesection_.left)>0: 
+                if len(lanesectionright.right_boundary) >0:   
+                  print("__curbe__") 
+                  for points in lanesectionright.right_boundary:              
+                      right_boundary_points.append([points.x, points.y])  
+                # else:
+                #   for points in lanesectionright.right_boundary:              
+                #         right_boundary_points.append([points.x, points.y])   
+                    
+            elif  lanesectionright.lane_type != "driving":# and lanesectionright.lane_type != "shoulder": 
               # print("laneleft.lane_id.right: ", lanesectionright.lane_id)
               # print("laneleft.type: ", lanesectionright.lane_type)
               if incomRoadID in right_incomroadlist:
                 break
               right_incomroadlist.append(incomRoadID) 
-              if len(lanesection_.right)>0 and len(lanesection_.left)>0:   
+              # if len(lanesection_.right)>0 and len(lanesection_.left)>0:  
+              if len(lanesectionright.right_boundary) >0: 
+                print("__tyep__:", lanesectionright.lane_type) 
                 for points in lanesectionright.right_boundary:              
-                      right_boundary_points.append([points.x, points.y])  
-              else:
-                for points in lanesectionright.right_boundary:              
-                      right_boundary_points.append([points.x, points.y])          
-                     
-                             
+                    right_boundary_points.append([points.x, points.y])  
+              # else:
+              #   for points in lanesectionright.right_boundary:              
+              #         right_boundary_points.append([points.x, points.y])          
+
+          # if lanesectionleft.road_marks[0].roadmark_type == "curb":
+          have_left_curb = False           
+          for lanesectionleft in lanesection_.left:
+              for roadmark in lanesectionleft.road_marks:
+                if roadmark.roadmark_type == "curb":
+                  have_left_curb = True
+
           for lanesectionleft in lanesection_.left: # + 
-            if lanesectionleft.lane_type != "driving" and lanesectionleft.lane_type != "shoulder":
+            # if lanesectionleft.road_marks[0].roadmark_type == "curb":
+            if have_left_curb==True:
+              record = False
+              for roadmark in lanesectionleft.road_marks:
+                if roadmark.roadmark_type == "curb":
+                  record = True
+              if record == True:   
+                if incomRoadID in left_incomroadlist:
+                  break
+                left_incomroadlist.append(incomRoadID)
+                # if len(lanesection_.right)>0 and len(lanesection_.left)>0:   
+                if len(lanesectionleft.left_boundary) >0:  
+                  print("__curbe__")           
+                  for points in lanesectionleft.left_boundary:                           
+                    left_boundary_points.append([points.x, points.y])
+                # else:
+                #   for points in lanesectionleft.left_boundary:                           
+                #       left_boundary_points.append([points.x, points.y])
+            elif lanesectionleft.lane_type != "driving": # and lanesectionleft.lane_type != "shoulder":
               # print("laneleft.lane_id.left: ", lanesectionleft.lane_id)
               # print("laneleft.type: ", lanesectionleft.lane_type)  
               if incomRoadID in left_incomroadlist:
                 break
               left_incomroadlist.append(incomRoadID)
-              if len(lanesection_.right)>0 and len(lanesection_.left)>0:                
+              # if len(lanesection_.right)>0 and len(lanesection_.left)>0:    
+              if len(lanesectionleft.left_boundary) >0:       
+                print("__tyep__:", lanesectionleft.lane_type)      
                 for points in lanesectionleft.left_boundary:                           
-                    left_boundary_points.append([points.x, points.y])
-              else:
-                for points in lanesectionleft.left_boundary:                           
-                    left_boundary_points.append([points.x, points.y])
+                  left_boundary_points.append([points.x, points.y])
+              # else:
+              #   for points in lanesectionleft.left_boundary:                           
+              #       left_boundary_points.append([points.x, points.y])
           
           if len(right_boundary_points)>3:
             boundary_point_temp.append([right_boundary_points, link_name, "right"])
           elif len(left_boundary_points)>3:  
             boundary_point_temp.append([left_boundary_points, link_name, "left"])
 
       if len(boundary_point_temp)==3:
```

### Comparing `imap_box_up-0.0.3/imap/lib/convex_hull.py` & `imap_box_up-0.0.4/imap/lib/convex_hull.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.3/imap/lib/draw.py` & `imap_box_up-0.0.4/imap/lib/draw.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.3/imap/lib/odr_spiral.py` & `imap_box_up-0.0.4/imap/lib/odr_spiral.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.3/imap/lib/opendrive/common.py` & `imap_box_up-0.0.4/imap/lib/opendrive/common.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.3/imap/lib/opendrive/header.py` & `imap_box_up-0.0.4/imap/lib/opendrive/header.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.3/imap/lib/opendrive/junction.py` & `imap_box_up-0.0.4/imap/lib/opendrive/junction.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.3/imap/lib/opendrive/lanes.py` & `imap_box_up-0.0.4/imap/lib/opendrive/lanes.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.3/imap/lib/opendrive/map.py` & `imap_box_up-0.0.4/imap/lib/opendrive/map.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.3/imap/lib/opendrive/plan_view.py` & `imap_box_up-0.0.4/imap/lib/opendrive/plan_view.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.3/imap/lib/opendrive/profile.py` & `imap_box_up-0.0.4/imap/lib/opendrive/profile.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.3/imap/lib/opendrive/road.py` & `imap_box_up-0.0.4/imap/lib/opendrive/road.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.3/imap/lib/opendrive/signals.py` & `imap_box_up-0.0.4/imap/lib/opendrive/signals.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.3/imap/lib/opendrive/user_data.py` & `imap_box_up-0.0.4/imap/lib/opendrive/user_data.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.3/imap/lib/polynoms.py` & `imap_box_up-0.0.4/imap/lib/polynoms.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.3/imap/lib/proj_helper.py` & `imap_box_up-0.0.4/imap/lib/proj_helper.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.3/imap/lib/proto_utils.py` & `imap_box_up-0.0.4/imap/lib/proto_utils.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.3/imap/lib/transform.py` & `imap_box_up-0.0.4/imap/lib/transform.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.3/imap/main.py` & `imap_box_up-0.0.4/imap/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,18 +85,18 @@
         "-s", "--sampling", action="store", type=float, required=False,
         default=1.0, help="sampling length")
     parser.add_argument(
         "-d", "--debug", action="store", type=bool, required=False,
         nargs='?', const=True, default=False, help="debug mode")
     parser.add_argument(
         "-r", "--relative", action="store", type=bool, required=False,
-        nargs='?', default=False, help="convert opendrive map to appollo map without GIS projection")
+        nargs='?', const=True, default=False, help="convert opendrive map to appollo map without GIS projection")
     parser.add_argument(
         "-b", "--box", action="store", type=bool, required=False,
-        nargs='?', default=False, help="convert opendrive map to appollo map junction with box(not recommend)")
+        nargs='?', const=True, default=False, help="convert opendrive map to appollo map junction with box(not recommend)")
     args = parser.parse_args(args[1:])
 
     # 1. Init global var
     global_var._init()
     global_var.set_element_vaule("sampling_length", args.sampling)
     global_var.set_element_vaule("debug_mode", args.debug)
     global_var.set_element_vaule("enable_z_axis", args.enable_z_axis)
```

### Comparing `imap_box_up-0.0.3/imap/map.py` & `imap_box_up-0.0.4/imap/map.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.3/imap_box_up.egg-info/PKG-INFO` & `imap_box_up-0.0.4/imap_box_up.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imap_box_up
-Version: 0.0.3
+Version: 0.0.4
 Summary: High-resolution map visualization and conversion tool, opendrive hdmap convert to appollo base map!
 Home-page: https://github.com/porterpan/imap_box_up
 Author: porter
 Author-email: porter.pan@outlook.com
 Project-URL: Bug Tracker, https://github.com/porterpan/imap_box_up/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -19,37 +19,34 @@
 Requires-Dist: concave-hull<=0.0.7
 Requires-Dist: scipy<=1.13.0
 
 # imap_box_up
 
 [![Documentation Status](https://readthedocs.org/projects/imap/badge/?version=latest)](https://imap.readthedocs.io/en/latest/?badge=latest)
 
-**[imap_box_up](https://imap.readthedocs.io/en/latest/)** is a tool for visualize and convert format of the hd-map. This project was inspired by Apollo, modified by [imap](https://github.com/daohu527/imap), the imap tool is very useful. 
+**[imap_box_up](https://imap.readthedocs.io/en/latest/)** is a tool for visualize and convert format of the hd-map. This project was inspired by Apollo, modified by [imap](https://github.com/daohu527/imap/releases/tag/v0.1.7), the imap tool is very useful. 
 
 The name of **imap_box_up** , Just to modified from imap_box
 
 The modified tool is named **imap_box_up** just to distinguish it from **imap_box**
 
 imap_box_up source code: [https://github.com/porterpan/imap_box_up](https://github.com/porterpan/imap_box_up)
 
 **Note:**
 
-The project is Modify on project of [https://github.com/daohu527/imap](https://github.com/daohu527/imap)
+- the map road lane attribution should have curb, if not have curb, task will random selection shouler, stop, walking to create apoolo map.
 
-> I found that imap_box had the problem of inaccurate junction drawing, which could not meet the needs of my project. Therefore, I modified imap_box based on it to adapt to appollo hdmap code. 
-
-## now(fix junction bug)
-
-![valid junction](https://img2.imgtp.com/2024/04/12/aHEcAl7a.png)
+- The project is Modify on project of [https://github.com/daohu527/imap](https://github.com/daohu527/imap)
 
+> I found that imap_box had the problem of inaccurate junction drawing, which could not meet the needs of my project. Therefore, I modified imap_box based on it to adapt to appollo hdmap code. 
 
-## the old tool bug
 
-![invalid junction](https://img2.imgtp.com/2024/04/12/hOWOvqyr.jpg)
+## fix junction bug
 
+![valid junction](https://img2.imgtp.com/2024/04/12/aHEcAl7a.png)
 
 **Supported features**:
 1. Visualize the hd-map, supported formats: Apollo, OpenDrive.
 2. Find lane by id
 3. Convert format: Opendrive to Apollo format.
 
 | os      | support                 | remark |
```

### Comparing `imap_box_up-0.0.3/imap_box_up.egg-info/SOURCES.txt` & `imap_box_up-0.0.4/imap_box_up.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.3/setup.py` & `imap_box_up-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="imap_box_up",
-    version="0.0.3",
+    version="0.0.4",
     author="porter",
     author_email="porter.pan@outlook.com",
     description="High-resolution map visualization and conversion tool, opendrive hdmap convert to appollo base map!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/porterpan/imap_box_up",
     project_urls={
```

