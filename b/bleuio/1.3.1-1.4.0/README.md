# Comparing `tmp/bleuio-1.3.1-py3-none-any.whl.zip` & `tmp/bleuio-1.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 20033 bytes, number of entries: 12
+Zip file size: 21277 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat        0 b- defN 20-Nov-05 12:17 bleuio_lib/__init__.py
--rw-rw-rw-  2.0 fat    69935 b- defN 23-Oct-02 13:31 bleuio_lib/bleuio_funcs.py
+-rw-rw-rw-  2.0 fat    77873 b- defN 24-Apr-24 07:48 bleuio_lib/bleuio_funcs.py
 -rw-rw-rw-  2.0 fat      150 b- defN 20-Nov-06 08:33 bleuio_lib/exceptions.py
 -rw-rw-rw-  2.0 fat        0 b- defN 20-Nov-05 12:20 bleuio_tests/__init__.py
 -rw-rw-rw-  2.0 fat     9476 b- defN 21-Jul-01 11:49 bleuio_tests/test_bleuio_funcs.py
 -rw-rw-rw-  2.0 fat        0 b- defN 20-Nov-05 12:20 tests/__init__.py
 -rw-rw-rw-  2.0 fat     2840 b- defN 20-Nov-10 12:43 tests/test_bleuio_funcs.py
--rw-rw-rw-  2.0 fat     1086 b- defN 23-Oct-02 14:15 bleuio-1.3.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat    32440 b- defN 23-Oct-02 14:15 bleuio-1.3.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Oct-02 14:15 bleuio-1.3.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Oct-02 14:15 bleuio-1.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      948 b- defN 23-Oct-02 14:15 bleuio-1.3.1.dist-info/RECORD
-12 files, 116983 bytes uncompressed, 18439 bytes compressed:  84.2%
+-rw-rw-rw-  2.0 fat     1086 b- defN 24-Apr-24 07:59 bleuio-1.4.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat    34384 b- defN 24-Apr-24 07:59 bleuio-1.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 24-Apr-24 07:59 bleuio-1.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 24-Apr-24 07:59 bleuio-1.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      948 b- defN 24-Apr-24 07:59 bleuio-1.4.0.dist-info/RECORD
+12 files, 126865 bytes uncompressed, 19683 bytes compressed:  84.5%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_bleuio_funcs.py
 Comment: 
 
-Filename: bleuio-1.3.1.dist-info/LICENSE.txt
+Filename: bleuio-1.4.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: bleuio-1.3.1.dist-info/METADATA
+Filename: bleuio-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: bleuio-1.3.1.dist-info/WHEEL
+Filename: bleuio-1.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: bleuio-1.3.1.dist-info/top_level.txt
+Filename: bleuio-1.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: bleuio-1.3.1.dist-info/RECORD
+Filename: bleuio-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bleuio_lib/bleuio_funcs.py

```diff
@@ -1,24 +1,28 @@
-# (C) 2023 Smart Sensor Devices AB
+# (C) 2024 Smart Sensor Devices AB
 
 import sys
 import threading
 import time
 import json
 import signal
 import atexit
+from copy import deepcopy
 
 import serial.tools.list_ports
 
 DONGLE_ARRAY = []
 
 DUAL = "dual"
 CENTRAL = "central"
 PERIPHERAL = "peripheral"
 
+# version: 1.4.0
+# updated: 2024-04-24
+
 
 class BleuIO(object):
     def __init__(self, port="auto", baud=115200, timeout=0.01, debug=False):
         """
         Initiates the dongle. If port param is left as 'auto' it will auto-detect if bleuio dongle is connected.
         :param port: str
         :param baud: int
@@ -180,46 +184,156 @@
             self.Ack = None
             self.Rsp = []
             self.End = None
 
     class BleuIOException(Exception):
         pass
 
+    # def openPort(self, port="auto", baud=115200, timeout=0.01):
+    #     DONGLE_ARRAY = []
+    #     retry_count = 0
+    #     if port == "auto":
+    #         dongle_count = 1
+    #         port_list = []
+    #         while len(DONGLE_ARRAY) == 0 and retry_count < 10:
+    #             all_ports = serial.tools.list_ports.comports(include_links=False)
+    #             for d_port in all_ports:
+    #                 if str(d_port.hwid).__contains__("VID:PID=2DCF"):
+    #                     bleuio_dongle = (
+    #                         str(dongle_count) + ") " + d_port.device + " " + d_port.hwid
+    #                     )
+    #                     if bleuio_dongle.__contains__("VID:PID=2DCF:6002"):
+    #                         if self._debug:
+    #                             print("Found dongle in port: " + d_port.device)
+    #                         DONGLE_ARRAY.append(bleuio_dongle)
+    #                         port_list.append(d_port)
+    #                         dongle_count += 1
+    #                     if bleuio_dongle.__contains__("VID:PID=2DCF:6001"):
+    #                         if self._debug:
+    #                             print("Bootloader in port: " + d_port.device)
+    #                         time.sleep(2)
+    #                         retry_count = 0
+    #                 else:
+    #                     pass
+    #             retry_count += 1
+
+    #         try:
+    #             self._serial = serial.Serial(
+    #                 port=port_list[0].device, baudrate=baud, timeout=timeout
+    #             )
+    #             self._port = port_list[0].device
+    #         except (serial.SerialException, IndexError):
+    #             raise
+
+    #     else:
+    #         if not isinstance(port, str):
+    #             raise ValueError("Invalid port specified: {}".format(port))
+    #         while self._serial is None:
+    #             try:
+    #                 self._serial = serial.Serial(
+    #                     port=port, baudrate=baud, timeout=timeout, write_timeout=timeout
+    #                 )
+    #                 self._port = port
+    #             except (ValueError, serial.SerialException) as e:
+    #                 retry_count += 1
+    #                 if retry_count > 3:
+    #                     print("Error: " + str(e))
+    #                     print("Make sure the dongle is not already in use.")
+    #                     exit()
+    #                 else:
+    #                     if self._debug:
+    #                         print(
+    #                             "Error occurred while trying to open port. "
+    #                             + str(e)
+    #                             + " Retrying",
+    #                             retry_count,
+    #                             "/",
+    #                             3,
+    #                             "...",
+    #                         )
+    #                     time.sleep(5)
+
+    #         self._serial.flushInput()
+    #         self._serial.flushOutput()
+
+    #     # rx task state
+    #     self.rx_buffer = b""
+    #     self.rx_response = []
+    #     self.rx_scanning_results = []
+    #     self.rx_evt_results = []
+
+    #     self._start_reader()
+    #     self.send_command("stop")
+    #     self.send_command("ATV1")
+    #     self.send_command("ATE1")
+    #     self.send_command("ATI")
+
+    # def closePort(self):
+    #     self._stop_reader()
+    #     if self._debug:
+    #         print("Closing reader...")
+    #     self._serial.close()
+    #     if self._debug:
+    #         print("Closing Port...")
+
     def __signal_handler(self, signum, frame):
+        if self._debug:
+            print("Exit Signal Handler...")
         sys.exit(1)
 
-    def __parseRspIntoJSON(self, response, careObj):
+    def __parseRspIntoJSON(self, inputData, careObj):
+        response = deepcopy(inputData)
+        newResp = []
+
+        if b"\r" in response:
+            for line in response.splitlines():
+                if not line == b"":
+                    newResp.append(line)
+            response = newResp
+
         try:
             for line in response:
                 if ('{"C"') in line.decode("utf-8", "ignore"):
                     careObj.Cmd = json.loads(line)
                 if ('{"A"') in line.decode("utf-8", "ignore"):
                     careObj.Ack = json.loads(line)
                 if ('{"R"') in line.decode("utf-8", "ignore"):
                     careObj.Rsp.append(json.loads(line))
                 if ('{"E"') in line.decode("utf-8", "ignore"):
                     careObj.End = json.loads(line)
                 if ('{"SE":') in line.decode("utf-8", "ignore"):
                     careObj.Ack = json.loads(line)
         except Exception as e:
             raise self.BleuIOException(
-                "Exception: " + str(e) + "\r\nError line: " + str(line) + "\r\n(Response: " + str(response) + ")"
+                "Exception: "
+                + str(e)
+                + "\r\nError line: "
+                + str(line)
+                + "\r\n(Response: "
+                + str(response)
+                + ")"
             )
         if self._debug:
             try:
                 print("debug(__parseRspIntoJSON response): " + str(response))
                 print("debug(__parseRspIntoJSON line): " + str(line))
             except Exception:
                 pass
 
     def exit_handler(self):
-        self._serial.write("\x03".encode())
-        self._serial.write("\x1B".encode())
-        self._stop_reader()
-        self._serial.close()
+        if self._debug:
+            print("Exit Handler Cleanup...")
+        if self._serial.is_open:
+            try:
+                self._serial.write("\x03".encode())
+                self._serial.write("\x1B".encode())
+                self._stop_reader()
+                self._serial.close()
+            except Exception:
+                pass
 
     def _start_reader(self):
         """Start reader thread"""
         self._reader_alive = True
         # start serial->reader thread
         self.receiver_thread = threading.Thread(target=self.__poll_serial, name="rx")
         self.receiver_thread.daemon = True
@@ -231,15 +345,15 @@
         self.receiver_thread.join()
 
     def __poll_serial(self):
         """Polls Dongle RX Data"""
         while self._reader_alive:
             try:
                 self.rx_buffer += self._serial.read(self._serial.in_waiting)
-                if self.rx_buffer and self.rx_buffer[-1:] == b'\n':
+                if self.rx_buffer and self.rx_buffer[-1:] == b"\n":
                     if str.encode('"action":"scan completed"') in self.rx_buffer:
                         self.__threadLock.acquire()
                         self.status.isScanning = False
                         self.__saveScanRsp = False
                         self.__threadLock.release()
                         if not self.__cmdDone:
                             self.__threadLock.acquire()
@@ -414,15 +528,15 @@
                             self.__cmdDone = True
                             self.__threadLock.release()
                     if self._debug:
                         try:
                             print("debug(rx_buffer): " + str(self.rx_buffer))
                         except Exception:
                             pass
-                    self.rx_buffer = b''
+                    self.rx_buffer = b""
             except serial.SerialException as e:
                 print("exception: " + str(e))
                 self.alive = False
                 sys.exit(1)
 
     def register_scan_cb(self, callback):
         """Registers callback function for recieving scan results.
@@ -451,14 +565,17 @@
 
     def unregister_evt_cb(self):
         """Unregister the callback function for recieving events."""
         self.__saveEvtRsp = False
         self._evt_cb = None
 
     def send_command(self, cmd):
+        if not self._serial.is_open:
+            raise self.BleuIOException("Port to BleuIO is not open!")
+
         if self.status.isSPSStreamOn and cmd != "esc":
             self._serial.write(cmd.encode())
             self.rx_response.append(str('{"A":"","err": 0, "status": "ok"}').encode())
             return self.rx_response
         else:
             if self._debug:
                 print("send_command: " + cmd)
@@ -585,14 +702,21 @@
     def __at_advresp(self, respData):
 
         if respData == "":
             return self.send_command("AT+ADVRESP")
         else:
             return self.send_command("AT+ADVRESP=" + respData)
 
+    def __at_auto_exec(self, cmds):
+
+        if cmds == "":
+            return self.send_command("AT+AUTOEXEC")
+        else:
+            return self.send_command("AT+AUTOEXEC=" + cmds)
+
     def __at_cancel_connect(self):
 
         return self.send_command("AT+CANCELCONNECT")
 
     def __at_central(self):
 
         return self.send_command("AT+CENTRAL")
@@ -605,14 +729,39 @@
 
         return self.send_command("AT+CLEARINDI=" + handle)
 
     def __at_client(self):
 
         return self.send_command("AT+CLIENT")
 
+    def __at_clrautoexec(self):
+
+        return self.send_command("AT+CLRAUTOEXEC")
+
+    def __at_connparam(self, intv_min, intv_max, slave_latency, sup_timeout):
+
+        adv_params = False
+        if intv_min:
+            if intv_max:
+                if slave_latency:
+                    if sup_timeout:
+                        adv_params = True
+                        return self.send_command(
+                            "AT+CONNPARAM="
+                            + intv_min
+                            + "="
+                            + intv_max
+                            + "="
+                            + slave_latency
+                            + "="
+                            + sup_timeout
+                        )
+        if not adv_params:
+            return self.send_command("AT+CONNPARAM")
+
     def __at_devicename(self, name):
 
         if name == "":
             return self.send_command("AT+DEVICENAME")
         else:
             return self.send_command("AT+DEVICENAME=" + name)
 
@@ -728,14 +877,18 @@
 
         return self.send_command("AT+GATTCWRITEWR=" + uuid + " " + data)
 
     def __at_gattcwritewrb(self, uuid, data):
 
         return self.send_command("AT+GATTCWRITEWRB=" + uuid + " " + data)
 
+    def __at_getbond(self):
+
+        return self.send_command("AT+GETBOND")
+
     def __at_get_services(self):
 
         return self.send_command("AT+GETSERVICES")
 
     def __at_get_services_only(self):
 
         return self.send_command("AT+GETSERVICESONLY")
@@ -865,20 +1018,20 @@
         return self.send_command("AT+CUSTOMSERVICESTART")
 
     def __at_customservice_stop(self):
         return self.send_command("AT+CUSTOMSERVICESTOP")
 
     def __at_customservice_reset(self):
         return self.send_command("AT+CUSTOMSERVICERESET")
-    
+
     def __at_suota_start(self):
         return self.send_command("AT+SUOTASTART")
 
     def __at_suota_stop(self):
-        return self.send_command("AT+SUOTASTOP")        
+        return self.send_command("AT+SUOTASTOP")
 
     def __help(self):
 
         return self.send_command("--H")
 
     def __stop_scan(self):
 
@@ -1074,14 +1227,28 @@
         """
         care = self.__at_advresp(respData)
         response = self.BleuIORESP()
         self.__parseRspIntoJSON(care, response)
 
         return response
 
+    def at_autoexec(self, cmds=""):
+        """Sets or displays up to 10 commands that will be run upon the BleuIO starting up. Max command lenght is currently set at 255 characters.
+
+        :param: Sets commands. If left empty it will query set commands.
+        :type cmds: str
+        :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
+        :rtype: obj BleuIORESP
+        """
+        care = self.__at_auto_exec(cmds)
+        response = self.BleuIORESP()
+        self.__parseRspIntoJSON(care, response)
+
+        return response
+
     def at_cancel_connect(self):
         """While in Central Mode, cancels any ongoing connection attempts.
 
         :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
         :rtype: obj BleuIORESP
         """
         care = self.__at_cancel_connect()
@@ -1134,14 +1301,42 @@
         """
         care = self.__at_client()
         response = self.BleuIORESP()
         self.__parseRspIntoJSON(care, response)
 
         return response
 
+    def at_clrautoexec(self):
+        """Clear any commands in the auto execute (AUTOEXEC) list.
+
+        :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
+        :rtype: obj BleuIORESP
+        """
+        care = self.__at_clrautoexec()
+        response = self.BleuIORESP()
+        self.__parseRspIntoJSON(care, response)
+
+        return response
+
+    def at_connparam(self, intv_min="", intv_max="", slave_latency="", sup_timeout=""):
+        """Sets or displays preferred connection parameters. When run while connected will update connection parameters on the current target connection.
+
+        :param intv_min: str
+        :param intv_max: str
+        :param slave_latency: str
+        :param sup_timeout: str
+        :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
+        :rtype: obj BleuIORESP
+        """
+        care = self.__at_connparam(intv_min, intv_max, slave_latency, sup_timeout)
+        response = self.BleuIORESP()
+        self.__parseRspIntoJSON(care, response)
+
+        return response
+
     def at_divicename(self, name=""):
         """Gets or sets the device name.
 
         :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
         :rtype: obj BleuIORESP
         """
         care = self.__at_devicename(name)
@@ -1422,14 +1617,26 @@
         """
         care = self.__at_gattcwritewrb(uuid, data)
         response = self.BleuIORESP()
         self.__parseRspIntoJSON(care, response)
 
         return response
 
+    def at_getbond(self):
+        """Displays all MAC address of bonded devices.
+
+        :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
+        :rtype: obj BleuIORESP
+        """
+        care = self.__at_getbond()
+        response = self.BleuIORESP()
+        self.__parseRspIntoJSON(care, response)
+
+        return response
+
     def at_get_conn(self):
         """Gets a list of currently connected devices along with their mac addresses and conn_idx.
 
         :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
         :rtype: obj BleuIORESP
         """
         care = self.__at_get_conn()
@@ -1748,15 +1955,15 @@
         :rtype: obj BleuIORESP
         """
         care = self.__at_customservice_reset()
         response = self.BleuIORESP()
         self.__parseRspIntoJSON(care, response)
 
         return response
-    
+
     def at_suota_start(self):
         """Enables the SUOTA Service and start the SUOTA Advertising.
            Cannot be started while connected/connecting or advertising.
 
         :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
         :rtype: obj BleuIORESP
         """
@@ -1773,15 +1980,15 @@
         :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
         :rtype: obj BleuIORESP
         """
         care = self.__at_suota_stop()
         response = self.BleuIORESP()
         self.__parseRspIntoJSON(care, response)
 
-        return response        
+        return response
 
     def help(self):
         """Shows all AT-Commands.
 
         :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects. except for Rsp which contains a list of JSON objects.
         :rtype obj BleuIORESP
         """
```

## Comparing `bleuio-1.3.1.dist-info/LICENSE.txt` & `bleuio-1.4.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `bleuio-1.3.1.dist-info/METADATA` & `bleuio-1.4.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 Metadata-Version: 2.1
 Name: bleuio
-Version: 1.3.1
+Version: 1.4.0
 Summary: Library for using the bleuio dongle.
 Home-page: https://smart-sensor-devices-ab.github.io/ssd005-manual/
 Author: Smart Sensor Devices
 Author-email: smartzenzor@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Requires-Dist: pyserial
 
-## Python library v1.3.1 for BleuIO
+## Python library v1.4.0 for BleuIO
 
-### Supports BleuIO v.2.3.0 or later
+### Supports BleuIO v.2.7.1
 
 > NOTE: Does not support 2.2.0 or earlier version of BleuIO firmware
 
 ### Changes
 
+#### 1.4.0
+
+- Added functions for commands introduced up to BleuIO fw version 2.7.1. Following command functions have been added:
+  - at*autoexec() ( \_AT+AUTOEXEC* )
+  - at*clrautoexec() ( \_AT+CLRAUTOEXEC* )
+  - at*connparam() ( \_AT+CONNPARAM* )
+  - at*getbond() ( \_AT+GETBOND* )
+
 #### 1.3.1
 
 - Added support for SUOTA commands introduced in BleuIO fw version 2.4.0
 - Fixed a bug when running on MacOS where the serial responses sometimes are returned in two parts instead of just one. The library expected one but can now handle two or more.
 
 #### 1.3.0
 
@@ -350,14 +358,23 @@
 
         :param: Sets scan response data. If left empty it will query what advdata is set. Format: xx:xx:xx:xx:xx.. (max 31 bytes)
         :type respData: hex str
         :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
         :rtype: obj BleuIORESP
         """
 
+    def at_autoexec(self, cmds=""):
+        """Sets or displays up to 10 commands that will be run upon the BleuIO starting up. Max command lenght is currently set at 255 characters.
+
+        :param: Sets commands. If left empty it will query set commands.
+        :type cmds: str
+        :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
+        :rtype: obj BleuIORESP
+        """
+
     def at_cancel_connect(self):
         """While in Central Mode, cancels any ongoing connection attempts.
 
         :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
         :rtype: obj BleuIORESP
         """
 
@@ -385,14 +402,32 @@
     def at_client(self):
         """Sets the device role towards the targeted connection to client. Only in dual role.
 
         :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
         :rtype: obj BleuIORESP
         """
 
+    def at_clrautoexec(self):
+        """Clear any commands in the auto execute (AUTOEXEC) list.
+
+        :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
+        :rtype: obj BleuIORESP
+        """
+
+    def at_connparam(self, intv_min="", intv_max="", slave_latency="", sup_timeout=""):
+        """Sets or displays preferred connection parameters. When run while connected will update connection parameters on the current target connection.
+
+        :param intv_min: str
+        :param intv_max: str
+        :param slave_latency: str
+        :param sup_timeout: str
+        :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
+        :rtype: obj BleuIORESP
+        """
+
     def at_divicename(self, name=""):
         """Gets or sets the device name.
 
         :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
         :rtype: obj BleuIORESP
         """
 
@@ -561,14 +596,21 @@
 
         :param uuid: hex str format: XXXX
         :param data: hex str format: XXXXXXX..
         :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
         :rtype: obj BleuIORESP
         """
 
+    def at_getbond(self):
+        """Displays all MAC address of bonded devices.
+
+        :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
+        :rtype: obj BleuIORESP
+        """
+
     def at_get_conn(self):
         """Gets a list of currently connected devices along with their mac addresses and conn_idx.
 
         :returns: Object with 4 object properties: Cmd, Ack, Rsp and End. Each property contains a JSON object, except for Rsp which contains a list of JSON objects.
         :rtype: obj BleuIORESP
         """
```

## Comparing `bleuio-1.3.1.dist-info/RECORD` & `bleuio-1.4.0.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 bleuio_lib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-bleuio_lib/bleuio_funcs.py,sha256=knqv-Kwx7OSSiZiJQ7RE_PAB2hmiZmQA38wnpjk6-a0,69935
+bleuio_lib/bleuio_funcs.py,sha256=jNUdqq7-2p4C_I5BK50643EZaXabHoqqUoclPSLVOb4,77873
 bleuio_lib/exceptions.py,sha256=nhsxieAzx-XkSOIDzOuIN4puTvqby4QW3DH-JIxfSxQ,150
 bleuio_tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bleuio_tests/test_bleuio_funcs.py,sha256=dCjpg3dOM5rZY75BReJj2oiow1GVTXBSgebBsmT4ztg,9476
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_bleuio_funcs.py,sha256=lSewBOnSJVnMGlQZqXFG2KDaFnp7nRDFTzShZqr4imc,2840
-bleuio-1.3.1.dist-info/LICENSE.txt,sha256=_MmtOZ8tMxjdtEDkBcnSHLzX7b2JQP7sqMz_LChR4TQ,1086
-bleuio-1.3.1.dist-info/METADATA,sha256=drCy_vcdCSV56DPDFL1498vD0L9hokx-gUV79esE1Yk,32440
-bleuio-1.3.1.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
-bleuio-1.3.1.dist-info/top_level.txt,sha256=U4c2S2JgfJYrt3NsAsmbxMlWPtWuAuhdHzIYtahVtyg,11
-bleuio-1.3.1.dist-info/RECORD,,
+bleuio-1.4.0.dist-info/LICENSE.txt,sha256=_MmtOZ8tMxjdtEDkBcnSHLzX7b2JQP7sqMz_LChR4TQ,1086
+bleuio-1.4.0.dist-info/METADATA,sha256=spNJaCO2TOeU9AjO3KpILJmkbypZT_RYB6VkRmOGKvk,34384
+bleuio-1.4.0.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
+bleuio-1.4.0.dist-info/top_level.txt,sha256=U4c2S2JgfJYrt3NsAsmbxMlWPtWuAuhdHzIYtahVtyg,11
+bleuio-1.4.0.dist-info/RECORD,,
```

