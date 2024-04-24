# Comparing `tmp/pyastroweatherio-0.43.1.dev8.tar.gz` & `tmp/pyastroweatherio-0.43.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastroweatherio-0.43.1.dev8.tar", last modified: Mon Apr 22 09:43:07 2024, max compression
+gzip compressed data, was "pyastroweatherio-0.43.1.dev9.tar", last modified: Tue Apr 23 10:48:06 2024, max compression
```

## Comparing `pyastroweatherio-0.43.1.dev8.tar` & `pyastroweatherio-0.43.1.dev9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-22 09:43:07.587887 pyastroweatherio-0.43.1.dev8/
--rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev8/LICENSE
--rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-22 09:43:07.583887 pyastroweatherio-0.43.1.dev8/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.43.1.dev8/README.md
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-22 09:43:07.583887 pyastroweatherio-0.43.1.dev8/pyastroweatherio/
--rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev8/pyastroweatherio/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    32960 2024-04-22 09:43:03.000000 pyastroweatherio-0.43.1.dev8/pyastroweatherio/client.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     3639 2024-04-17 18:18:53.000000 pyastroweatherio-0.43.1.dev8/pyastroweatherio/const.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    20074 2024-04-14 12:24:57.000000 pyastroweatherio-0.43.1.dev8/pyastroweatherio/dataclasses.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.43.1.dev8/pyastroweatherio/errors.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    32312 2023-11-12 10:53:43.000000 pyastroweatherio-0.43.1.dev8/pyastroweatherio/helper_functions.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-22 09:43:07.583887 pyastroweatherio-0.43.1.dev8/pyastroweatherio.egg-info/
--rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-22 09:43:07.000000 pyastroweatherio-0.43.1.dev8/pyastroweatherio.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-04-22 09:43:07.000000 pyastroweatherio-0.43.1.dev8/pyastroweatherio.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-04-22 09:43:07.000000 pyastroweatherio-0.43.1.dev8/pyastroweatherio.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-04-22 09:43:07.000000 pyastroweatherio-0.43.1.dev8/pyastroweatherio.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-04-22 09:43:07.000000 pyastroweatherio-0.43.1.dev8/pyastroweatherio.egg-info/top_level.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-04-22 09:43:07.587887 pyastroweatherio-0.43.1.dev8/setup.cfg
--rw-rw-r--   0 markus    (1000) markus    (1000)     1340 2024-04-22 09:42:52.000000 pyastroweatherio-0.43.1.dev8/setup.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-23 10:48:06.903584 pyastroweatherio-0.43.1.dev9/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev9/LICENSE
+-rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-23 10:48:06.903584 pyastroweatherio-0.43.1.dev9/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.43.1.dev9/README.md
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-23 10:48:06.899584 pyastroweatherio-0.43.1.dev9/pyastroweatherio/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev9/pyastroweatherio/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    33774 2024-04-23 10:16:21.000000 pyastroweatherio-0.43.1.dev9/pyastroweatherio/client.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     3639 2024-04-22 11:00:22.000000 pyastroweatherio-0.43.1.dev9/pyastroweatherio/const.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    20074 2024-04-22 11:00:22.000000 pyastroweatherio-0.43.1.dev9/pyastroweatherio/dataclasses.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.43.1.dev9/pyastroweatherio/errors.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    37621 2024-04-23 10:29:18.000000 pyastroweatherio-0.43.1.dev9/pyastroweatherio/helper_functions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-23 10:48:06.903584 pyastroweatherio-0.43.1.dev9/pyastroweatherio.egg-info/
+-rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-23 10:48:06.000000 pyastroweatherio-0.43.1.dev9/pyastroweatherio.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-04-23 10:48:06.000000 pyastroweatherio-0.43.1.dev9/pyastroweatherio.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-04-23 10:48:06.000000 pyastroweatherio-0.43.1.dev9/pyastroweatherio.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-04-23 10:48:06.000000 pyastroweatherio-0.43.1.dev9/pyastroweatherio.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-04-23 10:48:06.000000 pyastroweatherio-0.43.1.dev9/pyastroweatherio.egg-info/top_level.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-04-23 10:48:06.907584 pyastroweatherio-0.43.1.dev9/setup.cfg
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1340 2024-04-23 10:47:56.000000 pyastroweatherio-0.43.1.dev9/setup.py
```

### Comparing `pyastroweatherio-0.43.1.dev8/LICENSE` & `pyastroweatherio-0.43.1.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev8/PKG-INFO` & `pyastroweatherio-0.43.1.dev9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.43.1.dev8
+Version: 0.43.1.dev9
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.43.1.dev8/README.md` & `pyastroweatherio-0.43.1.dev9/README.md`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev8/pyastroweatherio/client.py` & `pyastroweatherio-0.43.1.dev9/pyastroweatherio/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from pyastroweatherio.dataclasses import (
     ForecastData,
     LocationData,
     NightlyConditionsData,
     DSOUpTonight,
 )
 from pyastroweatherio.errors import RequestError
-from pyastroweatherio.helper_functions import ConversionFunctions, AstronomicalRoutines
+from pyastroweatherio.helper_functions import ConversionFunctions, AstronomicalRoutines, AstronomicalSeeing
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class AstroWeather:
     """AstroWeather Communication Client."""
 
@@ -94,14 +94,16 @@
             self._latitude,
             self._longitude,
             self._elevation,
             self._timezone_info,
             self._test_datetime,
         )
 
+        self._astro_seeing = AstronomicalSeeing()
+        
         # Testing
         self._test_mode = False
         if self._test_datetime is not None:
             self._test_mode = True
 
     # Public functions
     async def get_location_data(
@@ -193,15 +195,15 @@
                 # Remaining forecast data point in 7timer data
                 "forecast_length": (len(self._weather_data_seventimer) - forecast_skipped) * 3,
                 # Location
                 "latitude": self._latitude,
                 "longitude": self._longitude,
                 "elevation": self._elevation,
                 # 7timer
-                "seeing": row["seeing"],
+                "seeing": await self._astro_seeing.calculate_seeing_model4(details.get("air_temperature", -1), details.get("wind_speed", -1), details.get("relative_humidity", -1), self._elevation), #row["seeing"],
                 "transparency": row["transparency"],
                 "lifted_index": row["lifted_index"],
                 # Calculate
                 "sun_next_rising": await self._astro_routines.sun_next_rising_civil(),
                 "sun_next_rising_nautical": await self._astro_routines.sun_next_rising_nautical(),
                 "sun_next_rising_astro": await self._astro_routines.sun_next_rising_astro(),
                 "sun_next_setting": await self._astro_routines.sun_next_setting_civil(),
@@ -251,15 +253,15 @@
                     .get("next_1_hours", {})
                     .get("details", {})
                     .get("precipitation_amount", "")
                 ),
                 # Condition
                 "condition_percentage": await self.calc_condition_percentage(
                     details.get("cloud_area_fraction", -1) / 12.5 + 1,
-                    row["seeing"],
+                    await self._astro_seeing.calculate_seeing_model4(details.get("air_temperature", -1), details.get("wind_speed", -1), details.get("relative_humidity", -1), self._elevation), #row["seeing"],
                     row["transparency"],
                     details.get("wind_speed", -1),
                 ),
                 # Uptonight objects
                 "uptonight": await self._get_deepsky_objects(),
             }
 
@@ -301,15 +303,15 @@
             if metno_index == -1:
                 for datapoint in self._weather_data_metno:
                     metno_index += 1
                     if forecast_time == datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"):
                         break
                 _LOGGER.debug("Met.no start index: %s", str(metno_index))
 
-            seeing = row["seeing"]
+            seeing = 0  #row["seeing"]
             transparency = row["transparency"]
             item = {
                 "seventimer_init": init_ts,
                 "seventimer_timepoint": row["timepoint"],
                 "forecast_time": forecast_time,
                 "hour": forecast_time.hour % 24,
                 "seeing": seeing,
@@ -340,18 +342,19 @@
                     item["cloud_area_fraction"] = details.get("cloud_area_fraction", -1)
                     item["cloud_area_fraction_high"] = details.get("cloud_area_fraction_high", -1)
                     item["cloud_area_fraction_low"] = details.get("cloud_area_fraction_low", -1)
                     item["cloud_area_fraction_medium"] = details.get("cloud_area_fraction_medium", -1)
                     item["fog_area_fraction"] = details.get("fog_area_fraction", -1)
                     item["rh2m"] = details.get("relative_humidity", -1)
                     item["wind_speed"] = details.get("wind_speed", -1)
+                    item["seeing"] = await self._astro_seeing.calculate_seeing_model4(details.get("air_temperature", -1), details.get("wind_speed", -1), details.get("relative_humidity", -1), self._elevation)
 
                     item["condition_percentage"] = await self.calc_condition_percentage(
                         item["cloud_area_fraction"] / 12.5 + 1,
-                        row["seeing"],
+                        await self._astro_seeing.calculate_seeing_model4(details.get("air_temperature", -1), details.get("wind_speed", -1), details.get("relative_humidity", -1), self._elevation), #row["seeing"],
                         row["transparency"],
                         item["wind_speed"],
                     )
 
                     item["wind_from_direction"] = details.get("wind_from_direction", -1)
                     item["temp2m"] = details.get("air_temperature", -1)
                     item["dewpoint2m"] = details.get("dew_point_temperature", -1)
@@ -621,16 +624,16 @@
                 self._weather_data_seventimer_init = json_data_astro.get("init")
             else:
                 # Fake 7timer weather data if service is broken
                 # This eliminates consideration of seeing, transparency, and lifted_index
                 # TODO: Think about a complete redesign of the calculations and potentially
                 #       make met.no the leading source instead of 7timer
                 # TODO: Find another source for seeing and transparency
-                self._seeing_weight = 0
-                self._transparency_weight = 0
+                # self._seeing_weight = 0
+                # self._transparency_weight = 0
                 self._weather_data_seventimer = []
                 for index in range(0, 20):
                     self._weather_data_seventimer.append({"timepoint": index * 3, "seeing": 0, "transparency": 0, "lifted_index": 0})
                 self._weather_data_seventimer_init = datetime.now().strftime("%Y%m%d%H")
         else:
             _LOGGER.debug("Using cached data for 7Timer")
```

### Comparing `pyastroweatherio-0.43.1.dev8/pyastroweatherio/const.py` & `pyastroweatherio-0.43.1.dev9/pyastroweatherio/const.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev8/pyastroweatherio/dataclasses.py` & `pyastroweatherio-0.43.1.dev9/pyastroweatherio/dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev8/pyastroweatherio/helper_functions.py` & `pyastroweatherio-0.43.1.dev9/pyastroweatherio/helper_functions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ Contains Helper functions for AstroWeather."""
 from datetime import datetime, timedelta
 import logging
 import ephem
+import math
 from ephem import degree
 from math import degrees as deg
 import pytz
 
 # The introduction of the module [timezonefinder](https://github.com/jannikmi/timezonefinder)
 # with it's nested dependency to [py-h3](https://github.com/uber/h3-py) failed while compiling
 # the `c`-module h3 on some home assistant deployment variants (e.g. Home Assistant
@@ -36,14 +37,122 @@
 
     async def anchor_timestamp(self, value) -> datetime:
         """Converts the datetime string from 7Timer to DateTime."""
         _LOGGER.debug("7timer anchor timestamp: %s", str(datetime.strptime(value, "%Y%m%d%H")))
         return datetime.strptime(value, "%Y%m%d%H")
 
 
+class AstronomicalSeeing:
+    """Calculate different astronomical objects"""
+
+    def __init__(
+        self,
+    ):
+        _LOGGER.debug("AstronomicalSeeing calculation mode active")
+        # temperature = 15  # in Celsius
+        # wind_speed = 5  # in m/s
+        # humidity = 50  # in Percent
+        # aerosol_density = 0.1  # in kg/m^3
+        # altitude = 1000  # in Meters
+
+    # Modell 0: Simple linear Model
+    async def calculate_seeing_model0(self, temperature, wind_speed, humidity, altitude):
+        constant_1 = 0.314 * temperature / 273
+        constant_2 = 20.8 * (1 - math.exp(-0.0695 * humidity))
+        constant_3 = 0.0017 * wind_speed ** 1.5
+        seeing = constant_1 + constant_2 + constant_3
+        _LOGGER.debug("AstronomicalSeeing calculation model1: T %s, W %s, H %s, E %s - S %s", str(temperature), str(wind_speed), str(humidity), str(altitude), str(seeing))
+        if seeing >= 2.5: return 7
+        if seeing >= 2.0: return 6
+        if seeing >= 1.5: return 5
+        if seeing >= 1.25: return 4
+        if seeing >= 1.0: return 3
+        if seeing >= 0.75: return 2
+        if seeing >= 0.5: return 1
+        return 0
+        # return 0.1 * temperature + 0.2 * wind_speed + 0.05 * humidity + 0.1 * aerosol_density - 0.05 * altitude
+
+    # Modell 1: Simple linear Model
+    async def calculate_seeing_model1(self, temperature, wind_speed, humidity, altitude):
+        seeing = 0.1 * temperature + 0.2 * wind_speed + 0.05 * humidity # - 0.05 * altitude
+        _LOGGER.debug("AstronomicalSeeing calculation model1: T %s, W %s, H %s, E %s - S %s", str(temperature), str(wind_speed), str(humidity), str(altitude), str(seeing))
+        if seeing >= 2.5: return 7
+        if seeing >= 2.0: return 6
+        if seeing >= 1.5: return 5
+        if seeing >= 1.25: return 4
+        if seeing >= 1.0: return 3
+        if seeing >= 0.75: return 2
+        if seeing >= 0.5: return 1
+        return 0
+        # return 0.1 * temperature + 0.2 * wind_speed + 0.05 * humidity + 0.1 * aerosol_density - 0.05 * altitude
+
+    # Modell 2: Modell with Exponential functions
+    async def calculate_seeing_model2(self, temperature, wind_speed, humidity, altitude):
+        seeing = 0.05 * temperature + 0.1 * wind_speed ** 1.5 + 0.02 * humidity ** 2 - 0.03 * altitude ** 1.5
+        _LOGGER.debug("AstronomicalSeeing calculation model2: T %s, W %s, H %s, E %s - S %s", str(temperature), str(wind_speed), str(humidity), str(altitude), str(seeing))
+        if seeing >= 2.5: return 7
+        if seeing >= 2.0: return 6
+        if seeing >= 1.5: return 5
+        if seeing >= 1.25: return 4
+        if seeing >= 1.0: return 3
+        if seeing >= 0.75: return 2
+        if seeing >= 0.5: return 1
+        return 0
+        # return 0.05 * temperature + 0.1 * wind_speed ** 1.5 + 0.02 * humidity ** 2 + 0.08 * aerosol_density - 0.03 * altitude ** 1.5
+
+    # Modell 3: Modell basierend auf empirischen Daten
+    async def calculate_seeing_model3(self, temperature, wind_speed, humidity, altitude):
+        seeing = 0.08 * temperature + 0.15 * math.log(wind_speed + 1) + 0.03 * humidity - 0.02 * altitude
+        _LOGGER.debug("AstronomicalSeeing calculation model3: T %s, W %s, H %s, E %s - S %s", str(temperature), str(wind_speed), str(humidity), str(altitude), str(seeing))
+        if seeing >= 2.5: return 7
+        if seeing >= 2.0: return 6
+        if seeing >= 1.5: return 5
+        if seeing >= 1.25: return 4
+        if seeing >= 1.0: return 3
+        if seeing >= 0.75: return 2
+        if seeing >= 0.5: return 1
+        return 0
+        # return 0.08 * temperature + 0.15 * math.log(wind_speed + 1) + 0.03 * humidity + 0.1 * aerosol_density - 0.02 * altitude
+
+    def calculate_dew_point(self, temperature, humidity):
+        a = 17.62
+        b = 243.12
+        gamma = math.log(humidity / 100) + (a * temperature) / (b + temperature)
+        dew_point = (b * gamma) / (a - gamma)
+        return dew_point
+
+    def calculate_saturation_vapor_pressure(self, dew_point):
+        es = 6.11 * (10 ** (7.5 * dew_point / (237.7 + dew_point)))
+        return es
+
+    def calculate_water_vapor_pressure(self, temperature, humidity):
+        dew_point = self.calculate_dew_point(temperature, humidity)
+        es = self.calculate_saturation_vapor_pressure(dew_point)
+        water_vapor_pressure = (humidity / 100) * es
+        return water_vapor_pressure
+
+    async def calculate_seeing_model4(self, temperature, humidity, wind_speed, altitude):
+        water_vapor_pressure = self.calculate_water_vapor_pressure(temperature, humidity)
+        adjusted_pressure = 1013.25 * math.exp(-0.00012 * altitude)
+        relative_pressure = adjusted_pressure / 1013.25
+        seeing_factor = 0.8 * (water_vapor_pressure / 10) ** 0.25 * (wind_speed / 10) ** 0.75 * relative_pressure
+        seeing = 0.98 / seeing_factor
+        _LOGGER.debug("AstronomicalSeeing calculation model3: T %s, W %s, H %s, E %s - S %s", str(temperature), str(wind_speed), str(humidity), str(altitude), str(seeing))
+        if seeing >= 2.5: return 7
+        if seeing >= 2.0: return 6
+        if seeing >= 1.5: return 5
+        if seeing >= 1.25: return 4
+        if seeing >= 1.0: return 3
+        if seeing >= 0.75: return 2
+        if seeing >= 0.5: return 1
+        return 0
+        # return seeing_factor
+
+
+
 class AstronomicalRoutines:
     """Calculate different astronomical objects"""
 
     def __init__(
         self,
         latitude=HOME_LATITUDE,
         longitude=HOME_LONGITUDE,
```

### Comparing `pyastroweatherio-0.43.1.dev8/pyastroweatherio.egg-info/PKG-INFO` & `pyastroweatherio-0.43.1.dev9/pyastroweatherio.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.43.1.dev8
+Version: 0.43.1.dev9
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.43.1.dev8/setup.py` & `pyastroweatherio-0.43.1.dev9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="pyastroweatherio",
     packages=["pyastroweatherio"],
-    version="0.43.1.dev8",
+    version="0.43.1.dev9",
     license="MIT",
     description="Python Wrapper for 7Timer and Met.no REST API",
     long_description=" ".join(
         [
             "Lightweight Python 3 module to receive data via",
             "REST API from 7Timer and Met.no.",
         ],
```

