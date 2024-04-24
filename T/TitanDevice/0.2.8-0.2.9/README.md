# Comparing `tmp/TitanDevice-0.2.8.tar.gz` & `tmp/TitanDevice-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TitanDevice-0.2.8.tar", last modified: Wed Apr 24 08:47:35 2024, max compression
+gzip compressed data, was "TitanDevice-0.2.9.tar", last modified: Wed Apr 24 08:53:25 2024, max compression
```

## Comparing `TitanDevice-0.2.8.tar` & `TitanDevice-0.2.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 08:47:35.707024 TitanDevice-0.2.8/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 08:47:35.707024 TitanDevice-0.2.8/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.2.8/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 08:47:35.707024 TitanDevice-0.2.8/TitanDevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 08:47:35.000000 TitanDevice-0.2.8/TitanDevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-24 08:47:35.000000 TitanDevice-0.2.8/TitanDevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-24 08:47:35.000000 TitanDevice-0.2.8/TitanDevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-24 08:47:35.000000 TitanDevice-0.2.8/TitanDevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-24 08:47:35.000000 TitanDevice-0.2.8/TitanDevice.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-24 08:47:35.707024 TitanDevice-0.2.8/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-24 08:47:33.000000 TitanDevice-0.2.8/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 08:47:35.707024 TitanDevice-0.2.8/titan/
--rw-rw-r--   0 mark      (1000) mark      (1000)     2114 2024-04-24 07:26:17.000000 TitanDevice-0.2.8/titan/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      841 2024-04-24 07:31:02.000000 TitanDevice-0.2.8/titan/_device_exception.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     4450 2024-04-24 08:47:34.000000 TitanDevice-0.2.8/titan/_device_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      242 2024-04-23 10:24:56.000000 TitanDevice-0.2.8/titan/_device_models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 08:53:25.348823 TitanDevice-0.2.9/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 08:53:25.348823 TitanDevice-0.2.9/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.2.9/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 08:53:25.348823 TitanDevice-0.2.9/TitanDevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 08:53:25.000000 TitanDevice-0.2.9/TitanDevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-24 08:53:25.000000 TitanDevice-0.2.9/TitanDevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-24 08:53:25.000000 TitanDevice-0.2.9/TitanDevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-24 08:53:25.000000 TitanDevice-0.2.9/TitanDevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-24 08:53:25.000000 TitanDevice-0.2.9/TitanDevice.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-24 08:53:25.348823 TitanDevice-0.2.9/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-24 08:53:23.000000 TitanDevice-0.2.9/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 08:53:25.348823 TitanDevice-0.2.9/titan/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2114 2024-04-24 07:26:17.000000 TitanDevice-0.2.9/titan/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      841 2024-04-24 07:31:02.000000 TitanDevice-0.2.9/titan/_device_exception.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4527 2024-04-24 08:53:23.000000 TitanDevice-0.2.9/titan/_device_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      242 2024-04-23 10:24:56.000000 TitanDevice-0.2.9/titan/_device_models.py
```

### Comparing `TitanDevice-0.2.8/PKG-INFO` & `TitanDevice-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.2.8
+Version: 0.2.9
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.2.8/TitanDevice.egg-info/PKG-INFO` & `TitanDevice-0.2.9/TitanDevice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.2.8
+Version: 0.2.9
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.2.8/setup.py` & `TitanDevice-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name="TitanDevice",
-    version="0.2.8",
+    version="0.2.9",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `TitanDevice-0.2.8/titan/__init__.py` & `TitanDevice-0.2.9/titan/__init__.py`

 * *Files identical despite different names*

### Comparing `TitanDevice-0.2.8/titan/_device_exception.py` & `TitanDevice-0.2.9/titan/_device_exception.py`

 * *Files identical despite different names*

### Comparing `TitanDevice-0.2.8/titan/_device_manager.py` & `TitanDevice-0.2.9/titan/_device_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -93,16 +93,18 @@
             version=self.__get_frida_version(frida_server_path)
         )
 
     @check_is_root
     def start_frida(self, frida_server_path):
         if not self.__is_frida_installed(frida_server_path):
             raise FridaServerNotInstalled(self._serial, frida_server_path)
+        adb_path = subprocess.run(['which', 'adb'])
         subprocess.run(
-            ['adb', '-s', self._serial, 'shell', 'su -c', frida_server_path, '&']
+            [adb_path, '-s', self._serial, 'shell', 'su -c', 'nohup', frida_server_path,
+             '&']
         )
         # self._device.shell(f"su -c {frida_server_path} &")
 
         return self.get_frida_info(frida_server_path)
 
     @check_is_root
     def stop_frida(self, frida_server_path):
```

