# Comparing `tmp/machineroom-0.46.0.tar.gz` & `tmp/machineroom-0.46.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machineroom-0.46.0.tar", last modified: Wed Apr 24 19:11:24 2024, max compression
+gzip compressed data, was "machineroom-0.46.1.tar", last modified: Wed Apr 24 19:27:38 2024, max compression
```

## Comparing `machineroom-0.46.0.tar` & `machineroom-0.46.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:11:24.315408 machineroom-0.46.0/
--rw-r--r--   0 root         (0) staff       (20)     2365 2024-04-24 18:48:26.000000 machineroom-0.46.0/.gitignore
--rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.46.0/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     4714 2024-04-24 19:11:24.315236 machineroom-0.46.0/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     3597 2024-02-29 11:21:25.000000 machineroom-0.46.0/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:11:24.303222 machineroom-0.46.0/cmdbin/
--rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.46.0/cmdbin/connect
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:11:24.306086 machineroom-0.46.0/machineroom/
--rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-24 19:11:24.000000 machineroom-0.46.0/machineroom/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     9410 2024-04-24 17:40:53.000000 machineroom-0.46.0/machineroom/const.py
--rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.46.0/machineroom/schema.json
--rw-r--r--   0 root         (0) staff       (20)    14812 2024-04-24 19:05:42.000000 machineroom-0.46.0/machineroom/sql.py
--rw-r--r--   0 root         (0) staff       (20)    28485 2024-04-24 18:48:01.000000 machineroom-0.46.0/machineroom/taskbase.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:11:24.309472 machineroom-0.46.0/machineroom/tunnels/
--rw-r--r--   0 root         (0) staff       (20)       23 2024-04-24 17:37:19.000000 machineroom-0.46.0/machineroom/tunnels/__init__.py
--rwxr-xr-x   0 root         (0) staff       (20)     8069 2024-04-24 17:12:31.000000 machineroom-0.46.0/machineroom/tunnels/conn.py
--rw-r--r--   0 root         (0) staff       (20)      468 2024-04-24 17:12:31.000000 machineroom-0.46.0/machineroom/tunnels/fork.py
--rw-r--r--   0 root         (0) staff       (20)    15343 2024-04-24 19:09:16.000000 machineroom-0.46.0/machineroom/util.py
--rw-r--r--   0 root         (0) staff       (20)     5637 2024-04-24 19:11:04.000000 machineroom-0.46.0/machineroom/worker.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:11:24.314593 machineroom-0.46.0/machineroom.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     4714 2024-04-24 19:11:24.000000 machineroom-0.46.0/machineroom.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      493 2024-04-24 19:11:24.000000 machineroom-0.46.0/machineroom.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-04-24 19:11:24.000000 machineroom-0.46.0/machineroom.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       28 2024-04-24 19:11:24.000000 machineroom-0.46.0/machineroom.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       12 2024-04-24 19:11:24.000000 machineroom-0.46.0/machineroom.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       79 2024-04-24 19:11:24.315974 machineroom-0.46.0/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     2620 2024-04-24 14:34:36.000000 machineroom-0.46.0/setup.py
--rw-r--r--   0 root         (0) staff       (20)     1532 2024-04-15 07:27:18.000000 machineroom-0.46.0/update
--rw-r--r--   0 root         (0) staff       (20)        7 2024-04-24 19:11:21.000000 machineroom-0.46.0/version
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:27:38.594446 machineroom-0.46.1/
+-rw-r--r--   0 root         (0) staff       (20)     2365 2024-04-24 18:48:26.000000 machineroom-0.46.1/.gitignore
+-rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.46.1/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     4714 2024-04-24 19:27:38.594269 machineroom-0.46.1/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     3597 2024-02-29 11:21:25.000000 machineroom-0.46.1/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:27:38.584088 machineroom-0.46.1/cmdbin/
+-rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.46.1/cmdbin/connect
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:27:38.588373 machineroom-0.46.1/machineroom/
+-rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-24 19:27:38.000000 machineroom-0.46.1/machineroom/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     9410 2024-04-24 17:40:53.000000 machineroom-0.46.1/machineroom/const.py
+-rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.46.1/machineroom/schema.json
+-rw-r--r--   0 root         (0) staff       (20)    14812 2024-04-24 19:05:42.000000 machineroom-0.46.1/machineroom/sql.py
+-rw-r--r--   0 root         (0) staff       (20)    28511 2024-04-24 19:27:24.000000 machineroom-0.46.1/machineroom/taskbase.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:27:38.593011 machineroom-0.46.1/machineroom/tunnels/
+-rw-r--r--   0 root         (0) staff       (20)       23 2024-04-24 17:37:19.000000 machineroom-0.46.1/machineroom/tunnels/__init__.py
+-rwxr-xr-x   0 root         (0) staff       (20)     8069 2024-04-24 17:12:31.000000 machineroom-0.46.1/machineroom/tunnels/conn.py
+-rw-r--r--   0 root         (0) staff       (20)      468 2024-04-24 17:12:31.000000 machineroom-0.46.1/machineroom/tunnels/fork.py
+-rw-r--r--   0 root         (0) staff       (20)    15343 2024-04-24 19:09:16.000000 machineroom-0.46.1/machineroom/util.py
+-rw-r--r--   0 root         (0) staff       (20)     5698 2024-04-24 19:27:24.000000 machineroom-0.46.1/machineroom/worker.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:27:38.593568 machineroom-0.46.1/machineroom.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     4714 2024-04-24 19:27:38.000000 machineroom-0.46.1/machineroom.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      493 2024-04-24 19:27:38.000000 machineroom-0.46.1/machineroom.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-24 19:27:38.000000 machineroom-0.46.1/machineroom.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       28 2024-04-24 19:27:38.000000 machineroom-0.46.1/machineroom.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       12 2024-04-24 19:27:38.000000 machineroom-0.46.1/machineroom.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       79 2024-04-24 19:27:38.595269 machineroom-0.46.1/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     2620 2024-04-24 14:34:36.000000 machineroom-0.46.1/setup.py
+-rw-r--r--   0 root         (0) staff       (20)     1532 2024-04-15 07:27:18.000000 machineroom-0.46.1/update
+-rw-r--r--   0 root         (0) staff       (20)        7 2024-04-24 19:27:31.000000 machineroom-0.46.1/version
```

### Comparing `machineroom-0.46.0/.gitignore` & `machineroom-0.46.1/.gitignore`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.0/LICENSE` & `machineroom-0.46.1/LICENSE`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.0/PKG-INFO` & `machineroom-0.46.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.46.0
+Version: 0.46.1
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.46.0/README.md` & `machineroom-0.46.1/README.md`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.0/cmdbin/connect` & `machineroom-0.46.1/cmdbin/connect`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.0/machineroom/__init__.py` & `machineroom-0.46.1/machineroom/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 logger5 = logging.getLogger("invoke")
 logger2.setLevel(logging.ERROR)
 logger1.setLevel(logging.ERROR)
 logger3.setLevel(logging.ERROR)
 logger4.setLevel(logging.ERROR)
 logger5.setLevel(logging.ERROR)
 
-__version__ = '0.46.0'
+__version__ = '0.46.1'
```

### Comparing `machineroom-0.46.0/machineroom/const.py` & `machineroom-0.46.1/machineroom/const.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.0/machineroom/schema.json` & `machineroom-0.46.1/machineroom/schema.json`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.0/machineroom/sql.py` & `machineroom-0.46.1/machineroom/sql.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.0/machineroom/taskbase.py` & `machineroom-0.46.1/machineroom/taskbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -629,16 +629,17 @@
                     DummyWatcher(),
                 ],
             },
         })
 
     def run_tunnel_detection(self):
         if self.srv.tunnel_type == TunnelType.NO_TUNNEL:
-            return
+            return False
         conn.use_macos_vpn_on(self.srv.profile_name)
+        return True
 
     def run_tunnel_detection_off(self):
         if self.srv.tunnel_type == TunnelType.NO_TUNNEL:
             return
         conn.use_macos_vpn_off(self.srv.profile_name)
 
     def _est_connection(self) -> Connection:
```

### Comparing `machineroom-0.46.0/machineroom/tunnels/conn.py` & `machineroom-0.46.1/machineroom/tunnels/conn.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.0/machineroom/util.py` & `machineroom-0.46.1/machineroom/util.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.0/machineroom/worker.py` & `machineroom-0.46.1/machineroom/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,18 @@
         self.db = ServerRoom()
 
     def __run_connect(self, callback_x=None):
         k = self.start_server_from
         if self.srv.serv_count < k:
             print("cannot start from out of range server number")
             return
-        self.run_tunnel_detection()
+        if self.run_tunnel_detection():
+            self.srv.use_next_node()
+            k += 1
+
         while k < self.srv.serv_count:
             self.db.set_server_id(self.srv.current_id)
             self.stage_0()
             c = self._est_connection()
             try:
                 self.stage_1(c)
                 if callable(callback_x):
```

### Comparing `machineroom-0.46.0/machineroom.egg-info/PKG-INFO` & `machineroom-0.46.1/machineroom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.46.0
+Version: 0.46.1
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.46.0/setup.py` & `machineroom-0.46.1/setup.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.0/update` & `machineroom-0.46.1/update`

 * *Files identical despite different names*

