# Comparing `tmp/yoto_api-1.7.3.tar.gz` & `tmp/yoto_api-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoto_api-1.7.3.tar", last modified: Tue Apr 23 16:06:58 2024, max compression
+gzip compressed data, was "yoto_api-1.7.4.tar", last modified: Tue Apr 23 16:16:54 2024, max compression
```

## Comparing `yoto_api-1.7.3.tar` & `yoto_api-1.7.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:06:58.798578 yoto_api-1.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-23 16:06:15.000000 yoto_api-1.7.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-23 16:06:15.000000 yoto_api-1.7.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 16:06:15.000000 yoto_api-1.7.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 16:06:15.000000 yoto_api-1.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 16:06:15.000000 yoto_api-1.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-23 16:06:58.798578 yoto_api-1.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-23 16:06:15.000000 yoto_api-1.7.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 16:06:15.000000 yoto_api-1.7.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:06:58.798578 yoto_api-1.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-23 16:06:46.000000 yoto_api-1.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:06:58.794578 yoto_api-1.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:06:15.000000 yoto_api-1.7.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-23 16:06:15.000000 yoto_api-1.7.3/tests/login_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:06:58.798578 yoto_api-1.7.3/yoto_api/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-23 16:06:15.000000 yoto_api-1.7.3/yoto_api/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-23 16:06:15.000000 yoto_api-1.7.3/yoto_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)    27737 2024-04-23 16:06:15.000000 yoto_api-1.7.3/yoto_api/YotoAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-23 16:06:15.000000 yoto_api-1.7.3/yoto_api/YotoManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-23 16:06:15.000000 yoto_api-1.7.3/yoto_api/YotoPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-23 16:06:15.000000 yoto_api-1.7.3/yoto_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-23 16:06:15.000000 yoto_api-1.7.3/yoto_api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:06:58.798578 yoto_api-1.7.3/yoto_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-23 16:06:58.000000 yoto_api-1.7.3/yoto_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-23 16:06:58.000000 yoto_api-1.7.3/yoto_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:06:58.000000 yoto_api-1.7.3/yoto_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:06:58.000000 yoto_api-1.7.3/yoto_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 16:06:58.000000 yoto_api-1.7.3/yoto_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 16:06:58.000000 yoto_api-1.7.3/yoto_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:54.806393 yoto_api-1.7.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-23 16:16:25.000000 yoto_api-1.7.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-23 16:16:25.000000 yoto_api-1.7.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 16:16:25.000000 yoto_api-1.7.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 16:16:25.000000 yoto_api-1.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 16:16:25.000000 yoto_api-1.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-23 16:16:54.806393 yoto_api-1.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-23 16:16:25.000000 yoto_api-1.7.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 16:16:25.000000 yoto_api-1.7.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:16:54.806393 yoto_api-1.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-23 16:16:46.000000 yoto_api-1.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:54.806393 yoto_api-1.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:25.000000 yoto_api-1.7.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-23 16:16:25.000000 yoto_api-1.7.4/tests/login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:54.806393 yoto_api-1.7.4/yoto_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-23 16:16:25.000000 yoto_api-1.7.4/yoto_api/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-23 16:16:25.000000 yoto_api-1.7.4/yoto_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27735 2024-04-23 16:16:25.000000 yoto_api-1.7.4/yoto_api/YotoAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-23 16:16:25.000000 yoto_api-1.7.4/yoto_api/YotoManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-23 16:16:25.000000 yoto_api-1.7.4/yoto_api/YotoPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-23 16:16:25.000000 yoto_api-1.7.4/yoto_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-23 16:16:25.000000 yoto_api-1.7.4/yoto_api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:54.806393 yoto_api-1.7.4/yoto_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-23 16:16:54.000000 yoto_api-1.7.4/yoto_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-23 16:16:54.000000 yoto_api-1.7.4/yoto_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:16:54.000000 yoto_api-1.7.4/yoto_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:16:54.000000 yoto_api-1.7.4/yoto_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 16:16:54.000000 yoto_api-1.7.4/yoto_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 16:16:54.000000 yoto_api-1.7.4/yoto_api.egg-info/top_level.txt
```

### Comparing `yoto_api-1.7.3/CONTRIBUTING.rst` & `yoto_api-1.7.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.3/LICENSE` & `yoto_api-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.3/PKG-INFO` & `yoto_api-1.7.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.7.3
-Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
+Version: 1.7.4
+Summary: A python package that makes it a bit easier to work with the yoto play API. Not associated with Yoto in any way.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `yoto_api-1.7.3/README.rst` & `yoto_api-1.7.4/README.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.3/setup.py` & `yoto_api-1.7.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,21 +27,21 @@
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.9",
     ],
-    description="Python Boilerplate contains all the boilerplate you need to create a Python package.",
+    description="A python package that makes it a bit easier to work with the yoto play API. Not associated with Yoto in any way.",
     install_requires=requirements,
     license="MIT license",
     long_description=long_description,
     include_package_data=True,
     keywords="yoto_api",
     name="yoto_api",
     packages=find_packages(include=["yoto_api", "yoto_api.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/cdnninja/yoto_api",
-    version="1.7.3",
+    version="1.7.4",
     zip_safe=False,
 )
```

### Comparing `yoto_api-1.7.3/yoto_api/Card.py` & `yoto_api-1.7.4/yoto_api/Card.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.3/yoto_api/YotoAPI.py` & `yoto_api-1.7.4/yoto_api/YotoAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             )
             players[deviceId].ambient_light_sensor_reading = self.get_child_value(
                 player_status_response, "ambientLightSensorReading"
             )
             players[deviceId].battery_level_percentage = self.get_child_value(
                 player_status_response, "batteryLevelPercentage"
             )
-            players[deviceId].night_mode_on = self.get_child_value(
+            players[deviceId].day_mode_on = self.get_child_value(
                 player_status_response, "dayMode"
             )
             players[deviceId].user_volume = self.get_child_value(
                 player_status_response, "userVolumePercentage"
             )
             players[deviceId].system_volume = self.get_child_value(
                 player_status_response, "systemVolumePercentage"
```

### Comparing `yoto_api-1.7.3/yoto_api/YotoManager.py` & `yoto_api-1.7.4/yoto_api/YotoManager.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.3/yoto_api/YotoPlayer.py` & `yoto_api-1.7.4/yoto_api/YotoPlayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     # Status API
     active_card: str = None
     is_playing: bool = None
     playing_source: str = None
     ambient_light_sensor_reading: int = None
     battery_level_percentage: int = None
-    night_mode_on: bool = None
+    day_mode_on: bool = None
     night_light_mode: str = None
     user_volume: int = None
     system_volume: int = None
     temperature_celcius: int = None
     bluetooth_audio_connected: bool = None
     charging: bool = None
     audio_device_connected: bool = None
```

### Comparing `yoto_api-1.7.3/yoto_api.egg-info/PKG-INFO` & `yoto_api-1.7.4/yoto_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.7.3
-Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
+Version: 1.7.4
+Summary: A python package that makes it a bit easier to work with the yoto play API. Not associated with Yoto in any way.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

