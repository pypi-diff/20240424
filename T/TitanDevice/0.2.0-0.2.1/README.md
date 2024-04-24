# Comparing `tmp/TitanDevice-0.2.0.tar.gz` & `tmp/TitanDevice-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TitanDevice-0.2.0.tar", last modified: Tue Apr 23 10:39:52 2024, max compression
+gzip compressed data, was "TitanDevice-0.2.1.tar", last modified: Wed Apr 24 06:24:17 2024, max compression
```

## Comparing `TitanDevice-0.2.0.tar` & `TitanDevice-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 10:39:52.305563 TitanDevice-0.2.0/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 10:39:52.305563 TitanDevice-0.2.0/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.2.0/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 10:39:52.305563 TitanDevice-0.2.0/TitanDevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 10:39:52.000000 TitanDevice-0.2.0/TitanDevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-23 10:39:52.000000 TitanDevice-0.2.0/TitanDevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-23 10:39:52.000000 TitanDevice-0.2.0/TitanDevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-23 10:39:52.000000 TitanDevice-0.2.0/TitanDevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-23 10:39:52.000000 TitanDevice-0.2.0/TitanDevice.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-23 10:39:52.305563 TitanDevice-0.2.0/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-23 10:39:49.000000 TitanDevice-0.2.0/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 10:39:52.305563 TitanDevice-0.2.0/titan/
--rw-rw-r--   0 mark      (1000) mark      (1000)      683 2024-04-23 10:39:33.000000 TitanDevice-0.2.0/titan/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      358 2024-04-23 10:36:15.000000 TitanDevice-0.2.0/titan/_device_exception.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     2609 2024-04-23 10:36:15.000000 TitanDevice-0.2.0/titan/_device_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      242 2024-04-23 10:24:56.000000 TitanDevice-0.2.0/titan/_device_models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 06:24:17.830801 TitanDevice-0.2.1/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 06:24:17.830801 TitanDevice-0.2.1/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.2.1/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 06:24:17.830801 TitanDevice-0.2.1/TitanDevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 06:24:17.000000 TitanDevice-0.2.1/TitanDevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-24 06:24:17.000000 TitanDevice-0.2.1/TitanDevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-24 06:24:17.000000 TitanDevice-0.2.1/TitanDevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-24 06:24:17.000000 TitanDevice-0.2.1/TitanDevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-24 06:24:17.000000 TitanDevice-0.2.1/TitanDevice.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-24 06:24:17.830801 TitanDevice-0.2.1/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-24 06:24:11.000000 TitanDevice-0.2.1/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 06:24:17.830801 TitanDevice-0.2.1/titan/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1032 2024-04-24 06:22:19.000000 TitanDevice-0.2.1/titan/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      358 2024-04-23 10:36:15.000000 TitanDevice-0.2.1/titan/_device_exception.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2972 2024-04-24 06:24:11.000000 TitanDevice-0.2.1/titan/_device_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      242 2024-04-23 10:24:56.000000 TitanDevice-0.2.1/titan/_device_models.py
```

### Comparing `TitanDevice-0.2.0/PKG-INFO` & `TitanDevice-0.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.2.0/TitanDevice.egg-info/PKG-INFO` & `TitanDevice-0.2.1/TitanDevice.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.2.0/setup.py` & `TitanDevice-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name="TitanDevice",
-    version="0.2.0",
+    version="0.2.1",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `TitanDevice-0.2.0/titan/__init__.py` & `TitanDevice-0.2.1/titan/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,7 +12,17 @@
 
 
 def get_frida_info(device_serial: str) -> FridaInfo:
     for device in device_manager_list:
         if device.get_info().serial == device_serial:
             return device.get_frida_info()
     raise DeviceNoFoundException(device_serial)
+
+
+def install_frida(
+        device_serial: str, frida_server_path: str,
+        dist_path='/data/local/tmp/frida-server'
+) -> FridaInfo:
+    for device in device_manager_list:
+        if device.get_info().serial == device_serial:
+            return device.install_frida(frida_server_path, dist_path)
+    raise DeviceNoFoundException(device_serial)
```

### Comparing `TitanDevice-0.2.0/titan/_device_manager.py` & `TitanDevice-0.2.1/titan/_device_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+from typing import Optional
+
 from adbutils import adb
 
 from titan._device_exception import DeviceNoFoundException, DeviceMustBeRootedException
 from titan._device_models import DeviceInfo, FridaInfo
 
 
 class _DeviceManager(object):
     _device: adb.device
     _serial: str
     _is_root: bool = False
-    _device_info: DeviceInfo = None
-    _frida_info: FridaInfo = None
+    _device_info: Optional[DeviceInfo] = None
+    _frida_info: Optional[FridaInfo] = None
 
     @staticmethod
     def check_is_root(func):
         def wrapper(self, *args, **kwargs):
             if not self._is_root:
                 raise DeviceMustBeRootedException(self._serial)
             return func(self, *args, **kwargs)
@@ -30,35 +32,14 @@
     @staticmethod
     def get_all_device_manager_list() -> list["_DeviceManager"]:
         return [
             _DeviceManager(device.serial)
             for device in adb.device_list()
         ]
 
-    def get_info(self) -> DeviceInfo:
-        if self._device_info is None:
-            self._device_info = DeviceInfo(
-                serial=self._device.serial,
-                product=self._device.prop.name,
-                model=self._device.prop.model,
-                device=self._device.prop.device,
-                is_root=self._is_root,
-            )
-        return self._device_info
-
-    @check_is_root
-    def get_frida_info(self) -> FridaInfo:
-        if self._frida_info is None:
-            self._frida_info = FridaInfo(
-                is_running=self.__is_frida_running(),
-                is_installed=self.__is_frida_installed(),
-                version=self.__get_frida_version()
-            )
-        return self._frida_info
-
     def __is_frida_running(self) -> bool:
         return self._device.shell("pgrep frida-server").strip() != ""
 
     def __is_frida_installed(self) -> bool:
         return self.__file_exists("/data/local/tmp/frida-server")
 
     def __get_frida_version(self) -> str | None:
@@ -73,7 +54,36 @@
             f"ls {path}"
         ).strip()
 
     def __is_root(self):
         return self.__file_exists("/system/xbin/su") or self.__file_exists(
             "/system/bin/su"
         )
+
+    def get_info(self) -> DeviceInfo:
+        if self._device_info is None:
+            self._device_info = DeviceInfo(
+                serial=self._device.serial,
+                product=self._device.prop.name,
+                model=self._device.prop.model,
+                device=self._device.prop.device,
+                is_root=self._is_root,
+            )
+        return self._device_info
+
+    @check_is_root
+    def install_frida(self, frida_server_path, dist_path):
+        self._device.push(frida_server_path, dist_path)
+        self._device.shell(f"su -c chmod 755 {dist_path}")
+        self._device.shell(f"su -c {dist_path} &")
+        self._frida_info = None
+        return self.get_frida_info()
+
+    @check_is_root
+    def get_frida_info(self) -> FridaInfo:
+        if self._frida_info is None:
+            self._frida_info = FridaInfo(
+                is_running=self.__is_frida_running(),
+                is_installed=self.__is_frida_installed(),
+                version=self.__get_frida_version()
+            )
+        return self._frida_info
```

