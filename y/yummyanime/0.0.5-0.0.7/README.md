# Comparing `tmp/yummyanime-0.0.5.tar.gz` & `tmp/yummyanime-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yummyanime-0.0.5.tar", last modified: Wed Apr 24 18:24:23 2024, max compression
+gzip compressed data, was "yummyanime-0.0.7.tar", last modified: Wed Apr 24 19:08:29 2024, max compression
```

## Comparing `yummyanime-0.0.5.tar` & `yummyanime-0.0.7.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 im        (1000) im        (1000)        0 2024-04-24 18:24:23.692712 yummyanime-0.0.5/
--rw-r--r--   0 im        (1000) im        (1000)     1052 2024-04-24 16:23:58.000000 yummyanime-0.0.5/LICENSE
--rw-r--r--   0 im        (1000) im        (1000)     1428 2024-04-24 18:24:23.692712 yummyanime-0.0.5/PKG-INFO
--rw-r--r--   0 im        (1000) im        (1000)      925 2024-04-24 16:50:52.000000 yummyanime-0.0.5/README.md
--rw-r--r--   0 im        (1000) im        (1000)      582 2024-04-24 18:24:21.000000 yummyanime-0.0.5/pyproject.toml
--rw-r--r--   0 im        (1000) im        (1000)       52 2024-04-24 17:42:27.000000 yummyanime-0.0.5/requirements.txt
--rw-r--r--   0 im        (1000) im        (1000)       38 2024-04-24 18:24:23.692712 yummyanime-0.0.5/setup.cfg
-drwxr-xr-x   0 im        (1000) im        (1000)        0 2024-04-24 18:24:23.689379 yummyanime-0.0.5/src/
-drwxr-xr-x   0 im        (1000) im        (1000)        0 2024-04-24 18:24:23.689379 yummyanime-0.0.5/src/yummyanime/
--rw-r--r--   0 im        (1000) im        (1000)       96 2024-04-24 18:24:21.000000 yummyanime-0.0.5/src/yummyanime/__init__.py
--rw-r--r--   0 im        (1000) im        (1000)     7208 2024-04-24 13:04:20.000000 yummyanime-0.0.5/src/yummyanime/api.py
--rw-r--r--   0 im        (1000) im        (1000)       98 2024-04-24 10:36:59.000000 yummyanime-0.0.5/src/yummyanime/enums.py
--rw-r--r--   0 im        (1000) im        (1000)     1497 2024-04-24 11:18:04.000000 yummyanime-0.0.5/src/yummyanime/exceptions.py
-drwxr-xr-x   0 im        (1000) im        (1000)        0 2024-04-24 18:24:23.692712 yummyanime-0.0.5/src/yummyanime/parsers/
--rw-r--r--   0 im        (1000) im        (1000)      293 2024-04-24 15:51:27.000000 yummyanime-0.0.5/src/yummyanime/parsers/__init__.py
--rw-r--r--   0 im        (1000) im        (1000)     2779 2024-04-24 15:43:25.000000 yummyanime-0.0.5/src/yummyanime/parsers/abstract_parser.py
-drwxr-xr-x   0 im        (1000) im        (1000)        0 2024-04-24 18:24:23.692712 yummyanime-0.0.5/src/yummyanime/parsers/kodik/
--rw-r--r--   0 im        (1000) im        (1000)       40 2023-12-14 14:26:59.000000 yummyanime-0.0.5/src/yummyanime/parsers/kodik/__init__.py
--rw-r--r--   0 im        (1000) im        (1000)     4257 2024-04-24 16:08:09.000000 yummyanime-0.0.5/src/yummyanime/parsers/kodik/downloader.py
--rw-r--r--   0 im        (1000) im        (1000)      213 2024-04-24 15:43:25.000000 yummyanime-0.0.5/src/yummyanime/parsers/utils.py
-drwxr-xr-x   0 im        (1000) im        (1000)        0 2024-04-24 18:24:23.692712 yummyanime-0.0.5/src/yummyanime/routes/
--rw-r--r--   0 im        (1000) im        (1000)       24 2024-04-24 10:55:08.000000 yummyanime-0.0.5/src/yummyanime/routes/__init__.py
--rw-r--r--   0 im        (1000) im        (1000)      410 2024-04-24 12:56:37.000000 yummyanime-0.0.5/src/yummyanime/routes/_abs.py
--rw-r--r--   0 im        (1000) im        (1000)     2955 2024-04-24 14:50:41.000000 yummyanime-0.0.5/src/yummyanime/routes/anime.py
--rw-r--r--   0 im        (1000) im        (1000)      170 2024-04-24 16:31:16.000000 yummyanime-0.0.5/src/yummyanime/routes/trailers.py
-drwxr-xr-x   0 im        (1000) im        (1000)        0 2024-04-24 18:24:23.692712 yummyanime-0.0.5/src/yummyanime/structs/
--rw-r--r--   0 im        (1000) im        (1000)       87 2024-04-24 14:57:06.000000 yummyanime-0.0.5/src/yummyanime/structs/__init__.py
--rw-r--r--   0 im        (1000) im        (1000)     3233 2024-04-24 15:32:44.000000 yummyanime-0.0.5/src/yummyanime/structs/_base.py
--rw-r--r--   0 im        (1000) im        (1000)      486 2024-04-24 16:31:16.000000 yummyanime-0.0.5/src/yummyanime/structs/_enums.py
--rw-r--r--   0 im        (1000) im        (1000)     6276 2024-04-24 15:21:49.000000 yummyanime-0.0.5/src/yummyanime/structs/anime.py
--rw-r--r--   0 im        (1000) im        (1000)      459 2024-04-24 16:31:16.000000 yummyanime-0.0.5/src/yummyanime/structs/trailers.py
--rw-r--r--   0 im        (1000) im        (1000)     1083 2024-04-24 16:31:16.000000 yummyanime-0.0.5/src/yummyanime/structs/video.py
-drwxr-xr-x   0 im        (1000) im        (1000)        0 2024-04-24 18:24:23.692712 yummyanime-0.0.5/src/yummyanime.egg-info/
--rw-r--r--   0 im        (1000) im        (1000)     1428 2024-04-24 18:24:23.000000 yummyanime-0.0.5/src/yummyanime.egg-info/PKG-INFO
--rw-r--r--   0 im        (1000) im        (1000)      861 2024-04-24 18:24:23.000000 yummyanime-0.0.5/src/yummyanime.egg-info/SOURCES.txt
--rw-r--r--   0 im        (1000) im        (1000)        1 2024-04-24 18:24:23.000000 yummyanime-0.0.5/src/yummyanime.egg-info/dependency_links.txt
--rw-r--r--   0 im        (1000) im        (1000)       52 2024-04-24 18:24:23.000000 yummyanime-0.0.5/src/yummyanime.egg-info/requires.txt
--rw-r--r--   0 im        (1000) im        (1000)       11 2024-04-24 18:24:23.000000 yummyanime-0.0.5/src/yummyanime.egg-info/top_level.txt
+drwxr-xr-x   0 im        (1000) im        (1000)        0 2024-04-24 19:08:29.577181 yummyanime-0.0.7/
+-rw-r--r--   0 im        (1000) im        (1000)     1052 2024-04-24 16:23:58.000000 yummyanime-0.0.7/LICENSE
+-rw-r--r--   0 im        (1000) im        (1000)     1428 2024-04-24 19:08:29.577181 yummyanime-0.0.7/PKG-INFO
+-rw-r--r--   0 im        (1000) im        (1000)      925 2024-04-24 16:50:52.000000 yummyanime-0.0.7/README.md
+-rw-r--r--   0 im        (1000) im        (1000)      582 2024-04-24 19:08:27.000000 yummyanime-0.0.7/pyproject.toml
+-rw-r--r--   0 im        (1000) im        (1000)       52 2024-04-24 17:42:27.000000 yummyanime-0.0.7/requirements.txt
+-rw-r--r--   0 im        (1000) im        (1000)       38 2024-04-24 19:08:29.577181 yummyanime-0.0.7/setup.cfg
+drwxr-xr-x   0 im        (1000) im        (1000)        0 2024-04-24 19:08:29.577181 yummyanime-0.0.7/src/
+drwxr-xr-x   0 im        (1000) im        (1000)        0 2024-04-24 19:08:29.577181 yummyanime-0.0.7/src/yummyanime/
+-rw-r--r--   0 im        (1000) im        (1000)       96 2024-04-24 19:08:27.000000 yummyanime-0.0.7/src/yummyanime/__init__.py
+-rw-r--r--   0 im        (1000) im        (1000)     7248 2024-04-24 19:03:11.000000 yummyanime-0.0.7/src/yummyanime/api.py
+-rw-r--r--   0 im        (1000) im        (1000)       98 2024-04-24 10:36:59.000000 yummyanime-0.0.7/src/yummyanime/enums.py
+-rw-r--r--   0 im        (1000) im        (1000)     1497 2024-04-24 11:18:04.000000 yummyanime-0.0.7/src/yummyanime/exceptions.py
+drwxr-xr-x   0 im        (1000) im        (1000)        0 2024-04-24 19:08:29.577181 yummyanime-0.0.7/src/yummyanime/parsers/
+-rw-r--r--   0 im        (1000) im        (1000)      293 2024-04-24 15:51:27.000000 yummyanime-0.0.7/src/yummyanime/parsers/__init__.py
+-rw-r--r--   0 im        (1000) im        (1000)     2779 2024-04-24 15:43:25.000000 yummyanime-0.0.7/src/yummyanime/parsers/abstract_parser.py
+drwxr-xr-x   0 im        (1000) im        (1000)        0 2024-04-24 19:08:29.577181 yummyanime-0.0.7/src/yummyanime/parsers/kodik/
+-rw-r--r--   0 im        (1000) im        (1000)       40 2023-12-14 14:26:59.000000 yummyanime-0.0.7/src/yummyanime/parsers/kodik/__init__.py
+-rw-r--r--   0 im        (1000) im        (1000)     4257 2024-04-24 16:08:09.000000 yummyanime-0.0.7/src/yummyanime/parsers/kodik/downloader.py
+-rw-r--r--   0 im        (1000) im        (1000)      213 2024-04-24 15:43:25.000000 yummyanime-0.0.7/src/yummyanime/parsers/utils.py
+drwxr-xr-x   0 im        (1000) im        (1000)        0 2024-04-24 19:08:29.577181 yummyanime-0.0.7/src/yummyanime/routes/
+-rw-r--r--   0 im        (1000) im        (1000)       49 2024-04-24 19:03:11.000000 yummyanime-0.0.7/src/yummyanime/routes/__init__.py
+-rw-r--r--   0 im        (1000) im        (1000)      410 2024-04-24 12:56:37.000000 yummyanime-0.0.7/src/yummyanime/routes/_abs.py
+-rw-r--r--   0 im        (1000) im        (1000)     2955 2024-04-24 14:50:41.000000 yummyanime-0.0.7/src/yummyanime/routes/anime.py
+-rw-r--r--   0 im        (1000) im        (1000)      170 2024-04-24 16:31:16.000000 yummyanime-0.0.7/src/yummyanime/routes/trailers.py
+-rw-r--r--   0 im        (1000) im        (1000)      193 2024-04-24 19:08:26.000000 yummyanime-0.0.7/src/yummyanime/routes/users.py
+drwxr-xr-x   0 im        (1000) im        (1000)        0 2024-04-24 19:08:29.577181 yummyanime-0.0.7/src/yummyanime/structs/
+-rw-r--r--   0 im        (1000) im        (1000)       87 2024-04-24 14:57:06.000000 yummyanime-0.0.7/src/yummyanime/structs/__init__.py
+-rw-r--r--   0 im        (1000) im        (1000)     3233 2024-04-24 15:32:44.000000 yummyanime-0.0.7/src/yummyanime/structs/_base.py
+-rw-r--r--   0 im        (1000) im        (1000)      486 2024-04-24 16:31:16.000000 yummyanime-0.0.7/src/yummyanime/structs/_enums.py
+-rw-r--r--   0 im        (1000) im        (1000)     6276 2024-04-24 15:21:49.000000 yummyanime-0.0.7/src/yummyanime/structs/anime.py
+-rw-r--r--   0 im        (1000) im        (1000)      459 2024-04-24 16:31:16.000000 yummyanime-0.0.7/src/yummyanime/structs/trailers.py
+-rw-r--r--   0 im        (1000) im        (1000)      903 2024-04-24 19:03:11.000000 yummyanime-0.0.7/src/yummyanime/structs/user.py
+-rw-r--r--   0 im        (1000) im        (1000)     1083 2024-04-24 16:31:16.000000 yummyanime-0.0.7/src/yummyanime/structs/video.py
+drwxr-xr-x   0 im        (1000) im        (1000)        0 2024-04-24 19:08:29.577181 yummyanime-0.0.7/src/yummyanime.egg-info/
+-rw-r--r--   0 im        (1000) im        (1000)     1428 2024-04-24 19:08:29.000000 yummyanime-0.0.7/src/yummyanime.egg-info/PKG-INFO
+-rw-r--r--   0 im        (1000) im        (1000)      923 2024-04-24 19:08:29.000000 yummyanime-0.0.7/src/yummyanime.egg-info/SOURCES.txt
+-rw-r--r--   0 im        (1000) im        (1000)        1 2024-04-24 19:08:29.000000 yummyanime-0.0.7/src/yummyanime.egg-info/dependency_links.txt
+-rw-r--r--   0 im        (1000) im        (1000)       52 2024-04-24 19:08:29.000000 yummyanime-0.0.7/src/yummyanime.egg-info/requires.txt
+-rw-r--r--   0 im        (1000) im        (1000)       11 2024-04-24 19:08:29.000000 yummyanime-0.0.7/src/yummyanime.egg-info/top_level.txt
```

### Comparing `yummyanime-0.0.5/LICENSE` & `yummyanime-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yummyanime-0.0.5/PKG-INFO` & `yummyanime-0.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yummyanime
-Version: 0.0.5
+Version: 0.0.7
 Summary: Yummy Anime API wrapper
 Author-email: "IM.Corp" <root@yummyani.me>
 Project-URL: Homepage, https://yummyani.me/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `yummyanime-0.0.5/README.md` & `yummyanime-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `yummyanime-0.0.5/pyproject.toml` & `yummyanime-0.0.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "yummyanime"
-version = "0.0.5"
+version = "0.0.7"
 authors = [
   { name="IM.Corp", email="root@yummyani.me" },
 ]
 dynamic = ["dependencies"]
 description = "Yummy Anime API wrapper"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `yummyanime-0.0.5/src/yummyanime/api.py` & `yummyanime-0.0.7/src/yummyanime/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Callable
 
 import aiohttp
 import json5
 
 from .enums import Format
 from .exceptions import YummyAPIError, YummyError, YummyRateLimitError, YummyNotFoundError, YummyResponseParseFailed
-from .routes import Anime
+from .routes import Anime, Users
 from .structs import YummyAnswer, Timing, AbsDict
 
 
 class YummyApi:
     """
     The YummyApi class is used to interact with the Yummy API.
     It provides methods for making HTTP requests to the API's endpoints.
@@ -37,14 +37,15 @@
         """
         self._format = format
         self._x_application = x_application_token
         self.api_gateway = api_gateway
         self._accept = accept
         self._custom_headers = custom_headers or {}
         self.anime = Anime(self)
+        self.users = Users(self)
         self.token = user_token
 
     async def method(self, path: str, method: str, data: dict | None = None, retry_count: int = 3,
                      type: Any = None) -> Any:
         """
         Makes an HTTP request to the specified path.
```

### Comparing `yummyanime-0.0.5/src/yummyanime/exceptions.py` & `yummyanime-0.0.7/src/yummyanime/exceptions.py`

 * *Files identical despite different names*

### Comparing `yummyanime-0.0.5/src/yummyanime/parsers/abstract_parser.py` & `yummyanime-0.0.7/src/yummyanime/parsers/abstract_parser.py`

 * *Files identical despite different names*

### Comparing `yummyanime-0.0.5/src/yummyanime/parsers/kodik/downloader.py` & `yummyanime-0.0.7/src/yummyanime/parsers/kodik/downloader.py`

 * *Files identical despite different names*

### Comparing `yummyanime-0.0.5/src/yummyanime/routes/anime.py` & `yummyanime-0.0.7/src/yummyanime/routes/anime.py`

 * *Files identical despite different names*

### Comparing `yummyanime-0.0.5/src/yummyanime/structs/_base.py` & `yummyanime-0.0.7/src/yummyanime/structs/_base.py`

 * *Files identical despite different names*

### Comparing `yummyanime-0.0.5/src/yummyanime/structs/anime.py` & `yummyanime-0.0.7/src/yummyanime/structs/anime.py`

 * *Files identical despite different names*

### Comparing `yummyanime-0.0.5/src/yummyanime/structs/video.py` & `yummyanime-0.0.7/src/yummyanime/structs/video.py`

 * *Files identical despite different names*

### Comparing `yummyanime-0.0.5/src/yummyanime.egg-info/PKG-INFO` & `yummyanime-0.0.7/src/yummyanime.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yummyanime
-Version: 0.0.5
+Version: 0.0.7
 Summary: Yummy Anime API wrapper
 Author-email: "IM.Corp" <root@yummyani.me>
 Project-URL: Homepage, https://yummyani.me/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `yummyanime-0.0.5/src/yummyanime.egg-info/SOURCES.txt` & `yummyanime-0.0.7/src/yummyanime.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -16,13 +16,15 @@
 src/yummyanime/parsers/utils.py
 src/yummyanime/parsers/kodik/__init__.py
 src/yummyanime/parsers/kodik/downloader.py
 src/yummyanime/routes/__init__.py
 src/yummyanime/routes/_abs.py
 src/yummyanime/routes/anime.py
 src/yummyanime/routes/trailers.py
+src/yummyanime/routes/users.py
 src/yummyanime/structs/__init__.py
 src/yummyanime/structs/_base.py
 src/yummyanime/structs/_enums.py
 src/yummyanime/structs/anime.py
 src/yummyanime/structs/trailers.py
+src/yummyanime/structs/user.py
 src/yummyanime/structs/video.py
```

