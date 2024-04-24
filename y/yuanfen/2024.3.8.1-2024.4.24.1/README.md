# Comparing `tmp/yuanfen-2024.3.8.1.tar.gz` & `tmp/yuanfen-2024.4.24.1.tar.gz`

## Comparing `yuanfen-2024.3.8.1.tar` & `yuanfen-2024.4.24.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 yuanfen-2024.3.8.1/src/yuanfen/__init__.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 yuanfen-2024.3.8.1/src/yuanfen/config.py
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 yuanfen-2024.3.8.1/src/yuanfen/email.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 yuanfen-2024.3.8.1/src/yuanfen/env.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 yuanfen-2024.3.8.1/src/yuanfen/group_robot.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 yuanfen-2024.3.8.1/src/yuanfen/ip.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 yuanfen-2024.3.8.1/src/yuanfen/logger.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 yuanfen-2024.3.8.1/src/yuanfen/redis.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 yuanfen-2024.3.8.1/src/yuanfen/response.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 yuanfen-2024.3.8.1/src/yuanfen/time.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 yuanfen-2024.3.8.1/src/yuanfen/version.py
--rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 yuanfen-2024.3.8.1/.gitignore
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 yuanfen-2024.3.8.1/README.md
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 yuanfen-2024.3.8.1/pyproject.toml
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 yuanfen-2024.3.8.1/PKG-INFO
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/src/yuanfen/__init__.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/src/yuanfen/config.py
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/src/yuanfen/email.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/src/yuanfen/env.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/src/yuanfen/group_robot.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/src/yuanfen/ip.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/src/yuanfen/logger.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/src/yuanfen/redis.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/src/yuanfen/response.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/src/yuanfen/time.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/src/yuanfen/version.py
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/.gitignore
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/README.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/pyproject.toml
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/PKG-INFO
```

### Comparing `yuanfen-2024.3.8.1/src/yuanfen/__init__.py` & `yuanfen-2024.4.24.1/src/yuanfen/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .env import APP_ENV
 from .group_robot import GroupRobot
 from .logger import Logger
 from .redis import Redis
 from .response import BaseResponse, ErrorResponse, SuccessResponse
 from .version import Version
 
-__version__ = "2024.3.8.1"
+__version__ = "2024.4.24.1"
 
 __all__ = [
     "APP_ENV",
     "BaseResponse",
     "Config",
     "Email",
     "ErrorResponse",
```

### Comparing `yuanfen-2024.3.8.1/src/yuanfen/config.py` & `yuanfen-2024.4.24.1/src/yuanfen/config.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.3.8.1/src/yuanfen/email.py` & `yuanfen-2024.4.24.1/src/yuanfen/email.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.3.8.1/src/yuanfen/ip.py` & `yuanfen-2024.4.24.1/src/yuanfen/ip.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.3.8.1/src/yuanfen/logger.py` & `yuanfen-2024.4.24.1/src/yuanfen/logger.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.3.8.1/src/yuanfen/redis.py` & `yuanfen-2024.4.24.1/src/yuanfen/redis.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.3.8.1/src/yuanfen/time.py` & `yuanfen-2024.4.24.1/src/yuanfen/time.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,27 @@
 import time
 from datetime import datetime
 
 import pytz
 
 
-def now():
-    return datetime.now()
+def now(tz: str = "Asia/Shanghai", with_tz: bool = False) -> datetime:
+    now_with_tz = datetime.now(tz=pytz.timezone(tz))
+    return now_with_tz if with_tz else now_with_tz.replace(tzinfo=None)
+
+
+# get current timestamp
+def current_timestamp(length: int = 16) -> int:
+    return get_timestamp(None, length)
+
+
+# get timestamp from datetime
+def get_timestamp(dt: datetime = None, length: int = 16) -> int:
+    _timestamp = dt.timestamp() if dt else time.time()
+    return int(_timestamp * 10 ** (length - 10))
 
 
 def format(dt: datetime = None, format: str = "%Y-%m-%dT%H:%M:%S.%f") -> str:
     if dt is None:
         dt = now()
     return dt.strftime(format)
 
@@ -17,16 +29,15 @@
 def parse(dt_str: str, format: str = "%Y-%m-%dT%H:%M:%S.%f") -> datetime:
     return datetime.strptime(dt_str, format)
 
 
 def remove_tz(dt: datetime, tz: str = "Asia/Shanghai") -> datetime:
     if dt.tzinfo is None:
         return dt
-    timezone = pytz.timezone(tz)
-    return dt.astimezone(timezone).replace(tzinfo=None)
+    return dt.astimezone(pytz.timezone(tz)).replace(tzinfo=None)
 
 
 def format_duration(seconds: int) -> str:
     minutes, seconds = divmod(seconds, 60)
     hours, minutes = divmod(minutes, 60)
     if hours > 0:
         return f"{hours:02d}:{minutes:02d}:{seconds:02d}"
```

### Comparing `yuanfen-2024.3.8.1/src/yuanfen/version.py` & `yuanfen-2024.4.24.1/src/yuanfen/version.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.3.8.1/.gitignore` & `yuanfen-2024.4.24.1/.gitignore`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.3.8.1/README.md` & `yuanfen-2024.4.24.1/README.md`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.3.8.1/pyproject.toml` & `yuanfen-2024.4.24.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.3.8.1/PKG-INFO` & `yuanfen-2024.4.24.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: yuanfen
-Version: 2024.3.8.1
+Version: 2024.4.24.1
 Summary: Yuanfen Python Library
 Project-URL: Homepage, https://github.com/YuanfenNet/yf-lib-py
 Author-email: Bean <bean@yuanfen.net>
 License-Expression: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

