# Comparing `tmp/python-can-mcpcan-0.2.0.tar.gz` & `tmp/python-can-mcpcan-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-can-mcpcan-0.2.0.tar", last modified: Tue Mar 12 14:15:11 2024, max compression
+gzip compressed data, was "python-can-mcpcan-0.2.1.tar", last modified: Wed Apr 24 14:01:43 2024, max compression
```

## Comparing `python-can-mcpcan-0.2.0.tar` & `python-can-mcpcan-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-12 14:15:11.551953 python-can-mcpcan-0.2.0/
--rw-rw-rw-   0        0        0      990 2024-03-12 14:15:11.548945 python-can-mcpcan-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      698 2023-11-20 21:30:51.000000 python-can-mcpcan-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-12 14:15:11.465947 python-can-mcpcan-0.2.0/mcpcan/
--rw-rw-rw-   0        0        0        0 2023-11-20 19:30:16.000000 python-can-mcpcan-0.2.0/mcpcan/__init__.py
--rw-rw-rw-   0        0        0    18965 2024-03-05 22:39:27.000000 python-can-mcpcan-0.2.0/mcpcan/mcpcan.py
-drwxrwxrwx   0        0        0        0 2024-03-12 14:15:11.545946 python-can-mcpcan-0.2.0/mcpcan/python_can_mcpcan.egg-info/
--rw-rw-rw-   0        0        0      990 2024-03-12 14:15:11.000000 python-can-mcpcan-0.2.0/mcpcan/python_can_mcpcan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2024-03-12 14:15:11.000000 python-can-mcpcan-0.2.0/mcpcan/python_can_mcpcan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-12 14:15:11.000000 python-can-mcpcan-0.2.0/mcpcan/python_can_mcpcan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-03-12 14:15:11.000000 python-can-mcpcan-0.2.0/mcpcan/python_can_mcpcan.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2024-03-12 14:15:11.000000 python-can-mcpcan-0.2.0/mcpcan/python_can_mcpcan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-03-12 14:15:11.000000 python-can-mcpcan-0.2.0/mcpcan/python_can_mcpcan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1802 2024-02-07 20:16:58.000000 python-can-mcpcan-0.2.0/mcpcan/utils.py
--rw-rw-rw-   0        0        0       99 2023-11-20 19:16:00.000000 python-can-mcpcan-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-12 14:15:11.552952 python-can-mcpcan-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      813 2024-03-05 21:43:52.000000 python-can-mcpcan-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:01:43.587199 python-can-mcpcan-0.2.1/
+-rw-rw-rw-   0        0        0      990 2024-04-24 14:01:43.581678 python-can-mcpcan-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      698 2023-11-20 21:30:51.000000 python-can-mcpcan-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 14:01:43.526049 python-can-mcpcan-0.2.1/mcpcan/
+-rw-rw-rw-   0        0        0        0 2023-11-20 19:30:16.000000 python-can-mcpcan-0.2.1/mcpcan/__init__.py
+-rw-rw-rw-   0        0        0    18697 2024-04-24 13:58:53.000000 python-can-mcpcan-0.2.1/mcpcan/mcpcan.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:01:43.576154 python-can-mcpcan-0.2.1/mcpcan/python_can_mcpcan.egg-info/
+-rw-rw-rw-   0        0        0      990 2024-04-24 14:01:43.000000 python-can-mcpcan-0.2.1/mcpcan/python_can_mcpcan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2024-04-24 14:01:43.000000 python-can-mcpcan-0.2.1/mcpcan/python_can_mcpcan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 14:01:43.000000 python-can-mcpcan-0.2.1/mcpcan/python_can_mcpcan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 14:01:43.000000 python-can-mcpcan-0.2.1/mcpcan/python_can_mcpcan.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2024-04-24 14:01:43.000000 python-can-mcpcan-0.2.1/mcpcan/python_can_mcpcan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-24 14:01:43.000000 python-can-mcpcan-0.2.1/mcpcan/python_can_mcpcan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1802 2024-02-07 20:16:58.000000 python-can-mcpcan-0.2.1/mcpcan/utils.py
+-rw-rw-rw-   0        0        0       99 2023-11-20 19:16:00.000000 python-can-mcpcan-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-24 14:01:43.588211 python-can-mcpcan-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      813 2024-04-24 13:57:37.000000 python-can-mcpcan-0.2.1/setup.py
```

### Comparing `python-can-mcpcan-0.2.0/PKG-INFO` & `python-can-mcpcan-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-can-mcpcan
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python-can MCPcan
 Home-page: https://github.com/hardbyte/python-can
 Author: SoftMagic
 Author-email: softmajik@gmail.com
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: python-can
```

### Comparing `python-can-mcpcan-0.2.0/README.md` & `python-can-mcpcan-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `python-can-mcpcan-0.2.0/mcpcan/mcpcan.py` & `python-can-mcpcan-0.2.1/mcpcan/mcpcan.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,42 +2,39 @@
 To Support the MCP-Can analyzer interface. The device will appear
 as a serial port, for example "/dev/ttyUSB0" on Linux machines
 or "COM1" on Windows.
 
 """
 
 import logging
-import struct
 import io
 import utils
 from time import time
 from typing import Optional
 
 import can
 from can import BusABC, Message, CanProtocol
 
-# from can.util import check_or_adjust_timing_clock, dlc2len, len2dlc
-
 logger = logging.getLogger(__name__)
 
 try:
     import serial
     import serial.tools.list_ports
     from serial.tools.list_ports_common import ListPortInfo
 except ImportError:
     logger.warning(
-        "You won't be able to use the mcp can backend without "
+        "You won't be able to use the mcpcan backend without "
         "the serial module installed!"
     )
     serial = None
 
 
 class MCPcanBus(BusABC):
     """
-    Enable basic can communication over d10 mcp2515 can interface.
+    Enable basic can communication over d10 mcp2518 can interface.
     """
 
     BITRATE = {
         5000: 1,
         10000: 2,
         20000: 3,
         31250: 4,
@@ -155,39 +152,31 @@
 
         self.channel_info = "Serial interface: " + channel
         self._can_protocol = CanProtocol.CAN_FD if fd else CanProtocol.CAN_20
         self.is_fd = fd
         self.mcp18fd = False
         self.flag = True
         self.fw_ver = 0
+        self.is_connected = False  # v2.1
         tries = 3  # set number of retries if serial is spotty
         ctype = ""
 
         # helper:
         ports: list[ListPortInfo] = serial.tools.list_ports.comports()
         for port in ports:
             if channel in port[0] and "SER=MFD" in port[2]:
                 self.mcp18fd = True
-
         for n in range(tries):
             try:
                 self.ser = serial.serial_for_url(
                     channel, baudrate=baudrate, timeout=timeout, rtscts=False
                 )
                 ctype = self._get_device()  # get device hardware version
-                if ctype == "DT2515":
-                    if fd:
-                        self.ser.close()
-                        raise can.CanInitializationError(
-                            "Mcpcan device does not exist yet :) !"
-                        )
-                    else:
-                        self.flush_input_buffer()
-                        break
-                elif ctype == "DT2518":
+                if ctype == "DT2518":
+                    self.is_connected = True
                     self.flush_input_buffer()
                     break
                 else:
                     self.ser.close()
                     if n == (tries - 1):
                         raise can.CanInitializationError("Cannot initialized mcpcan.")
             except ValueError as error:
@@ -205,36 +194,30 @@
             if fdbitrate in MCPcanBus.FDBITRATE:
                 self._set_bitrate(MCPcanBus.FDBITRATE[fdbitrate])
             else:
                 raise can.CanInitializationError(
                     "Bitrate and dbitrate combination not allowed!"
                 )
         else:
-            if self.mcp18fd:
-                self._set_bitrate(MCPcanBus.FDBITRATE[bitrate])
-            else:
-                self._set_bitrate(MCPcanBus.BITRATE[bitrate])
+            self._set_bitrate(MCPcanBus.FDBITRATE[bitrate])
 
         super().__init__(channel=channel, can_filters=can_filters, *args, **kwargs)
 
     def _get_device(self):
         """
         Identify mcp device. Called only during interface creation.
         """
         # close can
         if self.serial_write_read("C") != None:
             # get mcp type
             self.flush_input_buffer()
             str_msg = "V"
             device = self.serial_write_read(str_msg).strip().decode()
             logger.debug("get device type: %s", device)
-            if device in [
-                'DT2515',
-                'DT2518',
-            ]:  #'DT2515' is only a placeholder for future devices
+            if device == 'DT2518':
                 str_msg = "v"
                 self.fw_ver = int(self.serial_write_read(str_msg).strip().decode())
                 logger.debug("get device fw version: %d", self.fw_ver)
                 # open can
                 if self.serial_write_read("O") != None:
                     return device
             else:
@@ -264,27 +247,36 @@
         raise can.CanInitializationError("Could not set device bitrate")
 
     def shutdown(self):
         """
         Close the serial interface.
         """
         super().shutdown()
-        self.ser.close()
+        logger.info(
+            "send hardware reset upon shutdown and be ready for the next session"
+        )
+        if self.is_connected:
+            self._write("H")  # hardware reset
+            self.ser.close()
+            self.is_connected = False
 
     def flush_input_buffer(self):
         self.ser.reset_input_buffer()
 
     def serial_write_read(self, smsg):
         try:
             self._write(smsg)
             stime = time()
             while not self.ser.in_waiting and time() - stime < 10:
                 pass
             if self.ser.in_waiting:
-                return self.ser.read(self.ser.in_waiting)
+                rmsg = self.ser.read()
+                while chr(rmsg[-1]) != '\r':
+                    rmsg += self.ser.read()
+                return rmsg
             else:
                 raise can.CanTimeoutError()
         except serial.PortNotOpenError as error:
             raise can.CanOperationError(
                 "writing to or reading from a closed port"
             ) from error
         except serial.SerialTimeoutException as error:
```

### Comparing `python-can-mcpcan-0.2.0/mcpcan/python_can_mcpcan.egg-info/PKG-INFO` & `python-can-mcpcan-0.2.1/mcpcan/python_can_mcpcan.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-can-mcpcan
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python-can MCPcan
 Home-page: https://github.com/hardbyte/python-can
 Author: SoftMagic
 Author-email: softmajik@gmail.com
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: python-can
```

### Comparing `python-can-mcpcan-0.2.0/mcpcan/utils.py` & `python-can-mcpcan-0.2.1/mcpcan/utils.py`

 * *Files identical despite different names*

### Comparing `python-can-mcpcan-0.2.0/setup.py` & `python-can-mcpcan-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="python-can-mcpcan",
-    version="0.2.0",
+    version="0.2.1",
     author="SoftMagic",
     author_email="softmajik@gmail.com",
     description="Python-can MCPcan",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/hardbyte/python-can",
     package_dir={"": "mcpcan"},
```

