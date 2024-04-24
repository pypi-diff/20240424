# Comparing `tmp/pyfibaro-0.7.7.tar.gz` & `tmp/pyfibaro-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfibaro-0.7.7.tar", last modified: Sun Apr  7 20:20:40 2024, max compression
+gzip compressed data, was "pyfibaro-0.7.8.tar", last modified: Wed Apr 24 19:58:27 2024, max compression
```

## Comparing `pyfibaro-0.7.7.tar` & `pyfibaro-0.7.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:20:40.557742 pyfibaro-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-07 20:20:40.557742 pyfibaro-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:20:40.553742 pyfibaro-0.7.7/pyfibaro/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:20:40.553742 pyfibaro-0.7.7/pyfibaro/common/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/common/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/common/rest_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/fibaro_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18818 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/fibaro_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/fibaro_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/fibaro_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/fibaro_room.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/fibaro_scene.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/fibaro_state_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/fibaro_state_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:20:40.557742 pyfibaro-0.7.7/pyfibaro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-07 20:20:40.000000 pyfibaro-0.7.7/pyfibaro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-07 20:20:40.000000 pyfibaro-0.7.7/pyfibaro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 20:20:40.000000 pyfibaro-0.7.7/pyfibaro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 20:20:40.000000 pyfibaro-0.7.7/pyfibaro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 20:20:40.000000 pyfibaro-0.7.7/pyfibaro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-07 20:20:40.557742 pyfibaro-0.7.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:20:40.557742 pyfibaro-0.7.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11151 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_device_armed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_device_hc3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_device_scene_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_device_scene_support_hc3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_room.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_scene.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_scene_hc3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_state_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_rest_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:58:27.373295 pyfibaro-0.7.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-24 19:58:27.373295 pyfibaro-0.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:58:27.365295 pyfibaro-0.7.8/pyfibaro/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/pyfibaro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:58:27.369295 pyfibaro-0.7.8/pyfibaro/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/pyfibaro/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/pyfibaro/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/pyfibaro/common/rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/pyfibaro/fibaro_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18832 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/pyfibaro/fibaro_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/pyfibaro/fibaro_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/pyfibaro/fibaro_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/pyfibaro/fibaro_room.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/pyfibaro/fibaro_scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/pyfibaro/fibaro_state_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/pyfibaro/fibaro_state_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:58:27.369295 pyfibaro-0.7.8/pyfibaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-24 19:58:27.000000 pyfibaro-0.7.8/pyfibaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-24 19:58:27.000000 pyfibaro-0.7.8/pyfibaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:58:27.000000 pyfibaro-0.7.8/pyfibaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 19:58:27.000000 pyfibaro-0.7.8/pyfibaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 19:58:27.000000 pyfibaro-0.7.8/pyfibaro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-24 19:58:27.373295 pyfibaro-0.7.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:58:27.369295 pyfibaro-0.7.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11151 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/tests/test_fibaro_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/tests/test_fibaro_device_armed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/tests/test_fibaro_device_hc3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/tests/test_fibaro_device_scene_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/tests/test_fibaro_device_scene_support_hc3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/tests/test_fibaro_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/tests/test_fibaro_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/tests/test_fibaro_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/tests/test_fibaro_room.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/tests/test_fibaro_scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/tests/test_fibaro_scene_hc3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/tests/test_fibaro_state_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/tests/test_rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-24 19:58:12.000000 pyfibaro-0.7.8/tests/test_utils.py
```

### Comparing `pyfibaro-0.7.7/LICENSE` & `pyfibaro-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.7/PKG-INFO` & `pyfibaro-0.7.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfibaro
-Version: 0.7.7
+Version: 0.7.8
 Summary: Simple API to access fibaro home center from any Python 3 script. Designed for Home Assistant (but not only)
 Home-page: https://github.com/rappenze/pyfibaro
 Author: Roman Appenzeller
 Author-email: 
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyfibaro-0.7.7/README.md` & `pyfibaro-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.7/pyfibaro/common/const.py` & `pyfibaro-0.7.8/pyfibaro/common/const.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.7/pyfibaro/common/rest_client.py` & `pyfibaro-0.7.8/pyfibaro/common/rest_client.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.7/pyfibaro/fibaro_client.py` & `pyfibaro-0.7.8/pyfibaro/fibaro_client.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.7/pyfibaro/fibaro_device.py` & `pyfibaro-0.7.8/pyfibaro/fibaro_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -512,15 +512,15 @@
     @property
     def has_color(self) -> bool:
         """Returns true if the device has a value property."""
         if self._property_name in self._properties:
             try:
                 self.rgbw_color
                 return True
-            except TypeError:
+            except (TypeError, ValueError):
                 return False
         return False
 
     @property
     def rgbw_color(self) -> tuple[int, int, int, int]:
         """Returns the color as RGBW value.
         For RGB devices the white value is reported as 0.
```

### Comparing `pyfibaro-0.7.7/pyfibaro/fibaro_info.py` & `pyfibaro-0.7.8/pyfibaro/fibaro_info.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.7/pyfibaro/fibaro_room.py` & `pyfibaro-0.7.8/pyfibaro/fibaro_room.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.7/pyfibaro/fibaro_scene.py` & `pyfibaro-0.7.8/pyfibaro/fibaro_scene.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.7/pyfibaro/fibaro_state_handler.py` & `pyfibaro-0.7.8/pyfibaro/fibaro_state_handler.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.7/pyfibaro/fibaro_state_resolver.py` & `pyfibaro-0.7.8/pyfibaro/fibaro_state_resolver.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.7/pyfibaro.egg-info/PKG-INFO` & `pyfibaro-0.7.8/pyfibaro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfibaro
-Version: 0.7.7
+Version: 0.7.8
 Summary: Simple API to access fibaro home center from any Python 3 script. Designed for Home Assistant (but not only)
 Home-page: https://github.com/rappenze/pyfibaro
 Author: Roman Appenzeller
 Author-email: 
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyfibaro-0.7.7/pyfibaro.egg-info/SOURCES.txt` & `pyfibaro-0.7.8/pyfibaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.7/setup.cfg` & `pyfibaro-0.7.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyfibaro
-version = 0.7.7
+version = 0.7.8
 description = Simple API to access fibaro home center from any Python 3 script. Designed for Home Assistant (but not only)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/rappenze/pyfibaro
 author = Roman Appenzeller
 author_email = 
 license = MIT
```

### Comparing `pyfibaro-0.7.7/tests/test_fibaro_device.py` & `pyfibaro-0.7.8/tests/test_fibaro_device.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.7/tests/test_fibaro_device_armed.py` & `pyfibaro-0.7.8/tests/test_fibaro_device_armed.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.7/tests/test_fibaro_device_hc3.py` & `pyfibaro-0.7.8/tests/test_fibaro_device_hc3.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.7/tests/test_fibaro_device_scene_support.py` & `pyfibaro-0.7.8/tests/test_fibaro_device_scene_support.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.7/tests/test_fibaro_device_scene_support_hc3.py` & `pyfibaro-0.7.8/tests/test_fibaro_device_scene_support_hc3.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.7/tests/test_fibaro_info.py` & `pyfibaro-0.7.8/tests/test_fibaro_info.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.7/tests/test_fibaro_login.py` & `pyfibaro-0.7.8/tests/test_fibaro_login.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.7/tests/test_fibaro_refresh.py` & `pyfibaro-0.7.8/tests/test_fibaro_refresh.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.7/tests/test_fibaro_room.py` & `pyfibaro-0.7.8/tests/test_fibaro_room.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.7/tests/test_fibaro_scene.py` & `pyfibaro-0.7.8/tests/test_fibaro_scene.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.7/tests/test_fibaro_scene_hc3.py` & `pyfibaro-0.7.8/tests/test_fibaro_scene_hc3.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.7/tests/test_fibaro_state_resolver.py` & `pyfibaro-0.7.8/tests/test_fibaro_state_resolver.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.7/tests/test_rest_client.py` & `pyfibaro-0.7.8/tests/test_rest_client.py`

 * *Files identical despite different names*

