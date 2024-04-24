# Comparing `tmp/smartcitizen-connector-1.0.0.tar.gz` & `tmp/smartcitizen_connector-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartcitizen-connector-1.0.0.tar", last modified: Sun Apr  7 15:53:08 2024, max compression
+gzip compressed data, was "smartcitizen_connector-1.0.1.tar", last modified: Wed Apr 24 08:53:22 2024, max compression
```

## Comparing `smartcitizen-connector-1.0.0.tar` & `smartcitizen_connector-1.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:53:08.050855 smartcitizen-connector-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-07 15:53:08.050855 smartcitizen-connector-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-07 15:53:08.050855 smartcitizen-connector-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:53:08.046855 smartcitizen-connector-1.0.0/smartcitizen_connector/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:53:08.046855 smartcitizen-connector-1.0.0/smartcitizen_connector/_config/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/_config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:53:08.046855 smartcitizen-connector-1.0.0/smartcitizen_connector/device/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24197 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/device/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:53:08.046855 smartcitizen-connector-1.0.0/smartcitizen_connector/measurement/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/measurement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/measurement/measurement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:53:08.046855 smartcitizen-connector-1.0.0/smartcitizen_connector/models/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/models/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:53:08.050855 smartcitizen-connector-1.0.0/smartcitizen_connector/search/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/search/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:53:08.050855 smartcitizen-connector-1.0.0/smartcitizen_connector/sensor/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/sensor/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:53:08.050855 smartcitizen-connector-1.0.0/smartcitizen_connector/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:53:08.050855 smartcitizen-connector-1.0.0/smartcitizen_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-07 15:53:08.000000 smartcitizen-connector-1.0.0/smartcitizen_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-07 15:53:08.000000 smartcitizen-connector-1.0.0/smartcitizen_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:53:08.000000 smartcitizen-connector-1.0.0/smartcitizen_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:53:08.000000 smartcitizen-connector-1.0.0/smartcitizen_connector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-07 15:53:08.000000 smartcitizen-connector-1.0.0/smartcitizen_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-07 15:53:08.000000 smartcitizen-connector-1.0.0/smartcitizen_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:53:22.250019 smartcitizen_connector-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-24 08:53:22.250019 smartcitizen_connector-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 08:53:22.250019 smartcitizen_connector-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:53:22.246019 smartcitizen_connector-1.0.1/smartcitizen_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:53:22.250019 smartcitizen_connector-1.0.1/smartcitizen_connector/_config/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/_config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:53:22.250019 smartcitizen_connector-1.0.1/smartcitizen_connector/device/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/device/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:53:22.250019 smartcitizen_connector-1.0.1/smartcitizen_connector/measurement/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/measurement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/measurement/measurement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:53:22.250019 smartcitizen_connector-1.0.1/smartcitizen_connector/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/models/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:53:22.250019 smartcitizen_connector-1.0.1/smartcitizen_connector/search/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/search/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:53:22.250019 smartcitizen_connector-1.0.1/smartcitizen_connector/sensor/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/sensor/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:53:22.250019 smartcitizen_connector-1.0.1/smartcitizen_connector/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-04-24 08:53:17.000000 smartcitizen_connector-1.0.1/smartcitizen_connector/tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:53:22.250019 smartcitizen_connector-1.0.1/smartcitizen_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-24 08:53:22.000000 smartcitizen_connector-1.0.1/smartcitizen_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-24 08:53:22.000000 smartcitizen_connector-1.0.1/smartcitizen_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:53:22.000000 smartcitizen_connector-1.0.1/smartcitizen_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:53:22.000000 smartcitizen_connector-1.0.1/smartcitizen_connector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 08:53:22.000000 smartcitizen_connector-1.0.1/smartcitizen_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-24 08:53:22.000000 smartcitizen_connector-1.0.1/smartcitizen_connector.egg-info/top_level.txt
```

### Comparing `smartcitizen-connector-1.0.0/LICENSE` & `smartcitizen_connector-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smartcitizen-connector-1.0.0/PKG-INFO` & `smartcitizen_connector-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartcitizen-connector
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python connector to download information collected in SmartCitizen API
 Home-page: https://github.com/fablabbcn/smartcitizen-connector
 Author: oscgonfer
 License: GNU General Public License v3
 Project-URL: Documentation, https://docs.smartcitizen.me/
 Project-URL: Source Code, https://github.com/fablabbcn/smartcitizen-connector
 Keywords: sensors,Smart Citizen
```

### Comparing `smartcitizen-connector-1.0.0/README.md` & `smartcitizen_connector-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `smartcitizen-connector-1.0.0/setup.py` & `smartcitizen_connector-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 PROJECT_URLS = {
     "Documentation": "https://docs.smartcitizen.me/",
     "Source Code": "https://github.com/fablabbcn/smartcitizen-connector",
 }
 
 setup(
     name="smartcitizen-connector",
-    version="1.0.0",
+    version="1.0.1",
     description="Python connector to download information collected in SmartCitizen API",
     author="oscgonfer",
     license="GNU General Public License v3",
     keywords=['sensors', 'Smart Citizen'],
     long_description = open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/fablabbcn/smartcitizen-connector",
```

### Comparing `smartcitizen-connector-1.0.0/smartcitizen_connector/_config/config.py` & `smartcitizen_connector-1.0.1/smartcitizen_connector/_config/config.py`

 * *Files identical despite different names*

### Comparing `smartcitizen-connector-1.0.0/smartcitizen_connector/device/device.py` & `smartcitizen_connector-1.0.1/smartcitizen_connector/device/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,26 +86,21 @@
             pass
     else:
         _hardware_url = ''
 
     return _hardware_url, _hardware_postprocessing, _ok
 
 class SCDevice:
-    id: int
-    url: str
-    page: str
-    timezone: str
-    json: Device
-    data: DataFrame
 
     def __init__(self, id, check_postprocessing=True):
         self.id = id
         self.url = f'{config.DEVICES_URL}{self.id}'
         self.page = f'{config.FRONTEND_URL}{self.id}'
         self.method = 'async'
+        self.data = DataFrame()
         self._metrics: List[Metric] = []
         self.__load__()
         self.__get_timezone__()
         if check_postprocessing:
             self.__check_postprocessing__()
             self._filled_properties = list()
             self._properties = dict()
@@ -260,38 +255,36 @@
         if max_date is not None:
             max_date = localise_date(to_datetime(max_date), 'UTC')
             logger.info(f'Max Date: {max_date}')
 
         # Trim based on actual data available
         if min_date is not None and self.json.last_reading_at is not None:
             if min_date > self.json.last_reading_at:
-                logger.warning('Device request would yield empty data (min_date). Returning')
+                logger.warning(f'Device {self.id} request would yield empty data (min_date). Returning')
                 return self.data
 
         if max_date is not None and self.json.created_at is not None:
             if max_date < self.json.created_at:
-                logger.warning('Device request would yield empty data (max_date). Returning')
+                logger.warning(f'Device {self.id} request would yield empty data (max_date). Returning')
                 return self.data
 
         if max_date is not None and self.json.last_reading_at is not None:
             if max_date > self.json.last_reading_at:
                 logger.warning('Trimming max_date to last reading')
                 max_date = self.json.last_reading_at
 
-        if self.json.kit is not None:
-            logger.info(f'Kit ID: {self.json.kit.id}')
-        logger.info(f'Device timezone: {self.timezone}')
+        logger.info(f'Device {self.id} timezone: {self.timezone}')
 
         if not self.json.data.sensors:
-            logger.info('Device is empty')
+            logger.info(f'Device {self.id} is empty', 'WARNING')
             return self.data
         else: logger.info(f"Sensor IDs: {[f'{sensor.name}: {sensor.id}' for sensor in self.json.data.sensors]}")
 
         df = DataFrame()
-        logger.info(f'Requesting from {min_date} to {max_date}')
+        logger.info(f'Requesting device {self.id} from {min_date} to {max_date}')
 
         semaphore = asyncio.Semaphore(config._max_concurrent_requests)
         async with aiohttp.ClientSession() as session:
 
             tasks = []
             for sensor in self.json.data.sensors:
 
@@ -316,15 +309,15 @@
             df = df.combine_first(df_sensor)
 
         try:
             df = df.reindex(df.index.rename('TIME'))
             df = clean(df, clean_na, how = 'all')
             self.data = df
         except:
-            logger.error('Problem closing up the API dataframe')
+            logger.error(f'Problem closing up the API dataframe for {self.id}')
             pass
 
         logger.info(f'Device {self.id} loaded successfully from API')
         return self.data
 
     async def post_data(self, columns = 'sensors', rename = None, clean_na = 'drop', chunk_size = 500, dry_run = False, max_retries = 2, delay = None):
         '''
```

### Comparing `smartcitizen-connector-1.0.0/smartcitizen_connector/measurement/measurement.py` & `smartcitizen_connector-1.0.1/smartcitizen_connector/measurement/measurement.py`

 * *Files identical despite different names*

### Comparing `smartcitizen-connector-1.0.0/smartcitizen_connector/models/models.py` & `smartcitizen_connector-1.0.1/smartcitizen_connector/models/models.py`

 * *Files identical despite different names*

### Comparing `smartcitizen-connector-1.0.0/smartcitizen_connector/search/search.py` & `smartcitizen_connector-1.0.1/smartcitizen_connector/search/search.py`

 * *Files identical despite different names*

### Comparing `smartcitizen-connector-1.0.0/smartcitizen_connector/sensor/sensor.py` & `smartcitizen_connector-1.0.1/smartcitizen_connector/sensor/sensor.py`

 * *Files identical despite different names*

### Comparing `smartcitizen-connector-1.0.0/smartcitizen_connector/tools/tools.py` & `smartcitizen_connector-1.0.1/smartcitizen_connector/tools/tools.py`

 * *Files identical despite different names*

### Comparing `smartcitizen-connector-1.0.0/smartcitizen_connector.egg-info/PKG-INFO` & `smartcitizen_connector-1.0.1/smartcitizen_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartcitizen-connector
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python connector to download information collected in SmartCitizen API
 Home-page: https://github.com/fablabbcn/smartcitizen-connector
 Author: oscgonfer
 License: GNU General Public License v3
 Project-URL: Documentation, https://docs.smartcitizen.me/
 Project-URL: Source Code, https://github.com/fablabbcn/smartcitizen-connector
 Keywords: sensors,Smart Citizen
```

### Comparing `smartcitizen-connector-1.0.0/smartcitizen_connector.egg-info/SOURCES.txt` & `smartcitizen_connector-1.0.1/smartcitizen_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

