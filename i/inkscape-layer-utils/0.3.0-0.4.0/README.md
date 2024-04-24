# Comparing `tmp/inkscape_layer_utils-0.3.0.tar.gz` & `tmp/inkscape_layer_utils-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inkscape_layer_utils-0.3.0.tar", last modified: Sun Apr 14 22:30:21 2024, max compression
+gzip compressed data, was "inkscape_layer_utils-0.4.0.tar", last modified: Wed Apr 24 21:50:39 2024, max compression
```

## Comparing `inkscape_layer_utils-0.3.0.tar` & `inkscape_layer_utils-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:30:21.305784 inkscape_layer_utils-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-14 22:30:21.305784 inkscape_layer_utils-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:30:21.305784 inkscape_layer_utils-0.3.0/inkscape_layer_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/inkscape_layer_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/inkscape_layer_utils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-14 22:30:21.305784 inkscape_layer_utils-0.3.0/inkscape_layer_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    20568 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/inkscape_layer_utils/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/inkscape_layer_utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:30:21.305784 inkscape_layer_utils-0.3.0/inkscape_layer_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-14 22:30:21.000000 inkscape_layer_utils-0.3.0/inkscape_layer_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-14 22:30:21.000000 inkscape_layer_utils-0.3.0/inkscape_layer_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 22:30:21.000000 inkscape_layer_utils-0.3.0/inkscape_layer_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-14 22:30:21.000000 inkscape_layer_utils-0.3.0/inkscape_layer_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-14 22:30:21.000000 inkscape_layer_utils-0.3.0/inkscape_layer_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-14 22:30:21.305784 inkscape_layer_utils-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:30:21.305784 inkscape_layer_utils-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/tests/image_test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/tests/test_image_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/tests/test_image_1.py
--rw-r--r--   0 runner    (1001) docker     (127)    83572 2024-04-14 22:30:17.000000 inkscape_layer_utils-0.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:50:39.027842 inkscape_layer_utils-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 21:50:34.000000 inkscape_layer_utils-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-24 21:50:39.027842 inkscape_layer_utils-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-24 21:50:34.000000 inkscape_layer_utils-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:50:39.027842 inkscape_layer_utils-0.4.0/inkscape_layer_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-24 21:50:34.000000 inkscape_layer_utils-0.4.0/inkscape_layer_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 21:50:34.000000 inkscape_layer_utils-0.4.0/inkscape_layer_utils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-24 21:50:39.027842 inkscape_layer_utils-0.4.0/inkscape_layer_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21458 2024-04-24 21:50:34.000000 inkscape_layer_utils-0.4.0/inkscape_layer_utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-24 21:50:34.000000 inkscape_layer_utils-0.4.0/inkscape_layer_utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:50:39.027842 inkscape_layer_utils-0.4.0/inkscape_layer_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-24 21:50:39.000000 inkscape_layer_utils-0.4.0/inkscape_layer_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-24 21:50:39.000000 inkscape_layer_utils-0.4.0/inkscape_layer_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 21:50:39.000000 inkscape_layer_utils-0.4.0/inkscape_layer_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-24 21:50:39.000000 inkscape_layer_utils-0.4.0/inkscape_layer_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 21:50:39.000000 inkscape_layer_utils-0.4.0/inkscape_layer_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-24 21:50:39.027842 inkscape_layer_utils-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-24 21:50:34.000000 inkscape_layer_utils-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:50:39.027842 inkscape_layer_utils-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:50:34.000000 inkscape_layer_utils-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-24 21:50:34.000000 inkscape_layer_utils-0.4.0/tests/image_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-04-24 21:50:34.000000 inkscape_layer_utils-0.4.0/tests/test_image_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-24 21:50:34.000000 inkscape_layer_utils-0.4.0/tests/test_image_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83572 2024-04-24 21:50:34.000000 inkscape_layer_utils-0.4.0/versioneer.py
```

### Comparing `inkscape_layer_utils-0.3.0/LICENSE` & `inkscape_layer_utils-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inkscape_layer_utils-0.3.0/PKG-INFO` & `inkscape_layer_utils-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inkscape_layer_utils
-Version: 0.3.0
+Version: 0.4.0
 Summary: Simple library to extract and manipulate layers in inkscape SVGs
 Home-page: https://github.com/twyleg/inkscape_layer_utils
 Author: Torsten Wylegala
 Author-email: mail@twyleg.de
 License: GPL 3.0
 Keywords: inkscape svg layer utilities
 License-File: LICENSE
```

### Comparing `inkscape_layer_utils-0.3.0/README.rst` & `inkscape_layer_utils-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `inkscape_layer_utils-0.3.0/inkscape_layer_utils/__init__.py` & `inkscape_layer_utils-0.4.0/inkscape_layer_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `inkscape_layer_utils-0.3.0/inkscape_layer_utils/image.py` & `inkscape_layer_utils-0.4.0/inkscape_layer_utils/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -398,14 +398,37 @@
         """
         super().stroke_paint_all_objects(color, force=force)
 
         if recursive:
             for layer in self.layers.values():
                 layer.stroke_paint_all_objects(color, force=force, recursive=recursive)
 
+    def set_visibility(self, visibility: bool, recursive=False) -> None:
+        """
+        Set the visibility of a specific layer and its children (when recursive flag is set)
+
+        Parameters
+        ----------
+        visibility: bool
+            Visibility to set for layer.
+        recursive: bool
+            Flag to enable recursive modification of visibility.
+
+        """
+        if recursive:
+            for layer in self.layers.values():
+                layer.set_visibility(visibility, recursive)
+
+        if "style" in self.layer_element.attrib:
+            style = self.layer_element.attrib["style"]
+            style_dict = OrderedDict(item.split(":") for item in style.split(";"))
+
+            style_dict["display"] = "inline" if visibility else "none"
+            self.layer_element.attrib["style"] = ";".join([f"{key}:{value}" for key, value in style_dict.items()])
+
 
 class Image(Layer):
     """
     Represents an Inkscape SVG image.
 
     Attributes
     ----------
```

### Comparing `inkscape_layer_utils-0.3.0/inkscape_layer_utils/main.py` & `inkscape_layer_utils-0.4.0/inkscape_layer_utils/main.py`

 * *Files identical despite different names*

### Comparing `inkscape_layer_utils-0.3.0/inkscape_layer_utils.egg-info/PKG-INFO` & `inkscape_layer_utils-0.4.0/inkscape_layer_utils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inkscape_layer_utils
-Version: 0.3.0
+Version: 0.4.0
 Summary: Simple library to extract and manipulate layers in inkscape SVGs
 Home-page: https://github.com/twyleg/inkscape_layer_utils
 Author: Torsten Wylegala
 Author-email: mail@twyleg.de
 License: GPL 3.0
 Keywords: inkscape svg layer utilities
 License-File: LICENSE
```

### Comparing `inkscape_layer_utils-0.3.0/inkscape_layer_utils.egg-info/SOURCES.txt` & `inkscape_layer_utils-0.4.0/inkscape_layer_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inkscape_layer_utils-0.3.0/setup.py` & `inkscape_layer_utils-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `inkscape_layer_utils-0.3.0/tests/image_test_case.py` & `inkscape_layer_utils-0.4.0/tests/image_test_case.py`

 * *Files identical despite different names*

### Comparing `inkscape_layer_utils-0.3.0/tests/test_image_0.py` & `inkscape_layer_utils-0.4.0/tests/test_image_0.py`

 * *Files identical despite different names*

### Comparing `inkscape_layer_utils-0.3.0/tests/test_image_1.py` & `inkscape_layer_utils-0.4.0/tests/test_image_1.py`

 * *Files identical despite different names*

### Comparing `inkscape_layer_utils-0.3.0/versioneer.py` & `inkscape_layer_utils-0.4.0/versioneer.py`

 * *Files identical despite different names*

