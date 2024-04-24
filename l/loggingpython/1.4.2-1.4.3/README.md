# Comparing `tmp/loggingpython-1.4.2.tar.gz` & `tmp/loggingpython-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggingpython-1.4.2.tar", last modified: Fri Apr 19 13:26:27 2024, max compression
+gzip compressed data, was "loggingpython-1.4.3.tar", last modified: Wed Apr 24 15:07:15 2024, max compression
```

## Comparing `loggingpython-1.4.2.tar` & `loggingpython-1.4.3.tar`

### file list

```diff
@@ -1,35 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 13:26:27.424312 loggingpython-1.4.2/
--rw-rw-rw-   0        0        0     1087 2024-03-04 14:25:44.000000 loggingpython-1.4.2/LICENSE
--rw-rw-rw-   0        0        0     3264 2024-04-19 13:26:27.423313 loggingpython-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     2366 2024-04-12 18:05:53.000000 loggingpython-1.4.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-19 13:26:27.424812 loggingpython-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1257 2024-04-19 13:25:54.000000 loggingpython-1.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 13:26:27.357312 loggingpython-1.4.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-19 13:26:27.375314 loggingpython-1.4.2/src/loggingpython/
--rw-rw-rw-   0        0        0     3763 2024-04-15 19:39:30.000000 loggingpython-1.4.2/src/loggingpython/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 13:26:27.409313 loggingpython-1.4.2/src/loggingpython/error/
--rw-rw-rw-   0        0        0      905 2024-04-05 12:51:00.000000 loggingpython-1.4.2/src/loggingpython/error/__init__.py
--rw-rw-rw-   0        0        0      439 2024-04-05 12:59:23.000000 loggingpython-1.4.2/src/loggingpython/error/client_method_call_error.py
--rw-rw-rw-   0        0        0      382 2024-04-05 12:57:01.000000 loggingpython-1.4.2/src/loggingpython/error/handler_not_found_error.py
--rw-rw-rw-   0        0        0      516 2024-04-07 13:27:03.000000 loggingpython-1.4.2/src/loggingpython/error/invalid_handler_method_error.py
--rw-rw-rw-   0        0        0      369 2024-04-07 13:41:59.000000 loggingpython-1.4.2/src/loggingpython/error/invalid_log_level_error.py
--rw-rw-rw-   0        0        0      439 2024-04-05 13:01:02.000000 loggingpython-1.4.2/src/loggingpython/error/server_method_call_error.py
--rw-rw-rw-   0        0        0      460 2024-04-07 13:28:09.000000 loggingpython-1.4.2/src/loggingpython/error/server_unreachable_error.py
-drwxrwxrwx   0        0        0        0 2024-04-19 13:26:27.418312 loggingpython-1.4.2/src/loggingpython/handler/
--rw-rw-rw-   0        0        0      777 2024-04-03 19:28:43.000000 loggingpython-1.4.2/src/loggingpython/handler/__init__.py
--rw-rw-rw-   0        0        0     3440 2024-04-17 14:05:56.000000 loggingpython-1.4.2/src/loggingpython/handler/consolehandler.py
--rw-rw-rw-   0        0        0     3937 2024-04-17 14:05:58.000000 loggingpython-1.4.2/src/loggingpython/handler/csvhandler.py
--rw-rw-rw-   0        0        0     4441 2024-04-19 13:11:20.000000 loggingpython-1.4.2/src/loggingpython/handler/filehandler.py
--rw-rw-rw-   0        0        0     1653 2024-04-14 13:50:01.000000 loggingpython-1.4.2/src/loggingpython/handler/handler.py
--rw-rw-rw-   0        0        0     5554 2024-04-17 14:06:10.000000 loggingpython-1.4.2/src/loggingpython/handler/jsonhandler.py
--rw-rw-rw-   0        0        0     4743 2024-04-17 14:06:26.000000 loggingpython-1.4.2/src/loggingpython/handler/sqlhandler.py
--rw-rw-rw-   0        0        0    12186 2024-04-15 19:20:42.000000 loggingpython-1.4.2/src/loggingpython/handler/syshandler.py
--rw-rw-rw-   0        0        0      163 2024-03-04 14:56:48.000000 loggingpython-1.4.2/src/loggingpython/log_levels.py
--rw-rw-rw-   0        0        0    16486 2024-04-14 14:44:12.000000 loggingpython-1.4.2/src/loggingpython/logger.py
--rw-rw-rw-   0        0        0      129 2024-04-03 16:16:15.000000 loggingpython-1.4.2/src/loggingpython/sys_procolls.py
-drwxrwxrwx   0        0        0        0 2024-04-19 13:26:27.419813 loggingpython-1.4.2/src/loggingpython.egg-info/
--rw-rw-rw-   0        0        0     3264 2024-04-19 13:26:27.000000 loggingpython-1.4.2/src/loggingpython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1025 2024-04-19 13:26:27.000000 loggingpython-1.4.2/src/loggingpython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 13:26:27.000000 loggingpython-1.4.2/src/loggingpython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-19 13:26:27.000000 loggingpython-1.4.2/src/loggingpython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-19 13:26:27.000000 loggingpython-1.4.2/src/loggingpython.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 15:07:15.022703 loggingpython-1.4.3/
+-rw-rw-rw-   0        0        0     1087 2024-03-04 14:25:44.000000 loggingpython-1.4.3/LICENSE
+-rw-rw-rw-   0        0        0     3264 2024-04-24 15:07:15.019702 loggingpython-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2366 2024-04-12 18:05:53.000000 loggingpython-1.4.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 15:07:15.022703 loggingpython-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1254 2024-04-24 15:06:42.000000 loggingpython-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:07:14.954703 loggingpython-1.4.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 15:07:14.962704 loggingpython-1.4.3/src/loggingpython/
+-rw-rw-rw-   0        0        0     5387 2024-04-24 11:59:06.000000 loggingpython-1.4.3/src/loggingpython/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:07:14.997702 loggingpython-1.4.3/src/loggingpython/error/
+-rw-rw-rw-   0        0        0     2553 2024-04-24 11:59:15.000000 loggingpython-1.4.3/src/loggingpython/error/__init__.py
+-rw-rw-rw-   0        0        0     1844 2024-04-24 12:01:18.000000 loggingpython-1.4.3/src/loggingpython/error/client_method_call_error.py
+-rw-rw-rw-   0        0        0     1733 2024-04-24 12:01:53.000000 loggingpython-1.4.3/src/loggingpython/error/handler_not_found_error.py
+-rw-rw-rw-   0        0        0     1911 2024-04-24 12:02:15.000000 loggingpython-1.4.3/src/loggingpython/error/invalid_handler_method_error.py
+-rw-rw-rw-   0        0        0     1693 2024-04-24 12:02:33.000000 loggingpython-1.4.3/src/loggingpython/error/invalid_log_level_error.py
+-rw-rw-rw-   0        0        0     1845 2024-04-24 12:02:49.000000 loggingpython-1.4.3/src/loggingpython/error/server_method_call_error.py
+-rw-rw-rw-   0        0        0     1857 2024-04-24 12:03:04.000000 loggingpython-1.4.3/src/loggingpython/error/server_unreachable_error.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:07:15.012702 loggingpython-1.4.3/src/loggingpython/handler/
+-rw-rw-rw-   0        0        0     2399 2024-04-24 11:58:58.000000 loggingpython-1.4.3/src/loggingpython/handler/__init__.py
+-rw-rw-rw-   0        0        0     4883 2024-04-24 12:03:29.000000 loggingpython-1.4.3/src/loggingpython/handler/consolehandler.py
+-rw-rw-rw-   0        0        0     5533 2024-04-24 12:04:33.000000 loggingpython-1.4.3/src/loggingpython/handler/csvhandler.py
+-rw-rw-rw-   0        0        0     5544 2024-04-24 12:04:58.000000 loggingpython-1.4.3/src/loggingpython/handler/filehandler.py
+-rw-rw-rw-   0        0        0     3019 2024-04-24 12:05:15.000000 loggingpython-1.4.3/src/loggingpython/handler/handler.py
+-rw-rw-rw-   0        0        0     7291 2024-04-24 12:05:33.000000 loggingpython-1.4.3/src/loggingpython/handler/jsonhandler.py
+-rw-rw-rw-   0        0        0     6494 2024-04-24 12:05:52.000000 loggingpython-1.4.3/src/loggingpython/handler/sqlhandler.py
+-rw-rw-rw-   0        0        0    13938 2024-04-24 12:08:57.000000 loggingpython-1.4.3/src/loggingpython/handler/syshandler.py
+-rw-rw-rw-   0        0        0     2307 2024-04-24 13:02:57.000000 loggingpython-1.4.3/src/loggingpython/log_levels.py
+-rw-rw-rw-   0        0        0    19026 2024-04-24 12:06:37.000000 loggingpython-1.4.3/src/loggingpython/logger.py
+-rw-rw-rw-   0        0        0     2038 2024-04-24 12:09:12.000000 loggingpython-1.4.3/src/loggingpython/sys_protocolls.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:07:15.018702 loggingpython-1.4.3/src/loggingpython.egg-info/
+-rw-rw-rw-   0        0        0     3264 2024-04-24 15:07:14.000000 loggingpython-1.4.3/src/loggingpython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1117 2024-04-24 15:07:14.000000 loggingpython-1.4.3/src/loggingpython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 15:07:14.000000 loggingpython-1.4.3/src/loggingpython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-24 15:07:14.000000 loggingpython-1.4.3/src/loggingpython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-24 15:07:14.000000 loggingpython-1.4.3/src/loggingpython.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 15:07:15.017702 loggingpython-1.4.3/test/
+-rw-rw-rw-   0        0        0     1021 2024-04-23 13:59:00.000000 loggingpython-1.4.3/test/test_init.py
+-rw-rw-rw-   0        0        0      496 2024-04-23 13:58:57.000000 loggingpython-1.4.3/test/test_log_levels.py
+-rw-rw-rw-   0        0        0     1611 2024-04-21 17:52:48.000000 loggingpython-1.4.3/test/test_logger.py
+-rw-rw-rw-   0        0        0      388 2024-04-23 16:32:24.000000 loggingpython-1.4.3/test/test_sys_protocolls.py
```

### Comparing `loggingpython-1.4.2/LICENSE` & `loggingpython-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.2/PKG-INFO` & `loggingpython-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggingpython
-Version: 1.4.2
+Version: 1.4.3
 Summary: Loggingpython is a Python package that provides a simple and extensible way to integrate logging into your applications. The package starts with a simple logger and can be extended with additional functions to meet the requirements of your application.
 Home-page: https://github.com/loggingpython-Community/loggingpython
 Author: mrmajor.programmer
 Author-email: mrmajork.programmer@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `loggingpython-1.4.2/README.md` & `loggingpython-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `loggingpython-1.4.2/setup.py` & `loggingpython-1.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='loggingpython',
-    version='1.4.2',
+    version='1.4.3',
     description='Loggingpython is a Python package that provides a simple and\
  extensible way to integrate logging into your applications. The package\
  starts with a simple logger and can be extended with additional functions to\
  meet the requirements of your application.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='mrmajor.programmer',
@@ -25,10 +25,10 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: System :: Logging',
     ],
     include_package_data=True,
     package_data={
-        '': ['docs/*.md'],
+        '': ['docs/*'],
     },
 )
```

### Comparing `loggingpython-1.4.2/src/loggingpython/handler/sqlhandler.py` & `loggingpython-1.4.3/src/loggingpython/handler/csvhandler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,105 +1,117 @@
+# MIT License
+
+# Copyright (c) 2024 Mr-Major-K
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+"""
+A class for handling log messages in CSV format.
+
+This class inherits from the Handler class and implements specific
+methods for formatting and outputting log messages in CSV files. It
+supports the creation of new log files based on the current date and
+allows customization of the log format string. The CSVHandler ensures
+that log messages are stored in a structured and easily accessible format,
+making it suitable for further analysis or review.
+"""
+
 import os
 from datetime import datetime
-import sqlite3
+import pandas as pd
 
 from .handler import Handler
 
 
-class SQLHandler(Handler):
+class CSVHandler(Handler):
     """
-    A class for handling log messages in SQL databases.
+    A class for handling log messages in CSV format.
 
     This class inherits from the Handler class and implements specific
-    methods for formatting and outputting log messages into SQL databases. It
-    supports the creation of new log databases based on the current date and
-    allows customization of the log format string. The SQLHandler ensures
+    methods for formatting and outputting log messages in CSV files. It
+    supports the creation of new log files based on the current date and
+    allows customization of the log format string. The CSVHandler ensures
     that log messages are stored in a structured and easily accessible format,
-    making it suitable for further analysis or review. It also includes
-    features for updating the log database if the current date has changed and
-    for creating the necessary database structure.
+    making it suitable for further analysis or review.
     """
+
     def __init__(self,
                  name: str,
-                 path: str = "logs") -> None:
+                 path: str = "logs",
+                 logformat_string: str = "%(asctime)s: [%(loggername)s]: \
+[%(loglevel)s]: %(message)s") -> None:
         """
-        Initializes the SQLHandler with the given name, log path, and log
+        Initializes the CSVHandler with the given name, log path, and log
             format string.
 
         Args:
             name (str): The name of the log file.
             path (str, optional): The path where the log files will be
                 stored. Defaults to "logs".
             logformat_string (str, optional): The format string for the log
                 messages. Defaults to "%(asctime)s: [%(loggername)s]:
                 [%(loglevel)s]: %(message)s".
         """
         self._mk_logdir(path)
         self.name: str = name
         self.path: str = path
         self._current_date: str = datetime.now().strftime("%Y-%m-%d")
-        self.file: str = f"{self.path}/{self.name}_{self._current_date}.db"
+        self.file: str = f"{self.path}/{self.name}_{self._current_date}.csv"
         self._mk_logfile(self.file)
-        self._creat_db()
+        self.file = open(self.file, "a")
+
+        self.logformat_string: str = logformat_string
 
     def emit(self, record: dict) -> None:
         """
-        Writes a log record to the database.
+        Writes a log record to the file.
 
         Args:
             record (dict): A dictionary containing the log record details.
         """
-        hash_message = hash(str(record))
-        message = record.get("message", "")
-        loglevel = record.get("loglevel", "")
-        asctime = record.get("asctime", "")
-        iso_8601_time = record.get("iso_8601_time", "")
-        loggername = record.get("loggername", "")
-
-        with sqlite3.connect(self.file) as conn:
-            cursor = conn.cursor()
-            cursor.execute(
-                """
-                INSERT INTO logs (hash_message, message, loglevel, asctime, \
-iso_8601_time, loggername)
-                VALUES (?, ?, ?, ?, ?, ?)
-                """,
-                (hash_message, message, loglevel, asctime, iso_8601_time,
-                 loggername)
-            )
-            conn.commit()
-
-    def _creat_db(self) -> None:
-        with sqlite3.connect(self.file) as conn:
-            cursor = conn.cursor()
-            cursor.execute(
-                """
-                CREATE TABLE IF NOT EXISTS logs (
-                    hash_message TEXT PRIMARY KEY,
-                    message TEXT,
-                    loglevel TEXT,
-                    asctime TEXT,
-                    iso_8601_time TEXT,
-                    loggername TEXT
-                )"""
-            )
-            conn.commit()
+        formatted_message_values = self._format_message(record)
+
+        df = pd.DataFrame([formatted_message_values])
+
+        formatted_message = df.to_csv(index=False, header=False, sep=";",
+                                      lineterminator="\n")
+
+        return formatted_message
+        self._update_file()
+        self.file.write(formatted_message)
+        self.file.flush()
 
-    def _update_file(self) -> None:
+    def _update_file(self):
         """
         Updates the log file if the current date has changed.
         """
         current_date = datetime.now().strftime("%Y-%m-%d")
         if current_date != self._current_date:
-            self._current_date = current_date
-            self.file = f"{self.path}/{self.name}_{self._current_date}.db"
-            self._mk_logfile(self.file)
-            self._creat_db()
+            self.current_date = current_date
+            self._close_file()
+            filename = f"{self.logpath}/{self.name}_{self._current_date}.csv"
+            self.file = open(filename, "a")
 
-    def _close_file(self) -> None:
+    def _close_file(self):
         """
         Closes the current log file.
         """
         if self.file:
             self.file.close()
 
     def _mk_logdir(self, logpath: str) -> None:
@@ -128,11 +140,12 @@
 
         Returns:
             str: The current date.
         """
         return datetime.now().strftime("%Y-%m-%d")
 
     def __repr__(self) -> str:
-        return f"SQLHandler({self.name}, {self.path})"
+        return f"CSVHandler({self.name}, {self.path}, {self.logformat_string})"
 
     def __str__(self) -> str:
-        return f"SQLHandler with:{self.name} and {self.path}"
+        return f"CSVHandler with: {self.name}, {self.path} and \
+{self.logformat_string}"
```

### Comparing `loggingpython-1.4.2/src/loggingpython/handler/syshandler.py` & `loggingpython-1.4.3/src/loggingpython/handler/syshandler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,48 @@
+# MIT License
+
+# Copyright (c) 2024 Mr-Major-K
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+"""
+A class for handling log messages over a network connection.
+
+This class inherits from the Handler class and implements specific methods
+for sending and receiving log messages over a network connection. It
+supports both client and server modes, allowing for the establishment of
+connections, sending log messages, and handling incoming messages. The
+class provides decorators to ensure that certain methods can only be
+called by the client or server, enforcing the correct usage of the handler.
+It also includes error handling for scenarios such as server
+unreachability and incorrect method calls.
+   """
+
 import socket
 import json
 from functools import partial
 
 from .handler import Handler
-from ..sys_procolls import SysProtocolls
+from ..sys_protocolls import SysProtocolls
 from ..error.server_unreachable_error import ServerUnreachableError
 from ..error.server_method_call_error import ServerMethodCallError
 from ..error.client_method_call_error import ClientMethodCallError
 
 
 class SysHandler(Handler):
     """
@@ -18,14 +53,15 @@
     supports both client and server modes, allowing for the establishment of
     connections, sending log messages, and handling incoming messages. The
     class provides decorators to ensure that certain methods can only be
     called by the client or server, enforcing the correct usage of the handler.
     It also includes error handling for scenarios such as server
     unreachability and incorrect method calls.
     """
+
     def __init__(self,
                  name: str = "client",
                  client: bool = True,
                  protocoll: SysProtocolls = SysProtocolls.TCP,
                  server_name: str = "localhost",
                  port: int = 8080,
                  logformat_string: str = "%(asctime)s: [%(client_name)s] \
```

### Comparing `loggingpython-1.4.2/src/loggingpython/logger.py` & `loggingpython-1.4.3/src/loggingpython/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,57 @@
+# MIT License
+
+# Copyright (c) 2024 Mr-Major-K
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+"""
+A class for handling log messages in a structured and extensible way.
+
+This class, `Logger`, is designed to provide a simple and customizable
+logging solution for Python applications. It inherits from a base `Handler`
+class and implements specific methods for formatting and outputting log
+messages. The `Logger` class supports various log levels, including DEBUG,
+INFO, WARNING, ERROR, and CRITICAL, allowing for detailed and flexible
+logging.
+
+The `Logger` class is equipped with methods for adding and removing
+handlers, which are responsible for processing and outputting log messages.
+Handlers can be customized to output log messages to various destinations,
+such as the console, files, databases, or external systems. This
+extensibility makes the `Logger` class suitable for a wide range of
+applications, from simple scripts to complex systems.
+
+The `Logger` class also includes methods for logging messages at different
+severity levels, ensuring that developers can easily categorize and
+prioritize log messages based on their importance. Additionally, the class
+provides a mechanism for catching exceptions and logging them,
+facilitating error handling and debugging.
+
+In summary, the `Logger` class offers a straightforward and powerful way
+to integrate logging into Python applications, providing a foundation for
+both basic and advanced logging requirements.
+"""
+
 from datetime import datetime, timezone
 
 from .log_levels import LogLevel
 from .handler import Handler
 from .error.invalid_log_level_error import InvalidLogLevelError
 from .error.invalid_handler_method_error import InvalidHandlerMethodError
 from .error.handler_not_found_error import HandlerNotFoundError
@@ -78,15 +128,15 @@
             loglevel (LogLevel): The log level to be validated.
 
         Raises:
             InvalidLogLevelError: If the loglevel is not supported.
         """
 
         if loglevel not in self._SUPPORTED_LEVELS:
-            raise InvalidLogLevelError()
+            raise InvalidLogLevelError(loglevel)
 
     def _loglevel_over_min_loglevel(self, loglevel: LogLevel) -> bool:
         """
         Checks if the provided log level is over the minimum log level.
 
         Args:
             loglevel (LogLevel): The log level to check.
```

### Comparing `loggingpython-1.4.2/src/loggingpython.egg-info/PKG-INFO` & `loggingpython-1.4.3/src/loggingpython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggingpython
-Version: 1.4.2
+Version: 1.4.3
 Summary: Loggingpython is a Python package that provides a simple and extensible way to integrate logging into your applications. The package starts with a simple logger and can be extended with additional functions to meet the requirements of your application.
 Home-page: https://github.com/loggingpython-Community/loggingpython
 Author: mrmajor.programmer
 Author-email: mrmajork.programmer@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `loggingpython-1.4.2/src/loggingpython.egg-info/SOURCES.txt` & `loggingpython-1.4.3/src/loggingpython.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 LICENSE
 README.md
 setup.py
 src/loggingpython/__init__.py
 src/loggingpython/log_levels.py
 src/loggingpython/logger.py
-src/loggingpython/sys_procolls.py
+src/loggingpython/sys_protocolls.py
 src/loggingpython.egg-info/PKG-INFO
 src/loggingpython.egg-info/SOURCES.txt
 src/loggingpython.egg-info/dependency_links.txt
 src/loggingpython.egg-info/requires.txt
 src/loggingpython.egg-info/top_level.txt
 src/loggingpython/error/__init__.py
 src/loggingpython/error/client_method_call_error.py
@@ -20,8 +20,12 @@
 src/loggingpython/handler/__init__.py
 src/loggingpython/handler/consolehandler.py
 src/loggingpython/handler/csvhandler.py
 src/loggingpython/handler/filehandler.py
 src/loggingpython/handler/handler.py
 src/loggingpython/handler/jsonhandler.py
 src/loggingpython/handler/sqlhandler.py
-src/loggingpython/handler/syshandler.py
+src/loggingpython/handler/syshandler.py
+test/test_init.py
+test/test_log_levels.py
+test/test_logger.py
+test/test_sys_protocolls.py
```

