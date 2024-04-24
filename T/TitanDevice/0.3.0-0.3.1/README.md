# Comparing `tmp/TitanDevice-0.3.0.tar.gz` & `tmp/TitanDevice-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TitanDevice-0.3.0.tar", last modified: Wed Apr 24 09:47:07 2024, max compression
+gzip compressed data, was "TitanDevice-0.3.1.tar", last modified: Wed Apr 24 10:06:41 2024, max compression
```

## Comparing `TitanDevice-0.3.0.tar` & `TitanDevice-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 09:47:07.354430 TitanDevice-0.3.0/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 09:47:07.354430 TitanDevice-0.3.0/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.3.0/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 09:47:07.354430 TitanDevice-0.3.0/TitanDevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 09:47:07.000000 TitanDevice-0.3.0/TitanDevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-24 09:47:07.000000 TitanDevice-0.3.0/TitanDevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-24 09:47:07.000000 TitanDevice-0.3.0/TitanDevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-24 09:47:07.000000 TitanDevice-0.3.0/TitanDevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-24 09:47:07.000000 TitanDevice-0.3.0/TitanDevice.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-24 09:47:07.354430 TitanDevice-0.3.0/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-24 09:47:05.000000 TitanDevice-0.3.0/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 09:47:07.354430 TitanDevice-0.3.0/titan/
--rw-rw-r--   0 mark      (1000) mark      (1000)     2114 2024-04-24 07:26:17.000000 TitanDevice-0.3.0/titan/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      841 2024-04-24 07:31:02.000000 TitanDevice-0.3.0/titan/_device_exception.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     4436 2024-04-24 09:47:05.000000 TitanDevice-0.3.0/titan/_device_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      242 2024-04-23 10:24:56.000000 TitanDevice-0.3.0/titan/_device_models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 10:06:41.173552 TitanDevice-0.3.1/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 10:06:41.173552 TitanDevice-0.3.1/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.3.1/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 10:06:41.173552 TitanDevice-0.3.1/TitanDevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 10:06:41.000000 TitanDevice-0.3.1/TitanDevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-24 10:06:41.000000 TitanDevice-0.3.1/TitanDevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-24 10:06:41.000000 TitanDevice-0.3.1/TitanDevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-24 10:06:41.000000 TitanDevice-0.3.1/TitanDevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-24 10:06:41.000000 TitanDevice-0.3.1/TitanDevice.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-24 10:06:41.173552 TitanDevice-0.3.1/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-24 10:06:39.000000 TitanDevice-0.3.1/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 10:06:41.173552 TitanDevice-0.3.1/titan/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2114 2024-04-24 07:26:17.000000 TitanDevice-0.3.1/titan/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      841 2024-04-24 07:31:02.000000 TitanDevice-0.3.1/titan/_device_exception.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4704 2024-04-24 10:06:39.000000 TitanDevice-0.3.1/titan/_device_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      242 2024-04-23 10:24:56.000000 TitanDevice-0.3.1/titan/_device_models.py
```

### Comparing `TitanDevice-0.3.0/setup.py` & `TitanDevice-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name="TitanDevice",
-    version="0.3.0",
+    version="0.3.1",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `TitanDevice-0.3.0/titan/__init__.py` & `TitanDevice-0.3.1/titan/__init__.py`

 * *Files identical despite different names*

### Comparing `TitanDevice-0.3.0/titan/_device_exception.py` & `TitanDevice-0.3.1/titan/_device_exception.py`

 * *Files identical despite different names*

### Comparing `TitanDevice-0.3.0/titan/_device_manager.py` & `TitanDevice-0.3.1/titan/_device_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os.path
 import subprocess
+import time
 from typing import Optional
 
 from adbutils import adb, adb_path
 
 from titan._device_exception import DeviceNoFoundException, DeviceMustBeRootedException, \
     FridaServerNotInstalled, FridaServerNotRunning
 from titan._device_models import DeviceInfo, FridaInfo
@@ -93,26 +94,32 @@
             version=self.__get_frida_version(frida_server_path)
         )
 
     @check_is_root
     def start_frida(self, frida_server_path):
         if not self.__is_frida_installed(frida_server_path):
             raise FridaServerNotInstalled(self._serial, frida_server_path)
-        subprocess.Popen(
-            [adb_path(), '-s', self._serial, 'shell', 'nohup',
-             'su -c "{}" &'.format(frida_server_path)]
-        )
+        while self.__is_frida_running(
+                self.get_frida_server_name_from_path(frida_server_path)
+        ):
+            subprocess.Popen(
+                [adb_path(), '-s', self._serial, 'shell', 'nohup',
+                 'su -c "{}" &'.format(frida_server_path)]
+            )
+            time.sleep(0.1)
         return self.get_frida_info(frida_server_path)
 
     @check_is_root
     def stop_frida(self, frida_server_path):
         frida_server_name = self.get_frida_server_name_from_path(frida_server_path)
         if not self.__is_frida_running(frida_server_name):
             raise FridaServerNotRunning(self._serial, frida_server_name)
-        self._device.shell(f"su -c pkill {frida_server_name}")
+        while self.__is_frida_running(frida_server_name):
+            self._device.shell(f"su -c pkill {frida_server_name}")
+            time.sleep(0.1)
         return self.get_frida_info(frida_server_path)
 
     @check_is_root
     def uninstall_frida(self, frida_server_path):
         if not self.__is_frida_installed(frida_server_path):
             raise FridaServerNotInstalled(self._serial, frida_server_path)
         self._device.shell(f"su -c rm {frida_server_path}")
```

