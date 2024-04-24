# Comparing `tmp/TitanDevice-0.2.5.tar.gz` & `tmp/TitanDevice-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TitanDevice-0.2.5.tar", last modified: Wed Apr 24 07:20:34 2024, max compression
+gzip compressed data, was "TitanDevice-0.2.6.tar", last modified: Wed Apr 24 07:26:20 2024, max compression
```

## Comparing `TitanDevice-0.2.5.tar` & `TitanDevice-0.2.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 07:20:34.813780 TitanDevice-0.2.5/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 07:20:34.813780 TitanDevice-0.2.5/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.2.5/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 07:20:34.813780 TitanDevice-0.2.5/TitanDevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 07:20:34.000000 TitanDevice-0.2.5/TitanDevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-24 07:20:34.000000 TitanDevice-0.2.5/TitanDevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-24 07:20:34.000000 TitanDevice-0.2.5/TitanDevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-24 07:20:34.000000 TitanDevice-0.2.5/TitanDevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-24 07:20:34.000000 TitanDevice-0.2.5/TitanDevice.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-24 07:20:34.813780 TitanDevice-0.2.5/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-24 07:20:32.000000 TitanDevice-0.2.5/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 07:20:34.813780 TitanDevice-0.2.5/titan/
--rw-rw-r--   0 mark      (1000) mark      (1000)     2098 2024-04-24 07:19:04.000000 TitanDevice-0.2.5/titan/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      602 2024-04-24 06:43:29.000000 TitanDevice-0.2.5/titan/_device_exception.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3733 2024-04-24 07:20:32.000000 TitanDevice-0.2.5/titan/_device_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      242 2024-04-23 10:24:56.000000 TitanDevice-0.2.5/titan/_device_models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 07:26:20.455047 TitanDevice-0.2.6/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 07:26:20.455047 TitanDevice-0.2.6/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.2.6/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 07:26:20.455047 TitanDevice-0.2.6/TitanDevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 07:26:20.000000 TitanDevice-0.2.6/TitanDevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-24 07:26:20.000000 TitanDevice-0.2.6/TitanDevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-24 07:26:20.000000 TitanDevice-0.2.6/TitanDevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-24 07:26:20.000000 TitanDevice-0.2.6/TitanDevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-24 07:26:20.000000 TitanDevice-0.2.6/TitanDevice.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-24 07:26:20.455047 TitanDevice-0.2.6/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-24 07:26:17.000000 TitanDevice-0.2.6/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 07:26:20.455047 TitanDevice-0.2.6/titan/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2114 2024-04-24 07:26:17.000000 TitanDevice-0.2.6/titan/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      602 2024-04-24 06:43:29.000000 TitanDevice-0.2.6/titan/_device_exception.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4022 2024-04-24 07:26:17.000000 TitanDevice-0.2.6/titan/_device_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      242 2024-04-23 10:24:56.000000 TitanDevice-0.2.6/titan/_device_models.py
```

### Comparing `TitanDevice-0.2.5/PKG-INFO` & `TitanDevice-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.2.5/TitanDevice.egg-info/PKG-INFO` & `TitanDevice-0.2.6/TitanDevice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.2.5/setup.py` & `TitanDevice-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name="TitanDevice",
-    version="0.2.5",
+    version="0.2.6",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `TitanDevice-0.2.5/titan/__init__.py` & `TitanDevice-0.2.6/titan/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,19 +38,19 @@
     for device in device_manager_list:
         if device.get_info().serial == device_serial:
             return device.start_frida(frida_server_path)
     raise DeviceNoFoundException(device_serial)
 
 
 def stop_frida(
-        device_serial: str, frida_server_name='frida-server'
+        device_serial: str, frida_server_path='/data/local/tmp/frida-server'
 ) -> FridaInfo:
     for device in device_manager_list:
         if device.get_info().serial == device_serial:
-            return device.stop_frida(frida_server_name)
+            return device.stop_frida(frida_server_path)
     raise DeviceNoFoundException(device_serial)
 
 
 def uninstall_frida(
         device_serial: str, frida_server_path='/data/local/tmp/frida-server'
 ) -> FridaInfo:
     for device in device_manager_list:
```

### Comparing `TitanDevice-0.2.5/titan/_device_exception.py` & `TitanDevice-0.2.6/titan/_device_exception.py`

 * *Files identical despite different names*

### Comparing `TitanDevice-0.2.5/titan/_device_manager.py` & `TitanDevice-0.2.6/titan/_device_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,14 +33,18 @@
     @staticmethod
     def get_all_device_manager_list() -> list["_DeviceManager"]:
         return [
             _DeviceManager(device.serial)
             for device in adb.device_list()
         ]
 
+    @staticmethod
+    def get_frida_server_name_from_path(frida_server_path: str) -> str:
+        return os.path.basename(frida_server_path)
+
     def __is_frida_running(self, frida_server_name) -> bool:
         return self._device.shell(f"pgrep {frida_server_name}").strip() != ""
 
     def __is_frida_installed(self, frida_server_path) -> bool:
         return self.__file_exists(frida_server_path)
 
     def __get_frida_version(self, frida_server_path) -> str | None:
@@ -72,35 +76,36 @@
         return self._device_info
 
     @check_is_root
     def install_frida(self, file_path, dist_path):
         self._device.push(file_path, dist_path)
         self._device.shell(f"su -c chmod 755 {dist_path}")
         self._device.shell(f"su -c {dist_path} &")
-        return self.get_frida_info()
+        return self.get_frida_info(dist_path)
 
     @check_is_root
     def get_frida_info(self, frida_server_path, frida_server_name=None) -> FridaInfo:
         if frida_server_name is None:
-            frida_server_name = os.path.basename(frida_server_path)
+            frida_server_name = self.get_frida_server_name_from_path(frida_server_path)
         return FridaInfo(
             is_running=self.__is_frida_running(frida_server_name),
             is_installed=self.__is_frida_installed(frida_server_path),
             version=self.__get_frida_version(frida_server_path)
         )
 
     @check_is_root
     def start_frida(self, frida_server_path):
         if not self.__is_frida_installed(frida_server_path):
             raise FridaServerNotInstalled(self._serial, frida_server_path)
         self._device.shell(f"su -c {frida_server_path} &")
         return self.get_frida_info(frida_server_path)
 
     @check_is_root
-    def stop_frida(self, frida_server_name):
+    def stop_frida(self, frida_server_path):
+        frida_server_name = self.get_frida_server_name_from_path(frida_server_path)
         self._device.shell(f"su -c pkill {frida_server_name}")
-        return self.get_frida_info()
+        return self.get_frida_info(frida_server_path)
 
     @check_is_root
     def uninstall_frida(self, frida_server_path):
         self._device.shell(f"su -c rm {frida_server_path}")
-        return self.get_frida_info()
+        return self.get_frida_info(frida_server_path)
```

