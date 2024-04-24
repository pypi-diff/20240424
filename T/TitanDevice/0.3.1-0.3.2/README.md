# Comparing `tmp/TitanDevice-0.3.1.tar.gz` & `tmp/TitanDevice-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TitanDevice-0.3.1.tar", last modified: Wed Apr 24 10:06:41 2024, max compression
+gzip compressed data, was "TitanDevice-0.3.2.tar", last modified: Wed Apr 24 10:08:51 2024, max compression
```

## Comparing `TitanDevice-0.3.1.tar` & `TitanDevice-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 10:06:41.173552 TitanDevice-0.3.1/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 10:06:41.173552 TitanDevice-0.3.1/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.3.1/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 10:06:41.173552 TitanDevice-0.3.1/TitanDevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 10:06:41.000000 TitanDevice-0.3.1/TitanDevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-24 10:06:41.000000 TitanDevice-0.3.1/TitanDevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-24 10:06:41.000000 TitanDevice-0.3.1/TitanDevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-24 10:06:41.000000 TitanDevice-0.3.1/TitanDevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-24 10:06:41.000000 TitanDevice-0.3.1/TitanDevice.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-24 10:06:41.173552 TitanDevice-0.3.1/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-24 10:06:39.000000 TitanDevice-0.3.1/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 10:06:41.173552 TitanDevice-0.3.1/titan/
--rw-rw-r--   0 mark      (1000) mark      (1000)     2114 2024-04-24 07:26:17.000000 TitanDevice-0.3.1/titan/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      841 2024-04-24 07:31:02.000000 TitanDevice-0.3.1/titan/_device_exception.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     4704 2024-04-24 10:06:39.000000 TitanDevice-0.3.1/titan/_device_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      242 2024-04-23 10:24:56.000000 TitanDevice-0.3.1/titan/_device_models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 10:08:51.212168 TitanDevice-0.3.2/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 10:08:51.212168 TitanDevice-0.3.2/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 TitanDevice-0.3.2/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 10:08:51.212168 TitanDevice-0.3.2/TitanDevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-24 10:08:51.000000 TitanDevice-0.3.2/TitanDevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      286 2024-04-24 10:08:51.000000 TitanDevice-0.3.2/TitanDevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-24 10:08:51.000000 TitanDevice-0.3.2/TitanDevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-24 10:08:51.000000 TitanDevice-0.3.2/TitanDevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        6 2024-04-24 10:08:51.000000 TitanDevice-0.3.2/TitanDevice.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-24 10:08:51.212168 TitanDevice-0.3.2/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-24 10:08:49.000000 TitanDevice-0.3.2/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-24 10:08:51.212168 TitanDevice-0.3.2/titan/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2114 2024-04-24 07:26:17.000000 TitanDevice-0.3.2/titan/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      841 2024-04-24 07:31:02.000000 TitanDevice-0.3.2/titan/_device_exception.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4708 2024-04-24 10:08:49.000000 TitanDevice-0.3.2/titan/_device_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      242 2024-04-23 10:24:56.000000 TitanDevice-0.3.2/titan/_device_models.py
```

### Comparing `TitanDevice-0.3.1/setup.py` & `TitanDevice-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name="TitanDevice",
-    version="0.3.1",
+    version="0.3.2",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `TitanDevice-0.3.1/titan/__init__.py` & `TitanDevice-0.3.2/titan/__init__.py`

 * *Files identical despite different names*

### Comparing `TitanDevice-0.3.1/titan/_device_exception.py` & `TitanDevice-0.3.2/titan/_device_exception.py`

 * *Files identical despite different names*

### Comparing `TitanDevice-0.3.1/titan/_device_manager.py` & `TitanDevice-0.3.2/titan/_device_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             version=self.__get_frida_version(frida_server_path)
         )
 
     @check_is_root
     def start_frida(self, frida_server_path):
         if not self.__is_frida_installed(frida_server_path):
             raise FridaServerNotInstalled(self._serial, frida_server_path)
-        while self.__is_frida_running(
+        while not self.__is_frida_running(
                 self.get_frida_server_name_from_path(frida_server_path)
         ):
             subprocess.Popen(
                 [adb_path(), '-s', self._serial, 'shell', 'nohup',
                  'su -c "{}" &'.format(frida_server_path)]
             )
             time.sleep(0.1)
```

