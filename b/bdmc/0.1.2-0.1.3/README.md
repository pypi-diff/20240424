# Comparing `tmp/bdmc-0.1.2.tar.gz` & `tmp/bdmc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdmc-0.1.2.tar", last modified: Fri Apr 19 15:42:42 2024, max compression
+gzip compressed data, was "bdmc-0.1.3.tar", last modified: Wed Apr 24 15:34:35 2024, max compression
```

## Comparing `bdmc-0.1.2.tar` & `bdmc-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     5296 2024-04-19 15:42:23.082585 bdmc-0.1.2/README.md
--rw-r--r--   0        0        0      545 2024-04-19 15:42:42.478595 bdmc-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      526 2024-04-19 15:42:23.082585 bdmc-0.1.2/src/bdmc/__init__.py
--rw-r--r--   0        0        0      133 2024-04-19 15:42:23.082585 bdmc-0.1.2/src/bdmc/modules/cmd.py
--rw-r--r--   0        0        0     8896 2024-04-19 15:42:23.082585 bdmc-0.1.2/src/bdmc/modules/controller.py
--rw-r--r--   0        0        0     2266 2024-04-19 15:42:23.082585 bdmc-0.1.2/src/bdmc/modules/debug.py
--rw-r--r--   0        0        0      574 2024-04-19 15:42:23.082585 bdmc-0.1.2/src/bdmc/modules/logger.py
--rw-r--r--   0        0        0     1356 2024-04-19 15:42:23.082585 bdmc-0.1.2/src/bdmc/modules/port.py
--rw-r--r--   0        0        0     7404 2024-04-19 15:42:23.082585 bdmc-0.1.2/src/bdmc/modules/seriald.py
--rw-r--r--   0        0        0       64 2024-04-19 15:42:23.082585 bdmc-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     1983 2024-04-19 15:42:23.082585 bdmc-0.1.2/tests/tests.py
--rw-r--r--   0        0        0     5610 1970-01-01 00:00:00.000000 bdmc-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     5296 2024-04-24 15:34:16.527923 bdmc-0.1.3/README.md
+-rw-r--r--   0        0        0      545 2024-04-24 15:34:35.795927 bdmc-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      526 2024-04-24 15:34:16.527923 bdmc-0.1.3/src/bdmc/__init__.py
+-rw-r--r--   0        0        0      133 2024-04-24 15:34:16.527923 bdmc-0.1.3/src/bdmc/modules/cmd.py
+-rw-r--r--   0        0        0    13632 2024-04-24 15:34:16.527923 bdmc-0.1.3/src/bdmc/modules/controller.py
+-rw-r--r--   0        0        0     2266 2024-04-24 15:34:16.527923 bdmc-0.1.3/src/bdmc/modules/debug.py
+-rw-r--r--   0        0        0      574 2024-04-24 15:34:16.527923 bdmc-0.1.3/src/bdmc/modules/logger.py
+-rw-r--r--   0        0        0     1356 2024-04-24 15:34:16.527923 bdmc-0.1.3/src/bdmc/modules/port.py
+-rw-r--r--   0        0        0     7404 2024-04-24 15:34:16.527923 bdmc-0.1.3/src/bdmc/modules/seriald.py
+-rw-r--r--   0        0        0      682 2024-04-24 15:34:16.527923 bdmc-0.1.3/tests/find_tests.py
+-rw-r--r--   0        0        0     4405 2024-04-24 15:34:16.527923 bdmc-0.1.3/tests/test_context.py
+-rw-r--r--   0        0        0     1991 2024-04-24 15:34:16.527923 bdmc-0.1.3/tests/test_controller.py
+-rw-r--r--   0        0        0     5610 1970-01-01 00:00:00.000000 bdmc-0.1.3/PKG-INFO
```

### Comparing `bdmc-0.1.2/README.md` & `bdmc-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.2/pyproject.toml` & `bdmc-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bdmc"
-version = "0.1.2"
+version = "0.1.3"
 description = "An api wrapper lib designed for the uptech BDMC divers"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "pyserial>=3.5",
     "coloredlogs>=15.0.1",
```

### Comparing `bdmc-0.1.2/src/bdmc/__init__.py` & `bdmc-0.1.3/src/bdmc/__init__.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.2/src/bdmc/modules/debug.py` & `bdmc-0.1.3/src/bdmc/modules/debug.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.2/src/bdmc/modules/logger.py` & `bdmc-0.1.3/src/bdmc/modules/logger.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.2/src/bdmc/modules/port.py` & `bdmc-0.1.3/src/bdmc/modules/port.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.2/src/bdmc/modules/seriald.py` & `bdmc-0.1.3/src/bdmc/modules/seriald.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.2/tests/tests.py` & `bdmc-0.1.3/tests/test_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from bdmc.modules.controller import MotorInfo, CloseLoopController
 from bdmc.modules.debug import motor_speed_test
 
 VIZ_OUTPUT_DIR = pathlib.Path(__file__).parent / "viz_output"
 VIZ_OUTPUT_DIR.mkdir(exist_ok=True)
 
 
-class MyTestCase(unittest.TestCase):
+class TestControllerSend(unittest.TestCase):
     def setUp(self):
         self.test_port = "COM3"
         self.tracer = VizTracer()
 
     def test_send(self):
         set_log_level(10)
         m = [MotorInfo(code_sign=1, direction=-1), MotorInfo(code_sign=2, direction=-1)]
```

### Comparing `bdmc-0.1.2/PKG-INFO` & `bdmc-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdmc
-Version: 0.1.2
+Version: 0.1.3
 Summary: An api wrapper lib designed for the uptech BDMC divers
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: pyserial>=3.5
 Requires-Dist: coloredlogs>=15.0.1
 Description-Content-Type: text/markdown
```

