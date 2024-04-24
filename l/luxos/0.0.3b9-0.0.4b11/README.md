# Comparing `tmp/luxos-0.0.3b9.tar.gz` & `tmp/luxos-0.0.4b11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luxos-0.0.3b9.tar", last modified: Tue Apr 23 14:08:56 2024, max compression
+gzip compressed data, was "luxos-0.0.4b11.tar", last modified: Wed Apr 24 16:51:37 2024, max compression
```

## Comparing `luxos-0.0.3b9.tar` & `luxos-0.0.4b11.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:56.077522 luxos-0.0.3b9/
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-23 14:08:56.077522 luxos-0.0.3b9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-23 14:08:24.000000 luxos-0.0.3b9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-23 14:08:53.000000 luxos-0.0.3b9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:08:56.077522 luxos-0.0.3b9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:56.069522 luxos-0.0.3b9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:56.073522 luxos-0.0.3b9/src/luxos/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 14:08:53.000000 luxos-0.0.3b9/src/luxos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/api.json
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9663 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/asyncops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:56.073522 luxos-0.0.3b9/src/luxos/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/cli/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:56.073522 luxos-0.0.3b9/src/luxos/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/scripts/async_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/scripts/health_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-04-23 14:08:24.000000 luxos-0.0.3b9/src/luxos/scripts/luxos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:56.077522 luxos-0.0.3b9/src/luxos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-23 14:08:56.000000 luxos-0.0.3b9/src/luxos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-23 14:08:56.000000 luxos-0.0.3b9/src/luxos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:08:56.000000 luxos-0.0.3b9/src/luxos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 14:08:56.000000 luxos-0.0.3b9/src/luxos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-23 14:08:56.000000 luxos-0.0.3b9/src/luxos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 14:08:56.000000 luxos-0.0.3b9/src/luxos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:56.073522 luxos-0.0.3b9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-23 14:08:24.000000 luxos-0.0.3b9/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-23 14:08:24.000000 luxos-0.0.3b9/tests/test_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-04-23 14:08:24.000000 luxos-0.0.3b9/tests/test_luxos_asyncops.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-23 14:08:24.000000 luxos-0.0.3b9/tests/test_luxos_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:51:37.308940 luxos-0.0.4b11/
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-24 16:51:37.308940 luxos-0.0.4b11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-24 16:51:01.000000 luxos-0.0.4b11/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-24 16:51:35.000000 luxos-0.0.4b11/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 16:51:37.308940 luxos-0.0.4b11/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:51:37.300940 luxos-0.0.4b11/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:51:37.304940 luxos-0.0.4b11/src/luxos/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-24 16:51:35.000000 luxos-0.0.4b11/src/luxos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 16:51:01.000000 luxos-0.0.4b11/src/luxos/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-24 16:51:01.000000 luxos-0.0.4b11/src/luxos/api.json
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-24 16:51:01.000000 luxos-0.0.4b11/src/luxos/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10212 2024-04-24 16:51:01.000000 luxos-0.0.4b11/src/luxos/asyncops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:51:37.304940 luxos-0.0.4b11/src/luxos/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:51:01.000000 luxos-0.0.4b11/src/luxos/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-24 16:51:01.000000 luxos-0.0.4b11/src/luxos/cli/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-24 16:51:01.000000 luxos-0.0.4b11/src/luxos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-24 16:51:01.000000 luxos-0.0.4b11/src/luxos/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:51:01.000000 luxos-0.0.4b11/src/luxos/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:51:37.304940 luxos-0.0.4b11/src/luxos/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:51:01.000000 luxos-0.0.4b11/src/luxos/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-24 16:51:01.000000 luxos-0.0.4b11/src/luxos/scripts/async_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-04-24 16:51:01.000000 luxos-0.0.4b11/src/luxos/scripts/health_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-04-24 16:51:01.000000 luxos-0.0.4b11/src/luxos/scripts/luxos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:51:37.304940 luxos-0.0.4b11/src/luxos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-24 16:51:37.000000 luxos-0.0.4b11/src/luxos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-24 16:51:37.000000 luxos-0.0.4b11/src/luxos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:51:37.000000 luxos-0.0.4b11/src/luxos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-24 16:51:37.000000 luxos-0.0.4b11/src/luxos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-24 16:51:37.000000 luxos-0.0.4b11/src/luxos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 16:51:37.000000 luxos-0.0.4b11/src/luxos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:51:37.304940 luxos-0.0.4b11/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-24 16:51:01.000000 luxos-0.0.4b11/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-24 16:51:01.000000 luxos-0.0.4b11/tests/test_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-04-24 16:51:01.000000 luxos-0.0.4b11/tests/test_luxos_asyncops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-24 16:51:01.000000 luxos-0.0.4b11/tests/test_luxos_misc.py
```

### Comparing `luxos-0.0.3b9/PKG-INFO` & `luxos-0.0.4b11/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.3b9
+Version: 0.0.4b11
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -78,14 +78,23 @@
 
 ```python
 from luxos.api import (execute_command)
 
 execute_command("192.168.1.1", 4028, 2, "rebootdevice", "", False)
 ```
 
+There's an alternative api:
+```
+from luxos.asyncops import rexec
+
+rexec(host="192.168.1.1", port=4028, cmd="rebootdevice", parameters="", timeout=2., retry=1, retry_delay=3.)
+```
+(note the host/port/cmd etc. shouldn't needed, there are here for readability)
+
+
 ## LuxOS HealthChecker - health_checker.py
 
 The HealthChecker script is designed to continuously pull miner data from LuxOS, providing valuable insights into the health of your mining machines.
 
 You can customize the HealthChecker params using the `config.yaml` file provided. 
 To run the HealthChecker you can use `health-checker` if you installed using pip, or
 the cli `python3 -m luxos.scripts.health_checker`.
```

### Comparing `luxos-0.0.3b9/README.md` & `luxos-0.0.4b11/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,23 @@
 
 ```python
 from luxos.api import (execute_command)
 
 execute_command("192.168.1.1", 4028, 2, "rebootdevice", "", False)
 ```
 
+There's an alternative api:
+```
+from luxos.asyncops import rexec
+
+rexec(host="192.168.1.1", port=4028, cmd="rebootdevice", parameters="", timeout=2., retry=1, retry_delay=3.)
+```
+(note the host/port/cmd etc. shouldn't needed, there are here for readability)
+
+
 ## LuxOS HealthChecker - health_checker.py
 
 The HealthChecker script is designed to continuously pull miner data from LuxOS, providing valuable insights into the health of your mining machines.
 
 You can customize the HealthChecker params using the `config.yaml` file provided. 
 To run the HealthChecker you can use `health-checker` if you installed using pip, or
 the cli `python3 -m luxos.scripts.health_checker`.
```

### Comparing `luxos-0.0.3b9/pyproject.toml` & `luxos-0.0.4b11/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "luxos"
-version = "0.0.3b9"
+version = "0.0.4b11"
 description = "The all encompassing LuxOS python library."
 readme = "README.md"
 license = { text = "MIT" }  # TODO I don't think this is a MIT??
 requires-python = ">= 3.9"
 
 authors = [
   { name = "Antonio Cavallo", email = "antonio.cavallo@luxor.tech" },
```

### Comparing `luxos-0.0.3b9/src/luxos/api.json` & `luxos-0.0.4b11/src/luxos/api.json`

 * *Files identical despite different names*

### Comparing `luxos-0.0.3b9/src/luxos/api.py` & `luxos-0.0.4b11/src/luxos/api.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.3b9/src/luxos/asyncops.py` & `luxos-0.0.4b11/src/luxos/asyncops.py`

 * *Files 6% similar despite different names*

```diff
@@ -225,27 +225,45 @@
         log.debug("received from %s:%s: %s", host, port, str(ret))
         return ((host, port), ret) if add_address else ret
     finally:
         if sid:
             await logoff(host, port, sid)
 
 
+def _rexec_paramteres(
+    parameters: str | list[str] | dict[str, Any] | None = None,
+) -> list[str]:
+    if isinstance(parameters, dict):
+        data = []
+        for key, value in parameters.items():
+            if value is None:
+                value = "null"
+            elif value is True:
+                value = "true"
+            elif value is False:
+                value = "false"
+            data.append(f"{key}={value}")
+        parameters = data
+    parameters = ([parameters] if isinstance(parameters, str) else parameters) or []
+    parameters = [str(param) for param in parameters]
+    return parameters
+
+
 async def rexec(
     host: str,
     port: int,
     cmd: str,
-    parameters: str | list[str] | None = None,
+    parameters: str | list[str] | dict[str, Any] | None = None,
     timeout: float | None = None,
     retry: int | None = None,
     retry_delay: float | None = None,
 ) -> dict[str, Any] | None:
     from . import api
 
-    parameters = ([parameters] if isinstance(parameters, str) else parameters) or []
-    parameters = [str(param) for param in parameters]
+    parameters = _rexec_paramteres(parameters)
 
     timeout = TIMEOUT if timeout is None else timeout
     retry = RETRY if retry is None else retry
     retry_delay = RETRY_DELAY if retry_delay is None else retry_delay
 
     # if cmd is logon/logoff we dealt with it differently
     if cmd in {"logon", "logoff"}:
```

### Comparing `luxos-0.0.3b9/src/luxos/cli/v1.py` & `luxos-0.0.4b11/src/luxos/cli/v1.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 
 ```
 
 """
 
 from __future__ import annotations
 
+import sys
 import contextlib
 import inspect
 import logging
 import time
 from pathlib import Path
 import functools
 import argparse
@@ -114,26 +115,36 @@
     pass
 
 
 class AbortCliError(CliBaseError):
     pass
 
 
+class AbortWrongArgument(CliBaseError):
+    pass
+
+
 def setup_logging(config: dict[str, Any], count: int) -> None:
-    levelmap = {
-        1: logging.DEBUG,
-        0: logging.INFO,
-        -1: logging.WARNING,
-    }
+    levelmap = [
+        logging.WARNING,
+        logging.INFO,
+        logging.DEBUG,
+    ]
+    n = len(levelmap)
 
-    # we can set the default log level in LOGGING_CONFIG
+    # awlays start from info level
+    level = logging.INFO
+
+    # we can set the default start log level in LOGGING_CONFIG
     if config.get("level", None) is not None:
-        levelmap[0] = config["level"]
+        level = config["level"]
 
-    config["level"] = levelmap[count]
+    # we control if we go verbose or quite here
+    index = levelmap.index(level) + count
+    config["level"] = levelmap[max(min(index, n - 1), 0)]
     logging.basicConfig(**config)
 
 
 class LuxosParser(argparse.ArgumentParser):
     def __init__(self, module_variables, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -161,22 +172,26 @@
             help="path to a config file",
         )
 
     def parse_args(self, args=None, namespace=None):
         options = super().parse_args(args, namespace)
 
         # we provide an error function to nicely bail out the script
+        def error(msg):
+            raise AbortWrongArgument(msg)
+
+        self.error = error
         options.error = self.error
 
         # setup the logging
         config = {}
         if value := self.module_variables.get("LOGGING_CONFIG"):
             config = value.copy()
 
-        count = max(min((options.verbose or 0) - (options.quiet or 0), 1), -1)
+        count = (options.verbose or 0) - (options.quiet or 0)
         setup_logging(config, count)
 
         return options
 
     @classmethod
     def get_parser(cls, module_variables, **kwargs):
         class Formatter(
@@ -220,58 +235,57 @@
 
             if "parser" in sig.parameters:
                 kwargs["parser"] = parser
 
             t0 = time.monotonic()
             success = "completed"
             errormsg = ""
+            show_timing = True
             try:
                 if "parser" not in sig.parameters:
                     args = parser.parse_args()
                     if process_args:
                         args = process_args(args) or args
                     if "args" in sig.parameters:
                         kwargs["args"] = args
                 yield sig.bind(**kwargs)
             except AbortCliError as exc:
                 errormsg = str(exc)
                 success = "failed"
+            except AbortWrongArgument as exc:
+                show_timing = False
+                parser.print_usage(sys.stderr)
+                print(f"{parser.prog}: error: {exc.args[0]}", file=sys.stderr)
+                sys.exit(2)
             except Exception:
                 log.exception("un-handled exception")
                 success = "failed"
             finally:
-                delta = round(time.monotonic() - t0, 2)
-                log.info("task %s in %.2fs", success, delta)
+                if show_timing:
+                    delta = round(time.monotonic() - t0, 2)
+                    log.info("task %s in %.2fs", success, delta)
             if errormsg:
                 parser.error(errormsg)
 
+        def log_sys_info():
+            log.debug("interpreter: %s", sys.executable)
+            log.debug("version: %s", sys.version)
+
         if inspect.iscoroutinefunction(function):
 
             @functools.wraps(function)
             async def _cli2(*args, **kwargs):
                 with setup() as ba:
+                    log_sys_info()
                     return await function(*ba.args, **ba.kwargs)
 
         else:
 
             @functools.wraps(function)
             def _cli2(*args, **kwargs):
                 with setup() as ba:
+                    log_sys_info()
                     return function(*ba.args, **ba.kwargs)
 
         return _cli2
 
     return _cli1
-
-
-### standard arguments
-
-
-def add_argument_csv_miners(parser: argparse.ArgumentParser, *args, **kwargs):
-    """adds arguments handling miners config in a csv file"""
-
-    parser.add_argument("--ip-start", help="start of the IP range")
-    parser.add_argument("--ip-end", help="start of the IP range")
-    parser.add_argument("--ip-file", type=Path, help="csv file containing ip addresses")
-    parser.add_argument(
-        "--port", type=int, default=4028, help="Port number for the miner API"
-    )
```

### Comparing `luxos-0.0.3b9/src/luxos/exceptions.py` & `luxos-0.0.4b11/src/luxos/exceptions.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.3b9/src/luxos/misc.py` & `luxos-0.0.4b11/src/luxos/misc.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.3b9/src/luxos/scripts/async_luxos.py` & `luxos-0.0.4b11/src/luxos/scripts/async_luxos.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.3b9/src/luxos/scripts/health_checker.py` & `luxos-0.0.4b11/src/luxos/scripts/health_checker.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.3b9/src/luxos/scripts/luxos.py` & `luxos-0.0.4b11/src/luxos/scripts/luxos.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.3b9/src/luxos.egg-info/PKG-INFO` & `luxos-0.0.4b11/src/luxos.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.3b9
+Version: 0.0.4b11
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -78,14 +78,23 @@
 
 ```python
 from luxos.api import (execute_command)
 
 execute_command("192.168.1.1", 4028, 2, "rebootdevice", "", False)
 ```
 
+There's an alternative api:
+```
+from luxos.asyncops import rexec
+
+rexec(host="192.168.1.1", port=4028, cmd="rebootdevice", parameters="", timeout=2., retry=1, retry_delay=3.)
+```
+(note the host/port/cmd etc. shouldn't needed, there are here for readability)
+
+
 ## LuxOS HealthChecker - health_checker.py
 
 The HealthChecker script is designed to continuously pull miner data from LuxOS, providing valuable insights into the health of your mining machines.
 
 You can customize the HealthChecker params using the `config.yaml` file provided. 
 To run the HealthChecker you can use `health-checker` if you installed using pip, or
 the cli `python3 -m luxos.scripts.health_checker`.
```

### Comparing `luxos-0.0.3b9/src/luxos.egg-info/SOURCES.txt` & `luxos-0.0.4b11/src/luxos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `luxos-0.0.3b9/tests/test_cli.py` & `luxos-0.0.4b11/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.3b9/tests/test_luxos_asyncops.py` & `luxos-0.0.4b11/tests/test_luxos_asyncops.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,61 +9,84 @@
 
 ## NOTE ##
 # This tests spawn an underlying server, it might be better not run
 # unattended. Some also require a miner, we might not have it handy.
 pytestmark = pytest.mark.manual
 
 
-
 def getminer() -> None | tuple[str, int]:
     if not (minerd := os.getenv("LUXOS_TEST_MINER")):
         return None
     host, port = minerd.split(":")
     return host.strip(), int(port)
 
 
+def test_rexec_paramteres():
+    assert aapi._rexec_paramteres(None) == []
+    assert aapi._rexec_paramteres("hello") == ["hello"]
+    assert aapi._rexec_paramteres(["hello", "world"]) == ["hello", "world"]
+    assert aapi._rexec_paramteres(["hello", 1]) == ["hello", "1"]
+    assert aapi._rexec_paramteres({"hello": 1}) == ["hello=1"]
+    assert aapi._rexec_paramteres({"hello": True}) == ["hello=true"]
+
+
 def test_validate_message():
-    pytest.raises(exceptions.MinerCommandMalformedMessageError, aapi.validate_message, "a", 0, {})
+    pytest.raises(
+        exceptions.MinerCommandMalformedMessageError, aapi.validate_message, "a", 0, {}
+    )
     host, port = "a", 0
 
     assert aapi.validate_message(host, port, {"STATUS": 1, "id": 2})
 
     pytest.raises(
         exceptions.MinerCommandMalformedMessageError,
         aapi.validate_message,
-        host, port,
+        host,
+        port,
         {
             "STATUS": 1,
             "id": 2,
         },
         "wooow",
     )
 
-    assert aapi.validate_message(host, port, {"STATUS": 1, "id": 2, "wooow": [1, 2]}, "wooow")
+    assert aapi.validate_message(
+        host, port, {"STATUS": 1, "id": 2, "wooow": [1, 2]}, "wooow"
+    )
 
     with pytest.raises(exceptions.MinerCommandMalformedMessageError) as excinfo:
-        aapi.validate_message(host, port,
-            {"STATUS": 1, "id": 2, "wooow": [1, 2]}, "wooow", minfields=9
+        aapi.validate_message(
+            host, port, {"STATUS": 1, "id": 2, "wooow": [1, 2]}, "wooow", minfields=9
         )
     assert excinfo.value.args[2] == "found 2 fields for wooow invalid: 2 <= 9"
 
     with pytest.raises(exceptions.MinerCommandMalformedMessageError) as excinfo:
-        aapi.validate_message(host, port,
-            {"STATUS": 1, "id": 2, "wooow": [1, 2]}, "wooow", maxfields=1
+        aapi.validate_message(
+            host, port, {"STATUS": 1, "id": 2, "wooow": [1, 2]}, "wooow", maxfields=1
         )
     assert excinfo.value.args[2] == "found 2 fields for wooow invalid: 2 >= 1"
 
     with pytest.raises(exceptions.MinerCommandMalformedMessageError) as excinfo:
-        aapi.validate_message(host, port,
-            {"STATUS": 1, "id": 2, "wooow": [1, 2]}, "wooow", minfields=9, maxfields=10
+        aapi.validate_message(
+            host,
+            port,
+            {"STATUS": 1, "id": 2, "wooow": [1, 2]},
+            "wooow",
+            minfields=9,
+            maxfields=10,
         )
     assert excinfo.value.args[2] == "found 2 fields for wooow invalid: 2 <= 9"
 
-    assert aapi.validate_message(host, port,
-        {"STATUS": 1, "id": 2, "wooow": [1, 2]}, "wooow", minfields=2, maxfields=10
+    assert aapi.validate_message(
+        host,
+        port,
+        {"STATUS": 1, "id": 2, "wooow": [1, 2]},
+        "wooow",
+        minfields=2,
+        maxfields=10,
     )
 
 
 @pytest.mark.asyncio
 async def test_private_roundtrip_one_listener(echopool):
     """checks roundrtip sends and receive a message (1-listener)"""
     echopool.start(1, mode="echo+")
@@ -101,15 +124,14 @@
     except exceptions.MinerCommandSessionAlreadyActive as e:
         raise RuntimeError("a session is already active on {host}:{port}") from e
     finally:
         if sid:
             await aapi.logoff(host, port, sid)
 
 
-
 @pytest.mark.skipif(not getminer(), reason="need to set LUXOS_TEST_MINER")
 @pytest.mark.asyncio
 async def test_miner_double_logon_cycle():
     host, port = getminer()
 
     sid = await aapi.logon(host, port)
     try:
@@ -164,11 +186,7 @@
         await aapi.rexec(host, port, "profilerem", profile)
 
     # verify we restored the same profiles
     profiles2 = (await aapi.rexec(host, port, "profiles"))["PROFILES"]
     expected = {p["Profile Name"] for p in profiles}
     found = {p["Profile Name"] for p in profiles2}
     assert found == expected
-
-
-
-
```

### Comparing `luxos-0.0.3b9/tests/test_luxos_misc.py` & `luxos-0.0.4b11/tests/test_luxos_misc.py`

 * *Files identical despite different names*

