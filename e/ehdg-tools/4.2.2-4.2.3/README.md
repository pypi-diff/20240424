# Comparing `tmp/ehdg_tools-4.2.2.tar.gz` & `tmp/ehdg_tools-4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdg_tools-4.2.2.tar", last modified: Mon Apr 22 04:37:30 2024, max compression
+gzip compressed data, was "ehdg_tools-4.2.3.tar", last modified: Tue Apr 23 22:51:29 2024, max compression
```

## Comparing `ehdg_tools-4.2.2.tar` & `ehdg_tools-4.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 04:37:30.838505 ehdg_tools-4.2.2/
--rw-rw-rw-   0        0        0    11558 2023-11-17 13:32:14.000000 ehdg_tools-4.2.2/LICENSE
--rw-rw-rw-   0        0        0     3001 2024-04-22 04:37:30.837508 ehdg_tools-4.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2436 2023-11-22 03:02:06.000000 ehdg_tools-4.2.2/README.md
--rw-rw-rw-   0        0        0      699 2024-04-22 04:35:48.000000 ehdg_tools-4.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-22 04:37:30.838505 ehdg_tools-4.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-22 04:37:30.812773 ehdg_tools-4.2.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-22 04:37:30.822746 ehdg_tools-4.2.2/src/ehdg_tools/
--rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_tools-4.2.2/src/ehdg_tools/__init__.py
--rw-rw-rw-   0        0        0     4730 2023-11-21 22:16:22.000000 ehdg_tools-4.2.2/src/ehdg_tools/ehdg_buffers.py
--rw-rw-rw-   0        0        0     6886 2024-04-22 04:34:47.000000 ehdg_tools-4.2.2/src/ehdg_tools/ehdg_functions.py
--rw-rw-rw-   0        0        0     5831 2024-01-30 22:28:51.000000 ehdg_tools-4.2.2/src/ehdg_tools/ehdg_okn_checker.py
--rw-rw-rw-   0        0        0   117333 2024-04-17 02:32:38.000000 ehdg_tools-4.2.2/src/ehdg_tools/ehdg_plotter.py
--rw-rw-rw-   0        0        0    13490 2023-11-29 22:43:57.000000 ehdg_tools-4.2.2/src/ehdg_tools/ehdg_updater.py
-drwxrwxrwx   0        0        0        0 2024-04-22 04:37:30.836510 ehdg_tools-4.2.2/src/ehdg_tools.egg-info/
--rw-rw-rw-   0        0        0     3001 2024-04-22 04:37:30.000000 ehdg_tools-4.2.2/src/ehdg_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2024-04-22 04:37:30.000000 ehdg_tools-4.2.2/src/ehdg_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 04:37:30.000000 ehdg_tools-4.2.2/src/ehdg_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-22 04:37:30.000000 ehdg_tools-4.2.2/src/ehdg_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 22:51:29.959441 ehdg_tools-4.2.3/
+-rw-rw-rw-   0        0        0    11558 2023-11-17 13:32:14.000000 ehdg_tools-4.2.3/LICENSE
+-rw-rw-rw-   0        0        0     3001 2024-04-23 22:51:29.958444 ehdg_tools-4.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2436 2023-11-22 03:02:06.000000 ehdg_tools-4.2.3/README.md
+-rw-rw-rw-   0        0        0      699 2024-04-23 22:49:55.000000 ehdg_tools-4.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 22:51:29.959441 ehdg_tools-4.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-23 22:51:29.934505 ehdg_tools-4.2.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-23 22:51:29.942484 ehdg_tools-4.2.3/src/ehdg_tools/
+-rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_tools-4.2.3/src/ehdg_tools/__init__.py
+-rw-rw-rw-   0        0        0     4730 2023-11-21 22:16:22.000000 ehdg_tools-4.2.3/src/ehdg_tools/ehdg_buffers.py
+-rw-rw-rw-   0        0        0     6970 2024-04-23 22:48:47.000000 ehdg_tools-4.2.3/src/ehdg_tools/ehdg_functions.py
+-rw-rw-rw-   0        0        0     5831 2024-01-30 22:28:51.000000 ehdg_tools-4.2.3/src/ehdg_tools/ehdg_okn_checker.py
+-rw-rw-rw-   0        0        0   117333 2024-04-17 02:32:38.000000 ehdg_tools-4.2.3/src/ehdg_tools/ehdg_plotter.py
+-rw-rw-rw-   0        0        0    13490 2023-11-29 22:43:57.000000 ehdg_tools-4.2.3/src/ehdg_tools/ehdg_updater.py
+drwxrwxrwx   0        0        0        0 2024-04-23 22:51:29.957446 ehdg_tools-4.2.3/src/ehdg_tools.egg-info/
+-rw-rw-rw-   0        0        0     3001 2024-04-23 22:51:29.000000 ehdg_tools-4.2.3/src/ehdg_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2024-04-23 22:51:29.000000 ehdg_tools-4.2.3/src/ehdg_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 22:51:29.000000 ehdg_tools-4.2.3/src/ehdg_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-23 22:51:29.000000 ehdg_tools-4.2.3/src/ehdg_tools.egg-info/top_level.txt
```

### Comparing `ehdg_tools-4.2.2/LICENSE` & `ehdg_tools-4.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.2.2/PKG-INFO` & `ehdg_tools-4.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_tools
-Version: 4.2.2
+Version: 4.2.3
 Summary: Python library useful tools for ABI Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/ZawLinTun16925410/ehdg_tools
 Project-URL: Bug Tracker, https://github.com/ZawLinTun16925410/ehdg_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `ehdg_tools-4.2.2/README.md` & `ehdg_tools-4.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.2.2/pyproject.toml` & `ehdg_tools-4.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ehdg_tools"
-version = "4.2.2"
+version = "4.2.3"
 authors = [
   { name="Zaw Lin Tun", email="zawlintun1511@gmail.com" },
 ]
 description = "Python library useful tools for ABI Eye Health Diagnostic Group"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ehdg_tools-4.2.2/src/ehdg_tools/ehdg_buffers.py` & `ehdg_tools-4.2.3/src/ehdg_tools/ehdg_buffers.py`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.2.2/src/ehdg_tools/ehdg_functions.py` & `ehdg_tools-4.2.3/src/ehdg_tools/ehdg_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     'old lace': (253, 245, 230),
     'linen': (250, 240, 230),
     'antique white': (250, 235, 215),
     'papaya whip': (255, 239, 213),
     'blanched almond': (255, 235, 205),
     'bisque': (255, 228, 196),
     'peach puff': (255, 218, 185),
-    'PeachPuff': (255, 218, 185),
+    'peachpuff': (255, 218, 185),
     'navajo white': (255, 222, 173),
     'moccasin': (255, 228, 181),
     'cornsilk': (255, 248, 220),
     'ivory': (255, 255, 240),
     'lemon chiffon': (255, 250, 205),
     'seashell': (255, 245, 238),
     'honeydew': (240, 255, 240),
@@ -158,14 +158,15 @@
         print(error)
         is_there_program = False
     return is_there_program
 
 
 # This function is to change color string to color bgr tuple value
 def string_to_bgr_tuple(input_string):
+    input_string = str(input_string).lower()
     try:
         rgb_tuple = color_dictionary[input_string]
         red_index = rgb_tuple[0]
         green_index = rgb_tuple[1]
         blue_index = rgb_tuple[2]
         return blue_index, green_index, red_index
     except IndexError:
@@ -173,15 +174,16 @@
         print("It can be red, green, blue, black, white or magenta.")
         print("It also can be hex color code.")
         raise ValueError(f"Input string {input_string} is not a valid color string input.")
 
 
 # This function is to change hex color string to color bgr tuple value
 def hex_string_to_bgr_tuple(input_string):
-    if "#" in input_string.lower():
+    input_string = str(input_string).lower()
+    if "#" in input_string:
         value = input_string.lstrip('#')
         lv = len(value)
         if lv == 6:
             try:
                 tem_arr = tuple(int(value[xx:xx + lv // 3], 16) for xx in range(0, lv, lv // 3))
                 return tem_arr[::-1]
             except ValueError as e:
```

### Comparing `ehdg_tools-4.2.2/src/ehdg_tools/ehdg_okn_checker.py` & `ehdg_tools-4.2.3/src/ehdg_tools/ehdg_okn_checker.py`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.2.2/src/ehdg_tools/ehdg_plotter.py` & `ehdg_tools-4.2.3/src/ehdg_tools/ehdg_plotter.py`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.2.2/src/ehdg_tools/ehdg_updater.py` & `ehdg_tools-4.2.3/src/ehdg_tools/ehdg_updater.py`

 * *Files identical despite different names*

### Comparing `ehdg_tools-4.2.2/src/ehdg_tools.egg-info/PKG-INFO` & `ehdg_tools-4.2.3/src/ehdg_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_tools
-Version: 4.2.2
+Version: 4.2.3
 Summary: Python library useful tools for ABI Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/ZawLinTun16925410/ehdg_tools
 Project-URL: Bug Tracker, https://github.com/ZawLinTun16925410/ehdg_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

