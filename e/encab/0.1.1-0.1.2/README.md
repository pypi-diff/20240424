# Comparing `tmp/encab-0.1.1.tar.gz` & `tmp/encab-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encab-0.1.1.tar", last modified: Tue Dec  5 15:00:04 2023, max compression
+gzip compressed data, was "encab-0.1.2.tar", last modified: Wed Apr 24 15:23:53 2024, max compression
```

## Comparing `encab-0.1.1.tar` & `encab-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-12-05 15:00:04.001400 encab-0.1.1/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1074 2023-12-05 12:32:18.000000 encab-0.1.1/LICENSE
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)     5202 2023-12-05 15:00:04.001400 encab-0.1.1/PKG-INFO
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4360 2023-12-05 14:24:03.000000 encab-0.1.1/README.md
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      961 2023-12-05 14:23:55.000000 encab-0.1.1/pyproject.toml
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       38 2023-12-05 15:00:04.001400 encab-0.1.1/setup.cfg
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-12-05 15:00:04.001400 encab-0.1.1/src/
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-12-05 15:00:04.001400 encab-0.1.1/src/encab/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2023-12-05 12:32:18.000000 encab-0.1.1/src/encab/__init__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       34 2023-12-05 12:32:18.000000 encab-0.1.1/src/encab/__main__.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-12-05 15:00:04.001400 encab-0.1.1/src/encab/common/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      830 2023-12-05 12:32:18.000000 encab-0.1.1/src/encab/common/exit_codes.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2257 2023-12-05 12:32:18.000000 encab-0.1.1/src/encab/common/log_stream.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    11114 2023-12-05 14:21:40.000000 encab-0.1.1/src/encab/common/process.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    12293 2023-12-05 12:32:18.000000 encab-0.1.1/src/encab/config.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     8758 2023-12-05 14:24:33.000000 encab-0.1.1/src/encab/encab.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-12-05 15:00:04.001400 encab-0.1.1/src/encab/ext/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2023-12-05 12:32:18.000000 encab-0.1.1/src/encab/ext/__init__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    12597 2023-12-05 12:32:18.000000 encab-0.1.1/src/encab/ext/log_collector.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5995 2023-12-05 12:32:18.000000 encab-0.1.1/src/encab/ext/log_sanitizer.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     9694 2023-12-05 12:32:18.000000 encab-0.1.1/src/encab/ext/startup_script.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    14101 2023-12-05 12:32:18.000000 encab-0.1.1/src/encab/ext/validation.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5532 2023-12-05 12:32:18.000000 encab-0.1.1/src/encab/extensions.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5766 2023-12-05 12:32:18.000000 encab-0.1.1/src/encab/program.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    10172 2023-12-05 12:32:18.000000 encab-0.1.1/src/encab/program_state.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3407 2023-12-05 12:32:18.000000 encab-0.1.1/src/encab/programs.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-12-05 15:00:04.001400 encab-0.1.1/src/encab.egg-info/
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)     5202 2023-12-05 15:00:03.000000 encab-0.1.1/src/encab.egg-info/PKG-INFO
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      647 2023-12-05 15:00:04.000000 encab-0.1.1/src/encab.egg-info/SOURCES.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-12-05 15:00:03.000000 encab-0.1.1/src/encab.egg-info/dependency_links.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       44 2023-12-05 15:00:03.000000 encab-0.1.1/src/encab.egg-info/entry_points.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      178 2023-12-05 15:00:03.000000 encab-0.1.1/src/encab.egg-info/requires.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        6 2023-12-05 15:00:03.000000 encab-0.1.1/src/encab.egg-info/top_level.txt
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-04-24 15:23:53.611886 encab-0.1.2/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1074 2023-12-05 12:32:18.000000 encab-0.1.2/LICENSE
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)     5202 2024-04-24 15:23:53.611886 encab-0.1.2/PKG-INFO
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4360 2024-04-24 14:55:00.000000 encab-0.1.2/README.md
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      961 2024-04-24 14:53:03.000000 encab-0.1.2/pyproject.toml
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       38 2024-04-24 15:23:53.611886 encab-0.1.2/setup.cfg
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-04-24 15:23:53.611886 encab-0.1.2/src/
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-04-24 15:23:53.611886 encab-0.1.2/src/encab/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2023-12-05 12:32:18.000000 encab-0.1.2/src/encab/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       34 2023-12-05 12:32:18.000000 encab-0.1.2/src/encab/__main__.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-04-24 15:23:53.611886 encab-0.1.2/src/encab/common/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      830 2023-12-05 12:32:18.000000 encab-0.1.2/src/encab/common/exit_codes.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2257 2023-12-05 12:32:18.000000 encab-0.1.2/src/encab/common/log_stream.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    11101 2024-04-24 15:18:22.000000 encab-0.1.2/src/encab/common/process.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    12293 2023-12-05 12:32:18.000000 encab-0.1.2/src/encab/config.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     8758 2024-04-24 14:55:19.000000 encab-0.1.2/src/encab/encab.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-04-24 15:23:53.611886 encab-0.1.2/src/encab/ext/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2023-12-05 12:32:18.000000 encab-0.1.2/src/encab/ext/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    12597 2023-12-05 12:32:18.000000 encab-0.1.2/src/encab/ext/log_collector.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5995 2023-12-05 12:32:18.000000 encab-0.1.2/src/encab/ext/log_sanitizer.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     9694 2023-12-05 12:32:18.000000 encab-0.1.2/src/encab/ext/startup_script.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    14101 2023-12-05 12:32:18.000000 encab-0.1.2/src/encab/ext/validation.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5532 2023-12-05 12:32:18.000000 encab-0.1.2/src/encab/extensions.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5766 2023-12-05 12:32:18.000000 encab-0.1.2/src/encab/program.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    10172 2023-12-05 12:32:18.000000 encab-0.1.2/src/encab/program_state.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3407 2023-12-05 12:32:18.000000 encab-0.1.2/src/encab/programs.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2024-04-24 15:23:53.611886 encab-0.1.2/src/encab.egg-info/
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)     5202 2024-04-24 15:23:53.000000 encab-0.1.2/src/encab.egg-info/PKG-INFO
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      647 2024-04-24 15:23:53.000000 encab-0.1.2/src/encab.egg-info/SOURCES.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2024-04-24 15:23:53.000000 encab-0.1.2/src/encab.egg-info/dependency_links.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       44 2024-04-24 15:23:53.000000 encab-0.1.2/src/encab.egg-info/entry_points.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      178 2024-04-24 15:23:53.000000 encab-0.1.2/src/encab.egg-info/requires.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        6 2024-04-24 15:23:53.000000 encab-0.1.2/src/encab.egg-info/top_level.txt
```

### Comparing `encab-0.1.1/LICENSE` & `encab-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `encab-0.1.1/PKG-INFO` & `encab-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encab
-Version: 0.1.1
+Version: 0.1.2
 Summary: Process manager
 Author-email: Sebastian Kuebeck <sebastian.kuebeck@encab.io>
 Project-URL: Homepage, https://github.com/sebastian-kuebeck/encab
 Project-URL: Documentation, https://encab.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/sebastian-kuebeck/encab
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 License-File: LICENSE
 Requires-Dist: PyYAML<7,>=6.0
 Requires-Dist: types-PyYAML<7,>=6.0.12.2
 Requires-Dist: marshmallow<4,>=3.19.0
 Requires-Dist: marshmallow-dataclass[enum,union]<9,>=8.5.10
 Requires-Dist: marshmallow-enum<2,>=1.5.1
 Requires-Dist: pluggy<2,>=1.0.0
-Requires-Dist: python-dotenv<1,>=0.21.1
+Requires-Dist: python-dotenv<2,>=0.21.1
 
 # Encab: A Simple Process Manager
 
 **Encab** is a process manager that simplifies running multiple services in a container or from the command line.
 
 It's essentially a replacement for complex, hand-written Docker Container Entrypoint scripts,
 especially when dockerizing complex legacy applications.
@@ -48,15 +48,15 @@
          command: httpd-foreground
 ```
 
 and encab cares for the rest.
 Run it and you'll always know who's logging what...
 
 ```text
-   INFO  encab: encab 0.1.1
+   INFO  encab: encab 0.1.2
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: [Wed Jan 18 09:47:12.417275 2023] [mpm_event:notice] [pid 12:tid 140142563044672] AH00489: Apache/2.4.54 (Unix) configured -- resuming normal operations
    ERROR main: [Wed Jan 18 09:47:12.417830 2023] [core:notice] [pid 12:tid 140142563044672] AH00094: Command line: 'httpd -D FOREGROUND'
    INFO  cron: Hello Wed Jan 18 09:48:01 UTC 2023
 ```
@@ -107,15 +107,15 @@
 ```sh
    encab
 ```
 
 The result will be something like this:
 
 ```text
-INFO  encab: encab 0.1.1
+INFO  encab: encab 0.1.2
 INFO  encab: Using configuration file ./encab.yml, source: Default location.
 INFO  main: Hello Encab!
 INFO  main: Exited with rc: 0
    ```
 
 ### Install in Container
 
@@ -180,15 +180,15 @@
    ```sh
    docker run encab_minimum
    ```
 
    Result:
 
    ```text
-   INFO  encab: encab 0.1.1
+   INFO  encab: encab 0.1.2
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    INFO  main: Hello world!
    INFO  main: Exited with rc: 0
    ```
 
 ## Similar Projects
```

### Comparing `encab-0.1.1/README.md` & `encab-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
          command: httpd-foreground
 ```
 
 and encab cares for the rest.
 Run it and you'll always know who's logging what...
 
 ```text
-   INFO  encab: encab 0.1.1
+   INFO  encab: encab 0.1.2
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: [Wed Jan 18 09:47:12.417275 2023] [mpm_event:notice] [pid 12:tid 140142563044672] AH00489: Apache/2.4.54 (Unix) configured -- resuming normal operations
    ERROR main: [Wed Jan 18 09:47:12.417830 2023] [core:notice] [pid 12:tid 140142563044672] AH00094: Command line: 'httpd -D FOREGROUND'
    INFO  cron: Hello Wed Jan 18 09:48:01 UTC 2023
 ```
@@ -85,15 +85,15 @@
 ```sh
    encab
 ```
 
 The result will be something like this:
 
 ```text
-INFO  encab: encab 0.1.1
+INFO  encab: encab 0.1.2
 INFO  encab: Using configuration file ./encab.yml, source: Default location.
 INFO  main: Hello Encab!
 INFO  main: Exited with rc: 0
    ```
 
 ### Install in Container
 
@@ -158,15 +158,15 @@
    ```sh
    docker run encab_minimum
    ```
 
    Result:
 
    ```text
-   INFO  encab: encab 0.1.1
+   INFO  encab: encab 0.1.2
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    INFO  main: Hello world!
    INFO  main: Exited with rc: 0
    ```
 
 ## Similar Projects
```

### Comparing `encab-0.1.1/pyproject.toml` & `encab-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "encab"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Sebastian Kuebeck", email="sebastian.kuebeck@encab.io" },
 ]
 description = "Process manager"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -19,15 +19,15 @@
 dependencies = [
   "PyYAML >= 6.0, < 7",
   "types-PyYAML >= 6.0.12.2, < 7",
   "marshmallow >= 3.19.0, < 4",
   "marshmallow-dataclass[enum,union] >= 8.5.10, < 9",
   "marshmallow-enum >= 1.5.1, < 2",
   "pluggy >= 1.0.0, < 2",
-  "python-dotenv >= 0.21.1, < 1"
+  "python-dotenv >= 0.21.1, < 2"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/sebastian-kuebeck/encab"
 "Documentation" = "https://encab.readthedocs.io"
 "Bug Tracker" = "https://github.com/sebastian-kuebeck/encab"
```

### Comparing `encab-0.1.1/src/encab/common/exit_codes.py` & `encab-0.1.2/src/encab/common/exit_codes.py`

 * *Files identical despite different names*

### Comparing `encab-0.1.1/src/encab/common/log_stream.py` & `encab-0.1.2/src/encab/common/log_stream.py`

 * *Files identical despite different names*

### Comparing `encab-0.1.1/src/encab/common/process.py` & `encab-0.1.2/src/encab/common/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import pwd
-import time
 
 from typing import Dict, Optional, Callable, Any, List, Union
 
 from subprocess import Popen, PIPE
 from signal import SIGKILL, SIGTERM
 
 from logging import Logger, INFO, ERROR
@@ -143,15 +142,15 @@
         :type extra: Dict[str, str]
         """
 
         assert self._process
         child_process_pid = self._process.pid
 
         while True:
-            current_pid, status = os.waitpid(-child_process_pid, os.WUNTRACED) 
+            current_pid, status = os.waitpid(-child_process_pid, os.WUNTRACED)
             if current_pid == -1:
                 logger.debug("No child to wait", extra=extra)
                 return EX_NOCHILD
             elif current_pid == 0:
                 pass
             else:
                 if current_pid == child_process_pid:
```

### Comparing `encab-0.1.1/src/encab/config.py` & `encab-0.1.2/src/encab/config.py`

 * *Files identical despite different names*

### Comparing `encab-0.1.1/src/encab/encab.py` & `encab-0.1.2/src/encab/encab.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
     try:
         config, location = load_config(encab_stream)
 
         logger = set_up_logger(config)
 
         extra = {"program": ENCAB}
 
-        logger.info("encab 0.1.1", extra=extra)
+        logger.info("encab 0.1.2", extra=extra)
         logger.info("Using configuration %s", location, extra=extra)
 
         logger.debug(
             "Encab config: %s",
             shorten(str(config), width=127, placeholder="..."),
             extra=extra,
         )
```

### Comparing `encab-0.1.1/src/encab/ext/log_collector.py` & `encab-0.1.2/src/encab/ext/log_collector.py`

 * *Files identical despite different names*

### Comparing `encab-0.1.1/src/encab/ext/log_sanitizer.py` & `encab-0.1.2/src/encab/ext/log_sanitizer.py`

 * *Files identical despite different names*

### Comparing `encab-0.1.1/src/encab/ext/startup_script.py` & `encab-0.1.2/src/encab/ext/startup_script.py`

 * *Files identical despite different names*

### Comparing `encab-0.1.1/src/encab/ext/validation.py` & `encab-0.1.2/src/encab/ext/validation.py`

 * *Files identical despite different names*

### Comparing `encab-0.1.1/src/encab/extensions.py` & `encab-0.1.2/src/encab/extensions.py`

 * *Files identical despite different names*

### Comparing `encab-0.1.1/src/encab/program.py` & `encab-0.1.2/src/encab/program.py`

 * *Files identical despite different names*

### Comparing `encab-0.1.1/src/encab/program_state.py` & `encab-0.1.2/src/encab/program_state.py`

 * *Files identical despite different names*

### Comparing `encab-0.1.1/src/encab/programs.py` & `encab-0.1.2/src/encab/programs.py`

 * *Files identical despite different names*

### Comparing `encab-0.1.1/src/encab.egg-info/PKG-INFO` & `encab-0.1.2/src/encab.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encab
-Version: 0.1.1
+Version: 0.1.2
 Summary: Process manager
 Author-email: Sebastian Kuebeck <sebastian.kuebeck@encab.io>
 Project-URL: Homepage, https://github.com/sebastian-kuebeck/encab
 Project-URL: Documentation, https://encab.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/sebastian-kuebeck/encab
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 License-File: LICENSE
 Requires-Dist: PyYAML<7,>=6.0
 Requires-Dist: types-PyYAML<7,>=6.0.12.2
 Requires-Dist: marshmallow<4,>=3.19.0
 Requires-Dist: marshmallow-dataclass[enum,union]<9,>=8.5.10
 Requires-Dist: marshmallow-enum<2,>=1.5.1
 Requires-Dist: pluggy<2,>=1.0.0
-Requires-Dist: python-dotenv<1,>=0.21.1
+Requires-Dist: python-dotenv<2,>=0.21.1
 
 # Encab: A Simple Process Manager
 
 **Encab** is a process manager that simplifies running multiple services in a container or from the command line.
 
 It's essentially a replacement for complex, hand-written Docker Container Entrypoint scripts,
 especially when dockerizing complex legacy applications.
@@ -48,15 +48,15 @@
          command: httpd-foreground
 ```
 
 and encab cares for the rest.
 Run it and you'll always know who's logging what...
 
 ```text
-   INFO  encab: encab 0.1.1
+   INFO  encab: encab 0.1.2
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: [Wed Jan 18 09:47:12.417275 2023] [mpm_event:notice] [pid 12:tid 140142563044672] AH00489: Apache/2.4.54 (Unix) configured -- resuming normal operations
    ERROR main: [Wed Jan 18 09:47:12.417830 2023] [core:notice] [pid 12:tid 140142563044672] AH00094: Command line: 'httpd -D FOREGROUND'
    INFO  cron: Hello Wed Jan 18 09:48:01 UTC 2023
 ```
@@ -107,15 +107,15 @@
 ```sh
    encab
 ```
 
 The result will be something like this:
 
 ```text
-INFO  encab: encab 0.1.1
+INFO  encab: encab 0.1.2
 INFO  encab: Using configuration file ./encab.yml, source: Default location.
 INFO  main: Hello Encab!
 INFO  main: Exited with rc: 0
    ```
 
 ### Install in Container
 
@@ -180,15 +180,15 @@
    ```sh
    docker run encab_minimum
    ```
 
    Result:
 
    ```text
-   INFO  encab: encab 0.1.1
+   INFO  encab: encab 0.1.2
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    INFO  main: Hello world!
    INFO  main: Exited with rc: 0
    ```
 
 ## Similar Projects
```

### Comparing `encab-0.1.1/src/encab.egg-info/SOURCES.txt` & `encab-0.1.2/src/encab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

