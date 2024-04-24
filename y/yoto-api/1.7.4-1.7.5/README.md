# Comparing `tmp/yoto_api-1.7.4.tar.gz` & `tmp/yoto_api-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoto_api-1.7.4.tar", last modified: Tue Apr 23 16:16:54 2024, max compression
+gzip compressed data, was "yoto_api-1.7.5.tar", last modified: Wed Apr 24 13:32:47 2024, max compression
```

## Comparing `yoto_api-1.7.4.tar` & `yoto_api-1.7.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:54.806393 yoto_api-1.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-23 16:16:25.000000 yoto_api-1.7.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-23 16:16:25.000000 yoto_api-1.7.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 16:16:25.000000 yoto_api-1.7.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 16:16:25.000000 yoto_api-1.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 16:16:25.000000 yoto_api-1.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-23 16:16:54.806393 yoto_api-1.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-23 16:16:25.000000 yoto_api-1.7.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 16:16:25.000000 yoto_api-1.7.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:16:54.806393 yoto_api-1.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-23 16:16:46.000000 yoto_api-1.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:54.806393 yoto_api-1.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:25.000000 yoto_api-1.7.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-23 16:16:25.000000 yoto_api-1.7.4/tests/login_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:54.806393 yoto_api-1.7.4/yoto_api/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-23 16:16:25.000000 yoto_api-1.7.4/yoto_api/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-23 16:16:25.000000 yoto_api-1.7.4/yoto_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)    27735 2024-04-23 16:16:25.000000 yoto_api-1.7.4/yoto_api/YotoAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-23 16:16:25.000000 yoto_api-1.7.4/yoto_api/YotoManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-23 16:16:25.000000 yoto_api-1.7.4/yoto_api/YotoPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-23 16:16:25.000000 yoto_api-1.7.4/yoto_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-23 16:16:25.000000 yoto_api-1.7.4/yoto_api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:16:54.806393 yoto_api-1.7.4/yoto_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-23 16:16:54.000000 yoto_api-1.7.4/yoto_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-23 16:16:54.000000 yoto_api-1.7.4/yoto_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:16:54.000000 yoto_api-1.7.4/yoto_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:16:54.000000 yoto_api-1.7.4/yoto_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 16:16:54.000000 yoto_api-1.7.4/yoto_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 16:16:54.000000 yoto_api-1.7.4/yoto_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:32:47.917886 yoto_api-1.7.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-24 13:32:23.000000 yoto_api-1.7.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-24 13:32:23.000000 yoto_api-1.7.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 13:32:23.000000 yoto_api-1.7.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 13:32:23.000000 yoto_api-1.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-24 13:32:23.000000 yoto_api-1.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-24 13:32:47.913886 yoto_api-1.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-24 13:32:23.000000 yoto_api-1.7.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 13:32:23.000000 yoto_api-1.7.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:32:47.917886 yoto_api-1.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-24 13:32:39.000000 yoto_api-1.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:32:47.913886 yoto_api-1.7.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:32:23.000000 yoto_api-1.7.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-24 13:32:23.000000 yoto_api-1.7.5/tests/login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:32:47.913886 yoto_api-1.7.5/yoto_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-24 13:32:23.000000 yoto_api-1.7.5/yoto_api/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-24 13:32:23.000000 yoto_api-1.7.5/yoto_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27737 2024-04-24 13:32:23.000000 yoto_api-1.7.5/yoto_api/YotoAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-24 13:32:23.000000 yoto_api-1.7.5/yoto_api/YotoManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-24 13:32:23.000000 yoto_api-1.7.5/yoto_api/YotoPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-24 13:32:23.000000 yoto_api-1.7.5/yoto_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-24 13:32:23.000000 yoto_api-1.7.5/yoto_api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:32:47.913886 yoto_api-1.7.5/yoto_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-24 13:32:47.000000 yoto_api-1.7.5/yoto_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-24 13:32:47.000000 yoto_api-1.7.5/yoto_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:32:47.000000 yoto_api-1.7.5/yoto_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:32:47.000000 yoto_api-1.7.5/yoto_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 13:32:47.000000 yoto_api-1.7.5/yoto_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 13:32:47.000000 yoto_api-1.7.5/yoto_api.egg-info/top_level.txt
```

### Comparing `yoto_api-1.7.4/CONTRIBUTING.rst` & `yoto_api-1.7.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.4/LICENSE` & `yoto_api-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.4/PKG-INFO` & `yoto_api-1.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.7.4
+Version: 1.7.5
 Summary: A python package that makes it a bit easier to work with the yoto play API. Not associated with Yoto in any way.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `yoto_api-1.7.4/README.rst` & `yoto_api-1.7.5/README.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.4/setup.py` & `yoto_api-1.7.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="yoto_api",
     name="yoto_api",
     packages=find_packages(include=["yoto_api", "yoto_api.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/cdnninja/yoto_api",
-    version="1.7.4",
+    version="1.7.5",
     zip_safe=False,
 )
```

### Comparing `yoto_api-1.7.4/yoto_api/Card.py` & `yoto_api-1.7.5/yoto_api/Card.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.4/yoto_api/YotoAPI.py` & `yoto_api-1.7.5/yoto_api/YotoAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             )
             players[deviceId].playing_source = self.get_child_value(
                 player_status_response, "playingSource"
             )
             players[deviceId].night_light_mode = LIGHT_COLORS[
                 self.get_child_value(player_status_response, "nightlightMode")
             ]
-            players[deviceId].plugged_in = POWER_SOURCE[
+            players[deviceId].power_source = POWER_SOURCE[
                 self.get_child_value(player_status_response, "powerSource")
             ]
 
     def update_library(self, token: Token, library: dict[Card]) -> list[Card]:
         response = self._get_cards(token)
         for item in response["cards"]:
             if self.get_child_value(item, "cardId") not in library:
```

### Comparing `yoto_api-1.7.4/yoto_api/YotoManager.py` & `yoto_api-1.7.5/yoto_api/YotoManager.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.4/yoto_api/YotoPlayer.py` & `yoto_api-1.7.5/yoto_api/YotoPlayer.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     system_volume: int = None
     temperature_celcius: int = None
     bluetooth_audio_connected: bool = None
     charging: bool = None
     audio_device_connected: bool = None
     firmware_version: str = None
     wifi_strength: int = None
-    plugged_in: bool = None
+    power_source: str = None
 
 
 # {'devices': [{'deviceId': 'XXXX', 'name': 'Yoto Player', 'description': 'nameless.limit', 'online': False, 'releaseChannel': 'general', 'deviceType': 'v3', 'deviceFamily': 'v3', 'deviceGroup': '', 'hasUserGivenName': False}]}
 # Device Status API: {'activeCard': 'none', 'ambientLightSensorReading': 0, 'averageDownloadSpeedBytesSecond': 0, 'batteryLevelPercentage': 100, 'buzzErrors': 0, 'cardInsertionState': 2, 'dayMode': 0, 'deviceId': 'XXXX', 'errorsLogged': 210, 'firmwareVersion': 'v2.17.5', 'freeDiskSpaceBytes': 30250544, 'isAudioDeviceConnected': False, 'isBackgroundDownloadActive': False, 'isBluetoothAudioConnected': False, 'isCharging': False, 'isOnline': True, 'networkSsid': 'XXXX', 'nightlightMode': '0x000000', 'playingSource': 0, 'powerCapabilities': '0x02', 'powerSource': 2, 'systemVolumePercentage': 47, 'taskWatchdogTimeoutCount': 0, 'temperatureCelcius': '20', 'totalDiskSpaceBytes': 31385600, 'updatedAt': '2024-04-23T01:26:19.927Z', 'uptime': 252342, 'userVolumePercentage': 50, 'utcOffsetSeconds': -21600, 'utcTime': 1713835609, 'wifiStrength': -61}
 # Mqtt response:
 
 {
```

### Comparing `yoto_api-1.7.4/yoto_api.egg-info/PKG-INFO` & `yoto_api-1.7.5/yoto_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.7.4
+Version: 1.7.5
 Summary: A python package that makes it a bit easier to work with the yoto play API. Not associated with Yoto in any way.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

