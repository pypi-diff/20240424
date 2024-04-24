# Comparing `tmp/ned-py-0.2.tar.gz` & `tmp/ned-py-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ned-py-0.2.tar", last modified: Mon Apr  8 06:43:59 2024, max compression
+gzip compressed data, was "ned-py-0.3.tar", last modified: Wed Apr 24 11:42:10 2024, max compression
```

## Comparing `ned-py-0.2.tar` & `ned-py-0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 meh       (1000) meh       (1000)        0 2024-04-08 06:43:59.165239 ned-py-0.2/
--rw-rw-r--   0 meh       (1000) meh       (1000)     1077 2024-04-03 08:32:56.000000 ned-py-0.2/LICENSE
--rw-r--r--   0 meh       (1000) meh       (1000)     1160 2024-04-08 06:43:59.165239 ned-py-0.2/PKG-INFO
--rw-rw-r--   0 meh       (1000) meh       (1000)     1590 2024-04-08 06:39:07.000000 ned-py-0.2/README.md
-drwxrwxr-x   0 meh       (1000) meh       (1000)        0 2024-04-08 06:43:59.165239 ned-py-0.2/ned/
--rw-rw-r--   0 meh       (1000) meh       (1000)       24 2024-04-03 09:12:28.000000 ned-py-0.2/ned/__init__.py
--rw-rw-r--   0 meh       (1000) meh       (1000)     3188 2024-04-08 06:39:33.000000 ned-py-0.2/ned/helper.py
--rw-rw-r--   0 meh       (1000) meh       (1000)     2151 2024-04-06 11:53:41.000000 ned-py-0.2/ned/metadata.py
--rw-rw-r--   0 meh       (1000) meh       (1000)    16480 2024-04-08 06:39:33.000000 ned-py-0.2/ned/ned.py
-drwxrwxr-x   0 meh       (1000) meh       (1000)        0 2024-04-08 06:43:59.165239 ned-py-0.2/ned_py.egg-info/
--rw-r--r--   0 meh       (1000) meh       (1000)     1160 2024-04-08 06:43:59.000000 ned-py-0.2/ned_py.egg-info/PKG-INFO
--rw-rw-r--   0 meh       (1000) meh       (1000)      268 2024-04-08 06:43:59.000000 ned-py-0.2/ned_py.egg-info/SOURCES.txt
--rw-rw-r--   0 meh       (1000) meh       (1000)        1 2024-04-08 06:43:59.000000 ned-py-0.2/ned_py.egg-info/dependency_links.txt
--rw-rw-r--   0 meh       (1000) meh       (1000)       54 2024-04-08 06:43:59.000000 ned-py-0.2/ned_py.egg-info/requires.txt
--rw-rw-r--   0 meh       (1000) meh       (1000)       10 2024-04-08 06:43:59.000000 ned-py-0.2/ned_py.egg-info/top_level.txt
--rw-rw-r--   0 meh       (1000) meh       (1000)       38 2024-04-08 06:43:59.165239 ned-py-0.2/setup.cfg
--rw-rw-r--   0 meh       (1000) meh       (1000)     1323 2024-04-08 06:27:15.000000 ned-py-0.2/setup.py
-drwxrwxr-x   0 meh       (1000) meh       (1000)        0 2024-04-08 06:43:59.165239 ned-py-0.2/tests/
--rw-rw-r--   0 meh       (1000) meh       (1000)       20 2024-04-06 08:58:23.000000 ned-py-0.2/tests/__init__.py
--rw-rw-r--   0 meh       (1000) meh       (1000)     4341 2024-04-08 06:39:33.000000 ned-py-0.2/tests/test_ned.py
+drwxrwxr-x   0 meh       (1000) meh       (1000)        0 2024-04-24 11:42:10.007026 ned-py-0.3/
+-rw-rw-r--   0 meh       (1000) meh       (1000)     1077 2024-04-03 08:32:56.000000 ned-py-0.3/LICENSE
+-rw-r--r--   0 meh       (1000) meh       (1000)     1160 2024-04-24 11:42:10.007026 ned-py-0.3/PKG-INFO
+-rw-rw-r--   0 meh       (1000) meh       (1000)     1540 2024-04-24 11:40:59.000000 ned-py-0.3/README.md
+drwxrwxr-x   0 meh       (1000) meh       (1000)        0 2024-04-24 11:42:10.007026 ned-py-0.3/ned/
+-rw-rw-r--   0 meh       (1000) meh       (1000)       24 2024-04-03 09:12:28.000000 ned-py-0.3/ned/__init__.py
+-rw-rw-r--   0 meh       (1000) meh       (1000)     5031 2024-04-24 11:40:59.000000 ned-py-0.3/ned/helper.py
+-rw-rw-r--   0 meh       (1000) meh       (1000)     2151 2024-04-24 11:40:59.000000 ned-py-0.3/ned/metadata.py
+-rw-rw-r--   0 meh       (1000) meh       (1000)    18445 2024-04-24 11:40:59.000000 ned-py-0.3/ned/ned.py
+drwxrwxr-x   0 meh       (1000) meh       (1000)        0 2024-04-24 11:42:10.007026 ned-py-0.3/ned_py.egg-info/
+-rw-r--r--   0 meh       (1000) meh       (1000)     1160 2024-04-24 11:42:09.000000 ned-py-0.3/ned_py.egg-info/PKG-INFO
+-rw-rw-r--   0 meh       (1000) meh       (1000)      268 2024-04-24 11:42:09.000000 ned-py-0.3/ned_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 meh       (1000) meh       (1000)        1 2024-04-24 11:42:09.000000 ned-py-0.3/ned_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 meh       (1000) meh       (1000)       54 2024-04-24 11:42:09.000000 ned-py-0.3/ned_py.egg-info/requires.txt
+-rw-rw-r--   0 meh       (1000) meh       (1000)       10 2024-04-24 11:42:09.000000 ned-py-0.3/ned_py.egg-info/top_level.txt
+-rw-rw-r--   0 meh       (1000) meh       (1000)       38 2024-04-24 11:42:10.007026 ned-py-0.3/setup.cfg
+-rw-rw-r--   0 meh       (1000) meh       (1000)     1323 2024-04-24 11:40:59.000000 ned-py-0.3/setup.py
+drwxrwxr-x   0 meh       (1000) meh       (1000)        0 2024-04-24 11:42:10.007026 ned-py-0.3/tests/
+-rw-rw-r--   0 meh       (1000) meh       (1000)       20 2024-04-06 08:58:23.000000 ned-py-0.3/tests/__init__.py
+-rw-rw-r--   0 meh       (1000) meh       (1000)     4200 2024-04-24 11:40:59.000000 ned-py-0.3/tests/test_ned.py
```

### Comparing `ned-py-0.2/LICENSE` & `ned-py-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ned-py-0.2/PKG-INFO` & `ned-py-0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ned-py
-Version: 0.2
+Version: 0.3
 Summary: Python wrapper for Nationaal Energie Dashboard API.
 Home-page: https://github.com/profiteia/ned-py
 Author: Profiteia
 Author-email: victor@profiteia.io
 License: MIT
 Project-URL: Source, https://github.com/profiteia/ned-py
 Project-URL: Documentation, https://github.com/profiteia/ned-py
```

### Comparing `ned-py-0.2/README.md` & `ned-py-0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -14,39 +14,39 @@
 - [Disclaimer](#disclaimer)
 - [License](#license)
 - [Contact](#contact)
 
 ## Installation
 
 ```
-git clone https://github.com/profiteia/ned-py
-cd ned-py
-pip install . 
+pip install ned-py
 ```
 
 test functionality by:
 
 ```
 pip install pytest
 export NED_API_KEY='YOUR_API_KEY'
 pytest
 ```
 
 ## Functions
 
 ```
-authorisations()
 users()
+authorisations()
+
+get_forecast()
 get_consumption()
 get_production_provinces()
 get_production_offshore()
 get_production_netherlands()
 ```
 
-The API lacks clear documentation. Not all datapoints are available and forecast and backcast are not yet implemented. Checkout ned/helper.py for `is_valid_request` to see which requests are valid. 
+The API lacks clear documentation. Not all datapoints are available and backcast is not yet implemented. Checkout ned/helper.py for `is_valid_request` to see which requests are valid. 
 This package will be updated when more information becomes available.
 
 ## Usage
 
 ``` 
 import ned
```

### Comparing `ned-py-0.2/ned/metadata.py` & `ned-py-0.3/ned/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from bidict import bidict
 
 NED_ACTIVITIES = bidict({"Providing": 1, "Consuming": 2})
 
-NED_CLASSIFICATIONS = bidict({"Backcast": 1, "Current": 2, "Forecast": 3})
+NED_CLASSIFICATIONS = bidict({"Forecast": 1, "Current": 2, "Backcast": 3})
 
 NED_GRANULARITIES = bidict(
     {"10 minutes": 3, "15 minutes": 4, "Hour": 5, "Day": 6, "Month": 7, "Year": 8}
 )
 
 NED_GRANULARITY_TIME_ZONES = bidict({"UTC": 0, "CET (Central European Time)": 1})
```

### Comparing `ned-py-0.2/ned/ned.py` & `ned-py-0.3/ned/ned.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from requests.exceptions import ChunkedEncodingError
 from typing import List, Union, Optional, Dict, Generator
 from datetime import datetime, timedelta
+from simplejson.errors import JSONDecodeError
 import logging
 import requests
 import pandas as pd
 import json
 import time
 from .helper import generate_loop, is_valid_request
 
@@ -125,24 +127,32 @@
 
         Returns:
         Union[pd.DataFrame, dict]: A DataFrame or dict containing the response from request.
         """
 
         headers = {"X-AUTH-TOKEN": self._api_key, "accept": "application/ld+json"}
 
-        response = requests.get(
-            f"{self.API_URL}/{endpoint}", headers=headers, params=params
-        )
+        try:
+            response = requests.get(
+                f"{self.API_URL}/{endpoint}", headers=headers, params=params
+            )
+        except ChunkedEncodingError as ex:
+            # Could not decode the chunked encoding, try again
+            return self._do_api_request(endpoint, params)
 
         self.logger.debug(json.dumps(params, indent=4))
 
-        if "hydra:member" in response.json():
-            response = response.json()["hydra:member"]
-        else:
-            response = response.json()
+        try:
+            if "hydra:member" in response.json():
+                response = response.json()["hydra:member"]
+            else:
+                response = response.json()
+        except JSONDecodeError:
+            self.logger.error(f"Error decoding JSON response: {response.text}")
+            return []
 
         # if response is not a list, check for errors
         if not isinstance(response, list) and "hydra:description" in response:
             self.logger.info(
                 f"{response['hydra:title']}: {response['hydra:description']}"
             )
             return []
@@ -263,28 +273,30 @@
         if end_date is None:
             end_date = start_date + timedelta(days=timed_days)
 
         for current_date, end_date in generate_loop(start_date, end_date, timed_days):
             for point in points:
                 # Check if is valid request
                 for type in types:
-                    if (
-                        not is_valid_request(
-                            activity, classification, granularity, point, type
-                        )
-                        and not self._force_invalid_request
+                    if not is_valid_request(
+                        activity, classification, granularity, point, type
                     ):
+                        if not self._force_invalid_request:
+                            self.logger.debug(
+                                f"Not forcing invalid request for {NED_POINTS.inverse[point]} - {NED_TYPES.inverse[type]}."
+                            )
+                            continue
+                        else:
+                            self.logger.debug(
+                                f"Forcing invalid request for {NED_POINTS.inverse[point]} - {NED_TYPES.inverse[type]}."
+                            )
+                    else:
                         self.logger.debug(
-                            f"Not forcing invalid request for {NED_POINTS.inverse[point]} - {NED_TYPES.inverse[type]}."
+                            f"Valid request for {NED_POINTS.inverse[point]} - {NED_TYPES.inverse[type]}."
                         )
-                        continue
-
-                    self.logger.debug(
-                        f"Valid request for {NED_POINTS.inverse[point]} - {NED_TYPES.inverse[type]}."
-                    )
 
                     params = {
                         "itemsPerPage": self.MAX_ITEMS_PER_PAGE,
                         "point": point,
                         "type": type,
                         "classification": classification,
                         "granularity": granularity,
@@ -321,23 +333,23 @@
 
             # Sleep for self._sleep_time seconds to avoid rate limiting
             self.logger.debug(
                 f"Sleeping for {self._sleep_time} seconds to avoid API rate limits."
             )
             time.sleep(self._sleep_time)
 
-    def get_forecast(self):
+    def get_backcast(self):
         """
-        Placeholder function for getting forecast data. Currently not implemented.
+        Placeholder function for getting backcast data. Currently not implemented.
 
         Raises:
         NotImplementedError: Always raises this exception since the function is not yet implemented.
         """
 
-        raise NotImplementedError("Forecast is not yet implemented.")
+        raise NotImplementedError("Backcast is not yet implemented.")
 
     def get_request(
         self,
         granularity: int,
         classification: str,
         activity: str,
         start_date: datetime,
@@ -406,14 +418,58 @@
             start_date,
             end_date,
             granularitytimezone,
             types,
             points,
         )
 
+    def get_forecast(
+        self,
+        granularity: str,
+        start_date: datetime,
+        end_date: Optional[datetime] = None,
+        granularitytimezone: str = "CET (Central European Time)",
+        types: Optional[List[str]] = ["Solar", "Wind", "WindOffshore", "WindOffshoreC"],
+        points: Optional[List[str]] = [
+            "Nederland",
+            "Groningen",
+            "Friesland",
+            "Drenthe",
+            "Overijssel",
+            "Flevoland",
+            "Gelderland",
+            "Utrecht",
+            "Noord-Holland",
+            "Zuid-Holland",
+            "Zeeland",
+            "Noord-Brabant",
+            "Limburg",
+            "Offshore",
+            "Windpark Luchterduinen",
+            "Windpark Princes Amalia",
+            "Windpark Egmond aan Zee",
+            "Windpark Gemini",
+            "Windpark Borselle I&II",
+            "Windpark Borselle III&IV",
+            "Windpark Hollandse Kust Zuid",
+            "Windpark Hollandse Kust Noord",
+        ],
+    ) -> Union[pd.DataFrame, List[dict]]:
+
+        return self.get_request(
+            granularity,
+            "Forecast",
+            "Providing",
+            start_date,
+            end_date,
+            granularitytimezone,
+            types,
+            points,
+        )
+
     def get_production_provinces(
         self,
         granularity: str,
         start_date: datetime,
         end_date: Optional[datetime] = None,
         granularitytimezone: str = "CET (Central European Time)",
         types: Optional[List[str]] = ["Wind", "Solar"],
```

### Comparing `ned-py-0.2/ned_py.egg-info/PKG-INFO` & `ned-py-0.3/ned_py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ned-py
-Version: 0.2
+Version: 0.3
 Summary: Python wrapper for Nationaal Energie Dashboard API.
 Home-page: https://github.com/profiteia/ned-py
 Author: Profiteia
 Author-email: victor@profiteia.io
 License: MIT
 Project-URL: Source, https://github.com/profiteia/ned-py
 Project-URL: Documentation, https://github.com/profiteia/ned-py
```

### Comparing `ned-py-0.2/setup.py` & `ned-py-0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ned-py",
-    version="0.2",
+    version="0.3",
     packages=find_packages(),
     description="Python wrapper for Nationaal Energie Dashboard API.",
     long_description="Receive and parse data from the Nationaal Energie Dashboard (ned.nl).",
     author="Profiteia",
     author_email="victor@profiteia.io",
     license="MIT",
     classifiers=[
```

### Comparing `ned-py-0.2/tests/test_ned.py` & `ned-py-0.3/tests/test_ned.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 import time
 import pytest
 
 
 @pytest.fixture(autouse=True)
 def sleep_before_test():
-    # Sleep for 5 seconds before each test
+    # Sleep before each test
     time.sleep(5)
 
 
 def get_api_key():
     api_key = os.environ.get("NED_API_KEY")
 
     if api_key is None:
@@ -24,14 +24,18 @@
 
 def test_api_key():
     get_api_key()
     assert True
 
 
 nedapi = ned.NedAPI(get_api_key())
+nedapi.log_level = "DEBUG"
+nedapi.sleep_time = 5
+nedapi.pretty_print = False
+nedapi.force_invalid_request = False
 
 
 def test_metadata_types():
     from ned import metadata
 
     assert type(metadata.NED_ACTIVITIES == bidict) and len(metadata.NED_ACTIVITIES) > 0
     assert (
@@ -60,95 +64,104 @@
     )
     assert type(metadata.NED_POINTS == bidict) and len(metadata.NED_POINTS) > 0
     assert type(metadata.NED_TYPES == bidict) and len(metadata.NED_TYPES) > 0
 
 
 def test_authorisations():
     nedapi.as_dataframe = False
-    nedapi.pretty_print = False
-    nedapi.force_invalid_request = False
+
     result = nedapi.authorisations()
     assert type(result) == list and len(result) > 0
 
 
 def test_authorisations_df():
     nedapi.as_dataframe = True
-    nedapi.pretty_print = False
-    nedapi.force_invalid_request = False
+
     result = nedapi.authorisations()
     assert type(result) == pd.DataFrame and not result.empty
 
 
 def test_users():
     nedapi.as_dataframe = False
-    nedapi.pretty_print = False
-    nedapi.force_invalid_request = False
+
     result = nedapi.users()
     assert type(result) == list and len(result) > 0
 
 
 def test_users_df():
     nedapi.as_dataframe = True
-    nedapi.pretty_print = False
-    nedapi.force_invalid_request = False
+
     result = nedapi.users()
     assert type(result) == pd.DataFrame and not result.empty
 
 
 def test_production_netherlands():
     nedapi.as_dataframe = False
-    nedapi.pretty_print = False
-    nedapi.force_invalid_request = False
+
     result = nedapi.get_production_netherlands(
         "15 minutes", pd.Timestamp(2024, 1, 1), pd.Timestamp(2024, 1, 2)
     )
     assert type(result) == list and len(result) > 0
 
 
 def test_production_netherlands_df():
     nedapi.as_dataframe = True
-    nedapi.pretty_print = False
-    nedapi.force_invalid_request = False
+
     result = nedapi.get_production_netherlands(
         "15 minutes", pd.Timestamp(2024, 1, 1), pd.Timestamp(2024, 1, 2)
     )
     assert type(result) == pd.DataFrame and not result.empty
 
 
 def test_production_offshore():
     nedapi.as_dataframe = False
-    nedapi.pretty_print = False
-    nedapi.force_invalid_request = False
+
     result = nedapi.get_production_offshore(
         "15 minutes", pd.Timestamp(2024, 1, 1), pd.Timestamp(2024, 1, 2)
     )
     assert type(result) == list and len(result) > 0
 
 
 def test_production_offshore_df():
     nedapi.as_dataframe = True
-    nedapi.pretty_print = False
-    nedapi.force_invalid_request = False
+
     result = nedapi.get_production_offshore(
         "15 minutes", pd.Timestamp(2024, 1, 1), pd.Timestamp(2024, 1, 2)
     )
     assert type(result) == pd.DataFrame and not result.empty
 
 
 def test_consumption():
     nedapi.as_dataframe = False
-    nedapi.pretty_print = False
-    nedapi.force_invalid_request = False
+
     result = nedapi.get_consumption(
         "15 minutes", pd.Timestamp(2024, 1, 1), pd.Timestamp(2024, 1, 2)
     )
     assert type(result) == list and len(result) > 0
 
 
 def test_consumption_df():
     nedapi.as_dataframe = True
-    nedapi.pretty_print = False
-    nedapi.force_invalid_request = False
+
     result = nedapi.get_consumption(
         "15 minutes", pd.Timestamp(2024, 1, 1), pd.Timestamp(2024, 1, 2)
     )
     assert type(result) == pd.DataFrame and not result.empty
+
+
+def test_forecast():
+    nedapi.as_dataframe = False
+
+    nedapi.sleep_time = 5
+    result = nedapi.get_forecast(
+        "15 minutes", pd.Timestamp(2024, 1, 1), pd.Timestamp(2024, 1, 2)
+    )
+    assert type(result) == list and len(result) > 0
+
+
+def test_forecast_df():
+    nedapi.as_dataframe = True
+
+    result = nedapi.get_forecast(
+        "15 minutes", pd.Timestamp(2024, 1, 1), pd.Timestamp(2024, 1, 2)
+    )
+    assert type(result) == pd.DataFrame and not result.empty
```

