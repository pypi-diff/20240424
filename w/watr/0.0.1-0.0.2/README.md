# Comparing `tmp/watr-0.0.1.tar.gz` & `tmp/watr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watr-0.0.1.tar", last modified: Mon Apr  1 19:06:15 2024, max compression
+gzip compressed data, was "watr-0.0.2.tar", last modified: Wed Apr 24 16:45:28 2024, max compression
```

## Comparing `watr-0.0.1.tar` & `watr-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2024-04-01 19:06:15.834489 watr-0.0.1/
--rw-r--r--   0 gcpease  (1709703766) 1389146880      996 2024-04-01 19:06:15.834149 watr-0.0.1/PKG-INFO
--rw-r--r--   0 gcpease  (1709703766) 1389146880      559 2024-04-01 16:11:29.000000 watr-0.0.1/README.md
--rw-r--r--   0 gcpease  (1709703766) 1389146880       84 2024-03-31 17:29:21.000000 watr-0.0.1/pyproject.toml
--rw-r--r--   0 gcpease  (1709703766) 1389146880      593 2024-04-01 19:06:15.837254 watr-0.0.1/setup.cfg
--rw-r--r--   0 gcpease  (1709703766) 1389146880       68 2024-03-31 17:30:54.000000 watr-0.0.1/setup.py
-drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2024-04-01 19:06:15.795278 watr-0.0.1/src/
-drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2024-04-01 19:06:15.826446 watr-0.0.1/src/watr/
--rw-r--r--   0 gcpease  (1709703766) 1389146880      205 2024-04-01 16:00:25.000000 watr-0.0.1/src/watr/__init__.py
--rw-r--r--   0 gcpease  (1709703766) 1389146880     1169 2024-04-01 16:00:25.000000 watr-0.0.1/src/watr/entity.py
--rw-r--r--   0 gcpease  (1709703766) 1389146880      316 2024-03-31 21:51:05.000000 watr-0.0.1/src/watr/util.py
--rw-r--r--   0 gcpease  (1709703766) 1389146880    10449 2024-04-01 15:59:48.000000 watr-0.0.1/src/watr/watrapi.py
--rw-r--r--   0 gcpease  (1709703766) 1389146880      292 2024-04-01 15:59:48.000000 watr-0.0.1/src/watr/watrexceptions.py
--rw-r--r--   0 gcpease  (1709703766) 1389146880     3335 2024-04-01 15:57:42.000000 watr-0.0.1/src/watr/watrsprinklersystem.py
--rw-r--r--   0 gcpease  (1709703766) 1389146880     1531 2024-04-01 15:59:05.000000 watr-0.0.1/src/watr/watrsystem.py
--rw-r--r--   0 gcpease  (1709703766) 1389146880     3425 2024-04-01 15:56:17.000000 watr-0.0.1/src/watr/watrzone.py
-drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2024-04-01 19:06:15.833462 watr-0.0.1/src/watr.egg-info/
--rw-r--r--   0 gcpease  (1709703766) 1389146880      996 2024-04-01 19:06:15.000000 watr-0.0.1/src/watr.egg-info/PKG-INFO
--rw-r--r--   0 gcpease  (1709703766) 1389146880      351 2024-04-01 19:06:15.000000 watr-0.0.1/src/watr.egg-info/SOURCES.txt
--rw-r--r--   0 gcpease  (1709703766) 1389146880        1 2024-04-01 19:06:15.000000 watr-0.0.1/src/watr.egg-info/dependency_links.txt
--rw-r--r--   0 gcpease  (1709703766) 1389146880        5 2024-04-01 19:06:15.000000 watr-0.0.1/src/watr.egg-info/top_level.txt
+drwxr-xr-x   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)        0 2024-04-24 16:45:28.847182 watr-0.0.2/
+-rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)     1173 2024-04-24 16:45:28.846948 watr-0.0.2/PKG-INFO
+-rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)      736 2024-04-07 03:44:00.000000 watr-0.0.2/README.md
+-rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)       84 2024-03-31 17:29:21.000000 watr-0.0.2/pyproject.toml
+-rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)      593 2024-04-24 16:45:28.848628 watr-0.0.2/setup.cfg
+-rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)       68 2024-03-31 17:30:54.000000 watr-0.0.2/setup.py
+drwxr-xr-x   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)        0 2024-04-24 16:45:28.807577 watr-0.0.2/src/
+drwxr-xr-x   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)        0 2024-04-24 16:45:28.839892 watr-0.0.2/src/watr/
+-rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)      429 2024-04-07 03:40:25.000000 watr-0.0.2/src/watr/WatrEntity.py
+-rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)      240 2024-04-07 03:40:25.000000 watr-0.0.2/src/watr/__init__.py
+-rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)     1169 2024-04-01 16:00:25.000000 watr-0.0.2/src/watr/entity.py
+-rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)      316 2024-03-31 21:51:05.000000 watr-0.0.2/src/watr/util.py
+-rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)    10495 2024-04-07 03:40:25.000000 watr-0.0.2/src/watr/watrapi.py
+-rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)      292 2024-04-01 15:59:48.000000 watr-0.0.2/src/watr/watrexceptions.py
+-rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)     2977 2024-04-07 03:40:25.000000 watr-0.0.2/src/watr/watrsprinklersystem.py
+-rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)     1531 2024-04-01 15:59:05.000000 watr-0.0.2/src/watr/watrsystem.py
+-rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)     3105 2024-04-07 03:40:25.000000 watr-0.0.2/src/watr/watrzone.py
+drwxr-xr-x   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)        0 2024-04-24 16:45:28.846440 watr-0.0.2/src/watr.egg-info/
+-rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)     1173 2024-04-24 16:45:28.000000 watr-0.0.2/src/watr.egg-info/PKG-INFO
+-rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)      374 2024-04-24 16:45:28.000000 watr-0.0.2/src/watr.egg-info/SOURCES.txt
+-rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)        1 2024-04-24 16:45:28.000000 watr-0.0.2/src/watr.egg-info/dependency_links.txt
+-rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)        5 2024-04-24 16:45:28.000000 watr-0.0.2/src/watr.egg-info/top_level.txt
```

### Comparing `watr-0.0.1/PKG-INFO` & `watr-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-Metadata-Version: 2.1
-Name: watr
-Version: 0.0.1
-Summary: A python library to control a Watr system
-Home-page: https://capstone-cs.eng.utah.edu/Watr
-Author: Watr
-Author-email: watr@peasenet.com.com
-Project-URL: Bug Tracker, https://capstone-cs.eng.utah.edu/Watr/Watr/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
-# Watr Python
+# Watr Python 1.0.0
 
 A python library for the Watr API.
 
 ## Installation
 
 ```pip3 install watr```
 
+## Requirements
+
+- Python 3.6+
+
 ## Usage
 
 ```python
 from watr import WatrApi
 
 # some await things here...
-
 watrApi = WatrApi("your@email.com", "yourpassword123")
-
 # or if you have tokens already
 watrApi = WatrApi(access_token="youraccesstoken", refresh_token="yourrefreshtoken")
 watrSystem = WatrSystem({}, watrApi)
 sprinkler_systems = watrSystem.get_systems()
 home_system = sprinkler_systems[0]
 if home_system.enabled():
     sprinkler_systems[0].toggle()
 sprinkler_systems[0].zones[0].toggle()
 ```
+
+## Documentation
+
+More indepth documentation is available
+at [https://watr.peasenet.com/docs/python](https://watr.peasenet.com/docs/python)
```

### Comparing `watr-0.0.1/setup.cfg` & `watr-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = watr
-version = 0.0.1
+version = 0.0.2
 author = Watr
 author_email = watr@peasenet.com.com
 description = A python library to control a Watr system
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://capstone-cs.eng.utah.edu/Watr
 project_urls =
```

### Comparing `watr-0.0.1/src/watr/entity.py` & `watr-0.0.2/src/watr/entity.py`

 * *Files identical despite different names*

### Comparing `watr-0.0.1/src/watr/watrapi.py` & `watr-0.0.2/src/watr/watrapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,17 +87,17 @@
         :return: True if the token was refreshed, False otherwise.
         """
         data = {
             "refreshToken": self.__refresh_token,
             "accessToken": self.__access_token
         }
         resp = await self.__post(API_ACCOUNT_REFRESH, data)
-        if resp:
-            self.__access_token = resp["accessToken"]
-            self.__refresh_token = resp["refreshToken"]
+        if resp and resp["success"]:
+            self.__access_token = resp["newTokens"]["accessToken"]
+            self.__refresh_token = resp["newTokens"]["refreshToken"]
             _LOGGER.debug("Token refreshed")
             data = {
                 "accessToken": self.__access_token,
                 "refreshToken": self.__refresh_token
             }
             self.emit("token_refresh", data)
             return True
```

### Comparing `watr-0.0.1/src/watr/watrsprinklersystem.py` & `watr-0.0.2/src/watr/watrsprinklersystem.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
-from .entity import Entity
+from .WatrEntity import WatrEntity
 from .watrapi import WatrApi
 from .watrzone import WatrZone
 from .util import first_or_none
 
 _LOGGER = logging.getLogger(__name__)
 
 
-class WatrSprinklerSystem(Entity):
+class WatrSprinklerSystem(WatrEntity):
     """
     A class representing a sprinkler system which contains a collection of zones.
     """
 
     def __init__(self, data: dict, api: WatrApi, system):
         self.__system = system
         super().__init__(data)
@@ -29,30 +29,14 @@
         """
         Returns the zones for the system.
         :return: the zones for the system.
         """
         return self.__zones
 
     @property
-    def id(self) -> str:
-        """
-        Returns the id of the system.
-        :return: the id of the system.
-        """
-        return self.data["id"]
-
-    @property
-    def name(self) -> str:
-        """
-        Returns the name of the system.
-        :return: The name of the system.
-        """
-        return self.data["name"]
-
-    @property
     def events(self) -> list | None:
         """
         Returns the events for the system.
         :return: The events for the system.
         """
         return self.data["events"]
 
@@ -105,20 +89,20 @@
         if system_data is None:
             return
         self.update_data(system_data)
         for z in system_data["zones"]:
             # if the zone is not in the list of zones, add it
             _zone = first_or_none(self.zones, lambda _zz: _zz.id == z["id"])
             if not _zone:
-                self.__zones.append(WatrZone(self.__api, z, self.__system))
+                self.__zones.append(WatrZone(self.__api, z, self))
             else:
                 _zone.update_data(z)
 
     def __parse_data(self, data: dict) -> None:
         if data is None:
             _LOGGER.error("No data provided to parse")
             return
         # self.__zones = data["zones"]
         for z in data["zones"]:
-            self.__zones.append(WatrZone(self.__api, z, self.__system))
+            self.__zones.append(WatrZone(self.__api, z, self))
         self.__events = data["events"]
         self.__schedules = data["schedules"]
```

### Comparing `watr-0.0.1/src/watr/watrsystem.py` & `watr-0.0.2/src/watr/watrsystem.py`

 * *Files identical despite different names*

### Comparing `watr-0.0.1/src/watr/watrzone.py` & `watr-0.0.2/src/watr/watrzone.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
-from .entity import Entity
+from .WatrEntity import WatrEntity
 from .watrapi import WatrApi
 
 _LOGGER = logging.getLogger(__name__)
 
 
-class WatrZone(Entity):
+class WatrZone(WatrEntity):
     """
     A class representing a sprinkler zone.
     """
 
     def __init__(self, api: WatrApi, data: dict, system):
         self.__system = system
         super().__init__(data)
@@ -21,30 +21,14 @@
         self.__time_remaining = 0
         self.__id = ""
         self.__name = ""
         self.__system_id = system.id
         self.__parse_data(data)
 
     @property
-    def name(self) -> str:
-        """
-        Returns the name of the zone.
-        :return: The name of the zone.
-        """
-        return self.__name
-
-    @property
-    def id(self) -> str:
-        """
-        Returns the ID of the zone.
-        :return: The ID of the zone.
-        """
-        return self.__id
-
-    @property
     def is_on(self) -> bool:
         """
         Returns whether the zone is on.
         :return: Whether the zone is on.
         """
         return self.__is_on
```

### Comparing `watr-0.0.1/src/watr.egg-info/PKG-INFO` & `watr-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 Metadata-Version: 2.1
 Name: watr
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python library to control a Watr system
 Home-page: https://capstone-cs.eng.utah.edu/Watr
 Author: Watr
 Author-email: watr@peasenet.com.com
 Project-URL: Bug Tracker, https://capstone-cs.eng.utah.edu/Watr/Watr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-# Watr Python
+# Watr Python 1.0.0
 
 A python library for the Watr API.
 
 ## Installation
 
 ```pip3 install watr```
 
+## Requirements
+
+- Python 3.6+
+
 ## Usage
 
 ```python
 from watr import WatrApi
 
 # some await things here...
-
 watrApi = WatrApi("your@email.com", "yourpassword123")
-
 # or if you have tokens already
 watrApi = WatrApi(access_token="youraccesstoken", refresh_token="yourrefreshtoken")
 watrSystem = WatrSystem({}, watrApi)
 sprinkler_systems = watrSystem.get_systems()
 home_system = sprinkler_systems[0]
 if home_system.enabled():
     sprinkler_systems[0].toggle()
 sprinkler_systems[0].zones[0].toggle()
 ```
+
+## Documentation
+
+More indepth documentation is available
+at [https://watr.peasenet.com/docs/python](https://watr.peasenet.com/docs/python)
```

