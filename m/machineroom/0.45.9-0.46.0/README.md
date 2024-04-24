# Comparing `tmp/machineroom-0.45.9.tar.gz` & `tmp/machineroom-0.46.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machineroom-0.45.9.tar", last modified: Wed Apr 24 19:09:27 2024, max compression
+gzip compressed data, was "machineroom-0.46.0.tar", last modified: Wed Apr 24 19:11:24 2024, max compression
```

## Comparing `machineroom-0.45.9.tar` & `machineroom-0.46.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:09:27.323554 machineroom-0.45.9/
--rw-r--r--   0 root         (0) staff       (20)     2365 2024-04-24 18:48:26.000000 machineroom-0.45.9/.gitignore
--rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.45.9/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     4714 2024-04-24 19:09:27.323391 machineroom-0.45.9/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     3597 2024-02-29 11:21:25.000000 machineroom-0.45.9/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:09:27.316140 machineroom-0.45.9/cmdbin/
--rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.45.9/cmdbin/connect
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:09:27.318921 machineroom-0.45.9/machineroom/
--rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-24 19:09:27.000000 machineroom-0.45.9/machineroom/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     9410 2024-04-24 17:40:53.000000 machineroom-0.45.9/machineroom/const.py
--rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.45.9/machineroom/schema.json
--rw-r--r--   0 root         (0) staff       (20)    14812 2024-04-24 19:05:42.000000 machineroom-0.45.9/machineroom/sql.py
--rw-r--r--   0 root         (0) staff       (20)    28485 2024-04-24 18:48:01.000000 machineroom-0.45.9/machineroom/taskbase.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:09:27.322320 machineroom-0.45.9/machineroom/tunnels/
--rw-r--r--   0 root         (0) staff       (20)       23 2024-04-24 17:37:19.000000 machineroom-0.45.9/machineroom/tunnels/__init__.py
--rwxr-xr-x   0 root         (0) staff       (20)     8069 2024-04-24 17:12:31.000000 machineroom-0.45.9/machineroom/tunnels/conn.py
--rw-r--r--   0 root         (0) staff       (20)      468 2024-04-24 17:12:31.000000 machineroom-0.45.9/machineroom/tunnels/fork.py
--rw-r--r--   0 root         (0) staff       (20)    15343 2024-04-24 19:09:16.000000 machineroom-0.45.9/machineroom/util.py
--rw-r--r--   0 root         (0) staff       (20)     5564 2024-04-24 19:09:16.000000 machineroom-0.45.9/machineroom/worker.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:09:27.322841 machineroom-0.45.9/machineroom.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     4714 2024-04-24 19:09:27.000000 machineroom-0.45.9/machineroom.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      493 2024-04-24 19:09:27.000000 machineroom-0.45.9/machineroom.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-04-24 19:09:27.000000 machineroom-0.45.9/machineroom.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       28 2024-04-24 19:09:27.000000 machineroom-0.45.9/machineroom.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       12 2024-04-24 19:09:27.000000 machineroom-0.45.9/machineroom.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       79 2024-04-24 19:09:27.324103 machineroom-0.45.9/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     2620 2024-04-24 14:34:36.000000 machineroom-0.45.9/setup.py
--rw-r--r--   0 root         (0) staff       (20)     1532 2024-04-15 07:27:18.000000 machineroom-0.45.9/update
--rw-r--r--   0 root         (0) staff       (20)        7 2024-04-24 19:09:19.000000 machineroom-0.45.9/version
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:11:24.315408 machineroom-0.46.0/
+-rw-r--r--   0 root         (0) staff       (20)     2365 2024-04-24 18:48:26.000000 machineroom-0.46.0/.gitignore
+-rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.46.0/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     4714 2024-04-24 19:11:24.315236 machineroom-0.46.0/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     3597 2024-02-29 11:21:25.000000 machineroom-0.46.0/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:11:24.303222 machineroom-0.46.0/cmdbin/
+-rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.46.0/cmdbin/connect
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:11:24.306086 machineroom-0.46.0/machineroom/
+-rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-24 19:11:24.000000 machineroom-0.46.0/machineroom/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     9410 2024-04-24 17:40:53.000000 machineroom-0.46.0/machineroom/const.py
+-rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.46.0/machineroom/schema.json
+-rw-r--r--   0 root         (0) staff       (20)    14812 2024-04-24 19:05:42.000000 machineroom-0.46.0/machineroom/sql.py
+-rw-r--r--   0 root         (0) staff       (20)    28485 2024-04-24 18:48:01.000000 machineroom-0.46.0/machineroom/taskbase.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:11:24.309472 machineroom-0.46.0/machineroom/tunnels/
+-rw-r--r--   0 root         (0) staff       (20)       23 2024-04-24 17:37:19.000000 machineroom-0.46.0/machineroom/tunnels/__init__.py
+-rwxr-xr-x   0 root         (0) staff       (20)     8069 2024-04-24 17:12:31.000000 machineroom-0.46.0/machineroom/tunnels/conn.py
+-rw-r--r--   0 root         (0) staff       (20)      468 2024-04-24 17:12:31.000000 machineroom-0.46.0/machineroom/tunnels/fork.py
+-rw-r--r--   0 root         (0) staff       (20)    15343 2024-04-24 19:09:16.000000 machineroom-0.46.0/machineroom/util.py
+-rw-r--r--   0 root         (0) staff       (20)     5637 2024-04-24 19:11:04.000000 machineroom-0.46.0/machineroom/worker.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:11:24.314593 machineroom-0.46.0/machineroom.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     4714 2024-04-24 19:11:24.000000 machineroom-0.46.0/machineroom.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      493 2024-04-24 19:11:24.000000 machineroom-0.46.0/machineroom.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-24 19:11:24.000000 machineroom-0.46.0/machineroom.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       28 2024-04-24 19:11:24.000000 machineroom-0.46.0/machineroom.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       12 2024-04-24 19:11:24.000000 machineroom-0.46.0/machineroom.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       79 2024-04-24 19:11:24.315974 machineroom-0.46.0/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     2620 2024-04-24 14:34:36.000000 machineroom-0.46.0/setup.py
+-rw-r--r--   0 root         (0) staff       (20)     1532 2024-04-15 07:27:18.000000 machineroom-0.46.0/update
+-rw-r--r--   0 root         (0) staff       (20)        7 2024-04-24 19:11:21.000000 machineroom-0.46.0/version
```

### Comparing `machineroom-0.45.9/.gitignore` & `machineroom-0.46.0/.gitignore`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.9/LICENSE` & `machineroom-0.46.0/LICENSE`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.9/PKG-INFO` & `machineroom-0.46.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.45.9
+Version: 0.46.0
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.45.9/README.md` & `machineroom-0.46.0/README.md`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.9/cmdbin/connect` & `machineroom-0.46.0/cmdbin/connect`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.9/machineroom/__init__.py` & `machineroom-0.46.0/machineroom/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 logger5 = logging.getLogger("invoke")
 logger2.setLevel(logging.ERROR)
 logger1.setLevel(logging.ERROR)
 logger3.setLevel(logging.ERROR)
 logger4.setLevel(logging.ERROR)
 logger5.setLevel(logging.ERROR)
 
-__version__ = '0.45.9'
+__version__ = '0.46.0'
```

### Comparing `machineroom-0.45.9/machineroom/const.py` & `machineroom-0.46.0/machineroom/const.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.9/machineroom/schema.json` & `machineroom-0.46.0/machineroom/schema.json`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.9/machineroom/sql.py` & `machineroom-0.46.0/machineroom/sql.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.9/machineroom/taskbase.py` & `machineroom-0.46.0/machineroom/taskbase.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.9/machineroom/tunnels/conn.py` & `machineroom-0.46.0/machineroom/tunnels/conn.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.9/machineroom/util.py` & `machineroom-0.46.0/machineroom/util.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.9/machineroom/worker.py` & `machineroom-0.46.0/machineroom/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from machineroom import taskbase as tb
+from machineroom import taskbase as tb, __version__
 from machineroom.tunnels.conn import *
 
 try:
     import SQLiteAsJSON
 except:
     os.system('python3.11 -m pip install SQLiteAsJSON')
     import SQLiteAsJSON
@@ -111,14 +111,16 @@
 
     elif a == "import":
         file = os.path.join(Config.DATAPATH_BASE, b)
         if os.path.exists(file) is False:
             print("Wrong path cannot open this file")
         job = ServerDoorJob(b)
         job.action_import()
+    elif a == "v":
+        print(f"version. {__version__}")
     elif a == "retire":
         file = os.path.join(Config.DATAPATH_BASE, b)
         if os.path.exists(file) is False:
             print("Wrong path cannot open this file")
         job = ServerDoorJob(b)
         job.action_retire()
     elif a == "off-cert":
```

### Comparing `machineroom-0.45.9/machineroom.egg-info/PKG-INFO` & `machineroom-0.46.0/machineroom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.45.9
+Version: 0.46.0
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.45.9/setup.py` & `machineroom-0.46.0/setup.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.9/update` & `machineroom-0.46.0/update`

 * *Files identical despite different names*

