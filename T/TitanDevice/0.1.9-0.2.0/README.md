# Comparing `tmp/TitanDevice-0.1.9.tar.gz` & `tmp/TitanDevice-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TitanDevice-0.1.9.tar", last modified: Tue Apr 23 10:36:19 2024, max compression
+gzip compressed data, was "TitanDevice-0.2.0.tar", last modified: Tue Apr 23 10:39:52 2024, max compression
```

## Comparing `TitanDevice-0.1.9.tar` & `TitanDevice-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 10:36:19.545328 TitanDevice-0.1.9/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 10:36:19.545328 TitanDevice-0.1.9/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.1.9/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 10:36:19.545328 TitanDevice-0.1.9/TitanDevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 10:36:19.000000 TitanDevice-0.1.9/TitanDevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-23 10:36:19.000000 TitanDevice-0.1.9/TitanDevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-23 10:36:19.000000 TitanDevice-0.1.9/TitanDevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-23 10:36:19.000000 TitanDevice-0.1.9/TitanDevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-23 10:36:19.000000 TitanDevice-0.1.9/TitanDevice.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-23 10:36:19.545328 TitanDevice-0.1.9/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-23 10:36:15.000000 TitanDevice-0.1.9/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 10:36:19.545328 TitanDevice-0.1.9/titan/
--rw-rw-r--   0 mark      (1000) mark      (1000)      704 2024-04-23 10:13:25.000000 TitanDevice-0.1.9/titan/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      358 2024-04-23 10:36:15.000000 TitanDevice-0.1.9/titan/_device_exception.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     2609 2024-04-23 10:36:15.000000 TitanDevice-0.1.9/titan/_device_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      242 2024-04-23 10:24:56.000000 TitanDevice-0.1.9/titan/_device_models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 10:39:52.305563 TitanDevice-0.2.0/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 10:39:52.305563 TitanDevice-0.2.0/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.2.0/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 10:39:52.305563 TitanDevice-0.2.0/TitanDevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-23 10:39:52.000000 TitanDevice-0.2.0/TitanDevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-23 10:39:52.000000 TitanDevice-0.2.0/TitanDevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-23 10:39:52.000000 TitanDevice-0.2.0/TitanDevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-23 10:39:52.000000 TitanDevice-0.2.0/TitanDevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-23 10:39:52.000000 TitanDevice-0.2.0/TitanDevice.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-23 10:39:52.305563 TitanDevice-0.2.0/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-23 10:39:49.000000 TitanDevice-0.2.0/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-23 10:39:52.305563 TitanDevice-0.2.0/titan/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      683 2024-04-23 10:39:33.000000 TitanDevice-0.2.0/titan/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      358 2024-04-23 10:36:15.000000 TitanDevice-0.2.0/titan/_device_exception.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2609 2024-04-23 10:36:15.000000 TitanDevice-0.2.0/titan/_device_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      242 2024-04-23 10:24:56.000000 TitanDevice-0.2.0/titan/_device_models.py
```

### Comparing `TitanDevice-0.1.9/PKG-INFO` & `TitanDevice-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.1.9/TitanDevice.egg-info/PKG-INFO` & `TitanDevice-0.2.0/TitanDevice.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TitanDevice
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `TitanDevice-0.1.9/setup.py` & `TitanDevice-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name="TitanDevice",
-    version="0.1.9",
+    version="0.2.0",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `TitanDevice-0.1.9/titan/__init__.py` & `TitanDevice-0.2.0/titan/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from titan._device_exception import DeviceNoFoundException
+from titan._device_exception import *
 from titan._device_manager import _DeviceManager
 from titan._device_models import DeviceInfo, FridaInfo
 
 device_manager_list: list[_DeviceManager] = _DeviceManager.get_all_device_manager_list()
 
 
 def get_all_devices() -> list[DeviceInfo]:
```

### Comparing `TitanDevice-0.1.9/titan/_device_manager.py` & `TitanDevice-0.2.0/titan/_device_manager.py`

 * *Files identical despite different names*

