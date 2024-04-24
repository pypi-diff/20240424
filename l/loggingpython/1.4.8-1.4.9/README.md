# Comparing `tmp/loggingpython-1.4.8.tar.gz` & `tmp/loggingpython-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggingpython-1.4.8.tar", last modified: Wed Apr 24 16:03:52 2024, max compression
+gzip compressed data, was "loggingpython-1.4.9.tar", last modified: Wed Apr 24 16:15:44 2024, max compression
```

## Comparing `loggingpython-1.4.8.tar` & `loggingpython-1.4.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 16:03:52.576258 loggingpython-1.4.8/
--rw-rw-rw-   0        0        0     1087 2024-03-04 14:25:44.000000 loggingpython-1.4.8/LICENSE
--rw-rw-rw-   0        0        0     3264 2024-04-24 16:03:52.575258 loggingpython-1.4.8/PKG-INFO
--rw-rw-rw-   0        0        0     2366 2024-04-12 18:05:53.000000 loggingpython-1.4.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-24 16:03:52.576258 loggingpython-1.4.8/setup.cfg
--rw-rw-rw-   0        0        0     1254 2024-04-24 16:03:50.000000 loggingpython-1.4.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 16:03:52.521259 loggingpython-1.4.8/src/
-drwxrwxrwx   0        0        0        0 2024-04-24 16:03:52.528762 loggingpython-1.4.8/src/loggingpython/
--rw-rw-rw-   0        0        0     5386 2024-04-24 15:57:10.000000 loggingpython-1.4.8/src/loggingpython/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 16:03:52.559758 loggingpython-1.4.8/src/loggingpython/error/
--rw-rw-rw-   0        0        0     2553 2024-04-24 11:59:15.000000 loggingpython-1.4.8/src/loggingpython/error/__init__.py
--rw-rw-rw-   0        0        0     1844 2024-04-24 12:01:18.000000 loggingpython-1.4.8/src/loggingpython/error/client_method_call_error.py
--rw-rw-rw-   0        0        0     1732 2024-04-24 15:12:41.000000 loggingpython-1.4.8/src/loggingpython/error/handler_not_found_error.py
--rw-rw-rw-   0        0        0     1910 2024-04-24 15:12:42.000000 loggingpython-1.4.8/src/loggingpython/error/invalid_handler_method_error.py
--rw-rw-rw-   0        0        0     1692 2024-04-24 15:10:29.000000 loggingpython-1.4.8/src/loggingpython/error/invalid_log_level_error.py
--rw-rw-rw-   0        0        0     1844 2024-04-24 15:10:38.000000 loggingpython-1.4.8/src/loggingpython/error/server_method_call_error.py
--rw-rw-rw-   0        0        0     1856 2024-04-24 15:10:33.000000 loggingpython-1.4.8/src/loggingpython/error/server_unreachable_error.py
-drwxrwxrwx   0        0        0        0 2024-04-24 16:03:52.569258 loggingpython-1.4.8/src/loggingpython/handler/
--rw-rw-rw-   0        0        0     2401 2024-04-24 15:57:17.000000 loggingpython-1.4.8/src/loggingpython/handler/__init__.py
--rw-rw-rw-   0        0        0     4883 2024-04-24 12:03:29.000000 loggingpython-1.4.8/src/loggingpython/handler/consolehandler.py
--rw-rw-rw-   0        0        0     5533 2024-04-24 12:04:33.000000 loggingpython-1.4.8/src/loggingpython/handler/csvhandler.py
--rw-rw-rw-   0        0        0     5544 2024-04-24 12:04:58.000000 loggingpython-1.4.8/src/loggingpython/handler/filehandler.py
--rw-rw-rw-   0        0        0     3019 2024-04-24 12:05:15.000000 loggingpython-1.4.8/src/loggingpython/handler/handler.py
--rw-rw-rw-   0        0        0     7291 2024-04-24 12:05:33.000000 loggingpython-1.4.8/src/loggingpython/handler/jsonhandler.py
--rw-rw-rw-   0        0        0     6494 2024-04-24 12:05:52.000000 loggingpython-1.4.8/src/loggingpython/handler/sqlhandler.py
--rw-rw-rw-   0        0        0    13900 2024-04-24 15:35:51.000000 loggingpython-1.4.8/src/loggingpython/handler/syshandler.py
--rw-rw-rw-   0        0        0     2307 2024-04-24 13:02:57.000000 loggingpython-1.4.8/src/loggingpython/log_levels.py
--rw-rw-rw-   0        0        0    19077 2024-04-24 16:03:30.000000 loggingpython-1.4.8/src/loggingpython/logger.py
--rw-rw-rw-   0        0        0     2038 2024-04-24 12:09:12.000000 loggingpython-1.4.8/src/loggingpython/sys_protocolls.py
-drwxrwxrwx   0        0        0        0 2024-04-24 16:03:52.574258 loggingpython-1.4.8/src/loggingpython.egg-info/
--rw-rw-rw-   0        0        0     3264 2024-04-24 16:03:52.000000 loggingpython-1.4.8/src/loggingpython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1117 2024-04-24 16:03:52.000000 loggingpython-1.4.8/src/loggingpython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 16:03:52.000000 loggingpython-1.4.8/src/loggingpython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-24 16:03:52.000000 loggingpython-1.4.8/src/loggingpython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-24 16:03:52.000000 loggingpython-1.4.8/src/loggingpython.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-24 16:03:52.573258 loggingpython-1.4.8/test/
--rw-rw-rw-   0        0        0     1021 2024-04-23 13:59:00.000000 loggingpython-1.4.8/test/test_init.py
--rw-rw-rw-   0        0        0      496 2024-04-23 13:58:57.000000 loggingpython-1.4.8/test/test_log_levels.py
--rw-rw-rw-   0        0        0     1611 2024-04-24 15:10:19.000000 loggingpython-1.4.8/test/test_logger.py
--rw-rw-rw-   0        0        0      388 2024-04-23 16:32:24.000000 loggingpython-1.4.8/test/test_sys_protocolls.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:15:44.654035 loggingpython-1.4.9/
+-rw-rw-rw-   0        0        0     1087 2024-03-04 14:25:44.000000 loggingpython-1.4.9/LICENSE
+-rw-rw-rw-   0        0        0     3264 2024-04-24 16:15:44.652535 loggingpython-1.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2366 2024-04-12 18:05:53.000000 loggingpython-1.4.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 16:15:44.654035 loggingpython-1.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     1254 2024-04-24 16:05:38.000000 loggingpython-1.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:15:44.606035 loggingpython-1.4.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 16:15:44.614534 loggingpython-1.4.9/src/loggingpython/
+-rw-rw-rw-   0        0        0     5386 2024-04-24 16:14:52.000000 loggingpython-1.4.9/src/loggingpython/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:15:44.639536 loggingpython-1.4.9/src/loggingpython/error/
+-rw-rw-rw-   0        0        0     2553 2024-04-24 11:59:15.000000 loggingpython-1.4.9/src/loggingpython/error/__init__.py
+-rw-rw-rw-   0        0        0     1844 2024-04-24 12:01:18.000000 loggingpython-1.4.9/src/loggingpython/error/client_method_call_error.py
+-rw-rw-rw-   0        0        0     1732 2024-04-24 15:12:41.000000 loggingpython-1.4.9/src/loggingpython/error/handler_not_found_error.py
+-rw-rw-rw-   0        0        0     1910 2024-04-24 15:12:42.000000 loggingpython-1.4.9/src/loggingpython/error/invalid_handler_method_error.py
+-rw-rw-rw-   0        0        0     1692 2024-04-24 15:10:29.000000 loggingpython-1.4.9/src/loggingpython/error/invalid_log_level_error.py
+-rw-rw-rw-   0        0        0     1844 2024-04-24 15:10:38.000000 loggingpython-1.4.9/src/loggingpython/error/server_method_call_error.py
+-rw-rw-rw-   0        0        0     1856 2024-04-24 15:10:33.000000 loggingpython-1.4.9/src/loggingpython/error/server_unreachable_error.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:15:44.646534 loggingpython-1.4.9/src/loggingpython/handler/
+-rw-rw-rw-   0        0        0     2401 2024-04-24 15:57:17.000000 loggingpython-1.4.9/src/loggingpython/handler/__init__.py
+-rw-rw-rw-   0        0        0     4883 2024-04-24 12:03:29.000000 loggingpython-1.4.9/src/loggingpython/handler/consolehandler.py
+-rw-rw-rw-   0        0        0     5533 2024-04-24 12:04:33.000000 loggingpython-1.4.9/src/loggingpython/handler/csvhandler.py
+-rw-rw-rw-   0        0        0     5544 2024-04-24 12:04:58.000000 loggingpython-1.4.9/src/loggingpython/handler/filehandler.py
+-rw-rw-rw-   0        0        0     3019 2024-04-24 12:05:15.000000 loggingpython-1.4.9/src/loggingpython/handler/handler.py
+-rw-rw-rw-   0        0        0     7291 2024-04-24 12:05:33.000000 loggingpython-1.4.9/src/loggingpython/handler/jsonhandler.py
+-rw-rw-rw-   0        0        0     6494 2024-04-24 12:05:52.000000 loggingpython-1.4.9/src/loggingpython/handler/sqlhandler.py
+-rw-rw-rw-   0        0        0    13900 2024-04-24 15:35:51.000000 loggingpython-1.4.9/src/loggingpython/handler/syshandler.py
+-rw-rw-rw-   0        0        0     2307 2024-04-24 13:02:57.000000 loggingpython-1.4.9/src/loggingpython/log_levels.py
+-rw-rw-rw-   0        0        0    19055 2024-04-24 16:15:27.000000 loggingpython-1.4.9/src/loggingpython/logger.py
+-rw-rw-rw-   0        0        0     2038 2024-04-24 12:09:12.000000 loggingpython-1.4.9/src/loggingpython/sys_protocolls.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:15:44.651534 loggingpython-1.4.9/src/loggingpython.egg-info/
+-rw-rw-rw-   0        0        0     3264 2024-04-24 16:15:44.000000 loggingpython-1.4.9/src/loggingpython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1117 2024-04-24 16:15:44.000000 loggingpython-1.4.9/src/loggingpython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 16:15:44.000000 loggingpython-1.4.9/src/loggingpython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-24 16:15:44.000000 loggingpython-1.4.9/src/loggingpython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-24 16:15:44.000000 loggingpython-1.4.9/src/loggingpython.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 16:15:44.650534 loggingpython-1.4.9/test/
+-rw-rw-rw-   0        0        0     1021 2024-04-23 13:59:00.000000 loggingpython-1.4.9/test/test_init.py
+-rw-rw-rw-   0        0        0      496 2024-04-23 13:58:57.000000 loggingpython-1.4.9/test/test_log_levels.py
+-rw-rw-rw-   0        0        0     1611 2024-04-24 15:10:19.000000 loggingpython-1.4.9/test/test_logger.py
+-rw-rw-rw-   0        0        0      388 2024-04-23 16:32:24.000000 loggingpython-1.4.9/test/test_sys_protocolls.py
```

### Comparing `loggingpython-1.4.8/LICENSE` & `loggingpython-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.8/PKG-INFO` & `loggingpython-1.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggingpython
-Version: 1.4.8
+Version: 1.4.9
 Summary: Loggingpython is a Python package that provides a simple and extensible way to integrate logging into your applications. The package starts with a simple logger and can be extended with additional functions to meet the requirements of your application.
 Home-page: https://github.com/loggingpython-Community/loggingpython
 Author: mrmajor.programmer
 Author-email: mrmajork.programmer@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `loggingpython-1.4.8/README.md` & `loggingpython-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.8/setup.py` & `loggingpython-1.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='loggingpython',
-    version='1.4.8',
+    version='1.4.9',
     description='Loggingpython is a Python package that provides a simple and\
  extensible way to integrate logging into your applications. The package\
  starts with a simple logger and can be extended with additional functions to\
  meet the requirements of your application.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='mrmajor.programmer',
```

### Comparing `loggingpython-1.4.8/src/loggingpython/__init__.py` & `loggingpython-1.4.9/src/loggingpython/__init__.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.8/src/loggingpython/error/__init__.py` & `loggingpython-1.4.9/src/loggingpython/error/__init__.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.8/src/loggingpython/error/client_method_call_error.py` & `loggingpython-1.4.9/src/loggingpython/error/client_method_call_error.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.8/src/loggingpython/error/handler_not_found_error.py` & `loggingpython-1.4.9/src/loggingpython/error/handler_not_found_error.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.8/src/loggingpython/error/invalid_handler_method_error.py` & `loggingpython-1.4.9/src/loggingpython/error/invalid_handler_method_error.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.8/src/loggingpython/error/invalid_log_level_error.py` & `loggingpython-1.4.9/src/loggingpython/error/invalid_log_level_error.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.8/src/loggingpython/error/server_method_call_error.py` & `loggingpython-1.4.9/src/loggingpython/error/server_method_call_error.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.8/src/loggingpython/error/server_unreachable_error.py` & `loggingpython-1.4.9/src/loggingpython/error/server_unreachable_error.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.8/src/loggingpython/handler/__init__.py` & `loggingpython-1.4.9/src/loggingpython/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.8/src/loggingpython/handler/consolehandler.py` & `loggingpython-1.4.9/src/loggingpython/handler/consolehandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.8/src/loggingpython/handler/csvhandler.py` & `loggingpython-1.4.9/src/loggingpython/handler/csvhandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.8/src/loggingpython/handler/filehandler.py` & `loggingpython-1.4.9/src/loggingpython/handler/filehandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.8/src/loggingpython/handler/handler.py` & `loggingpython-1.4.9/src/loggingpython/handler/handler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.8/src/loggingpython/handler/jsonhandler.py` & `loggingpython-1.4.9/src/loggingpython/handler/jsonhandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.8/src/loggingpython/handler/sqlhandler.py` & `loggingpython-1.4.9/src/loggingpython/handler/sqlhandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.8/src/loggingpython/handler/syshandler.py` & `loggingpython-1.4.9/src/loggingpython/handler/syshandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.8/src/loggingpython/log_levels.py` & `loggingpython-1.4.9/src/loggingpython/log_levels.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.8/src/loggingpython/logger.py` & `loggingpython-1.4.9/src/loggingpython/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,16 +87,16 @@
     """
 
     _SUPPORTED_LEVELS: list = list(LogLevel)
     _ISO_8601_FORMAT: str = "%Y-%m-%dT%H:%M:%S.%f%z"
 
     def __init__(self, name: str,
                  time_format: str = None,
-                 min_loglevel: LogLevel = LogLevel.INFO,
-                 max_loglevel: LogLevel = LogLevel.CRITICAL) -> None:
+                 min_loglevel: LogLevel = None,
+                 max_loglevel: LogLevel = None) -> None:
         """
         Initializes the Logger with the given name, time format, and log
         levels.
 
         Args:
             name (str): The name of the logger.
             time_format (str, optional): The format string for the log
```

### Comparing `loggingpython-1.4.8/src/loggingpython/sys_protocolls.py` & `loggingpython-1.4.9/src/loggingpython/sys_protocolls.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.8/src/loggingpython.egg-info/PKG-INFO` & `loggingpython-1.4.9/src/loggingpython.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggingpython
-Version: 1.4.8
+Version: 1.4.9
 Summary: Loggingpython is a Python package that provides a simple and extensible way to integrate logging into your applications. The package starts with a simple logger and can be extended with additional functions to meet the requirements of your application.
 Home-page: https://github.com/loggingpython-Community/loggingpython
 Author: mrmajor.programmer
 Author-email: mrmajork.programmer@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `loggingpython-1.4.8/src/loggingpython.egg-info/SOURCES.txt` & `loggingpython-1.4.9/src/loggingpython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.8/test/test_init.py` & `loggingpython-1.4.9/test/test_init.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.8/test/test_logger.py` & `loggingpython-1.4.9/test/test_logger.py`

 * *Files identical despite different names*

