# Comparing `tmp/mloggers-1.3.0.tar.gz` & `tmp/mloggers-1.3.1.tar.gz`

## Comparing `mloggers-1.3.0.tar` & `mloggers-1.3.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mloggers-1.3.0/.taplo.toml
--rw-r--r--   0        0        0    23530 2020-02-02 00:00:00.000000 mloggers-1.3.0/test.ipynb
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 mloggers-1.3.0/test.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 mloggers-1.3.0/mloggers/__init__.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 mloggers-1.3.0/mloggers/_log_levels.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 mloggers-1.3.0/mloggers/console_logger.py
--rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 mloggers-1.3.0/mloggers/file_logger.py
--rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 mloggers-1.3.0/mloggers/logger.py
--rw-r--r--   0        0        0     7064 2020-02-02 00:00:00.000000 mloggers-1.3.0/mloggers/multi_logger.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 mloggers-1.3.0/mloggers/optional_logger.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 mloggers-1.3.0/mloggers/progress.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 mloggers-1.3.0/mloggers/wandb_logger.py
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 mloggers-1.3.0/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mloggers-1.3.0/LICENSE
--rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 mloggers-1.3.0/README.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 mloggers-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 mloggers-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mloggers-1.3.1/.taplo.toml
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 mloggers-1.3.1/log.json
+-rw-r--r--   0        0        0    23530 2020-02-02 00:00:00.000000 mloggers-1.3.1/test.ipynb
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 mloggers-1.3.1/test.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 mloggers-1.3.1/mloggers/__init__.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 mloggers-1.3.1/mloggers/_log_levels.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 mloggers-1.3.1/mloggers/console_logger.py
+-rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 mloggers-1.3.1/mloggers/file_logger.py
+-rw-r--r--   0        0        0     9649 2020-02-02 00:00:00.000000 mloggers-1.3.1/mloggers/logger.py
+-rw-r--r--   0        0        0     8703 2020-02-02 00:00:00.000000 mloggers-1.3.1/mloggers/multi_logger.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 mloggers-1.3.1/mloggers/optional_logger.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 mloggers-1.3.1/mloggers/progress.py
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 mloggers-1.3.1/mloggers/wandb_logger.py
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 mloggers-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mloggers-1.3.1/LICENSE
+-rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 mloggers-1.3.1/README.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 mloggers-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 mloggers-1.3.1/PKG-INFO
```

### Comparing `mloggers-1.3.0/test.ipynb` & `mloggers-1.3.1/test.ipynb`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.0/mloggers/_log_levels.py` & `mloggers-1.3.1/mloggers/_log_levels.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.0/mloggers/console_logger.py` & `mloggers-1.3.1/mloggers/console_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import json
 from datetime import datetime
 from typing import Any
 
+import numpy.typing as npt
 from termcolor import colored
 
 from mloggers._log_levels import LogLevel, _log_level_properties
 from mloggers.logger import Logger
 
 
 class ConsoleLogger(Logger):
     """Logs to the console (i.e., standard I/O)."""
 
     def __init__(self, default_priority: LogLevel = LogLevel.INFO):  # type:ignore[reportArgumentType]
         super().__init__(default_priority)
 
     def log(
         self,
-        *messages: str | dict[str, Any],
+        *messages: str | dict[str, Any] | list[Any] | npt.NDArray[Any],
         level: LogLevel | str | None = None,
         **kwargs: Any,
     ):
         if not super(ConsoleLogger, self).log(*messages, level=level, **kwargs):
             return
 
         time = "[" + datetime.now().strftime("%H:%M:%S") + "]"
```

### Comparing `mloggers-1.3.0/mloggers/file_logger.py` & `mloggers-1.3.1/mloggers/file_logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import json
 import os
 from datetime import datetime
 from typing import Any
 
 import numpy as np
+import numpy.typing as npt
 from termcolor import colored
 
 from mloggers._log_levels import LogLevel
 from mloggers.logger import Logger
 
 
 class FileLogger(Logger):
     """Logs to a file."""
 
-    def __init__(self, file_path: str, default_priority: LogLevel | int = LogLevel.INFO):  # type:ignore[reportArgumentType]
+    def __init__(
+        self,
+        file_path: str,
+        default_priority: LogLevel | int = LogLevel.INFO,  # type:ignore[reportArgumentType]
+    ):
         """
         Initializes a file logger.
 
         ### Parameters
         ----------
         `file_path`: the path to the file to log to.
         - The file will be created if it does not exist. If it does, the logs will be appended to it.
@@ -40,15 +45,15 @@
 
         print(f'{colored("[INFO]", "cyan")} [FileLogger] Logging to file {file_path}')
 
         self._file_path = file_path
 
     def log(
         self,
-        *messages: str | dict[str, Any],
+        *messages: str | dict[str, Any] | list[Any] | npt.NDArray[Any],
         level: LogLevel | str | None = None,
         **kwargs: Any,
     ):
         if not super(FileLogger, self).log(*messages, level=level, **kwargs):
             return
 
         # Handle multiple messages
@@ -67,14 +72,16 @@
                 for message in messages:
                     self.log(message, level=level)
                 return
         else:
             message = messages[0]
 
         # Convert numpy's ndarrays to lists so that they are JSON serializable
+        if isinstance(message, np.ndarray):
+            message = message.tolist()
         if isinstance(message, dict):
             for key, value in message.items():
                 if isinstance(value, np.ndarray):
                     message[key] = value.tolist()
         elif hasattr(message, "__str__") and callable(getattr(message, "__str__")):
             message = str(message)
```

### Comparing `mloggers-1.3.0/mloggers/logger.py` & `mloggers-1.3.1/mloggers/logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from abc import ABC, abstractmethod
 from typing import Any, Callable
 
+import numpy.typing as npt
+
 from mloggers._log_levels import LogLevel, _log_level_properties
 
 # This constant is used to assign an importance level to anything not using the LogLevel enum.
 # It was chosen to be the same as `LogLevel.INFO`, but it can be changed to any other value.
 DEFAULT_IMPORTANCE = _log_level_properties[LogLevel.INFO].priority  # type:ignore[reportAttributeAccessIssue]
 
 
@@ -13,48 +15,49 @@
 
     def __init__(self, default_priority: LogLevel | int = LogLevel.INFO):  # type:ignore[reportArgumentType]
         """
         Initialize the logger.
 
         ### Parameters
         ----------
-        `log_level`: The default log level priority to use.
+        `default_priority`: The default log level priority to use.
         - This parameter filters out messages with a lower importance level than the one provided. It can be either a `LogLevel` object or an integer.
         - When calling the logger with a level not from the `LogLevel` enum, the importance level will be set to 0 (same as `LogLevel.INFO`).
         - For example, if the log level is set to `LogLevel.INFO`, only messages with a level of `LogLevel.INFO` or higher will be printed (which excludes `LogLevel.DEBUG`).
         """
 
         self._min_priority = (
             _log_level_properties[default_priority].priority
             if isinstance(default_priority, LogLevel)
             else default_priority
         )
 
     @abstractmethod
     def log(
         self,
-        *messages: str | dict[str, Any],
+        *messages: str | dict[str, Any] | list[Any] | npt.NDArray[Any],
         level: LogLevel | str | None = None,
         **kwargs: Any,
     ):
         """
         Log a message.
 
         ### Parameters
         ----------
         `messages`: the messages to log.
         - These can be any number of messages, separated by commas. They can be of the following types:
             - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
+            - If a list or numpy array, the message will be logged as a stringified list.
             - If a dictionary, the message will be logged as a JSON string.
                 - The dictionary must be JSON serializable.
                 - You can provide None dictionary values to mean that the key is a header or title of the message.
-            `level`: the level of the message (e.g., INFO, WARN, ERROR, DEBUG, etc.).
-            - If None, no level will be printed.
-            - If a string is provided, it will be colored in green (when colors are used) and uppercased; otherwise, the color will be the one associated with the `LogLevel` at time of registration.
-        - If multiple messages are provided, they must be either all strings or all dictionaries. Strings will be joined into a single string, while dictionaries will be printed as separate log entries.
+        - If multiple messages are provided, they must be either all dictionaries or none of them. Strings, lists and arrays will be joined into a single string, while dictionaries will be printed as separate log entries.
+        `level`: the level of the message (e.g., INFO, WARN, ERROR, DEBUG, etc.).
+        - If None, no level will be printed.
+        - If a string is provided, it will be colored in green (when colors are used) and uppercased; otherwise, the color will be the one associated with the `LogLevel` at time of registration.
 
         ### Raises
         ----------
         `TypeError`: if the message is not a string, a dictionary or does not implement `__str__()`.
         `TypeError`: if the messages are a mix of strings and dictionaries.
         """
 
@@ -106,87 +109,95 @@
     def _call_impl(self, *args, **kwargs):
         return self.log(*args, **kwargs)
 
     __call__: Callable[..., Any] = _call_impl
 
     def info(
         self,
-        *messages: str | dict[str, Any],
+        *messages: str | dict[str, Any] | list[Any] | npt.NDArray[Any],
         **kwargs: Any,
     ):
         """
         Wrapper for calling `log` with `level=LogLevel.INFO`.
 
         ### Parameters
         ----------
         `messages`: the messages to log.
         - These can be any number of messages, separated by commas. They can be of the following types:
-        - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
-        - If a dictionary, the message will be logged as a JSON string.
-            - The dictionary must be JSON serializable.
-            - You can provide None dictionary values to mean that the key is a header or title of the message.
+            - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
+            - If a list or numpy array, the message will be logged as a stringified list.
+            - If a dictionary, the message will be logged as a JSON string.
+                - The dictionary must be JSON serializable.
+                - You can provide None dictionary values to mean that the key is a header or title of the message.
+        - If multiple messages are provided, they must be either all dictionaries or none of them. Strings, lists and arrays will be joined into a single string, while dictionaries will be printed as separate log entries.
         """
 
         self.log(*messages, level=LogLevel.INFO, **kwargs)  # type:ignore[reportArgumentType]
 
     def warn(
         self,
-        *messages: str | dict[str, Any],
+        *messages: str | dict[str, Any] | list[Any] | npt.NDArray[Any],
         **kwargs: Any,
     ):
         """
         Wrapper for calling `log` with `level=LogLevel.WARN`.
 
         ### Parameters
         ----------
         `messages`: the messages to log.
         - These can be any number of messages, separated by commas. They can be of the following types:
-        - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
-        - If a dictionary, the message will be logged as a JSON string.
-            - The dictionary must be JSON serializable.
-            - You can provide None dictionary values to mean that the key is a header or title of the message.
+            - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
+            - If a list or numpy array, the message will be logged as a stringified list.
+            - If a dictionary, the message will be logged as a JSON string.
+                - The dictionary must be JSON serializable.
+                - You can provide None dictionary values to mean that the key is a header or title of the message.
+        - If multiple messages are provided, they must be either all dictionaries or none of them. Strings, lists and arrays will be joined into a single string, while dictionaries will be printed as separate log entries.
         """
 
         self.log(*messages, level=LogLevel.WARN, **kwargs)  # type:ignore[reportArgumentType]
 
     # Alias warning to warn
     warning = warn
 
     def error(
         self,
-        *messages: str | dict[str, Any],
+        *messages: str | dict[str, Any] | list[Any] | npt.NDArray[Any],
         **kwargs: Any,
     ):
         """
         Wrapper for calling `log` with `level=LogLevel.ERROR`.
 
         ### Parameters
         ----------
         `messages`: the messages to log.
         - These can be any number of messages, separated by commas. They can be of the following types:
-        - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
-        - If a dictionary, the message will be logged as a JSON string.
-            - The dictionary must be JSON serializable.
-            - You can provide None dictionary values to mean that the key is a header or title of the message.
+            - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
+            - If a list or numpy array, the message will be logged as a stringified list.
+            - If a dictionary, the message will be logged as a JSON string.
+                - The dictionary must be JSON serializable.
+                - You can provide None dictionary values to mean that the key is a header or title of the message.
+        - If multiple messages are provided, they must be either all dictionaries or none of them. Strings, lists and arrays will be joined into a single string, while dictionaries will be printed as separate log entries.
         """
 
         self.log(*messages, level=LogLevel.ERROR, **kwargs)  # type:ignore[reportArgumentType]
 
     def debug(
         self,
-        *messages: str | dict[str, Any],
+        *messages: str | dict[str, Any] | list[Any] | npt.NDArray[Any],
         **kwargs: Any,
     ):
         """
         Wrapper for calling `log` with `level=LogLevel.DEBUG`.
 
         ### Parameters
         ----------
         `messages`: the messages to log.
         - These can be any number of messages, separated by commas. They can be of the following types:
-        - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
-        - If a dictionary, the message will be logged as a JSON string.
-            - The dictionary must be JSON serializable.
-            - You can provide None dictionary values to mean that the key is a header or title of the message.
+            - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
+            - If a list or numpy array, the message will be logged as a stringified list.
+            - If a dictionary, the message will be logged as a JSON string.
+                - The dictionary must be JSON serializable.
+                - You can provide None dictionary values to mean that the key is a header or title of the message.
+        - If multiple messages are provided, they must be either all dictionaries or none of them. Strings, lists and arrays will be joined into a single string, while dictionaries will be printed as separate log entries.
         """
 
         self.log(*messages, level=LogLevel.DEBUG, **kwargs)  # type:ignore[reportArgumentType]
```

### Comparing `mloggers-1.3.0/mloggers/multi_logger.py` & `mloggers-1.3.1/mloggers/multi_logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Any
 
+import numpy.typing as npt
+
 from mloggers._log_levels import LogLevel
 from mloggers.logger import Logger
 
 
 class MultiLogger(Logger):
     """Logs to multiple loggers."""
 
@@ -35,38 +37,39 @@
         super(MultiLogger, self).set_min_priority(level)
 
         for logger in self._loggers:
             logger.set_min_priority(level)
 
     def log(
         self,
-        *messages: str | dict[str, Any],
+        *messages: str | dict[str, Any] | list[Any] | npt.NDArray[Any],
         level: LogLevel | str | None = None,
         mask: list[type[Logger]] | None = None,
         **kwargs: Any,
     ):
         """
         Logs a message to multiple loggers.
 
         ### Parameters
         ----------
         `messages`: the messages to log.
         - These can be any number of messages, separated by commas. They can be of the following types:
-        - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
-        - If a dictionary, the message will be logged as a JSON string.
-            - The dictionary must be JSON serializable.
-            - You can provide None dictionary values to mean that the key is a header or title of the message.
+            - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
+            - If a list or numpy array, the message will be logged as a stringified list.
+            - If a dictionary, the message will be logged as a JSON string.
+                - The dictionary must be JSON serializable.
+                - You can provide None dictionary values to mean that the key is a header or title of the message.
+        - If multiple messages are provided, they must be either all dictionaries or none of them. Strings, lists and arrays will be joined into a single string, while dictionaries will be printed as separate log entries.
         `level`: the level of the message (e.g., INFO, WARN, ERROR, DEBUG, etc.).
         - If None, no level will be printed.
         - If a string is provided, it will be colored in green (when colors are used) and uppercased; otherwise, the color will be the one associated with the `LogLevel` at time of registration.
-        - If multiple messages are provided, they must be either all strings or all dictionaries. Strings will be joined into a single string, while dictionaries will be printed as separate log entries.
 
         ### Raises
         ----------
-        `TypeError`: if the message is not a string, a dictionary or does not implement `__str__()`.
+        `TypeError`: if the message is not a string, a dictionary, list, numpy array or does not implement `__str__()`.
         `TypeError`: if the messages are a mix of strings and dictionaries.
         """
 
         # NOTE: No need for checking the validity of the message, as the individual loggers will do that.
         # super(MultiLogger, self).log(message, level, *args, **kwargs)
 
         if mask is None:
@@ -77,99 +80,107 @@
             for logger in self._loggers
             if not any(isinstance(logger, type) for type in mask)
         ]:
             logger(*messages, level=level, **kwargs)
 
     def info(
         self,
-        *messages: str | dict[str, Any],
+        *messages: str | dict[str, Any] | list[Any] | npt.NDArray[Any],
         mask: list[type[Logger]] | None = None,
         **kwargs: Any,
     ):
         """
         Wrapper for calling `log` with `level=LogLevel.INFO`.
 
         ### Parameters
         ----------
         `messages`: the messages to log.
         - These can be any number of messages, separated by commas. They can be of the following types:
-        - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
-        - If a dictionary, the message will be logged as a JSON string.
-            - The dictionary must be JSON serializable.
-            - You can provide None dictionary values to mean that the key is a header or title of the message.
+            - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
+            - If a list or numpy array, the message will be logged as a stringified list.
+            - If a dictionary, the message will be logged as a JSON string.
+                - The dictionary must be JSON serializable.
+                - You can provide None dictionary values to mean that the key is a header or title of the message.
+        - If multiple messages are provided, they must be either all dictionaries or none of them. Strings, lists and arrays will be joined into a single string, while dictionaries will be printed as separate log entries.
         `mask`: a list of logger names to not be used to log this message.
         - If None, the default mask will be used.
         """
 
         self.log(*messages, level=LogLevel.INFO, mask=mask, **kwargs)  # type:ignore[reportArgumentType]
 
     def warn(
         self,
-        *messages: str | dict[str, Any],
+        *messages: str | dict[str, Any] | list[Any] | npt.NDArray[Any],
         mask: list[type[Logger]] | None = None,
         **kwargs: Any,
     ):
         """
         Wrapper for calling `log` with `level=LogLevel.WARN`.
 
         ### Parameters
         ----------
         `messages`: the messages to log.
         - These can be any number of messages, separated by commas. They can be of the following types:
-        - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
-        - If a dictionary, the message will be logged as a JSON string.
-            - The dictionary must be JSON serializable.
-            - You can provide None dictionary values to mean that the key is a header or title of the message.
+            - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
+            - If a list or numpy array, the message will be logged as a stringified list.
+            - If a dictionary, the message will be logged as a JSON string.
+                - The dictionary must be JSON serializable.
+                - You can provide None dictionary values to mean that the key is a header or title of the message.
+        - If multiple messages are provided, they must be either all dictionaries or none of them. Strings, lists and arrays will be joined into a single string, while dictionaries will be printed as separate log entries.
         `mask`: a list of logger names to not be used to log this message.
         - If None, the default mask will be used.
         """
 
         self.log(*messages, level=LogLevel.WARN, mask=mask, **kwargs)  # type:ignore[reportArgumentType]
 
     # Alias warning to warn
     warning = warn
 
     def error(
         self,
-        *messages: str | dict[str, Any],
+        *messages: str | dict[str, Any] | list[Any] | npt.NDArray[Any],
         mask: list[type[Logger]] | None = None,
         **kwargs: Any,
     ):
         """
         Wrapper for calling `log` with `level=LogLevel.ERROR`.
 
         ### Parameters
         ----------
         `messages`: the messages to log.
         - These can be any number of messages, separated by commas. They can be of the following types:
-        - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
-        - If a dictionary, the message will be logged as a JSON string.
-            - The dictionary must be JSON serializable.
-            - You can provide None dictionary values to mean that the key is a header or title of the message.
+            - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
+            - If a list or numpy array, the message will be logged as a stringified list.
+            - If a dictionary, the message will be logged as a JSON string.
+                - The dictionary must be JSON serializable.
+                - You can provide None dictionary values to mean that the key is a header or title of the message.
+        - If multiple messages are provided, they must be either all dictionaries or none of them. Strings, lists and arrays will be joined into a single string, while dictionaries will be printed as separate log entries.
         `mask`: a list of logger names to not be used to log this message.
         - If None, the default mask will be used.
         """
 
         self.log(*messages, level=LogLevel.ERROR, mask=mask, **kwargs)  # type:ignore[reportArgumentType]
 
     def debug(
         self,
-        *messages: str | dict[str, Any],
+        *messages: str | dict[str, Any] | list[Any] | npt.NDArray[Any],
         mask: list[type[Logger]] | None = None,
         **kwargs: Any,
     ):
         """
         Wrapper for calling `log` with `level=LogLevel.DEBUG`.
 
         ### Parameters
         ----------
         `messages`: the messages to log.
         - These can be any number of messages, separated by commas. They can be of the following types:
-        - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
-        - If a dictionary, the message will be logged as a JSON string.
-            - The dictionary must be JSON serializable.
-            - You can provide None dictionary values to mean that the key is a header or title of the message.
+            - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
+            - If a list or numpy array, the message will be logged as a stringified list.
+            - If a dictionary, the message will be logged as a JSON string.
+                - The dictionary must be JSON serializable.
+                - You can provide None dictionary values to mean that the key is a header or title of the message.
+        - If multiple messages are provided, they must be either all dictionaries or none of them. Strings, lists and arrays will be joined into a single string, while dictionaries will be printed as separate log entries.
         `mask`: a list of logger names to not be used to log this message.
         - If None, the default mask will be used.
         """
 
         self.log(*messages, level=LogLevel.DEBUG, mask=mask, **kwargs)  # type:ignore[reportArgumentType]
```

### Comparing `mloggers-1.3.0/mloggers/optional_logger.py` & `mloggers-1.3.1/mloggers/optional_logger.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.0/mloggers/progress.py` & `mloggers-1.3.1/mloggers/progress.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.0/mloggers/wandb_logger.py` & `mloggers-1.3.1/mloggers/wandb_logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Any
 
+import numpy.typing as npt
 import wandb
 from omegaconf import DictConfig
 from termcolor import colored
 
 from mloggers._log_levels import LogLevel
 from mloggers.logger import Logger
 
@@ -35,15 +36,15 @@
 
         if config is not None:
             config = vars(config)
         wandb.init(project=project, group=group, name=experiment, config=config)
 
     def log(
         self,
-        *messages: str | dict[str, Any],
+        *messages: str | dict[str, Any] | list[Any] | npt.NDArray[Any],
         level: LogLevel | str | None = None,
         **kwargs: Any,
     ):
         if not super(WandbLogger, self).log(*messages, level=level, **kwargs):
             return
 
         # Handle multiple messages
```

### Comparing `mloggers-1.3.0/.gitignore` & `mloggers-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.0/LICENSE` & `mloggers-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.0/README.md` & `mloggers-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.0/pyproject.toml` & `mloggers-1.3.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mloggers"
-version = "1.3.0"
+version = "1.3.1"
 authors = [
     { name = "Sergio Hernandez Gutierrez", email = "contact.sergiohernandez@gmail.com" },
     { name = "Matteo Merler", email = "matteo.merler@gmail.com" },
 ]
 description = "A collection of loggers well-suited for machine learning experiments."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `mloggers-1.3.0/PKG-INFO` & `mloggers-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mloggers
-Version: 1.3.0
+Version: 1.3.1
 Summary: A collection of loggers well-suited for machine learning experiments.
 Project-URL: Homepage, https://github.com/serhez/mloggers
 Project-URL: Issues, https://github.com/serhez/mloggers/issues
 Author-email: Sergio Hernandez Gutierrez <contact.sergiohernandez@gmail.com>, Matteo Merler <matteo.merler@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

