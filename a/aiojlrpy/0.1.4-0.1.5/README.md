# Comparing `tmp/aiojlrpy-0.1.4.tar.gz` & `tmp/aiojlrpy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiojlrpy-0.1.4.tar", last modified: Mon Apr 22 18:30:52 2024, max compression
+gzip compressed data, was "aiojlrpy-0.1.5.tar", last modified: Wed Apr 24 10:32:14 2024, max compression
```

## Comparing `aiojlrpy-0.1.4.tar` & `aiojlrpy-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:30:52.805213 aiojlrpy-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-22 18:30:48.000000 aiojlrpy-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-04-22 18:30:52.805213 aiojlrpy-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-22 18:30:48.000000 aiojlrpy-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:30:52.801213 aiojlrpy-0.1.4/aiojlrpy/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-22 18:30:48.000000 aiojlrpy-0.1.4/aiojlrpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11483 2024-04-22 18:30:48.000000 aiojlrpy-0.1.4/aiojlrpy/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-22 18:30:48.000000 aiojlrpy-0.1.4/aiojlrpy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-22 18:30:48.000000 aiojlrpy-0.1.4/aiojlrpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-04-22 18:30:48.000000 aiojlrpy-0.1.4/aiojlrpy/stomp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-22 18:30:48.000000 aiojlrpy-0.1.4/aiojlrpy/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21209 2024-04-22 18:30:48.000000 aiojlrpy-0.1.4/aiojlrpy/vehicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-04-22 18:30:48.000000 aiojlrpy-0.1.4/aiojlrpy/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:30:52.805213 aiojlrpy-0.1.4/aiojlrpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-04-22 18:30:52.000000 aiojlrpy-0.1.4/aiojlrpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-22 18:30:52.000000 aiojlrpy-0.1.4/aiojlrpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 18:30:52.000000 aiojlrpy-0.1.4/aiojlrpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-22 18:30:52.000000 aiojlrpy-0.1.4/aiojlrpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-22 18:30:52.000000 aiojlrpy-0.1.4/aiojlrpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-22 18:30:52.805213 aiojlrpy-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-22 18:30:48.000000 aiojlrpy-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:13.994371 aiojlrpy-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-24 10:32:06.000000 aiojlrpy-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-04-24 10:32:13.994371 aiojlrpy-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-24 10:32:06.000000 aiojlrpy-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:13.994371 aiojlrpy-0.1.5/aiojlrpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-24 10:32:06.000000 aiojlrpy-0.1.5/aiojlrpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11386 2024-04-24 10:32:06.000000 aiojlrpy-0.1.5/aiojlrpy/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-24 10:32:06.000000 aiojlrpy-0.1.5/aiojlrpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-24 10:32:06.000000 aiojlrpy-0.1.5/aiojlrpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-04-24 10:32:06.000000 aiojlrpy-0.1.5/aiojlrpy/stomp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-24 10:32:06.000000 aiojlrpy-0.1.5/aiojlrpy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21181 2024-04-24 10:32:06.000000 aiojlrpy-0.1.5/aiojlrpy/vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-04-24 10:32:06.000000 aiojlrpy-0.1.5/aiojlrpy/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:13.994371 aiojlrpy-0.1.5/aiojlrpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-04-24 10:32:13.000000 aiojlrpy-0.1.5/aiojlrpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-24 10:32:13.000000 aiojlrpy-0.1.5/aiojlrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:32:13.000000 aiojlrpy-0.1.5/aiojlrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 10:32:13.000000 aiojlrpy-0.1.5/aiojlrpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 10:32:13.000000 aiojlrpy-0.1.5/aiojlrpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 10:32:13.994371 aiojlrpy-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-24 10:32:06.000000 aiojlrpy-0.1.5/setup.py
```

### Comparing `aiojlrpy-0.1.4/LICENSE` & `aiojlrpy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiojlrpy-0.1.4/PKG-INFO` & `aiojlrpy-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiojlrpy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Async Library for JLRIncontrol
 Home-page: https://github.com/msp1974/aiojlrpy
 Author: msp1974
 Author-email: msparker@sky.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `aiojlrpy-0.1.4/README.md` & `aiojlrpy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `aiojlrpy-0.1.4/aiojlrpy/__init__.py` & `aiojlrpy-0.1.5/aiojlrpy/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Async python library to access to JLR InControl Services
 https://github.com/msp1974/aiojlrpy
 """
 
-__VERSION__ = "0.1.4"
+__VERSION__ = "0.1.5"
 
 from typing import Tuple
 
 from .connection import Connection
 from .const import JLRServices
 from .vehicle import Vehicle
 from .stomp import StatusMessage, STOMPCommands
```

### Comparing `aiojlrpy-0.1.4/aiojlrpy/connection.py` & `aiojlrpy-0.1.5/aiojlrpy/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,19 +164,16 @@
         }
         result = await self._request(url, headers, data, "POST")
         logger.debug(result)
 
     async def _login_user(self) -> dict:
         """Login the user"""
         url = f"{self.base.IF9}/users?loginName={self.email}"
-        headers = {
-            "Accept": HttpAccepts.USER,
-            "x-App-Id": "ICR_LAND_ROVER",
-            "x-App-Secret": "018dd169-94b7-7cb6-8f7f-c263c91f1121",
-        }
+        headers = self.headers.copy()
+        headers["Accept"] = HttpAccepts.USER
         user_data = await self._request(url, headers)
         logger.debug(user_data)
         self.user_id = user_data["userId"]
         return user_data
 
     # Websocket functions
```

### Comparing `aiojlrpy-0.1.4/aiojlrpy/const.py` & `aiojlrpy-0.1.5/aiojlrpy/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Constants to support aiojlrpy"""
+
 from enum import StrEnum
 
 TIMEOUT = 15
 
 
 class BaseURLs:
     """Rest Of World Base URLs"""
@@ -69,12 +70,11 @@
 class HTTPContentType(StrEnum):
     """Content-Type strings for headers"""
 
     JSON = "application/json"
     AUTH_REQUEST = "application/vnd.wirelesscar.ngtp.if9.AuthenticateRequest-v2+json; charset=utf-8"
     NOTIFICATION_TARGETS = "application/vnd.wirelesscar.ngtp.if9.NotificationTargets-v2+json"
     PHEV_SERVICE = "application/vnd.wirelesscar.ngtp.if9.PhevService-v1+json; charset=utf-8"
-    SERVICE_CONFIG_V2 = "application/vnd.wirelesscar.ngtp.if9.StartServiceConfiguration-v2+json"
-    SERVICE_CONFIG_V3 = (
+    SERVICE_CONFIG = (
         "application/vnd.wirelesscar.ngtp.if9.StartServiceConfiguration-v3+json; charset=utf-8"
     )
     USER = "application/vnd.wirelesscar.ngtp.if9.User-v3+json; charset=utf-8"
```

### Comparing `aiojlrpy-0.1.4/aiojlrpy/stomp.py` & `aiojlrpy-0.1.5/aiojlrpy/stomp.py`

 * *Files identical despite different names*

### Comparing `aiojlrpy-0.1.4/aiojlrpy/utils.py` & `aiojlrpy-0.1.5/aiojlrpy/utils.py`

 * *Files identical despite different names*

### Comparing `aiojlrpy-0.1.4/aiojlrpy/vehicle.py` & `aiojlrpy-0.1.5/aiojlrpy/vehicle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Class to represent a JLR vehicle"""
 
-
 from datetime import datetime, timedelta
 import logging
 import uuid
 from aiojlrpy.const import (
     ALERNATE_SERVICE_ID,
     NON_NOTIFICATION_SERVICES,
     HTTPContentType,
@@ -239,15 +238,15 @@
         }
         return await self._post("attributes", data=attributes_data)
 
     async def request_vehicle_health_status_update(self) -> dict | None:
         """Get vehicle health status from vehicle"""
         headers = {
             "Accept": HttpAccepts.SERVICE_STATUS_V4,
-            "Content-Type": HTTPContentType.SERVICE_CONFIG_V3,
+            "Content-Type": HTTPContentType.SERVICE_CONFIG,
         }
         vhs_data = await self._authenticate_service("", JLRServices.VEHICLE_HEALTH)
         return await self._post("healthstatus", headers, vhs_data)
 
     async def set_max_soc(self, max_charge_level):
         """Set max state of charge in percentage"""
         service_parameters = [{"key": "SET_PERMANENT_MAX_SOC", "value": max_charge_level}]
@@ -344,23 +343,23 @@
         """Enable transport mode. Will be disabled at the specified time (epoch millis)"""
         return await self._prov_command(pin, expiration_time, "protectionStrategy_transportMode")
 
     async def honk_blink(self):
         """Sound the horn and blink lights"""
         headers = {
             "Accept": HttpAccepts.SERVICE_STATUS_V4,
-            "Content-Type": HTTPContentType.SERVICE_CONFIG_V3,
+            "Content-Type": HTTPContentType.SERVICE_CONFIG,
         }
         # Authenticates using last 4 digits of vin as pin
         hblf_data = await self._authenticate_service(self.vin[-4:], JLRServices.HONK_BLINK)
         return await self._post("honkBlink", headers, hblf_data)
 
     async def lock(self, pin: str):
         """Lock vehicle. Requires personal PIN for authentication"""
-        headers = {"Content-Type": HTTPContentType.SERVICE_CONFIG_V3}
+        headers = {"Content-Type": HTTPContentType.SERVICE_CONFIG}
         rdl_data = await self._authenticate_service(pin, JLRServices.REMOTE_DOOR_LOCK)
         return await self._post("lock", headers, rdl_data)
 
     async def preconditioning_start(self, target_temp: int):
         """Start pre-conditioning for specified temperature (celsius)"""
         service_parameters = [
             {"key": "PRECONDITIONING", "value": "START"},
@@ -371,38 +370,38 @@
     async def preconditioning_stop(self):
         """Stop climate preconditioning"""
         service_parameters = [{"key": "PRECONDITIONING", "value": "STOP"}]
         return await self._preconditioning_control_command(service_parameters)
 
     async def remote_engine_start(self, pin: str, target_value: int):
         """Start Remote Engine preconditioning"""
-        headers = {"Content-Type": HTTPContentType.SERVICE_CONFIG_V2}
+        headers = {"Content-Type": HTTPContentType.SERVICE_CONFIG}
         await self.set_rcc_target_value(pin, target_value)
         reon_data = await self._authenticate_service(pin, JLRServices.REMOTE_ENGINE_ON)
         return await self._post("engineOn", headers, reon_data)
 
     async def remote_engine_stop(self, pin: str):
         """Stop Remote Engine preconditioning"""
-        headers = {"Content-Type": HTTPContentType.SERVICE_CONFIG_V2}
+        headers = {"Content-Type": HTTPContentType.SERVICE_CONFIG}
         reoff_data = await self._authenticate_service(pin, JLRServices.REMOTE_ENGINE_OFF)
 
         return await self._post("engineOff", headers, reoff_data)
 
     async def reset_alarm(self, pin: str):
         """Reset vehicle alarm"""
         headers = {
-            "Content-Type": HTTPContentType.SERVICE_CONFIG_V3,
+            "Content-Type": HTTPContentType.SERVICE_CONFIG,
             "Accept": HttpAccepts.SERVICE_STATUS_V4,
         }
         aloff_data = await self._authenticate_service(pin, JLRServices.ALARM_OFF)
         return await self._post("unlock", headers, aloff_data)
 
     async def unlock(self, pin: str):
         """Unlock vehicle. Requires personal PIN for authentication"""
-        headers = {"Content-Type": HTTPContentType.SERVICE_CONFIG_V3}
+        headers = {"Content-Type": HTTPContentType.SERVICE_CONFIG}
         rdu_data = await self._authenticate_service(pin, JLRServices.REMOTE_DOOR_UNLOCK)
         return await self._post("unlock", headers, rdu_data)
 
     # Internal helper functions
 
     async def _charging_profile_control_command(
         self, service_parameter_key: str, service_parameters: list
@@ -440,24 +439,24 @@
             self.vin[-4:], JLRServices.ELECTRIC_CLIMATE_CONTROL
         )
         ecc_data["serviceParameters"] = service_parameters
         return await self._post("preconditioning", headers, ecc_data)
 
     async def _prov_command(self, pin: str, expiration_time: int, mode: str):
         """Send prov endpoint commands. Used for service/transport/privacy mode"""
-        headers = {"Content-Type": HTTPContentType.SERVICE_CONFIG_V3}
+        headers = {"Content-Type": HTTPContentType.SERVICE_CONFIG}
         prov_data = await self._authenticate_service(pin, JLRServices.PROVISIONING_MODE)
         prov_data.update({"serviceCommand": mode, "startTime": None, "endTime": expiration_time})
         return await self._post("prov", headers, prov_data)
 
     async def _wakeup_timer_command(self, swu_data: dict):
         """Set the wakeup time for the specified time (epoch milliseconds)"""
         headers = {
             "Accept": HttpAccepts.SERVICE_STATUS_V4,
-            "Content-Type": HTTPContentType.SERVICE_CONFIG_V3,
+            "Content-Type": HTTPContentType.SERVICE_CONFIG,
         }
         return await self._post("swu", headers, swu_data)
 
     async def _authenticate_service(self, pin: str, service_name: str):
         """Authenticate to specified service with the provided PIN"""
         headers = {"Content-Type": HTTPContentType.AUTH_REQUEST}
         data = {"serviceName": service_name, "pin": str(pin)}
```

### Comparing `aiojlrpy-0.1.4/aiojlrpy/websocket.py` & `aiojlrpy-0.1.5/aiojlrpy/websocket.py`

 * *Files identical despite different names*

### Comparing `aiojlrpy-0.1.4/aiojlrpy.egg-info/PKG-INFO` & `aiojlrpy-0.1.5/aiojlrpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiojlrpy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Async Library for JLRIncontrol
 Home-page: https://github.com/msp1974/aiojlrpy
 Author: msp1974
 Author-email: msparker@sky.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `aiojlrpy-0.1.4/setup.py` & `aiojlrpy-0.1.5/setup.py`

 * *Files identical despite different names*

