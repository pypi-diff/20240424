# Comparing `tmp/loggingpython-1.4.3.tar.gz` & `tmp/loggingpython-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggingpython-1.4.3.tar", last modified: Wed Apr 24 15:07:15 2024, max compression
+gzip compressed data, was "loggingpython-1.4.4.tar", last modified: Wed Apr 24 15:11:31 2024, max compression
```

## Comparing `loggingpython-1.4.3.tar` & `loggingpython-1.4.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 15:07:15.022703 loggingpython-1.4.3/
--rw-rw-rw-   0        0        0     1087 2024-03-04 14:25:44.000000 loggingpython-1.4.3/LICENSE
--rw-rw-rw-   0        0        0     3264 2024-04-24 15:07:15.019702 loggingpython-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     2366 2024-04-12 18:05:53.000000 loggingpython-1.4.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-24 15:07:15.022703 loggingpython-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1254 2024-04-24 15:06:42.000000 loggingpython-1.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 15:07:14.954703 loggingpython-1.4.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-24 15:07:14.962704 loggingpython-1.4.3/src/loggingpython/
--rw-rw-rw-   0        0        0     5387 2024-04-24 11:59:06.000000 loggingpython-1.4.3/src/loggingpython/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 15:07:14.997702 loggingpython-1.4.3/src/loggingpython/error/
--rw-rw-rw-   0        0        0     2553 2024-04-24 11:59:15.000000 loggingpython-1.4.3/src/loggingpython/error/__init__.py
--rw-rw-rw-   0        0        0     1844 2024-04-24 12:01:18.000000 loggingpython-1.4.3/src/loggingpython/error/client_method_call_error.py
--rw-rw-rw-   0        0        0     1733 2024-04-24 12:01:53.000000 loggingpython-1.4.3/src/loggingpython/error/handler_not_found_error.py
--rw-rw-rw-   0        0        0     1911 2024-04-24 12:02:15.000000 loggingpython-1.4.3/src/loggingpython/error/invalid_handler_method_error.py
--rw-rw-rw-   0        0        0     1693 2024-04-24 12:02:33.000000 loggingpython-1.4.3/src/loggingpython/error/invalid_log_level_error.py
--rw-rw-rw-   0        0        0     1845 2024-04-24 12:02:49.000000 loggingpython-1.4.3/src/loggingpython/error/server_method_call_error.py
--rw-rw-rw-   0        0        0     1857 2024-04-24 12:03:04.000000 loggingpython-1.4.3/src/loggingpython/error/server_unreachable_error.py
-drwxrwxrwx   0        0        0        0 2024-04-24 15:07:15.012702 loggingpython-1.4.3/src/loggingpython/handler/
--rw-rw-rw-   0        0        0     2399 2024-04-24 11:58:58.000000 loggingpython-1.4.3/src/loggingpython/handler/__init__.py
--rw-rw-rw-   0        0        0     4883 2024-04-24 12:03:29.000000 loggingpython-1.4.3/src/loggingpython/handler/consolehandler.py
--rw-rw-rw-   0        0        0     5533 2024-04-24 12:04:33.000000 loggingpython-1.4.3/src/loggingpython/handler/csvhandler.py
--rw-rw-rw-   0        0        0     5544 2024-04-24 12:04:58.000000 loggingpython-1.4.3/src/loggingpython/handler/filehandler.py
--rw-rw-rw-   0        0        0     3019 2024-04-24 12:05:15.000000 loggingpython-1.4.3/src/loggingpython/handler/handler.py
--rw-rw-rw-   0        0        0     7291 2024-04-24 12:05:33.000000 loggingpython-1.4.3/src/loggingpython/handler/jsonhandler.py
--rw-rw-rw-   0        0        0     6494 2024-04-24 12:05:52.000000 loggingpython-1.4.3/src/loggingpython/handler/sqlhandler.py
--rw-rw-rw-   0        0        0    13938 2024-04-24 12:08:57.000000 loggingpython-1.4.3/src/loggingpython/handler/syshandler.py
--rw-rw-rw-   0        0        0     2307 2024-04-24 13:02:57.000000 loggingpython-1.4.3/src/loggingpython/log_levels.py
--rw-rw-rw-   0        0        0    19026 2024-04-24 12:06:37.000000 loggingpython-1.4.3/src/loggingpython/logger.py
--rw-rw-rw-   0        0        0     2038 2024-04-24 12:09:12.000000 loggingpython-1.4.3/src/loggingpython/sys_protocolls.py
-drwxrwxrwx   0        0        0        0 2024-04-24 15:07:15.018702 loggingpython-1.4.3/src/loggingpython.egg-info/
--rw-rw-rw-   0        0        0     3264 2024-04-24 15:07:14.000000 loggingpython-1.4.3/src/loggingpython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1117 2024-04-24 15:07:14.000000 loggingpython-1.4.3/src/loggingpython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 15:07:14.000000 loggingpython-1.4.3/src/loggingpython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-24 15:07:14.000000 loggingpython-1.4.3/src/loggingpython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-24 15:07:14.000000 loggingpython-1.4.3/src/loggingpython.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-24 15:07:15.017702 loggingpython-1.4.3/test/
--rw-rw-rw-   0        0        0     1021 2024-04-23 13:59:00.000000 loggingpython-1.4.3/test/test_init.py
--rw-rw-rw-   0        0        0      496 2024-04-23 13:58:57.000000 loggingpython-1.4.3/test/test_log_levels.py
--rw-rw-rw-   0        0        0     1611 2024-04-21 17:52:48.000000 loggingpython-1.4.3/test/test_logger.py
--rw-rw-rw-   0        0        0      388 2024-04-23 16:32:24.000000 loggingpython-1.4.3/test/test_sys_protocolls.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:11:31.144372 loggingpython-1.4.4/
+-rw-rw-rw-   0        0        0     1087 2024-03-04 14:25:44.000000 loggingpython-1.4.4/LICENSE
+-rw-rw-rw-   0        0        0     3264 2024-04-24 15:11:31.143372 loggingpython-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2366 2024-04-12 18:05:53.000000 loggingpython-1.4.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 15:11:31.144372 loggingpython-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1254 2024-04-24 15:11:28.000000 loggingpython-1.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:11:31.097872 loggingpython-1.4.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 15:11:31.106371 loggingpython-1.4.4/src/loggingpython/
+-rw-rw-rw-   0        0        0     5387 2024-04-24 11:59:06.000000 loggingpython-1.4.4/src/loggingpython/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:11:31.130872 loggingpython-1.4.4/src/loggingpython/error/
+-rw-rw-rw-   0        0        0     2553 2024-04-24 11:59:15.000000 loggingpython-1.4.4/src/loggingpython/error/__init__.py
+-rw-rw-rw-   0        0        0     1844 2024-04-24 12:01:18.000000 loggingpython-1.4.4/src/loggingpython/error/client_method_call_error.py
+-rw-rw-rw-   0        0        0     1733 2024-04-24 12:01:53.000000 loggingpython-1.4.4/src/loggingpython/error/handler_not_found_error.py
+-rw-rw-rw-   0        0        0     1911 2024-04-24 12:02:15.000000 loggingpython-1.4.4/src/loggingpython/error/invalid_handler_method_error.py
+-rw-rw-rw-   0        0        0     1692 2024-04-24 15:10:29.000000 loggingpython-1.4.4/src/loggingpython/error/invalid_log_level_error.py
+-rw-rw-rw-   0        0        0     1844 2024-04-24 15:10:38.000000 loggingpython-1.4.4/src/loggingpython/error/server_method_call_error.py
+-rw-rw-rw-   0        0        0     1856 2024-04-24 15:10:33.000000 loggingpython-1.4.4/src/loggingpython/error/server_unreachable_error.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:11:31.137873 loggingpython-1.4.4/src/loggingpython/handler/
+-rw-rw-rw-   0        0        0     2399 2024-04-24 11:58:58.000000 loggingpython-1.4.4/src/loggingpython/handler/__init__.py
+-rw-rw-rw-   0        0        0     4883 2024-04-24 12:03:29.000000 loggingpython-1.4.4/src/loggingpython/handler/consolehandler.py
+-rw-rw-rw-   0        0        0     5533 2024-04-24 12:04:33.000000 loggingpython-1.4.4/src/loggingpython/handler/csvhandler.py
+-rw-rw-rw-   0        0        0     5544 2024-04-24 12:04:58.000000 loggingpython-1.4.4/src/loggingpython/handler/filehandler.py
+-rw-rw-rw-   0        0        0     3019 2024-04-24 12:05:15.000000 loggingpython-1.4.4/src/loggingpython/handler/handler.py
+-rw-rw-rw-   0        0        0     7291 2024-04-24 12:05:33.000000 loggingpython-1.4.4/src/loggingpython/handler/jsonhandler.py
+-rw-rw-rw-   0        0        0     6494 2024-04-24 12:05:52.000000 loggingpython-1.4.4/src/loggingpython/handler/sqlhandler.py
+-rw-rw-rw-   0        0        0    13938 2024-04-24 12:08:57.000000 loggingpython-1.4.4/src/loggingpython/handler/syshandler.py
+-rw-rw-rw-   0        0        0     2307 2024-04-24 13:02:57.000000 loggingpython-1.4.4/src/loggingpython/log_levels.py
+-rw-rw-rw-   0        0        0    19026 2024-04-24 12:06:37.000000 loggingpython-1.4.4/src/loggingpython/logger.py
+-rw-rw-rw-   0        0        0     2038 2024-04-24 12:09:12.000000 loggingpython-1.4.4/src/loggingpython/sys_protocolls.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:11:31.142373 loggingpython-1.4.4/src/loggingpython.egg-info/
+-rw-rw-rw-   0        0        0     3264 2024-04-24 15:11:31.000000 loggingpython-1.4.4/src/loggingpython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1117 2024-04-24 15:11:31.000000 loggingpython-1.4.4/src/loggingpython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 15:11:31.000000 loggingpython-1.4.4/src/loggingpython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-24 15:11:31.000000 loggingpython-1.4.4/src/loggingpython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-24 15:11:31.000000 loggingpython-1.4.4/src/loggingpython.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 15:11:31.141373 loggingpython-1.4.4/test/
+-rw-rw-rw-   0        0        0     1021 2024-04-23 13:59:00.000000 loggingpython-1.4.4/test/test_init.py
+-rw-rw-rw-   0        0        0      496 2024-04-23 13:58:57.000000 loggingpython-1.4.4/test/test_log_levels.py
+-rw-rw-rw-   0        0        0     1611 2024-04-24 15:10:19.000000 loggingpython-1.4.4/test/test_logger.py
+-rw-rw-rw-   0        0        0      388 2024-04-23 16:32:24.000000 loggingpython-1.4.4/test/test_sys_protocolls.py
```

### Comparing `loggingpython-1.4.3/LICENSE` & `loggingpython-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.3/PKG-INFO` & `loggingpython-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggingpython
-Version: 1.4.3
+Version: 1.4.4
 Summary: Loggingpython is a Python package that provides a simple and extensible way to integrate logging into your applications. The package starts with a simple logger and can be extended with additional functions to meet the requirements of your application.
 Home-page: https://github.com/loggingpython-Community/loggingpython
 Author: mrmajor.programmer
 Author-email: mrmajork.programmer@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `loggingpython-1.4.3/README.md` & `loggingpython-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.3/setup.py` & `loggingpython-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='loggingpython',
-    version='1.4.3',
+    version='1.4.4',
     description='Loggingpython is a Python package that provides a simple and\
  extensible way to integrate logging into your applications. The package\
  starts with a simple logger and can be extended with additional functions to\
  meet the requirements of your application.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='mrmajor.programmer',
```

### Comparing `loggingpython-1.4.3/src/loggingpython/__init__.py` & `loggingpython-1.4.4/src/loggingpython/__init__.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.3/src/loggingpython/error/__init__.py` & `loggingpython-1.4.4/src/loggingpython/error/__init__.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.3/src/loggingpython/error/client_method_call_error.py` & `loggingpython-1.4.4/src/loggingpython/error/client_method_call_error.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.3/src/loggingpython/error/handler_not_found_error.py` & `loggingpython-1.4.4/src/loggingpython/error/handler_not_found_error.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.3/src/loggingpython/error/invalid_handler_method_error.py` & `loggingpython-1.4.4/src/loggingpython/error/invalid_handler_method_error.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.3/src/loggingpython/error/invalid_log_level_error.py` & `loggingpython-1.4.4/src/loggingpython/error/invalid_log_level_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 `loggingpython`
 Raised when an invalid log level is specified.
 This error indicates that the provided log level does not match any of the
 supported log levels.
 """
 
 
-class InvalidLogLevelErrorr(Exception):
+class InvalidLogLevelError(Exception):
     """
     `loggingpython`
     Raised when an invalid log level is specified.
     This error indicates that the provided log level does not match any of the
     supported log levels.
     """
     def __init__(self, log_level: str) -> None:
```

### Comparing `loggingpython-1.4.3/src/loggingpython/error/server_method_call_error.py` & `loggingpython-1.4.4/src/loggingpython/error/server_method_call_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 Raised when a method intended for the server is called on the client.
 This error indicates that a method that should only be executed by the
 server was mistakenly called by the client, which could lead to incorrect
 behavior.
 """
 
 
-class ServerMethodCallErrorr(Exception):
+class ServerMethodCallError(Exception):
     """
     `loggingpython`
     Raised when a method intended for the server is called on the client.
     This error indicates that a method that should only be executed by the
     server was mistakenly called by the client, which could lead to incorrect
     behavior.
     """
```

### Comparing `loggingpython-1.4.3/src/loggingpython/error/server_unreachable_error.py` & `loggingpython-1.4.4/src/loggingpython/error/server_unreachable_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 `loggingpython`
 Raised when the client fails to establish a connection to the server.
 This error indicates that the server might be unreachable due to network
 issues, incorrect server address or port, or the server not being active.
 """
 
 
-class ServerUnreachableErrorr(Exception):
+class ServerUnreachableError(Exception):
     """
     `loggingpython`
     Raised when the client fails to establish a connection to the server.
     This error indicates that the server might be unreachable due to network
     issues, incorrect server address or port, or the server not being active.
     """
     def __init__(self, servername: str, port: int):
```

### Comparing `loggingpython-1.4.3/src/loggingpython/handler/__init__.py` & `loggingpython-1.4.4/src/loggingpython/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.3/src/loggingpython/handler/consolehandler.py` & `loggingpython-1.4.4/src/loggingpython/handler/consolehandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.3/src/loggingpython/handler/csvhandler.py` & `loggingpython-1.4.4/src/loggingpython/handler/csvhandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.3/src/loggingpython/handler/filehandler.py` & `loggingpython-1.4.4/src/loggingpython/handler/filehandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.3/src/loggingpython/handler/handler.py` & `loggingpython-1.4.4/src/loggingpython/handler/handler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.3/src/loggingpython/handler/jsonhandler.py` & `loggingpython-1.4.4/src/loggingpython/handler/jsonhandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.3/src/loggingpython/handler/sqlhandler.py` & `loggingpython-1.4.4/src/loggingpython/handler/sqlhandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.3/src/loggingpython/handler/syshandler.py` & `loggingpython-1.4.4/src/loggingpython/handler/syshandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.3/src/loggingpython/log_levels.py` & `loggingpython-1.4.4/src/loggingpython/log_levels.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.3/src/loggingpython/logger.py` & `loggingpython-1.4.4/src/loggingpython/logger.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.3/src/loggingpython/sys_protocolls.py` & `loggingpython-1.4.4/src/loggingpython/sys_protocolls.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.3/src/loggingpython.egg-info/PKG-INFO` & `loggingpython-1.4.4/src/loggingpython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggingpython
-Version: 1.4.3
+Version: 1.4.4
 Summary: Loggingpython is a Python package that provides a simple and extensible way to integrate logging into your applications. The package starts with a simple logger and can be extended with additional functions to meet the requirements of your application.
 Home-page: https://github.com/loggingpython-Community/loggingpython
 Author: mrmajor.programmer
 Author-email: mrmajork.programmer@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `loggingpython-1.4.3/src/loggingpython.egg-info/SOURCES.txt` & `loggingpython-1.4.4/src/loggingpython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.3/test/test_init.py` & `loggingpython-1.4.4/test/test_init.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.3/test/test_logger.py` & `loggingpython-1.4.4/test/test_logger.py`

 * *Files identical despite different names*

