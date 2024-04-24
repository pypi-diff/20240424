# Comparing `tmp/TitanDevice-0.2.4.tar.gz` & `tmp/TitanDevice-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TitanDevice-0.2.4.tar", last modified: Wed Apr 24 07:16:33 2024, max compression
+gzip compressed data, was "TitanDevice-0.2.5.tar", last modified: Wed Apr 24 07:20:34 2024, max compression
```

## Comparing `TitanDevice-0.2.4.tar` & `TitanDevice-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 07:16:33.943131 TitanDevice-0.2.4/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 07:16:33.943131 TitanDevice-0.2.4/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.2.4/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 07:16:33.943131 TitanDevice-0.2.4/TitanDevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 07:16:33.000000 TitanDevice-0.2.4/TitanDevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-24 07:16:33.000000 TitanDevice-0.2.4/TitanDevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-24 07:16:33.000000 TitanDevice-0.2.4/TitanDevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-24 07:16:33.000000 TitanDevice-0.2.4/TitanDevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-24 07:16:33.000000 TitanDevice-0.2.4/TitanDevice.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-24 07:16:33.943131 TitanDevice-0.2.4/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-24 07:16:31.000000 TitanDevice-0.2.4/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 07:16:33.943131 TitanDevice-0.2.4/titan/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1488 2024-04-24 06:51:39.000000 TitanDevice-0.2.4/titan/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      602 2024-04-24 06:43:29.000000 TitanDevice-0.2.4/titan/_device_exception.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3401 2024-04-24 07:16:31.000000 TitanDevice-0.2.4/titan/_device_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      242 2024-04-23 10:24:56.000000 TitanDevice-0.2.4/titan/_device_models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 07:20:34.813780 TitanDevice-0.2.5/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 07:20:34.813780 TitanDevice-0.2.5/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.2.5/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 07:20:34.813780 TitanDevice-0.2.5/TitanDevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 07:20:34.000000 TitanDevice-0.2.5/TitanDevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-24 07:20:34.000000 TitanDevice-0.2.5/TitanDevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-24 07:20:34.000000 TitanDevice-0.2.5/TitanDevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-24 07:20:34.000000 TitanDevice-0.2.5/TitanDevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-24 07:20:34.000000 TitanDevice-0.2.5/TitanDevice.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-24 07:20:34.813780 TitanDevice-0.2.5/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-24 07:20:32.000000 TitanDevice-0.2.5/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 07:20:34.813780 TitanDevice-0.2.5/titan/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2098 2024-04-24 07:19:04.000000 TitanDevice-0.2.5/titan/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      602 2024-04-24 06:43:29.000000 TitanDevice-0.2.5/titan/_device_exception.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3733 2024-04-24 07:20:32.000000 TitanDevice-0.2.5/titan/_device_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      242 2024-04-23 10:24:56.000000 TitanDevice-0.2.5/titan/_device_models.py
```

### Comparing `TitanDevice-0.2.4/PKG-INFO` & `TitanDevice-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.2.4/TitanDevice.egg-info/PKG-INFO` & `TitanDevice-0.2.5/TitanDevice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.2.4/setup.py` & `TitanDevice-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name="TitanDevice",
-    version="0.2.4",
+    version="0.2.5",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `TitanDevice-0.2.4/titan/__init__.py` & `TitanDevice-0.2.5/titan/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,7 +35,25 @@
 def start_frida(
         device_serial: str, frida_server_path='/data/local/tmp/frida-server'
 ) -> FridaInfo:
     for device in device_manager_list:
         if device.get_info().serial == device_serial:
             return device.start_frida(frida_server_path)
     raise DeviceNoFoundException(device_serial)
+
+
+def stop_frida(
+        device_serial: str, frida_server_name='frida-server'
+) -> FridaInfo:
+    for device in device_manager_list:
+        if device.get_info().serial == device_serial:
+            return device.stop_frida(frida_server_name)
+    raise DeviceNoFoundException(device_serial)
+
+
+def uninstall_frida(
+        device_serial: str, frida_server_path='/data/local/tmp/frida-server'
+) -> FridaInfo:
+    for device in device_manager_list:
+        if device.get_info().serial == device_serial:
+            return device.uninstall_frida(frida_server_path)
+    raise DeviceNoFoundException(device_serial)
```

### Comparing `TitanDevice-0.2.4/titan/_device_exception.py` & `TitanDevice-0.2.5/titan/_device_exception.py`

 * *Files identical despite different names*

### Comparing `TitanDevice-0.2.4/titan/_device_manager.py` & `TitanDevice-0.2.5/titan/_device_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -90,7 +90,17 @@
 
     @check_is_root
     def start_frida(self, frida_server_path):
         if not self.__is_frida_installed(frida_server_path):
             raise FridaServerNotInstalled(self._serial, frida_server_path)
         self._device.shell(f"su -c {frida_server_path} &")
         return self.get_frida_info(frida_server_path)
+
+    @check_is_root
+    def stop_frida(self, frida_server_name):
+        self._device.shell(f"su -c pkill {frida_server_name}")
+        return self.get_frida_info()
+
+    @check_is_root
+    def uninstall_frida(self, frida_server_path):
+        self._device.shell(f"su -c rm {frida_server_path}")
+        return self.get_frida_info()
```

