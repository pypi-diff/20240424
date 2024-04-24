# Comparing `tmp/TitanDevice-0.2.2.tar.gz` & `tmp/TitanDevice-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TitanDevice-0.2.2.tar", last modified: Wed Apr 24 06:47:03 2024, max compression
+gzip compressed data, was "TitanDevice-0.2.3.tar", last modified: Wed Apr 24 06:51:44 2024, max compression
```

## Comparing `TitanDevice-0.2.2.tar` & `TitanDevice-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 06:47:03.460250 TitanDevice-0.2.2/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 06:47:03.460250 TitanDevice-0.2.2/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.2.2/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 06:47:03.460250 TitanDevice-0.2.2/TitanDevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 06:47:03.000000 TitanDevice-0.2.2/TitanDevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-24 06:47:03.000000 TitanDevice-0.2.2/TitanDevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-24 06:47:03.000000 TitanDevice-0.2.2/TitanDevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-24 06:47:03.000000 TitanDevice-0.2.2/TitanDevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-24 06:47:03.000000 TitanDevice-0.2.2/TitanDevice.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-24 06:47:03.460250 TitanDevice-0.2.2/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-24 06:43:29.000000 TitanDevice-0.2.2/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 06:47:03.460250 TitanDevice-0.2.2/titan/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1482 2024-04-24 06:43:29.000000 TitanDevice-0.2.2/titan/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      602 2024-04-24 06:43:29.000000 TitanDevice-0.2.2/titan/_device_exception.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3467 2024-04-24 06:43:29.000000 TitanDevice-0.2.2/titan/_device_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      242 2024-04-23 10:24:56.000000 TitanDevice-0.2.2/titan/_device_models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 06:51:44.842566 TitanDevice-0.2.3/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 06:51:44.842566 TitanDevice-0.2.3/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.2.3/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 06:51:44.842566 TitanDevice-0.2.3/TitanDevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 06:51:44.000000 TitanDevice-0.2.3/TitanDevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-24 06:51:44.000000 TitanDevice-0.2.3/TitanDevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-24 06:51:44.000000 TitanDevice-0.2.3/TitanDevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-24 06:51:44.000000 TitanDevice-0.2.3/TitanDevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-24 06:51:44.000000 TitanDevice-0.2.3/TitanDevice.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-24 06:51:44.842566 TitanDevice-0.2.3/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-24 06:51:39.000000 TitanDevice-0.2.3/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 06:51:44.842566 TitanDevice-0.2.3/titan/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1488 2024-04-24 06:51:39.000000 TitanDevice-0.2.3/titan/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      602 2024-04-24 06:43:29.000000 TitanDevice-0.2.3/titan/_device_exception.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3618 2024-04-24 06:51:39.000000 TitanDevice-0.2.3/titan/_device_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      242 2024-04-23 10:24:56.000000 TitanDevice-0.2.3/titan/_device_models.py
```

### Comparing `TitanDevice-0.2.2/PKG-INFO` & `TitanDevice-0.2.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.2.2/TitanDevice.egg-info/PKG-INFO` & `TitanDevice-0.2.3/TitanDevice.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.2.2/setup.py` & `TitanDevice-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name="TitanDevice",
-    version="0.2.2",
+    version="0.2.3",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `TitanDevice-0.2.2/titan/_device_exception.py` & `TitanDevice-0.2.3/titan/_device_exception.py`

 * *Files identical despite different names*

### Comparing `TitanDevice-0.2.2/titan/_device_manager.py` & `TitanDevice-0.2.3/titan/_device_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os.path
 from typing import Optional
 
 from adbutils import adb
 
 from titan._device_exception import DeviceNoFoundException, DeviceMustBeRootedException, \
     FridaServerNotInstalled
 from titan._device_models import DeviceInfo, FridaInfo
@@ -76,23 +77,25 @@
         self._device.push(file_path, dist_path)
         self._device.shell(f"su -c chmod 755 {dist_path}")
         self._device.shell(f"su -c {dist_path} &")
         self._frida_info = None
         return self.get_frida_info()
 
     @check_is_root
-    def get_frida_info(self, frida_server_name, frida_server_path) -> FridaInfo:
+    def get_frida_info(self, frida_server_path, frida_server_name=None) -> FridaInfo:
         if self._frida_info is None:
+            if frida_server_name is None:
+                frida_server_name = os.path.basename(frida_server_path)
             self._frida_info = FridaInfo(
                 is_running=self.__is_frida_running(frida_server_name),
                 is_installed=self.__is_frida_installed(frida_server_path),
                 version=self.__get_frida_version(frida_server_path)
             )
         return self._frida_info
 
     @check_is_root
     def start_frida(self, frida_server_path):
         if not self.__is_frida_installed(frida_server_path):
             raise FridaServerNotInstalled(self._serial, frida_server_path)
         self._device.shell(f"su -c {frida_server_path} &")
         self._frida_info = None
-        return self.get_frida_info()
+        return self.get_frida_info(frida_server_path)
```

