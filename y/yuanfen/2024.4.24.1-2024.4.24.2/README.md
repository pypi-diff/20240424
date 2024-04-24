# Comparing `tmp/yuanfen-2024.4.24.1.tar.gz` & `tmp/yuanfen-2024.4.24.2.tar.gz`

## Comparing `yuanfen-2024.4.24.1.tar` & `yuanfen-2024.4.24.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/src/yuanfen/__init__.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/src/yuanfen/config.py
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/src/yuanfen/email.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/src/yuanfen/env.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/src/yuanfen/group_robot.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/src/yuanfen/ip.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/src/yuanfen/logger.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/src/yuanfen/redis.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/src/yuanfen/response.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/src/yuanfen/time.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/src/yuanfen/version.py
--rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/.gitignore
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/README.md
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/pyproject.toml
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.1/PKG-INFO
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.2/src/yuanfen/__init__.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.2/src/yuanfen/config.py
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.2/src/yuanfen/email.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.2/src/yuanfen/env.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.2/src/yuanfen/group_robot.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.2/src/yuanfen/ip.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.2/src/yuanfen/logger.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.2/src/yuanfen/redis.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.2/src/yuanfen/response.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.2/src/yuanfen/time.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.2/src/yuanfen/version.py
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.2/.gitignore
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.2/README.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.2/pyproject.toml
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 yuanfen-2024.4.24.2/PKG-INFO
```

### Comparing `yuanfen-2024.4.24.1/src/yuanfen/__init__.py` & `yuanfen-2024.4.24.2/src/yuanfen/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .env import APP_ENV
 from .group_robot import GroupRobot
 from .logger import Logger
 from .redis import Redis
 from .response import BaseResponse, ErrorResponse, SuccessResponse
 from .version import Version
 
-__version__ = "2024.4.24.1"
+__version__ = "2024.4.24.2"
 
 __all__ = [
     "APP_ENV",
     "BaseResponse",
     "Config",
     "Email",
     "ErrorResponse",
```

### Comparing `yuanfen-2024.4.24.1/src/yuanfen/config.py` & `yuanfen-2024.4.24.2/src/yuanfen/config.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.24.1/src/yuanfen/email.py` & `yuanfen-2024.4.24.2/src/yuanfen/email.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.24.1/src/yuanfen/ip.py` & `yuanfen-2024.4.24.2/src/yuanfen/ip.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.24.1/src/yuanfen/logger.py` & `yuanfen-2024.4.24.2/src/yuanfen/logger.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.24.1/src/yuanfen/time.py` & `yuanfen-2024.4.24.2/src/yuanfen/time.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.24.1/src/yuanfen/version.py` & `yuanfen-2024.4.24.2/src/yuanfen/version.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.24.1/.gitignore` & `yuanfen-2024.4.24.2/.gitignore`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.24.1/README.md` & `yuanfen-2024.4.24.2/README.md`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.24.1/pyproject.toml` & `yuanfen-2024.4.24.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.24.1/PKG-INFO` & `yuanfen-2024.4.24.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: yuanfen
-Version: 2024.4.24.1
+Version: 2024.4.24.2
 Summary: Yuanfen Python Library
 Project-URL: Homepage, https://github.com/YuanfenNet/yf-lib-py
 Author-email: Bean <bean@yuanfen.net>
 License-Expression: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

