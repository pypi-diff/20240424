# Comparing `tmp/mloggers-1.2.0.tar.gz` & `tmp/mloggers-1.2.1.tar.gz`

## Comparing `mloggers-1.2.0.tar` & `mloggers-1.2.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mloggers-1.2.0/.taplo.toml
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mloggers-1.2.0/mloggers/__init__.py
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 mloggers-1.2.0/mloggers/_log_levels.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 mloggers-1.2.0/mloggers/console_logger.py
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 mloggers-1.2.0/mloggers/file_logger.py
--rw-r--r--   0        0        0     7813 2020-02-02 00:00:00.000000 mloggers-1.2.0/mloggers/logger.py
--rw-r--r--   0        0        0     7168 2020-02-02 00:00:00.000000 mloggers-1.2.0/mloggers/multi_logger.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 mloggers-1.2.0/mloggers/progress.py
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 mloggers-1.2.0/mloggers/wandb_logger.py
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 mloggers-1.2.0/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mloggers-1.2.0/LICENSE
--rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 mloggers-1.2.0/README.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 mloggers-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 mloggers-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mloggers-1.2.1/.taplo.toml
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 mloggers-1.2.1/test.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 mloggers-1.2.1/mloggers/__init__.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 mloggers-1.2.1/mloggers/_log_levels.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 mloggers-1.2.1/mloggers/console_logger.py
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 mloggers-1.2.1/mloggers/file_logger.py
+-rw-r--r--   0        0        0     7822 2020-02-02 00:00:00.000000 mloggers-1.2.1/mloggers/logger.py
+-rw-r--r--   0        0        0     7168 2020-02-02 00:00:00.000000 mloggers-1.2.1/mloggers/multi_logger.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 mloggers-1.2.1/mloggers/optional_logger.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 mloggers-1.2.1/mloggers/progress.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 mloggers-1.2.1/mloggers/wandb_logger.py
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 mloggers-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mloggers-1.2.1/LICENSE
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 mloggers-1.2.1/README.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 mloggers-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6295 2020-02-02 00:00:00.000000 mloggers-1.2.1/PKG-INFO
```

### Comparing `mloggers-1.2.0/mloggers/_log_levels.py` & `mloggers-1.2.1/mloggers/_log_levels.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.2.0/mloggers/console_logger.py` & `mloggers-1.2.1/mloggers/console_logger.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.2.0/mloggers/file_logger.py` & `mloggers-1.2.1/mloggers/file_logger.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.2.0/mloggers/logger.py` & `mloggers-1.2.1/mloggers/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,28 +90,29 @@
 
         ### Parameters
         ----------
         `level`: the log level to set.
         - If a string, it must be a valid log level (e.g., INFO, WARN, ERROR, DEBUG, etc.).
         - If a `LogLevel` object, it will be used as-is.
         """
+
         self._log_level = level.value["level"] if isinstance(level, LogLevel) else level
 
     def _call_impl(self, *args, **kwargs):
         return self.log(*args, **kwargs)
 
     __call__: Callable[..., Any] = _call_impl
 
     def info(
         self,
         *messages: str | dict[str, Any],
         **kwargs: Any,
     ):
         """
-        Wrapper for calling `log` with level=LogLevel.INFO.
+        Wrapper for calling `log` with `level=LogLevel.INFO`.
 
         ### Parameters
         ----------
         `messages`: the messages to log.
         - These can be any number of messages, separated by commas. They can be of the following types:
         - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
         - If a dictionary, the message will be logged as a JSON string.
@@ -123,15 +124,15 @@
 
     def warn(
         self,
         *messages: str | dict[str, Any],
         **kwargs: Any,
     ):
         """
-        Wrapper for calling `log` with level=LogLevel.WARN.
+        Wrapper for calling `log` with `level=LogLevel.WARN`.
 
         ### Parameters
         ----------
         `messages`: the messages to log.
         - These can be any number of messages, separated by commas. They can be of the following types:
         - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
         - If a dictionary, the message will be logged as a JSON string.
@@ -146,15 +147,15 @@
 
     def error(
         self,
         *messages: str | dict[str, Any],
         **kwargs: Any,
     ):
         """
-        Wrapper for calling `log` with level=LogLevel.ERROR.
+        Wrapper for calling `log` with `level=LogLevel.ERROR`.
 
         ### Parameters
         ----------
         `messages`: the messages to log.
         - These can be any number of messages, separated by commas. They can be of the following types:
         - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
         - If a dictionary, the message will be logged as a JSON string.
@@ -166,15 +167,15 @@
 
     def debug(
         self,
         *messages: str | dict[str, Any],
         **kwargs: Any,
     ):
         """
-        Wrapper for calling `log` with level=LogLevel.DEBUG.
+        Wrapper for calling `log` with `level=LogLevel.DEBUG`.
 
         ### Parameters
         ----------
         `messages`: the messages to log.
         - These can be any number of messages, separated by commas. They can be of the following types:
         - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
         - If a dictionary, the message will be logged as a JSON string.
```

### Comparing `mloggers-1.2.0/mloggers/multi_logger.py` & `mloggers-1.2.1/mloggers/multi_logger.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.2.0/mloggers/progress.py` & `mloggers-1.2.1/mloggers/progress.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.2.0/mloggers/wandb_logger.py` & `mloggers-1.2.1/mloggers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.2.0/.gitignore` & `mloggers-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mloggers-1.2.0/LICENSE` & `mloggers-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mloggers-1.2.0/README.md` & `mloggers-1.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -108,7 +108,39 @@
 ### Customized loggers
 
 You can extend the base class `Logger` in order to create a custom logger to suit your own needs. Make sure to implement all abstract methods.
 
 ### Customized log levels
 
 You can register new log levels by using `register_level(level, color)`. Once you register a level `"MyLevel"`, you can use it as `logger.log(message, LogLevel.MYLEVEL)`. The method `log` also supports a string as a level, which will be upper-cased and given a default color; the level can also be `None`, which will simply log the message as a stand-alone.
+
+### Optional loggers
+This library also includes a wrapper around the `Logger` class called `OptionalLogger`, which allows you to use a logger which could be `None` without having to check its validity before every use. Hence, instead of this:
+
+```python
+from mloggers import Logger
+
+
+class MyClass:
+    def __init__(self, logger: Logger | None):
+        self._logger = logger
+
+    def my_function(self):
+        if self._logger is not None:
+            self._logger.info("Message")
+```
+
+You can do this:
+
+```python
+from mloggers import Logger, OptionalLogger
+
+
+class MyClass:
+    def __init__(self, logger: Logger | None):
+        self._logger = OptionalLogger(logger)
+
+    def my_function(self):
+        self._logger.info("Message")
+```
+
+If the logger is `None`, nothing will happen (not even an error!).
```

### Comparing `mloggers-1.2.0/pyproject.toml` & `mloggers-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mloggers"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
     { name = "Sergio Hernandez Gutierrez", email = "contact.sergiohernandez@gmail.com" },
     { name = "Matteo Merler", email = "matteo.merler@gmail.com" },
 ]
 description = "A collection of loggers well-suited for machine learning experiments."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `mloggers-1.2.0/PKG-INFO` & `mloggers-1.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mloggers
-Version: 1.2.0
+Version: 1.2.1
 Summary: A collection of loggers well-suited for machine learning experiments.
 Project-URL: Homepage, https://github.com/serhez/mloggers
 Project-URL: Issues, https://github.com/serhez/mloggers/issues
 Author-email: Sergio Hernandez Gutierrez <contact.sergiohernandez@gmail.com>, Matteo Merler <matteo.merler@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -128,7 +128,39 @@
 ### Customized loggers
 
 You can extend the base class `Logger` in order to create a custom logger to suit your own needs. Make sure to implement all abstract methods.
 
 ### Customized log levels
 
 You can register new log levels by using `register_level(level, color)`. Once you register a level `"MyLevel"`, you can use it as `logger.log(message, LogLevel.MYLEVEL)`. The method `log` also supports a string as a level, which will be upper-cased and given a default color; the level can also be `None`, which will simply log the message as a stand-alone.
+
+### Optional loggers
+This library also includes a wrapper around the `Logger` class called `OptionalLogger`, which allows you to use a logger which could be `None` without having to check its validity before every use. Hence, instead of this:
+
+```python
+from mloggers import Logger
+
+
+class MyClass:
+    def __init__(self, logger: Logger | None):
+        self._logger = logger
+
+    def my_function(self):
+        if self._logger is not None:
+            self._logger.info("Message")
+```
+
+You can do this:
+
+```python
+from mloggers import Logger, OptionalLogger
+
+
+class MyClass:
+    def __init__(self, logger: Logger | None):
+        self._logger = OptionalLogger(logger)
+
+    def my_function(self):
+        self._logger.info("Message")
+```
+
+If the logger is `None`, nothing will happen (not even an error!).
```

