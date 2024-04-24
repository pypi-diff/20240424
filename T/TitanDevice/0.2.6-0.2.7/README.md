# Comparing `tmp/TitanDevice-0.2.6.tar.gz` & `tmp/TitanDevice-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TitanDevice-0.2.6.tar", last modified: Wed Apr 24 07:26:20 2024, max compression
+gzip compressed data, was "TitanDevice-0.2.7.tar", last modified: Wed Apr 24 07:31:04 2024, max compression
```

## Comparing `TitanDevice-0.2.6.tar` & `TitanDevice-0.2.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 07:26:20.455047 TitanDevice-0.2.6/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 07:26:20.455047 TitanDevice-0.2.6/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.2.6/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 07:26:20.455047 TitanDevice-0.2.6/TitanDevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 07:26:20.000000 TitanDevice-0.2.6/TitanDevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-24 07:26:20.000000 TitanDevice-0.2.6/TitanDevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-24 07:26:20.000000 TitanDevice-0.2.6/TitanDevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-24 07:26:20.000000 TitanDevice-0.2.6/TitanDevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-24 07:26:20.000000 TitanDevice-0.2.6/TitanDevice.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-24 07:26:20.455047 TitanDevice-0.2.6/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-24 07:26:17.000000 TitanDevice-0.2.6/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 07:26:20.455047 TitanDevice-0.2.6/titan/
--rw-rw-r--   0 mark      (1000) mark      (1000)     2114 2024-04-24 07:26:17.000000 TitanDevice-0.2.6/titan/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      602 2024-04-24 06:43:29.000000 TitanDevice-0.2.6/titan/_device_exception.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     4022 2024-04-24 07:26:17.000000 TitanDevice-0.2.6/titan/_device_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      242 2024-04-23 10:24:56.000000 TitanDevice-0.2.6/titan/_device_models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 07:31:04.481697 TitanDevice-0.2.7/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 07:31:04.481697 TitanDevice-0.2.7/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.2.7/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 07:31:04.477697 TitanDevice-0.2.7/TitanDevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 07:31:04.000000 TitanDevice-0.2.7/TitanDevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-24 07:31:04.000000 TitanDevice-0.2.7/TitanDevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-24 07:31:04.000000 TitanDevice-0.2.7/TitanDevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-24 07:31:04.000000 TitanDevice-0.2.7/TitanDevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-24 07:31:04.000000 TitanDevice-0.2.7/TitanDevice.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-24 07:31:04.481697 TitanDevice-0.2.7/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-24 07:31:02.000000 TitanDevice-0.2.7/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 07:31:04.477697 TitanDevice-0.2.7/titan/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2114 2024-04-24 07:26:17.000000 TitanDevice-0.2.7/titan/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      841 2024-04-24 07:31:02.000000 TitanDevice-0.2.7/titan/_device_exception.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4313 2024-04-24 07:31:02.000000 TitanDevice-0.2.7/titan/_device_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      242 2024-04-23 10:24:56.000000 TitanDevice-0.2.7/titan/_device_models.py
```

### Comparing `TitanDevice-0.2.6/PKG-INFO` & `TitanDevice-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.2.6/TitanDevice.egg-info/PKG-INFO` & `TitanDevice-0.2.7/TitanDevice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.2.6/setup.py` & `TitanDevice-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name="TitanDevice",
-    version="0.2.6",
+    version="0.2.7",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `TitanDevice-0.2.6/titan/__init__.py` & `TitanDevice-0.2.7/titan/__init__.py`

 * *Files identical despite different names*

### Comparing `TitanDevice-0.2.6/titan/_device_exception.py` & `TitanDevice-0.2.7/titan/_device_exception.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,7 +11,14 @@
 
 
 class FridaServerNotInstalled(Exception):
     def __init__(self, device_serial, frida_server_path):
         super().__init__(
             f'Frida server is not installed in {frida_server_path} on device with serial {device_serial}'
         )
+
+
+class FridaServerNotRunning(Exception):
+    def __init__(self, device_serial, frida_server_name):
+        super().__init__(
+            f'Frida server [{frida_server_name}] is not running on device with serial {device_serial}'
+        )
```

### Comparing `TitanDevice-0.2.6/titan/_device_manager.py` & `TitanDevice-0.2.7/titan/_device_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os.path
 from typing import Optional
 
 from adbutils import adb
 
 from titan._device_exception import DeviceNoFoundException, DeviceMustBeRootedException, \
-    FridaServerNotInstalled
+    FridaServerNotInstalled, FridaServerNotRunning
 from titan._device_models import DeviceInfo, FridaInfo
 
 
 class _DeviceManager(object):
     _device: adb.device
     _serial: str
     _is_root: bool = False
@@ -98,14 +98,18 @@
             raise FridaServerNotInstalled(self._serial, frida_server_path)
         self._device.shell(f"su -c {frida_server_path} &")
         return self.get_frida_info(frida_server_path)
 
     @check_is_root
     def stop_frida(self, frida_server_path):
         frida_server_name = self.get_frida_server_name_from_path(frida_server_path)
+        if not self.__is_frida_running(frida_server_name):
+            raise FridaServerNotRunning(self._serial, frida_server_name)
         self._device.shell(f"su -c pkill {frida_server_name}")
         return self.get_frida_info(frida_server_path)
 
     @check_is_root
     def uninstall_frida(self, frida_server_path):
+        if not self.__is_frida_installed(frida_server_path):
+            raise FridaServerNotInstalled(self._serial, frida_server_path)
         self._device.shell(f"su -c rm {frida_server_path}")
         return self.get_frida_info(frida_server_path)
```

