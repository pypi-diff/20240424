# Comparing `tmp/albatros_uav-0.8.1.tar.gz` & `tmp/albatros_uav-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "albatros_uav-0.8.1.tar", max compression
+gzip compressed data, was "albatros_uav-0.9.0.tar", max compression
```

## Comparing `albatros_uav-0.8.1.tar` & `albatros_uav-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     7652 2023-08-30 09:54:43.073549 albatros_uav-0.8.1/LICENSE
--rwxr-xr-x   0        0        0     2071 2023-10-26 20:31:42.964678 albatros_uav-0.8.1/README.md
--rwxr-xr-x   0        0        0      214 2023-10-18 21:09:11.431841 albatros_uav-0.8.1/albatros/__init__.py
--rw-r--r--   0        0        0     7626 2024-02-10 19:03:12.468805 albatros_uav-0.8.1/albatros/copter.py
--rwxr-xr-x   0        0        0     3481 2024-02-10 15:51:13.269431 albatros_uav-0.8.1/albatros/enums.py
--rwxr-xr-x   0        0        0       89 2024-02-10 19:03:12.468805 albatros_uav-0.8.1/albatros/nav/__init__.py
--rwxr-xr-x   0        0        0     3319 2024-02-10 19:03:12.468805 albatros_uav-0.8.1/albatros/nav/position.py
--rwxr-xr-x   0        0        0     7413 2023-10-24 16:29:27.998850 albatros_uav-0.8.1/albatros/outgoing/commands.py
--rw-r--r--   0        0        0     2127 2023-10-18 22:16:08.200087 albatros_uav-0.8.1/albatros/outgoing/param_messages.py
--rw-r--r--   0        0        0    10549 2024-02-12 22:29:53.323071 albatros_uav-0.8.1/albatros/plane.py
--rwxr-xr-x   0        0        0      179 2023-10-18 21:58:12.387888 albatros_uav-0.8.1/albatros/setup_logging.py
--rw-r--r--   0        0        0       76 2023-10-18 21:09:11.435174 albatros_uav-0.8.1/albatros/telem/__init__.py
--rwxr-xr-x   0        0        0     3132 2024-02-07 19:16:08.443817 albatros_uav-0.8.1/albatros/telem/drivers.py
--rwxr-xr-x   0        0        0    18114 2024-02-12 22:29:53.323071 albatros_uav-0.8.1/albatros/telem/message_models.py
--rw-r--r--   0        0        0      380 2023-12-02 16:57:32.119195 albatros_uav-0.8.1/albatros/telem/models.py
--rwxr-xr-x   0        0        0      976 2024-02-07 19:16:08.443817 albatros_uav-0.8.1/albatros/telem/receive_loop.py
--rwxr-xr-x   0        0        0     3193 2024-02-12 22:29:53.323071 albatros_uav-0.8.1/albatros/telem/uav_data.py
--rwxr-xr-x   0        0        0    14121 2024-02-10 19:03:12.468805 albatros_uav-0.8.1/albatros/uav.py
--rwxr-xr-x   0        0        0     1656 2024-02-12 22:29:53.326405 albatros_uav-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     2981 1970-01-01 00:00:00.000000 albatros_uav-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-08-30 09:54:43.073549 albatros_uav-0.9.0/LICENSE
+-rwxr-xr-x   0        0        0     2071 2023-10-26 20:31:42.964678 albatros_uav-0.9.0/README.md
+-rwxr-xr-x   0        0        0      214 2023-10-18 21:09:11.431841 albatros_uav-0.9.0/albatros/__init__.py
+-rw-r--r--   0        0        0     9297 2024-04-24 21:42:46.315495 albatros_uav-0.9.0/albatros/copter.py
+-rwxr-xr-x   0        0        0     3481 2024-02-10 15:51:13.269431 albatros_uav-0.9.0/albatros/enums.py
+-rwxr-xr-x   0        0        0       89 2024-02-10 19:03:12.468805 albatros_uav-0.9.0/albatros/nav/__init__.py
+-rwxr-xr-x   0        0        0     3800 2024-04-24 21:42:46.315495 albatros_uav-0.9.0/albatros/nav/position.py
+-rwxr-xr-x   0        0        0     7413 2023-10-24 16:29:27.998850 albatros_uav-0.9.0/albatros/outgoing/commands.py
+-rw-r--r--   0        0        0     2127 2023-10-18 22:16:08.200087 albatros_uav-0.9.0/albatros/outgoing/param_messages.py
+-rw-r--r--   0        0        0    10549 2024-02-12 22:29:53.323071 albatros_uav-0.9.0/albatros/plane.py
+-rwxr-xr-x   0        0        0      179 2023-10-18 21:58:12.387888 albatros_uav-0.9.0/albatros/setup_logging.py
+-rw-r--r--   0        0        0       76 2023-10-18 21:09:11.435174 albatros_uav-0.9.0/albatros/telem/__init__.py
+-rwxr-xr-x   0        0        0     3132 2024-02-07 19:16:08.443817 albatros_uav-0.9.0/albatros/telem/drivers.py
+-rwxr-xr-x   0        0        0    18114 2024-02-12 22:29:53.323071 albatros_uav-0.9.0/albatros/telem/message_models.py
+-rw-r--r--   0        0        0      380 2023-12-02 16:57:32.119195 albatros_uav-0.9.0/albatros/telem/models.py
+-rwxr-xr-x   0        0        0      976 2024-02-07 19:16:08.443817 albatros_uav-0.9.0/albatros/telem/receive_loop.py
+-rwxr-xr-x   0        0        0     3193 2024-02-12 22:29:53.323071 albatros_uav-0.9.0/albatros/telem/uav_data.py
+-rwxr-xr-x   0        0        0    15084 2024-04-24 21:42:46.315495 albatros_uav-0.9.0/albatros/uav.py
+-rwxr-xr-x   0        0        0     1656 2024-04-24 21:43:01.200305 albatros_uav-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2981 1970-01-01 00:00:00.000000 albatros_uav-0.9.0/PKG-INFO
```

### Comparing `albatros_uav-0.8.1/LICENSE` & `albatros_uav-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.8.1/README.md` & `albatros_uav-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.8.1/albatros/copter.py` & `albatros_uav-0.9.0/albatros/copter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import time
 from typing import Optional
 
 from pymavlink.dialects.v20.ardupilotmega import (
     MAV_CMD_CONDITION_YAW,
     MAV_CMD_DO_SET_MODE,
     MAV_CMD_NAV_LAND,
     MAV_CMD_NAV_TAKEOFF,
@@ -12,14 +13,15 @@
 from albatros.enums import (
     CommandResult,
     ConnectionType,
     CopterFlightModes,
     Direction,
     MavFrame,
 )
+from albatros.nav.position import PositionGPS, convert_raw_path_to_gps
 from albatros.telem import ComponentAddress
 from albatros.telem.message_models import PositionTargetLocalNED
 from albatros.uav import UAV
 
 from .outgoing.commands import (
     get_command_long_message,
     get_set_position_target_local_ned_message,
@@ -260,7 +262,43 @@
             target = self.wait_message(PositionTargetLocalNED())
             if target.x == north_m and target.y == east_m:
                 return True
             return False
 
         except TimeoutError:
             return False
+
+    def fly_along_path_raw(
+        self,
+        raw_path: list[tuple[float, float, float]],
+        precision: float = 1.0,
+    ) -> None:
+        """This function will fly the copter along the given path of GPS positions.
+        The point is reached when the distance to the target is less than the precision.
+
+        Parameters:
+            raw_path: list of (lat, lon, alt) points to fly to in provided order.
+            precision: Minimal distance between copter and target to consider
+                the target as visited.  Defaults to 1.0.
+        """
+        flight_path = convert_raw_path_to_gps(raw_path)
+        self.fly_along_path(flight_path, precision)
+
+    def fly_along_path(
+        self, flight_path: list[PositionGPS], precision: float = 1.0
+    ) -> None:
+        """This function will fly the copter along the given path of GPS positions.
+        The point is reached when the distance to the target is less than the precision.
+
+        Parameters:
+            flight_path: list of PositionGPS points to fly to in provided order.
+            precision: Minimal distance between copter and target to consider the
+                target as visited. Defaults to 1.0.
+        """
+        for target in flight_path:
+            self.fly_to_gps_position(target.lat, target.lon, target.alt_m)
+            while (
+                distance := target.distance_to_point(self.get_corrected_position())
+            ) > precision:
+                logger.debug("distance to next point: %f", distance)
+                time.sleep(1)
+        self.set_mode(CopterFlightModes.RTL)
```

### Comparing `albatros_uav-0.8.1/albatros/enums.py` & `albatros_uav-0.9.0/albatros/enums.py`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.8.1/albatros/nav/position.py` & `albatros_uav-0.9.0/albatros/nav/position.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,7 +107,23 @@
         GEO coordinate of point
     """
     lat = (point.north / (40075704.0 / 360)) + reference_point.lat
     lon = (
         point.east / (math.cos(math.radians(reference_point.lat)) * (40075704.0 / 360))
     ) + reference_point.lon
     return PositionGPS(lat, lon, point.down)
+
+
+def convert_raw_path_to_gps(
+    raw_path: list[tuple[float, float, float]]
+) -> list[PositionGPS]:
+    """This function will convert the raw path of GPS positions to the list of PositionGPS format.
+
+    Args:
+        raw_path (list[tuple[float, float, flost]]): list of (lat, lon, alt) points.
+
+    Returns:
+        list[PositionGPS]: list of PositionGPS points.
+    """
+    return [
+        PositionGPS(raw_point[0], raw_point[1], raw_point[2]) for raw_point in raw_path
+    ]
```

### Comparing `albatros_uav-0.8.1/albatros/outgoing/commands.py` & `albatros_uav-0.9.0/albatros/outgoing/commands.py`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.8.1/albatros/outgoing/param_messages.py` & `albatros_uav-0.9.0/albatros/outgoing/param_messages.py`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.8.1/albatros/plane.py` & `albatros_uav-0.9.0/albatros/plane.py`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.8.1/albatros/telem/drivers.py` & `albatros_uav-0.9.0/albatros/telem/drivers.py`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.8.1/albatros/telem/message_models.py` & `albatros_uav-0.9.0/albatros/telem/message_models.py`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.8.1/albatros/telem/receive_loop.py` & `albatros_uav-0.9.0/albatros/telem/receive_loop.py`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.8.1/albatros/telem/uav_data.py` & `albatros_uav-0.9.0/albatros/telem/uav_data.py`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.8.1/albatros/uav.py` & `albatros_uav-0.9.0/albatros/uav.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     MAV_DATA_STREAM_RAW_CONTROLLER,
     MAV_DATA_STREAM_RAW_SENSORS,
     MAV_DATA_STREAM_RC_CHANNELS,
     MAV_MODE_FLAG_SAFETY_ARMED,
     MAVLINK_MSG_ID_HOME_POSITION,
     MAVLink_encapsulated_data_message,
     MAVLink_message,
+    MAVLink_play_tune_message,
     MAVLink_request_data_stream_message,
 )
 
 from albatros.enums import ConnectionType
 from albatros.telem import ComponentAddress
 from albatros.telem.drivers import (
     DirectConnectionDriver,
@@ -383,15 +384,15 @@
 
         Parameters:
             msg: raw MAVLink messae to send.
         """
         self._driver.send(msg)
 
     def send_encapsulated_data(self, data: bytes, seq: int = 0) -> None:
-        """Send encapsulated data to boradcast.
+        """Send encapsulated data to broadcast.
 
         Parameters:
             data: data bytes.
             seq: sequence number (starting with 0 on every transmission).
         """
 
         data_size_bytes = len(data)
@@ -419,7 +420,33 @@
         Returns:
             distance to next waypoint in meters.
 
         Raises:
             `TimeoutError`: if the response time is exceeded.
         """
         return self.wait_message(NavControllerOutput()).wp_dist
+
+    def play_tune(self, tune: str, tune2: str = "") -> bool:
+        """Play a tune on the UAV. Tunes have to be in the MML format
+
+        Args:
+            tune (str): The first tune to be played, limited to 30 characters.
+            tune2 (str): The second tune to be played, limited to 230 characters. Defaults to an empty string.
+
+        Returns:
+            bool: True if the tune was played successfully, False otherwise.
+        """
+        if len(tune) > 30 or len(tune2) > 230:
+            logger.error("Tune too long")
+            return False
+
+        msg = MAVLink_play_tune_message(
+            target_system=self._uav_addr.system_id,
+            target_component=self._uav_addr.component_id,
+            tune=tune.encode("ascii"),
+            tune2=tune2.encode("ascii"),
+        )
+        self.send_raw_mavlink_message(msg)
+
+        self._driver.send(msg)
+        logger.debug("Tune played.")
+        return True
```

### Comparing `albatros_uav-0.8.1/pyproject.toml` & `albatros_uav-0.9.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "albatros-uav"
-version = "0.8.1"
+version = "0.9.0"
 description = "The tool for managing unmanned aerial vehicles missions."
 authors = ["Jędrzej Stasik <jedrzej.stasik@gmail.com>"]
 license = "LGPL-3.0-only"
 readme = "README.md"
 packages = [{include = "albatros"}]
 repository = "https://gitlab.com/albatros-uav/albatros"
 documentation = "https://albatros-uav.gitlab.io/albatros/"
```

### Comparing `albatros_uav-0.8.1/PKG-INFO` & `albatros_uav-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albatros-uav
-Version: 0.8.1
+Version: 0.9.0
 Summary: The tool for managing unmanned aerial vehicles missions.
 Home-page: https://gitlab.com/albatros-uav/albatros
 License: LGPL-3.0-only
 Author: Jędrzej Stasik
 Author-email: jedrzej.stasik@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

