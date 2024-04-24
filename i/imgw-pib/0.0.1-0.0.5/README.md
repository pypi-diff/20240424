# Comparing `tmp/imgw_pib-0.0.1.tar.gz` & `tmp/imgw_pib-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgw_pib-0.0.1.tar", last modified: Mon Apr 22 11:01:33 2024, max compression
+gzip compressed data, was "imgw_pib-0.0.5.tar", last modified: Wed Apr 24 15:14:49 2024, max compression
```

## Comparing `imgw_pib-0.0.1.tar` & `imgw_pib-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:01:33.055903 imgw_pib-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-22 11:01:18.000000 imgw_pib-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-22 11:01:18.000000 imgw_pib-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-22 11:01:33.055903 imgw_pib-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-22 11:01:18.000000 imgw_pib-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:01:33.051903 imgw_pib-0.0.1/imgw_pib/
--rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-04-22 11:01:18.000000 imgw_pib-0.0.1/imgw_pib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-22 11:01:18.000000 imgw_pib-0.0.1/imgw_pib/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-22 11:01:18.000000 imgw_pib-0.0.1/imgw_pib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-22 11:01:18.000000 imgw_pib-0.0.1/imgw_pib/model.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:01:18.000000 imgw_pib-0.0.1/imgw_pib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:01:33.055903 imgw_pib-0.0.1/imgw_pib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-22 11:01:33.000000 imgw_pib-0.0.1/imgw_pib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-22 11:01:33.000000 imgw_pib-0.0.1/imgw_pib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 11:01:33.000000 imgw_pib-0.0.1/imgw_pib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-22 11:01:33.000000 imgw_pib-0.0.1/imgw_pib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-22 11:01:33.000000 imgw_pib-0.0.1/imgw_pib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-22 11:01:18.000000 imgw_pib-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-22 11:01:18.000000 imgw_pib-0.0.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-22 11:01:18.000000 imgw_pib-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 11:01:33.055903 imgw_pib-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-22 11:01:18.000000 imgw_pib-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:01:33.051903 imgw_pib-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-04-22 11:01:18.000000 imgw_pib-0.0.1/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:14:49.276187 imgw_pib-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-24 15:14:49.276187 imgw_pib-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:14:49.276187 imgw_pib-0.0.5/imgw_pib/
+-rw-r--r--   0 runner    (1001) docker     (127)     9918 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/imgw_pib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/imgw_pib/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/imgw_pib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/imgw_pib/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/imgw_pib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/imgw_pib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:14:49.276187 imgw_pib-0.0.5/imgw_pib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-24 15:14:49.000000 imgw_pib-0.0.5/imgw_pib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-24 15:14:49.000000 imgw_pib-0.0.5/imgw_pib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:14:49.000000 imgw_pib-0.0.5/imgw_pib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 15:14:49.000000 imgw_pib-0.0.5/imgw_pib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 15:14:49.000000 imgw_pib-0.0.5/imgw_pib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:14:49.276187 imgw_pib-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:14:49.276187 imgw_pib-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-04-24 15:14:38.000000 imgw_pib-0.0.5/tests/test_init.py
```

### Comparing `imgw_pib-0.0.1/LICENSE` & `imgw_pib-0.0.5/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2024 Maciej Bieniek
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `imgw_pib-0.0.1/PKG-INFO` & `imgw_pib-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgw_pib
-Version: 0.0.1
+Version: 0.0.5
 Summary: Python wrapper for IMGW-PIB API.
 Home-page: https://github.com/bieniu/imgw-pib
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `imgw_pib-0.0.1/README.md` & `imgw_pib-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `imgw_pib-0.0.1/imgw_pib/__init__.py` & `imgw_pib-0.0.5/imgw_pib/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,25 @@
 """Python wrapper for IMGW-PIB API."""
 
 import logging
-from datetime import UTC, datetime
 from http import HTTPStatus
 from typing import Any, Self
 
 from aiohttp import ClientSession
 
 from .const import (
-    API_HUMIDITY,
+    API_HYDROLOGICAL_DETAILS_ENDPOINT,
     API_HYDROLOGICAL_ENDPOINT,
-    API_MEASUREMENT_DATE,
-    API_MEASUREMENT_TIME,
-    API_PRECIPITATION,
-    API_PRESSURE,
-    API_RIVER,
-    API_STATION,
-    API_STATION_ID,
-    API_TEMPERATURE,
-    API_WATER_LEVEL,
-    API_WATER_LEVEL_MEASUREMENT_DATE,
-    API_WATER_TEMPERATURE,
-    API_WATER_TEMPERATURE_MEASUREMENT_DATE,
     API_WEATHER_ENDPOINT,
-    API_WIND_DIRECTION,
-    API_WIND_SPEED,
     HEADERS,
     TIMEOUT,
-    UNIT_CELSIUS,
-    UNIT_CENTIMETERS,
-    UNIT_DEGREE,
-    UNIT_HPA,
-    UNIT_METERS_PER_SECOND,
-    UNIT_MILLIMETERS,
-    UNIT_PERCENT,
 )
 from .exceptions import ApiError
-from .model import HydrologicalData, SensorData, WeatherData
+from .model import ApiNames, HydrologicalData, SensorData, Units, WeatherData
+from .utils import gen_station_name, get_datetime
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class ImgwPib:
     """Main class of IMGW-PIB API wrapper."""
 
@@ -50,14 +29,16 @@
         weather_station_id: str | None = None,
         hydrological_station_id: str | None = None,
     ) -> None:
         """Initialize IMGW-PIB API wrapper."""
         self._session = session
         self._weather_station_list: dict[str, str] = {}
         self._hydrological_station_list: dict[str, str] = {}
+        self._alarm_water_level: float | None = None
+        self._warning_water_level: float | None = None
 
         self.weather_station_id = weather_station_id
         self.hydrological_station_id = hydrological_station_id
 
     @classmethod
     async def create(
         cls: type[Self],
@@ -80,61 +61,84 @@
     def hydrological_stations(self: Self) -> dict[str, str]:
         """Return list of hydrological stations."""
         return self._hydrological_station_list
 
     async def initialize(self: Self) -> None:
         """Initialize."""
         _LOGGER.debug("Initializing IMGW-PIB")
-        self._weather_station_list = await self.get_weather_stations()
-        self._hydrological_station_list = await self.get_hydrological_stations()
 
-        if (
-            self.weather_station_id is not None
-            and self.weather_station_id not in self.weather_stations
-        ):
-            msg = f"Invalid weather station ID: {self.weather_station_id}"
-            raise ApiError(msg)
-        if (
-            self.hydrological_station_id is not None
-            and self.hydrological_station_id not in self.hydrological_stations
-        ):
-            msg = f"Invalid hydrological station ID: {self.hydrological_station_id}"
-            raise ApiError(msg)
+        if self.weather_station_id is not None:
+            await self.update_weather_stations()
+
+            if self.weather_station_id not in self.weather_stations:
+                msg = f"Invalid weather station ID: {self.weather_station_id}"
+                raise ApiError(msg)
+
+        if self.hydrological_station_id is not None:
+            await self.update_hydrological_stations()
+
+            if self.hydrological_station_id not in self.hydrological_stations:
+                msg = f"Invalid hydrological station ID: {self.hydrological_station_id}"
+                raise ApiError(msg)
+
+            await self._update_hydrological_details()
 
-    async def get_weather_stations(self: Self) -> dict[str, str]:
-        """Get list of weather stations."""
+    async def update_weather_stations(self: Self) -> None:
+        """Update list of weather stations."""
         url = API_WEATHER_ENDPOINT
 
         stations_data = await self._http_request(url)
 
-        return {
-            station[API_STATION_ID]: station[API_STATION] for station in stations_data
+        self._weather_station_list = {
+            station[ApiNames.STATION_ID]: station[ApiNames.STATION]
+            for station in stations_data
         }
 
     async def get_weather_data(self: Self) -> WeatherData:
         """Get weather data."""
+        if self.weather_station_id is None:
+            msg = "Weather station ID is not set"
+            raise ApiError(msg)
+
         url = f"{API_WEATHER_ENDPOINT}/id/{self.weather_station_id}"
 
         weather_data = await self._http_request(url)
 
         return self._parse_weather_data(weather_data)
 
-    async def get_hydrological_stations(self: Self) -> dict[str, str]:
-        """Get list of hydrological stations."""
+    async def update_hydrological_stations(self: Self) -> None:
+        """Update list of hydrological stations."""
         url = API_HYDROLOGICAL_ENDPOINT
 
         stations_data = await self._http_request(url)
 
-        return {
-            station[API_STATION_ID]: f"{station[API_STATION]} ({station[API_RIVER]})"
+        self._hydrological_station_list = {
+            station[ApiNames.STATION_ID]: gen_station_name(
+                station[ApiNames.STATION], station[ApiNames.RIVER]
+            )
             for station in stations_data
         }
 
+    async def _update_hydrological_details(self: Self) -> None:
+        """Update hydrological details."""
+        url = API_HYDROLOGICAL_DETAILS_ENDPOINT.format(
+            hydrological_station_id=self.hydrological_station_id
+        )
+
+        hydrological_details = await self._http_request(url)
+
+        self._warning_water_level = hydrological_details["status"]["warningValue"]
+        self._alarm_water_level = hydrological_details["status"]["alarmValue"]
+
     async def get_hydrological_data(self: Self) -> HydrologicalData:
         """Get hydrological data."""
+        if self.hydrological_station_id is None:
+            msg = "Hydrological station ID is not set"
+            raise ApiError(msg)
+
         url = f"{API_HYDROLOGICAL_ENDPOINT}/id/{self.hydrological_station_id}"
 
         hydrological_data = await self._http_request(url)
 
         return self._parse_hydrological_data(hydrological_data)
 
     async def _http_request(self: Self, url: str) -> Any:  # noqa: ANN401
@@ -152,93 +156,113 @@
             raise ApiError(msg)
 
         return await response.json()
 
     @staticmethod
     def _parse_weather_data(data: dict[str, Any]) -> WeatherData:
         """Parse weather data."""
-        temperature = data[API_TEMPERATURE]
+        temperature = data[ApiNames.TEMPERATURE]
         temperature_sensor = SensorData(
             name="Temperature",
             value=float(temperature) if temperature is not None else None,
-            unit=UNIT_CELSIUS if temperature is not None else None,
+            unit=Units.CELSIUS.value if temperature is not None else None,
         )
-        humidity = data[API_HUMIDITY]
+        humidity = data[ApiNames.HUMIDITY]
         humidity_sensor = SensorData(
             name="Humidity",
             value=float(humidity) if humidity is not None else None,
-            unit=UNIT_PERCENT if humidity is not None else None,
+            unit=Units.PERCENT.value if humidity is not None else None,
         )
-        wind_speed = data[API_WIND_SPEED]
+        wind_speed = data[ApiNames.WIND_SPEED]
         wind_speed_sensor = SensorData(
             name="Wind Speed",
             value=float(wind_speed) if wind_speed is not None else None,
-            unit=UNIT_METERS_PER_SECOND if wind_speed is not None else None,
+            unit=Units.METERS_PER_SECOND.value if wind_speed is not None else None,
         )
-        wind_direction = data[API_WIND_DIRECTION]
+        wind_direction = data[ApiNames.WIND_DIRECTION]
         wind_direction_sensor = SensorData(
             name="Wind Direction",
             value=float(wind_direction) if wind_direction is not None else None,
-            unit=UNIT_DEGREE if wind_direction is not None else None,
+            unit=Units.DEGREE.value if wind_direction is not None else None,
         )
-        precipitation = data[API_PRECIPITATION]
+        precipitation = data[ApiNames.PRECIPITATION]
         precipitation_sensor = SensorData(
             name="Precipitation",
             value=float(precipitation) if precipitation is not None else None,
-            unit=UNIT_MILLIMETERS if precipitation is not None else None,
+            unit=Units.MILLIMETERS.value if precipitation is not None else None,
         )
-        pressure = data[API_PRESSURE]
+        pressure = data[ApiNames.PRESSURE]
         pressure_sensor = SensorData(
             name="Pressure",
             value=float(pressure) if pressure is not None else None,
-            unit=UNIT_HPA if pressure is not None else None,
+            unit=Units.HPA.value if pressure is not None else None,
         )
-        measurement_date = datetime.strptime(
-            f"{data[API_MEASUREMENT_DATE]} {data[API_MEASUREMENT_TIME]}",
+        measurement_date = get_datetime(
+            f"{data[ApiNames.MEASUREMENT_DATE]} {data[ApiNames.MEASUREMENT_TIME]}",
             "%Y-%m-%d %H",
-        ).replace(tzinfo=UTC)
+        )
 
         return WeatherData(
             temperature=temperature_sensor,
             humidity=humidity_sensor,
             pressure=pressure_sensor,
             wind_speed=wind_speed_sensor,
             wind_direction=wind_direction_sensor,
             precipitation=precipitation_sensor,
-            station=data[API_STATION],
-            station_id=data[API_STATION_ID],
+            station=data[ApiNames.STATION],
+            station_id=data[ApiNames.STATION_ID],
             measurement_date=measurement_date,
         )
 
-    @staticmethod
-    def _parse_hydrological_data(data: dict[str, Any]) -> HydrologicalData:
+    def _parse_hydrological_data(self: Self, data: dict[str, Any]) -> HydrologicalData:
         """Parse hydrological data."""
-        water_level = data[API_WATER_LEVEL]
+        water_level = data[ApiNames.WATER_LEVEL]
+
+        if water_level is None:
+            msg = "Invalid water level value"
+            raise ApiError(msg)
+
         water_level_sensor = SensorData(
             name="Water Level",
             value=float(water_level) if water_level is not None else None,
-            unit=UNIT_CENTIMETERS if water_level is not None else None,
+            unit=Units.CENTIMETERS.value if water_level is not None else None,
         )
-        water_level_measurement_date = datetime.strptime(
-            f"{data[API_WATER_LEVEL_MEASUREMENT_DATE]}",
+        water_level_measurement_date = get_datetime(
+            data[ApiNames.WATER_LEVEL_MEASUREMENT_DATE],
             "%Y-%m-%d %H:%M:%S",
-        ).replace(tzinfo=UTC)
-        water_temperature = data[API_WATER_TEMPERATURE]
+        )
+        flood_warning_level_sensor = SensorData(
+            name="Flood Warning Level",
+            value=self._warning_water_level,
+            unit=Units.CENTIMETERS.value
+            if self._warning_water_level is not None
+            else None,
+        )
+        flood_alarm_level_sensor = SensorData(
+            name="Flood Alarm Level",
+            value=self._alarm_water_level,
+            unit=Units.CENTIMETERS.value
+            if self._alarm_water_level is not None
+            else None,
+        )
+        water_temperature = data[ApiNames.WATER_TEMPERATURE]
         water_temperature_sensor = SensorData(
             name="Water Temperature",
             value=float(water_temperature) if water_temperature is not None else None,
-            unit=UNIT_CELSIUS if water_temperature is not None else None,
+            unit=Units.CELSIUS.value if water_temperature is not None else None,
         )
-        water_temperature_measurement_date = datetime.strptime(
-            f"{data[API_WATER_TEMPERATURE_MEASUREMENT_DATE]}",
+        water_temperature_measurement_date = get_datetime(
+            data[ApiNames.WATER_TEMPERATURE_MEASUREMENT_DATE],
             "%Y-%m-%d %H:%M:%S",
-        ).replace(tzinfo=UTC)
+        )
 
         return HydrologicalData(
             water_level=water_level_sensor,
+            flood_warning_level=flood_warning_level_sensor,
+            flood_alarm_level=flood_alarm_level_sensor,
             water_temperature=water_temperature_sensor,
-            station=data[API_STATION],
-            river=data[API_RIVER],
-            station_id=data[API_STATION_ID],
+            station=data[ApiNames.STATION],
+            river=data[ApiNames.RIVER],
+            station_id=data[ApiNames.STATION_ID],
             water_level_measurement_date=water_level_measurement_date,
             water_temperature_measurement_date=water_temperature_measurement_date,
         )
```

### Comparing `imgw_pib-0.0.1/imgw_pib.egg-info/PKG-INFO` & `imgw_pib-0.0.5/imgw_pib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgw_pib
-Version: 0.0.1
+Version: 0.0.5
 Summary: Python wrapper for IMGW-PIB API.
 Home-page: https://github.com/bieniu/imgw-pib
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `imgw_pib-0.0.1/pyproject.toml` & `imgw_pib-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `imgw_pib-0.0.1/setup.py` & `imgw_pib-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 
 from setuptools import setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "0.0.1"
+VERSION = "0.0.5"
 
 setup(
     name="imgw_pib",
     version=VERSION,
     author="Maciej Bieniek",
     description="Python wrapper for IMGW-PIB API.",
     long_description=README_FILE.read_text(encoding="utf-8"),
```

