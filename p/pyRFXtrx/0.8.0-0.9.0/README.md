# Comparing `tmp/pyRFXtrx-0.8.0.tar.gz` & `tmp/pyRFXtrx-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyRFXtrx-0.8.0.tar", last modified: Wed Jun  1 08:26:10 2016, max compression
+gzip compressed data, was "dist/pyRFXtrx-0.9.0.tar", last modified: Mon Jul 11 06:52:38 2016, max compression
```

## Comparing `pyRFXtrx-0.8.0.tar` & `pyRFXtrx-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-06-01 08:26:10.000000 pyRFXtrx-0.8.0/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-06-01 08:26:10.000000 pyRFXtrx-0.8.0/RFXtrx/
--rw-rw-r--   0 travis    (1000) travis    (1000)    23721 2016-06-01 08:25:34.000000 pyRFXtrx-0.8.0/RFXtrx/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    67402 2016-06-01 08:25:34.000000 pyRFXtrx-0.8.0/RFXtrx/lowlevel.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-06-01 08:26:10.000000 pyRFXtrx-0.8.0/pyRFXtrx.egg-info/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1005 2016-06-01 08:26:10.000000 pyRFXtrx-0.8.0/pyRFXtrx.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (1000) travis    (1000)      360 2016-06-01 08:26:10.000000 pyRFXtrx-0.8.0/pyRFXtrx.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)        1 2016-06-01 08:26:10.000000 pyRFXtrx-0.8.0/pyRFXtrx.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)       14 2016-06-01 08:26:10.000000 pyRFXtrx-0.8.0/pyRFXtrx.egg-info/requires.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)        7 2016-06-01 08:26:10.000000 pyRFXtrx-0.8.0/pyRFXtrx.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-06-01 08:26:10.000000 pyRFXtrx-0.8.0/tests/
--rw-rw-r--   0 travis    (1000) travis    (1000)    18807 2016-06-01 08:25:34.000000 pyRFXtrx-0.8.0/tests/test_base.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1644 2016-06-01 08:25:34.000000 pyRFXtrx-0.8.0/tests/test_energy.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     8523 2016-06-01 08:25:34.000000 pyRFXtrx-0.8.0/tests/test_lights.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1713 2016-06-01 08:25:34.000000 pyRFXtrx-0.8.0/tests/test_rfy.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1038 2016-06-01 08:25:34.000000 pyRFXtrx-0.8.0/tests/test_status.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1828 2016-06-01 08:25:34.000000 pyRFXtrx-0.8.0/tests/test_temphum.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      243 2016-06-01 08:25:34.000000 pyRFXtrx-0.8.0/MANIFEST.in
--rw-rw-r--   0 travis    (1000) travis    (1000)     1457 2016-06-01 08:25:34.000000 pyRFXtrx-0.8.0/README.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     2026 2016-06-01 08:25:34.000000 pyRFXtrx-0.8.0/setup.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1005 2016-06-01 08:26:10.000000 pyRFXtrx-0.8.0/PKG-INFO
--rw-rw-r--   0 travis    (1000) travis    (1000)       87 2016-06-01 08:26:10.000000 pyRFXtrx-0.8.0/setup.cfg
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-07-11 06:52:38.000000 pyRFXtrx-0.9.0/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-07-11 06:52:38.000000 pyRFXtrx-0.9.0/RFXtrx/
+-rw-rw-r--   0 travis    (1000) travis    (1000)    24008 2016-07-11 06:51:48.000000 pyRFXtrx-0.9.0/RFXtrx/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    67533 2016-07-11 06:51:48.000000 pyRFXtrx-0.9.0/RFXtrx/lowlevel.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-07-11 06:52:38.000000 pyRFXtrx-0.9.0/pyRFXtrx.egg-info/
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1005 2016-07-11 06:52:38.000000 pyRFXtrx-0.9.0/pyRFXtrx.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (1000) travis    (1000)      360 2016-07-11 06:52:38.000000 pyRFXtrx-0.9.0/pyRFXtrx.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)        1 2016-07-11 06:52:38.000000 pyRFXtrx-0.9.0/pyRFXtrx.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)       14 2016-07-11 06:52:38.000000 pyRFXtrx-0.9.0/pyRFXtrx.egg-info/requires.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)        7 2016-07-11 06:52:38.000000 pyRFXtrx-0.9.0/pyRFXtrx.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-07-11 06:52:38.000000 pyRFXtrx-0.9.0/tests/
+-rw-rw-r--   0 travis    (1000) travis    (1000)    18809 2016-07-11 06:51:48.000000 pyRFXtrx-0.9.0/tests/test_base.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1644 2016-07-11 06:51:48.000000 pyRFXtrx-0.9.0/tests/test_energy.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     8523 2016-07-11 06:51:48.000000 pyRFXtrx-0.9.0/tests/test_lights.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1713 2016-07-11 06:51:48.000000 pyRFXtrx-0.9.0/tests/test_rfy.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1038 2016-07-11 06:51:48.000000 pyRFXtrx-0.9.0/tests/test_status.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1828 2016-07-11 06:51:48.000000 pyRFXtrx-0.9.0/tests/test_temphum.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      243 2016-07-11 06:51:48.000000 pyRFXtrx-0.9.0/MANIFEST.in
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1457 2016-07-11 06:51:48.000000 pyRFXtrx-0.9.0/README.rst
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2026 2016-07-11 06:51:48.000000 pyRFXtrx-0.9.0/setup.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1005 2016-07-11 06:52:38.000000 pyRFXtrx-0.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (1000) travis    (1000)       87 2016-07-11 06:52:38.000000 pyRFXtrx-0.9.0/setup.cfg
```

### Comparing `pyRFXtrx-0.8.0/RFXtrx/__init__.py` & `pyRFXtrx-0.9.0/RFXtrx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is part of pyRFXtrx, a Python library to communicate with
 # the RFXtrx family of devices from http://www.rfxcom.com/
-# See https://github.com/woudt/pyRFXtrx for the latest version.
+# See https://github.com/Danielhiversen/pyRFXtrx for the latest version.
 #
 # Copyright (C) 2012  Edwin Woudt <edwin@woudt.nl>
 #
 # pyRFXtrx is free software: you can redistribute it and/or modify it
 # under the terms of the GNU Lesser General Public License as published
 # by the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -160,15 +160,15 @@
             pkt = lowlevel.Lighting6()
             pkt.set_transmit(self.subtype, 0, self.id_combined, self.groupcode,
                              self.unitcode,
                              not turn_on and 0x01 or 0x00, self.cmndseqnbr)
             self.cmndseqnbr = (self.cmndseqnbr + 1) % 5
             transport.send(pkt.data)
         else:
-            raise ValueError("Unsupported packettype")
+            return
 
     def send_on(self, transport):
         """ Send an 'On' command using the given transport """
         self.send_onoff(transport, True)
 
     def send_off(self, transport):
         """ Send an 'Off' command using the given transport """
@@ -243,26 +243,31 @@
 ###############################################################################
 # get_devide method
 ###############################################################################
 
 
 def get_device(packettype, subtype, id_string):
     """ Return a device base on its identifying values """
+    # pylint: disable=too-many-return-statements
     if packettype == 0x10:  # Lighting1
         pkt = lowlevel.Lighting1()
         pkt.parse_id(subtype, id_string)
         return LightingDevice(pkt)
     elif packettype == 0x11:  # Lighting2
         pkt = lowlevel.Lighting2()
         pkt.parse_id(subtype, id_string)
         return LightingDevice(pkt)
     elif packettype == 0x12:  # Lighting3
         pkt = lowlevel.Lighting3()
         pkt.parse_id(subtype, id_string)
         return LightingDevice(pkt)
+    elif packettype == 0x13:  # Lighting4
+        pkt = lowlevel.Lighting4()
+        pkt.parse_id(subtype, id_string)
+        return LightingDevice(pkt)
     elif packettype == 0x14:  # Lighting5
         pkt = lowlevel.Lighting5()
         pkt.parse_id(subtype, id_string)
         return LightingDevice(pkt)
     elif packettype == 0x15:  # Lighting6
         pkt = lowlevel.Lighting6()
         pkt.parse_id(subtype, id_string)
@@ -348,17 +353,19 @@
 # ControlEvent class
 ###############################################################################
 
 class ControlEvent(RFXtrxEvent):
     """ Concrete class for control events """
 
     def __init__(self, pkt):
+        # pylint: disable=too-many-boolean-expressions
         if isinstance(pkt, lowlevel.Lighting1) \
                 or isinstance(pkt, lowlevel.Lighting2) \
                 or isinstance(pkt, lowlevel.Lighting3) \
+                or isinstance(pkt, lowlevel.Lighting4) \
                 or isinstance(pkt, lowlevel.Lighting5) \
                 or isinstance(pkt, lowlevel.Lighting6):
             device = LightingDevice(pkt)
         elif isinstance(pkt, lowlevel.Rfy):
             device = RfyDevice(pkt)
         else:
             device = RFXtrxDevice(pkt)
```

### Comparing `pyRFXtrx-0.8.0/RFXtrx/lowlevel.py` & `pyRFXtrx-0.9.0/RFXtrx/lowlevel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable= too-many-lines
 # This file is part of pyRFXtrx, a Python library to communicate with
 # the RFXtrx family of devices from http://www.rfxcom.com/
-# See https://github.com/woudt/pyRFXtrx for the latest version.
+# See https://github.com/Danielhiversen/pyRFXtrx for the latest version.
 #
 # Copyright (C) 2012  Edwin Woudt <edwin@woudt.nl>
 #
 # pyRFXtrx is free software: you can redistribute it and/or modify it
 # under the terms of the GNU Lesser General Public License as published
 # by the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -618,14 +618,15 @@
         self.cmd1 = None
         self.cmd2 = None
         self.cmd3 = None
         self.cmd = None
         self.pulsehigh = None
         self.pulselow = None
         self.pulse = None
+        self.cmnd_string = ""
 
     def parse_id(self, subtype, id_string):
         """Parse a string id into individual components"""
         try:
             self.packettype = 0x13
             self.subtype = subtype
             self.cmd = int(id_string, 16)
@@ -682,14 +683,16 @@
         self.id_string = "{0:06x}".format(self.cmd)
         if self.subtype in self.TYPES:
             self.type_string = self.TYPES[self.subtype]
         else:
             # Degrade nicely for yet unknown subtypes
             self.type_string = self._UNKNOWN_TYPE.format(self.packettype,
                                                          self.subtype)
+        if self.cmd is not None:
+            self.cmnd_string = "{0:#04x}".format(self.cmd)
 
 
 ###############################################################################
 # Lighting5 class
 ###############################################################################
```

### Comparing `pyRFXtrx-0.8.0/pyRFXtrx.egg-info/PKG-INFO` & `pyRFXtrx-0.9.0/pyRFXtrx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyRFXtrx
-Version: 0.8.0
+Version: 0.9.0
 Summary: a library to communicate with the RFXtrx family of devices
 Home-page: https://github.com/Danielhiversen/pyRFXtrx
 Author: Edwin Woudt
 Author-email: edwin@woudt.nl
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `pyRFXtrx-0.8.0/tests/test_base.py` & `pyRFXtrx-0.9.0/tests/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         event.device.send_off(core.transport)
         self.assertRaises(ValueError,event.device.send_dim,core.transport,50)
 
         # Lighting4, not supported yet
         bytes_array = [0x09, 0x13, 0x00, 0x2a, 0x12, 0x34, 0x56, 0x01, 0x5e, 0x70]
         event = core.transport.parse(bytes_array)
         self.assertEquals(RFXtrx.ControlEvent, type(event))
-        self.assertEquals(RFXtrx.RFXtrxDevice, type(event.device))
+        self.assertEquals(RFXtrx.LightingDevice, type(event.device))
        # event.device.send_on(core.transport)
        # event.device.send_off(core.transport)
        # self.assertRaises(ValueError,event.device.send_dim,core.transport,50)
 
         # Lighting5, subtype0
         bytes_array = bytearray(b'\x0A\x14\x00\xAD\xF3\x94\xAB\x01\x10\x00\x60')
         event = core.transport.parse(bytes_array)
```

### Comparing `pyRFXtrx-0.8.0/tests/test_energy.py` & `pyRFXtrx-0.9.0/tests/test_energy.py`

 * *Files identical despite different names*

### Comparing `pyRFXtrx-0.8.0/tests/test_lights.py` & `pyRFXtrx-0.9.0/tests/test_lights.py`

 * *Files identical despite different names*

### Comparing `pyRFXtrx-0.8.0/tests/test_rfy.py` & `pyRFXtrx-0.9.0/tests/test_rfy.py`

 * *Files identical despite different names*

### Comparing `pyRFXtrx-0.8.0/tests/test_status.py` & `pyRFXtrx-0.9.0/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `pyRFXtrx-0.8.0/tests/test_temphum.py` & `pyRFXtrx-0.9.0/tests/test_temphum.py`

 * *Files identical despite different names*

### Comparing `pyRFXtrx-0.8.0/README.rst` & `pyRFXtrx-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyRFXtrx-0.8.0/setup.py` & `pyRFXtrx-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from setuptools import setup
 
 setup(
     name = 'pyRFXtrx',
     packages = ['RFXtrx'],
     install_requires=['pyserial>=2.7'],
-    version = '0.8.0',
+    version = '0.9.0',
     description = 'a library to communicate with the RFXtrx family of devices',
     author='Edwin Woudt',
     author_email='edwin@woudt.nl',
     url='https://github.com/Danielhiversen/pyRFXtrx',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Environment :: Other Environment',
```

### Comparing `pyRFXtrx-0.8.0/PKG-INFO` & `pyRFXtrx-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyRFXtrx
-Version: 0.8.0
+Version: 0.9.0
 Summary: a library to communicate with the RFXtrx family of devices
 Home-page: https://github.com/Danielhiversen/pyRFXtrx
 Author: Edwin Woudt
 Author-email: edwin@woudt.nl
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

