# Comparing `tmp/ubitlogger-0.3.0.tar.gz` & `tmp/ubitlogger-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubitlogger-0.3.0.tar", last modified: Mon Apr 22 11:54:01 2024, max compression
+gzip compressed data, was "ubitlogger-0.4.0.tar", last modified: Tue Apr 23 15:15:40 2024, max compression
```

## Comparing `ubitlogger-0.3.0.tar` & `ubitlogger-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-22 11:54:01.125757 ubitlogger-0.3.0/
--rw-r--r--   0 pairin    (1000) pairin    (1000)     1062 2024-04-15 23:12:06.000000 ubitlogger-0.3.0/LICENSE
--rw-r--r--   0 pairin    (1000) pairin    (1000)       42 2024-04-22 11:27:36.000000 ubitlogger-0.3.0/MANIFEST.in
--rw-r--r--   0 pairin    (1000) pairin    (1000)     7648 2024-04-22 11:54:01.125757 ubitlogger-0.3.0/PKG-INFO
--rw-r--r--   0 pairin    (1000) pairin    (1000)     6184 2024-04-22 11:08:20.000000 ubitlogger-0.3.0/README.md
--rw-r--r--   0 pairin    (1000) pairin    (1000)     1901 2024-04-22 11:51:02.000000 ubitlogger-0.3.0/pyproject.toml
--rw-r--r--   0 pairin    (1000) pairin    (1000)       38 2024-04-22 11:54:01.125757 ubitlogger-0.3.0/setup.cfg
--rw-r--r--   0 pairin    (1000) pairin    (1000)      529 2024-04-15 21:47:43.000000 ubitlogger-0.3.0/setup.py
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-22 11:54:01.115757 ubitlogger-0.3.0/src/
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-22 11:54:01.115757 ubitlogger-0.3.0/src/ubitlogger/
--rw-r--r--   0 pairin    (1000) pairin    (1000)     3220 2024-04-22 11:51:02.000000 ubitlogger-0.3.0/src/ubitlogger/__init__.py
--rw-r--r--   0 pairin    (1000) pairin    (1000)     3113 2024-04-22 10:58:35.000000 ubitlogger-0.3.0/src/ubitlogger/cli.py
--rw-r--r--   0 pairin    (1000) pairin    (1000)      429 2024-04-22 11:41:11.000000 ubitlogger-0.3.0/src/ubitlogger/read_sensor.py
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-22 11:54:01.125757 ubitlogger-0.3.0/src/ubitlogger.egg-info/
--rw-r--r--   0 pairin    (1000) pairin    (1000)     7648 2024-04-22 11:54:01.000000 ubitlogger-0.3.0/src/ubitlogger.egg-info/PKG-INFO
--rw-r--r--   0 pairin    (1000) pairin    (1000)      377 2024-04-22 11:54:01.000000 ubitlogger-0.3.0/src/ubitlogger.egg-info/SOURCES.txt
--rw-r--r--   0 pairin    (1000) pairin    (1000)        1 2024-04-22 11:54:01.000000 ubitlogger-0.3.0/src/ubitlogger.egg-info/dependency_links.txt
--rw-r--r--   0 pairin    (1000) pairin    (1000)       50 2024-04-22 11:54:01.000000 ubitlogger-0.3.0/src/ubitlogger.egg-info/entry_points.txt
--rw-r--r--   0 pairin    (1000) pairin    (1000)      218 2024-04-22 11:54:01.000000 ubitlogger-0.3.0/src/ubitlogger.egg-info/requires.txt
--rw-r--r--   0 pairin    (1000) pairin    (1000)       11 2024-04-22 11:54:01.000000 ubitlogger-0.3.0/src/ubitlogger.egg-info/top_level.txt
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-22 11:54:01.125757 ubitlogger-0.3.0/tests/
--rw-r--r--   0 pairin    (1000) pairin    (1000)        0 2024-04-17 14:44:36.000000 ubitlogger-0.3.0/tests/tests.py
+drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-23 15:15:40.706668 ubitlogger-0.4.0/
+-rw-r--r--   0 pairin    (1000) pairin    (1000)     1062 2024-04-15 23:12:06.000000 ubitlogger-0.4.0/LICENSE
+-rw-r--r--   0 pairin    (1000) pairin    (1000)       42 2024-04-22 11:27:36.000000 ubitlogger-0.4.0/MANIFEST.in
+-rw-r--r--   0 pairin    (1000) pairin    (1000)     7771 2024-04-23 15:15:40.706668 ubitlogger-0.4.0/PKG-INFO
+-rw-r--r--   0 pairin    (1000) pairin    (1000)     6307 2024-04-23 14:29:22.000000 ubitlogger-0.4.0/README.md
+-rw-r--r--   0 pairin    (1000) pairin    (1000)     1998 2024-04-23 15:13:23.000000 ubitlogger-0.4.0/pyproject.toml
+-rw-r--r--   0 pairin    (1000) pairin    (1000)       38 2024-04-23 15:15:40.706668 ubitlogger-0.4.0/setup.cfg
+-rw-r--r--   0 pairin    (1000) pairin    (1000)      529 2024-04-15 21:47:43.000000 ubitlogger-0.4.0/setup.py
+drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-23 15:15:40.696668 ubitlogger-0.4.0/src/
+drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-23 15:15:40.696668 ubitlogger-0.4.0/src/ubitlogger/
+-rw-r--r--   0 pairin    (1000) pairin    (1000)     3347 2024-04-23 15:13:23.000000 ubitlogger-0.4.0/src/ubitlogger/__init__.py
+-rw-r--r--   0 pairin    (1000) pairin    (1000)     3413 2024-04-23 14:01:10.000000 ubitlogger-0.4.0/src/ubitlogger/cli.py
+-rw-r--r--   0 pairin    (1000) pairin    (1000)      429 2024-04-22 11:41:11.000000 ubitlogger-0.4.0/src/ubitlogger/read_sensor.py
+drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-23 15:15:40.696668 ubitlogger-0.4.0/src/ubitlogger.egg-info/
+-rw-r--r--   0 pairin    (1000) pairin    (1000)     7771 2024-04-23 15:15:40.000000 ubitlogger-0.4.0/src/ubitlogger.egg-info/PKG-INFO
+-rw-r--r--   0 pairin    (1000) pairin    (1000)      377 2024-04-23 15:15:40.000000 ubitlogger-0.4.0/src/ubitlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 pairin    (1000) pairin    (1000)        1 2024-04-23 15:15:40.000000 ubitlogger-0.4.0/src/ubitlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 pairin    (1000) pairin    (1000)       50 2024-04-23 15:15:40.000000 ubitlogger-0.4.0/src/ubitlogger.egg-info/entry_points.txt
+-rw-r--r--   0 pairin    (1000) pairin    (1000)      218 2024-04-23 15:15:40.000000 ubitlogger-0.4.0/src/ubitlogger.egg-info/requires.txt
+-rw-r--r--   0 pairin    (1000) pairin    (1000)       11 2024-04-23 15:15:40.000000 ubitlogger-0.4.0/src/ubitlogger.egg-info/top_level.txt
+drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-23 15:15:40.696668 ubitlogger-0.4.0/tests/
+-rw-r--r--   0 pairin    (1000) pairin    (1000)        0 2024-04-17 14:44:36.000000 ubitlogger-0.4.0/tests/tests.py
```

### Comparing `ubitlogger-0.3.0/LICENSE` & `ubitlogger-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ubitlogger-0.3.0/PKG-INFO` & `ubitlogger-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubitlogger
-Version: 0.3.0
+Version: 0.4.0
 Summary: A micro:bit serial port logger
 Author-email: p4irin <p4irin.github.io@gmail.com>
 Project-URL: Homepage, https://github.com/p4irin/ubitlogger
 Project-URL: Bug Tracker, https://github.com/p4irin/ubitlogger/issues
 Keywords: microbit,microbit-v1,data-logger,serial-port-listener
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -100,29 +100,31 @@
                  /dev/<device> /media/MICROBIT" Figure out the <device>
                  with "sudo fdisk -l". To flash, you need sudo and the
                  path to ubitlogger! I.e., "sudo venv/bin/ubitlogger
                  flash -s light", assuming you use a virtualenv venv.
 
 # Show help on start sub command
 (venv) $ ubitlogger start -h
-usage: ubitlogger start [-h] [-d] [-t TIMEOUT]
+usage: ubitlogger start [-h] [-d] [-t TIMEOUT] [-i INTERVAL]
 
 options:
   -h, --help            show this help message and exit
   -d, --debug           show debugging output
   -t TIMEOUT, --timeout TIMEOUT
                         set a timeout (float)
+  -i INTERVAL, --interval INTERVAL
+                        time between readings
 
 # Show help on the flash sub command
 (venv) $ ubitlogger flash -h
 usage: ubitlogger flash [-h] -s {temperature,light}
 
 options:
   -h, --help            show this help message and exit
-  -s {temperature,light}, --sensor {temperature,light}
+  -s {temperature,light,accelerometer}, --sensor {temperature,light,accelerometer}
                         Specify the sensor to read
 
 # Log to the console with defaults
 (venv) $ ubitlogger start
 ...
 <data>
 ...
```

### Comparing `ubitlogger-0.3.0/README.md` & `ubitlogger-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -64,29 +64,31 @@
                  /dev/<device> /media/MICROBIT" Figure out the <device>
                  with "sudo fdisk -l". To flash, you need sudo and the
                  path to ubitlogger! I.e., "sudo venv/bin/ubitlogger
                  flash -s light", assuming you use a virtualenv venv.
 
 # Show help on start sub command
 (venv) $ ubitlogger start -h
-usage: ubitlogger start [-h] [-d] [-t TIMEOUT]
+usage: ubitlogger start [-h] [-d] [-t TIMEOUT] [-i INTERVAL]
 
 options:
   -h, --help            show this help message and exit
   -d, --debug           show debugging output
   -t TIMEOUT, --timeout TIMEOUT
                         set a timeout (float)
+  -i INTERVAL, --interval INTERVAL
+                        time between readings
 
 # Show help on the flash sub command
 (venv) $ ubitlogger flash -h
 usage: ubitlogger flash [-h] -s {temperature,light}
 
 options:
   -h, --help            show this help message and exit
-  -s {temperature,light}, --sensor {temperature,light}
+  -s {temperature,light,accelerometer}, --sensor {temperature,light,accelerometer}
                         Specify the sensor to read
 
 # Log to the console with defaults
 (venv) $ ubitlogger start
 ...
 <data>
 ...
```

### Comparing `ubitlogger-0.3.0/pyproject.toml` & `ubitlogger-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ubitlogger"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
   { name="p4irin", email="p4irin.github.io@gmail.com" },
 ]
 description = "A micro:bit serial port logger"
 readme = "README.md"
 requires-python = ">=3.8.10"
 keywords = [
@@ -60,15 +60,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 
 [tool.bumpver]
-current_version = "0.3.0"
+current_version = "0.4.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 commit = true
 tag = true
 push = false
 
@@ -78,12 +78,23 @@
   'version = "{version}"',
 ]
 "src/ubitlogger/__init__.py" = [
   "^__version__ = '{version}'$",
 ]
 
 
+[tool.ruff]
+exclude = [
+  "read_sensor*.py",
+]
+
+
 [tool.mypy]
+exclude = [
+  "read_sensor",
+]
 
 [[tool.mypy.overrides]]
-module = "serial.*"
+module = [
+  "serial.*", "uflash",
+]
 ignore_missing_imports = true
```

### Comparing `ubitlogger-0.3.0/setup.py` & `ubitlogger-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `ubitlogger-0.3.0/src/ubitlogger/__init__.py` & `ubitlogger-0.4.0/src/ubitlogger/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 """
 
 __author__ = 'p4irin'
 __email__ = 'p4irin.github.io@gmail.com'
-__version__ = '0.3.0'
+__version__ = '0.4.0'
 
 
 from threading import Thread, Event, enumerate
 from signal import signal, SIGINT, SIGTERM
 from time import sleep
 from serial import Serial
 from serial.tools.list_ports import comports
@@ -46,22 +46,24 @@
     _product_id = 516
     _vendor_id = 3368
 
     def __init__(
             self, handler = None,
             baudrate: int = 115200,
             timeout: float = 0.1,
+            interval: int = 1,
             debug: bool = False,
             block: bool = True
             ) -> None:
         
         self._debug = debug
         self.handler = handler or self._default_handler
         self._baudrate = baudrate
         self._timeout = timeout
+        self._interval = interval
         self._block = block
         self._serial_port = self._scan()
 
     def _default_handler(self, line:str):
         print(line)
 
     def _scan(self) -> Serial:
@@ -85,26 +87,27 @@
     
     def _listen(self):
         self._serial_port.reset_input_buffer()
         while not _stop_event.is_set():
             if self._serial_port.in_waiting > 0:
                 line = self._serial_port.readline().decode('utf-8').strip()
                 self.handler(line)
-            sleep(2)
+            sleep(self._interval)
         self._serial_port.close()
 
     def start(self):
         if self._debug:
             connection = self._serial_port
             print(f"Listening on port {connection.port}")
             print(f"Baudrate: {connection.baudrate}")
             print(f"Data bits: {connection.bytesize}")
             print(f"Stop bits: {connection.stopbits}")
             print(f"Parity: {connection.parity}")
             print(f"timeout: {connection.timeout}")
+            print(f"interval: {self._interval}")
 
         thread = Thread(target=self._listen, name="listening_thread")
         self._thread = thread
         self._thread.start()
         if self._block:
             self._thread.join()
```

### Comparing `ubitlogger-0.3.0/src/ubitlogger/cli.py` & `ubitlogger-0.4.0/src/ubitlogger/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,14 +39,21 @@
     sp_start.add_argument(
         '-t',
         '--timeout',
         action='store',
         type=float,
         help='set a timeout (float)'
     )
+    sp_start.add_argument(
+        '-i',
+        '--interval',
+        action='store',
+        type=int,
+        help='time between readings'
+    )
 
     sp_flash = sub_parsers.add_parser(
         'flash',
         help='Flash an example sensor reader script to the micro:bit. '
             + 'Does NOT work on WSL! On Ubuntu jammy the micro:bit is '
             + 'NOT auto mounted! You need to mount it like '
             + '"sudo mount /dev/<device> /media/MICROBIT". '
@@ -55,37 +62,40 @@
             + 'I.e., "sudo venv/bin/ubitlogger flash -s light", '
             + 'assuming you use a virtualenv venv.'
     )
     sp_flash.add_argument(
         '-s',
         '--sensor',
         action='store',
-        choices=['temperature', 'light'],
+        choices=['temperature', 'light', 'accelerometer'],
         required=True,
         help='Specify the sensor to read'
         )
 
     args = parser.parse_args()
     kwargs = {}
     if args.command == 'start':
         if args.debug:
             debug_flag = True
         else:
             debug_flag = False
         kwargs['debug'] = debug_flag
         if args.timeout:
-            timeout_flag = args.timeout
-            kwargs['timeout'] = timeout_flag
+            kwargs['timeout'] = args.timeout
+        if args.interval:
+            kwargs['interval'] = args.interval
 
     if args.command == 'flash':
         if args.sensor and 'WSL' not in os.uname().release:
             if args.sensor == 'temperature':
                 _function = args.sensor
             if args.sensor == 'light':
                 _function = 'display.read_light_level'
+            if args.sensor == 'accelerometer':
+                _function = 'accelerometer.get_values'
 
             package_dir = os.path.dirname(os.path.abspath(__file__))
             script_file_path = f'{package_dir}/read_sensor.py'
             script_file_copy_path = script_file_path.replace('.py', '_copy.py')
             with open(script_file_path, 'r') as fh:
                 script = fh.read()
                 script = script.replace('{% function %}', _function)
```

### Comparing `ubitlogger-0.3.0/src/ubitlogger.egg-info/PKG-INFO` & `ubitlogger-0.4.0/src/ubitlogger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubitlogger
-Version: 0.3.0
+Version: 0.4.0
 Summary: A micro:bit serial port logger
 Author-email: p4irin <p4irin.github.io@gmail.com>
 Project-URL: Homepage, https://github.com/p4irin/ubitlogger
 Project-URL: Bug Tracker, https://github.com/p4irin/ubitlogger/issues
 Keywords: microbit,microbit-v1,data-logger,serial-port-listener
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -100,29 +100,31 @@
                  /dev/<device> /media/MICROBIT" Figure out the <device>
                  with "sudo fdisk -l". To flash, you need sudo and the
                  path to ubitlogger! I.e., "sudo venv/bin/ubitlogger
                  flash -s light", assuming you use a virtualenv venv.
 
 # Show help on start sub command
 (venv) $ ubitlogger start -h
-usage: ubitlogger start [-h] [-d] [-t TIMEOUT]
+usage: ubitlogger start [-h] [-d] [-t TIMEOUT] [-i INTERVAL]
 
 options:
   -h, --help            show this help message and exit
   -d, --debug           show debugging output
   -t TIMEOUT, --timeout TIMEOUT
                         set a timeout (float)
+  -i INTERVAL, --interval INTERVAL
+                        time between readings
 
 # Show help on the flash sub command
 (venv) $ ubitlogger flash -h
 usage: ubitlogger flash [-h] -s {temperature,light}
 
 options:
   -h, --help            show this help message and exit
-  -s {temperature,light}, --sensor {temperature,light}
+  -s {temperature,light,accelerometer}, --sensor {temperature,light,accelerometer}
                         Specify the sensor to read
 
 # Log to the console with defaults
 (venv) $ ubitlogger start
 ...
 <data>
 ...
```

