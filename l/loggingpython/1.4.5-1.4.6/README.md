# Comparing `tmp/loggingpython-1.4.5.tar.gz` & `tmp/loggingpython-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggingpython-1.4.5.tar", last modified: Wed Apr 24 15:12:57 2024, max compression
+gzip compressed data, was "loggingpython-1.4.6.tar", last modified: Wed Apr 24 15:36:53 2024, max compression
```

## Comparing `loggingpython-1.4.5.tar` & `loggingpython-1.4.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 15:12:57.070076 loggingpython-1.4.5/
--rw-rw-rw-   0        0        0     1087 2024-03-04 14:25:44.000000 loggingpython-1.4.5/LICENSE
--rw-rw-rw-   0        0        0     3264 2024-04-24 15:12:57.069075 loggingpython-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     2366 2024-04-12 18:05:53.000000 loggingpython-1.4.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-24 15:12:57.070076 loggingpython-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1254 2024-04-24 15:12:54.000000 loggingpython-1.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 15:12:57.028076 loggingpython-1.4.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-24 15:12:57.036578 loggingpython-1.4.5/src/loggingpython/
--rw-rw-rw-   0        0        0     5387 2024-04-24 11:59:06.000000 loggingpython-1.4.5/src/loggingpython/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 15:12:57.057076 loggingpython-1.4.5/src/loggingpython/error/
--rw-rw-rw-   0        0        0     2553 2024-04-24 11:59:15.000000 loggingpython-1.4.5/src/loggingpython/error/__init__.py
--rw-rw-rw-   0        0        0     1844 2024-04-24 12:01:18.000000 loggingpython-1.4.5/src/loggingpython/error/client_method_call_error.py
--rw-rw-rw-   0        0        0     1732 2024-04-24 15:12:41.000000 loggingpython-1.4.5/src/loggingpython/error/handler_not_found_error.py
--rw-rw-rw-   0        0        0     1910 2024-04-24 15:12:42.000000 loggingpython-1.4.5/src/loggingpython/error/invalid_handler_method_error.py
--rw-rw-rw-   0        0        0     1692 2024-04-24 15:10:29.000000 loggingpython-1.4.5/src/loggingpython/error/invalid_log_level_error.py
--rw-rw-rw-   0        0        0     1844 2024-04-24 15:10:38.000000 loggingpython-1.4.5/src/loggingpython/error/server_method_call_error.py
--rw-rw-rw-   0        0        0     1856 2024-04-24 15:10:33.000000 loggingpython-1.4.5/src/loggingpython/error/server_unreachable_error.py
-drwxrwxrwx   0        0        0        0 2024-04-24 15:12:57.064074 loggingpython-1.4.5/src/loggingpython/handler/
--rw-rw-rw-   0        0        0     2399 2024-04-24 11:58:58.000000 loggingpython-1.4.5/src/loggingpython/handler/__init__.py
--rw-rw-rw-   0        0        0     4883 2024-04-24 12:03:29.000000 loggingpython-1.4.5/src/loggingpython/handler/consolehandler.py
--rw-rw-rw-   0        0        0     5533 2024-04-24 12:04:33.000000 loggingpython-1.4.5/src/loggingpython/handler/csvhandler.py
--rw-rw-rw-   0        0        0     5544 2024-04-24 12:04:58.000000 loggingpython-1.4.5/src/loggingpython/handler/filehandler.py
--rw-rw-rw-   0        0        0     3019 2024-04-24 12:05:15.000000 loggingpython-1.4.5/src/loggingpython/handler/handler.py
--rw-rw-rw-   0        0        0     7291 2024-04-24 12:05:33.000000 loggingpython-1.4.5/src/loggingpython/handler/jsonhandler.py
--rw-rw-rw-   0        0        0     6494 2024-04-24 12:05:52.000000 loggingpython-1.4.5/src/loggingpython/handler/sqlhandler.py
--rw-rw-rw-   0        0        0    13938 2024-04-24 12:08:57.000000 loggingpython-1.4.5/src/loggingpython/handler/syshandler.py
--rw-rw-rw-   0        0        0     2307 2024-04-24 13:02:57.000000 loggingpython-1.4.5/src/loggingpython/log_levels.py
--rw-rw-rw-   0        0        0    19026 2024-04-24 12:06:37.000000 loggingpython-1.4.5/src/loggingpython/logger.py
--rw-rw-rw-   0        0        0     2038 2024-04-24 12:09:12.000000 loggingpython-1.4.5/src/loggingpython/sys_protocolls.py
-drwxrwxrwx   0        0        0        0 2024-04-24 15:12:57.068075 loggingpython-1.4.5/src/loggingpython.egg-info/
--rw-rw-rw-   0        0        0     3264 2024-04-24 15:12:56.000000 loggingpython-1.4.5/src/loggingpython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1117 2024-04-24 15:12:56.000000 loggingpython-1.4.5/src/loggingpython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 15:12:56.000000 loggingpython-1.4.5/src/loggingpython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-24 15:12:56.000000 loggingpython-1.4.5/src/loggingpython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-24 15:12:56.000000 loggingpython-1.4.5/src/loggingpython.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-24 15:12:57.067075 loggingpython-1.4.5/test/
--rw-rw-rw-   0        0        0     1021 2024-04-23 13:59:00.000000 loggingpython-1.4.5/test/test_init.py
--rw-rw-rw-   0        0        0      496 2024-04-23 13:58:57.000000 loggingpython-1.4.5/test/test_log_levels.py
--rw-rw-rw-   0        0        0     1611 2024-04-24 15:10:19.000000 loggingpython-1.4.5/test/test_logger.py
--rw-rw-rw-   0        0        0      388 2024-04-23 16:32:24.000000 loggingpython-1.4.5/test/test_sys_protocolls.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:36:53.922481 loggingpython-1.4.6/
+-rw-rw-rw-   0        0        0     1087 2024-03-04 14:25:44.000000 loggingpython-1.4.6/LICENSE
+-rw-rw-rw-   0        0        0     3264 2024-04-24 15:36:53.920981 loggingpython-1.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2366 2024-04-12 18:05:53.000000 loggingpython-1.4.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 15:36:53.922481 loggingpython-1.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1254 2024-04-24 15:36:51.000000 loggingpython-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:36:53.858482 loggingpython-1.4.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 15:36:53.869481 loggingpython-1.4.6/src/loggingpython/
+-rw-rw-rw-   0        0        0     5387 2024-04-24 11:59:06.000000 loggingpython-1.4.6/src/loggingpython/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:36:53.906982 loggingpython-1.4.6/src/loggingpython/error/
+-rw-rw-rw-   0        0        0     2553 2024-04-24 11:59:15.000000 loggingpython-1.4.6/src/loggingpython/error/__init__.py
+-rw-rw-rw-   0        0        0     1844 2024-04-24 12:01:18.000000 loggingpython-1.4.6/src/loggingpython/error/client_method_call_error.py
+-rw-rw-rw-   0        0        0     1732 2024-04-24 15:12:41.000000 loggingpython-1.4.6/src/loggingpython/error/handler_not_found_error.py
+-rw-rw-rw-   0        0        0     1910 2024-04-24 15:12:42.000000 loggingpython-1.4.6/src/loggingpython/error/invalid_handler_method_error.py
+-rw-rw-rw-   0        0        0     1692 2024-04-24 15:10:29.000000 loggingpython-1.4.6/src/loggingpython/error/invalid_log_level_error.py
+-rw-rw-rw-   0        0        0     1844 2024-04-24 15:10:38.000000 loggingpython-1.4.6/src/loggingpython/error/server_method_call_error.py
+-rw-rw-rw-   0        0        0     1856 2024-04-24 15:10:33.000000 loggingpython-1.4.6/src/loggingpython/error/server_unreachable_error.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:36:53.914483 loggingpython-1.4.6/src/loggingpython/handler/
+-rw-rw-rw-   0        0        0     2399 2024-04-24 11:58:58.000000 loggingpython-1.4.6/src/loggingpython/handler/__init__.py
+-rw-rw-rw-   0        0        0     4883 2024-04-24 12:03:29.000000 loggingpython-1.4.6/src/loggingpython/handler/consolehandler.py
+-rw-rw-rw-   0        0        0     5533 2024-04-24 12:04:33.000000 loggingpython-1.4.6/src/loggingpython/handler/csvhandler.py
+-rw-rw-rw-   0        0        0     5544 2024-04-24 12:04:58.000000 loggingpython-1.4.6/src/loggingpython/handler/filehandler.py
+-rw-rw-rw-   0        0        0     3019 2024-04-24 12:05:15.000000 loggingpython-1.4.6/src/loggingpython/handler/handler.py
+-rw-rw-rw-   0        0        0     7291 2024-04-24 12:05:33.000000 loggingpython-1.4.6/src/loggingpython/handler/jsonhandler.py
+-rw-rw-rw-   0        0        0     6494 2024-04-24 12:05:52.000000 loggingpython-1.4.6/src/loggingpython/handler/sqlhandler.py
+-rw-rw-rw-   0        0        0    13900 2024-04-24 15:35:51.000000 loggingpython-1.4.6/src/loggingpython/handler/syshandler.py
+-rw-rw-rw-   0        0        0     2307 2024-04-24 13:02:57.000000 loggingpython-1.4.6/src/loggingpython/log_levels.py
+-rw-rw-rw-   0        0        0    19138 2024-04-24 15:21:15.000000 loggingpython-1.4.6/src/loggingpython/logger.py
+-rw-rw-rw-   0        0        0     2038 2024-04-24 12:09:12.000000 loggingpython-1.4.6/src/loggingpython/sys_protocolls.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:36:53.919981 loggingpython-1.4.6/src/loggingpython.egg-info/
+-rw-rw-rw-   0        0        0     3264 2024-04-24 15:36:53.000000 loggingpython-1.4.6/src/loggingpython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1117 2024-04-24 15:36:53.000000 loggingpython-1.4.6/src/loggingpython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 15:36:53.000000 loggingpython-1.4.6/src/loggingpython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-24 15:36:53.000000 loggingpython-1.4.6/src/loggingpython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-24 15:36:53.000000 loggingpython-1.4.6/src/loggingpython.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 15:36:53.918982 loggingpython-1.4.6/test/
+-rw-rw-rw-   0        0        0     1021 2024-04-23 13:59:00.000000 loggingpython-1.4.6/test/test_init.py
+-rw-rw-rw-   0        0        0      496 2024-04-23 13:58:57.000000 loggingpython-1.4.6/test/test_log_levels.py
+-rw-rw-rw-   0        0        0     1611 2024-04-24 15:10:19.000000 loggingpython-1.4.6/test/test_logger.py
+-rw-rw-rw-   0        0        0      388 2024-04-23 16:32:24.000000 loggingpython-1.4.6/test/test_sys_protocolls.py
```

### Comparing `loggingpython-1.4.5/LICENSE` & `loggingpython-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.5/PKG-INFO` & `loggingpython-1.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggingpython
-Version: 1.4.5
+Version: 1.4.6
 Summary: Loggingpython is a Python package that provides a simple and extensible way to integrate logging into your applications. The package starts with a simple logger and can be extended with additional functions to meet the requirements of your application.
 Home-page: https://github.com/loggingpython-Community/loggingpython
 Author: mrmajor.programmer
 Author-email: mrmajork.programmer@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `loggingpython-1.4.5/README.md` & `loggingpython-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.5/setup.py` & `loggingpython-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='loggingpython',
-    version='1.4.5',
+    version='1.4.6',
     description='Loggingpython is a Python package that provides a simple and\
  extensible way to integrate logging into your applications. The package\
  starts with a simple logger and can be extended with additional functions to\
  meet the requirements of your application.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='mrmajor.programmer',
```

### Comparing `loggingpython-1.4.5/src/loggingpython/__init__.py` & `loggingpython-1.4.6/src/loggingpython/__init__.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.5/src/loggingpython/error/__init__.py` & `loggingpython-1.4.6/src/loggingpython/error/__init__.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.5/src/loggingpython/error/client_method_call_error.py` & `loggingpython-1.4.6/src/loggingpython/error/client_method_call_error.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.5/src/loggingpython/error/handler_not_found_error.py` & `loggingpython-1.4.6/src/loggingpython/error/handler_not_found_error.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.5/src/loggingpython/error/invalid_handler_method_error.py` & `loggingpython-1.4.6/src/loggingpython/error/invalid_handler_method_error.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.5/src/loggingpython/error/invalid_log_level_error.py` & `loggingpython-1.4.6/src/loggingpython/error/invalid_log_level_error.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.5/src/loggingpython/error/server_method_call_error.py` & `loggingpython-1.4.6/src/loggingpython/error/server_method_call_error.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.5/src/loggingpython/error/server_unreachable_error.py` & `loggingpython-1.4.6/src/loggingpython/error/server_unreachable_error.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.5/src/loggingpython/handler/__init__.py` & `loggingpython-1.4.6/src/loggingpython/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.5/src/loggingpython/handler/consolehandler.py` & `loggingpython-1.4.6/src/loggingpython/handler/consolehandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.5/src/loggingpython/handler/csvhandler.py` & `loggingpython-1.4.6/src/loggingpython/handler/csvhandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.5/src/loggingpython/handler/filehandler.py` & `loggingpython-1.4.6/src/loggingpython/handler/filehandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.5/src/loggingpython/handler/handler.py` & `loggingpython-1.4.6/src/loggingpython/handler/handler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.5/src/loggingpython/handler/jsonhandler.py` & `loggingpython-1.4.6/src/loggingpython/handler/jsonhandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.5/src/loggingpython/handler/sqlhandler.py` & `loggingpython-1.4.6/src/loggingpython/handler/sqlhandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.5/src/loggingpython/handler/syshandler.py` & `loggingpython-1.4.6/src/loggingpython/handler/syshandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,14 @@
 
         if self.client:
             self._connect_client()
         else:
             self._logger = logger
             self._run_server()
 
-    @staticmethod
     def _client_only(func):
         """
         Decorator to ensure a method can only be called by a client.
 
         This decorator checks if the handler is in client mode before allowing
         the method to be called. If the handler is in server mode, it raises a
         ClientMethodCallError.
@@ -129,15 +128,14 @@
         def wrapper(self, *args, **kwargs):
             if self.client:
                 return func(self, *args, **kwargs)
             else:
                 raise ClientMethodCallError()
         return wrapper
 
-    @staticmethod
     def _server_only(func):
         """
         Decorator to ensure a method can only be called by a server.
 
         This decorator checks if the handler is in server mode before allowing
         the method to be called. If the handler is in client mode, it raises a
         ServerMethodCallError.
```

### Comparing `loggingpython-1.4.5/src/loggingpython/log_levels.py` & `loggingpython-1.4.6/src/loggingpython/log_levels.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.5/src/loggingpython/logger.py` & `loggingpython-1.4.6/src/loggingpython/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,19 +105,27 @@
             max_loglevel (LogLevel, optional): The maximum log level to be
                 logged. Defaults to LogLevel.CRITICAL.
 
         Raises:
             InvalidLogLevelError: If the provided log levels are not supported.
         """
 
+        if min_loglevel in LogLevel:
+            self.min_loglevel: LogLevel = min_loglevel
+
+        else:
+            self.min_loglevel: LogLevel = LogLevel.INFO
+
+        if min_loglevel in LogLevel:
+            self.min_loglevel: LogLevel = min_loglevel
+
+        else:
+            self.min_loglevel: LogLevel = LogLevel.CRITICAL
+
         self.name: str = name
-        self.min_loglevel: LogLevel = min_loglevel \
-            if min_loglevel in LogLevel else LogLevel.INFO
-        self.max_loglevel: LogLevel = max_loglevel \
-            if max_loglevel in LogLevel else LogLevel.CRITICAL
 
         self.handlers: list[Handler] = []
 
         self.iso_8601_format: str = "%Y-%m-%dT%H:%M:%S.%f%z"
         self.time_format: str = time_format
 
     def _validate_loglevel(self, loglevel: LogLevel) -> None:
```

### Comparing `loggingpython-1.4.5/src/loggingpython/sys_protocolls.py` & `loggingpython-1.4.6/src/loggingpython/sys_protocolls.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.5/src/loggingpython.egg-info/PKG-INFO` & `loggingpython-1.4.6/src/loggingpython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggingpython
-Version: 1.4.5
+Version: 1.4.6
 Summary: Loggingpython is a Python package that provides a simple and extensible way to integrate logging into your applications. The package starts with a simple logger and can be extended with additional functions to meet the requirements of your application.
 Home-page: https://github.com/loggingpython-Community/loggingpython
 Author: mrmajor.programmer
 Author-email: mrmajork.programmer@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `loggingpython-1.4.5/src/loggingpython.egg-info/SOURCES.txt` & `loggingpython-1.4.6/src/loggingpython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.5/test/test_init.py` & `loggingpython-1.4.6/test/test_init.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.5/test/test_logger.py` & `loggingpython-1.4.6/test/test_logger.py`

 * *Files identical despite different names*

