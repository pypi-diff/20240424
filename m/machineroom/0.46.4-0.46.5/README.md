# Comparing `tmp/machineroom-0.46.4.tar.gz` & `tmp/machineroom-0.46.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machineroom-0.46.4.tar", last modified: Wed Apr 24 20:04:07 2024, max compression
+gzip compressed data, was "machineroom-0.46.5.tar", last modified: Wed Apr 24 20:06:29 2024, max compression
```

## Comparing `machineroom-0.46.4.tar` & `machineroom-0.46.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 20:04:07.938494 machineroom-0.46.4/
--rw-r--r--   0 root         (0) staff       (20)     2365 2024-04-24 18:48:26.000000 machineroom-0.46.4/.gitignore
--rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.46.4/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     4714 2024-04-24 20:04:07.938222 machineroom-0.46.4/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     3597 2024-02-29 11:21:25.000000 machineroom-0.46.4/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 20:04:07.927775 machineroom-0.46.4/cmdbin/
--rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.46.4/cmdbin/connect
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 20:04:07.931692 machineroom-0.46.4/machineroom/
--rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-24 20:04:07.000000 machineroom-0.46.4/machineroom/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     9410 2024-04-24 17:40:53.000000 machineroom-0.46.4/machineroom/const.py
--rw-r--r--   0 root         (0) staff       (20)     1924 2024-04-24 19:33:31.000000 machineroom-0.46.4/machineroom/infra.py
--rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.46.4/machineroom/schema.json
--rw-r--r--   0 root         (0) staff       (20)    14903 2024-04-24 19:55:52.000000 machineroom-0.46.4/machineroom/sql.py
--rw-r--r--   0 root         (0) staff       (20)    28511 2024-04-24 19:27:24.000000 machineroom-0.46.4/machineroom/taskbase.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 20:04:07.936651 machineroom-0.46.4/machineroom/tunnels/
--rw-r--r--   0 root         (0) staff       (20)       23 2024-04-24 17:37:19.000000 machineroom-0.46.4/machineroom/tunnels/__init__.py
--rwxr-xr-x   0 root         (0) staff       (20)     8069 2024-04-24 17:12:31.000000 machineroom-0.46.4/machineroom/tunnels/conn.py
--rw-r--r--   0 root         (0) staff       (20)      468 2024-04-24 17:12:31.000000 machineroom-0.46.4/machineroom/tunnels/fork.py
--rw-r--r--   0 root         (0) staff       (20)    15337 2024-04-24 20:03:00.000000 machineroom-0.46.4/machineroom/util.py
--rw-r--r--   0 root         (0) staff       (20)     4489 2024-04-24 19:57:32.000000 machineroom-0.46.4/machineroom/worker.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 20:04:07.937529 machineroom-0.46.4/machineroom.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     4714 2024-04-24 20:04:07.000000 machineroom-0.46.4/machineroom.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      514 2024-04-24 20:04:07.000000 machineroom-0.46.4/machineroom.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-04-24 20:04:07.000000 machineroom-0.46.4/machineroom.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       28 2024-04-24 20:04:07.000000 machineroom-0.46.4/machineroom.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       12 2024-04-24 20:04:07.000000 machineroom-0.46.4/machineroom.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       79 2024-04-24 20:04:07.939200 machineroom-0.46.4/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     2620 2024-04-24 14:34:36.000000 machineroom-0.46.4/setup.py
--rw-r--r--   0 root         (0) staff       (20)     1532 2024-04-15 07:27:18.000000 machineroom-0.46.4/update
--rw-r--r--   0 root         (0) staff       (20)        7 2024-04-24 20:04:01.000000 machineroom-0.46.4/version
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 20:06:29.061241 machineroom-0.46.5/
+-rw-r--r--   0 root         (0) staff       (20)     2365 2024-04-24 18:48:26.000000 machineroom-0.46.5/.gitignore
+-rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.46.5/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     4714 2024-04-24 20:06:29.061052 machineroom-0.46.5/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     3597 2024-02-29 11:21:25.000000 machineroom-0.46.5/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 20:06:29.052606 machineroom-0.46.5/cmdbin/
+-rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.46.5/cmdbin/connect
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 20:06:29.056261 machineroom-0.46.5/machineroom/
+-rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-24 20:06:28.000000 machineroom-0.46.5/machineroom/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     9410 2024-04-24 17:40:53.000000 machineroom-0.46.5/machineroom/const.py
+-rw-r--r--   0 root         (0) staff       (20)     1917 2024-04-24 20:05:59.000000 machineroom-0.46.5/machineroom/infra.py
+-rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.46.5/machineroom/schema.json
+-rw-r--r--   0 root         (0) staff       (20)    14903 2024-04-24 19:55:52.000000 machineroom-0.46.5/machineroom/sql.py
+-rw-r--r--   0 root         (0) staff       (20)    28511 2024-04-24 19:27:24.000000 machineroom-0.46.5/machineroom/taskbase.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 20:06:29.059566 machineroom-0.46.5/machineroom/tunnels/
+-rw-r--r--   0 root         (0) staff       (20)       23 2024-04-24 17:37:19.000000 machineroom-0.46.5/machineroom/tunnels/__init__.py
+-rwxr-xr-x   0 root         (0) staff       (20)     8069 2024-04-24 17:12:31.000000 machineroom-0.46.5/machineroom/tunnels/conn.py
+-rw-r--r--   0 root         (0) staff       (20)      468 2024-04-24 17:12:31.000000 machineroom-0.46.5/machineroom/tunnels/fork.py
+-rw-r--r--   0 root         (0) staff       (20)    15337 2024-04-24 20:03:00.000000 machineroom-0.46.5/machineroom/util.py
+-rw-r--r--   0 root         (0) staff       (20)     4475 2024-04-24 20:05:59.000000 machineroom-0.46.5/machineroom/worker.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 20:06:29.060409 machineroom-0.46.5/machineroom.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     4714 2024-04-24 20:06:28.000000 machineroom-0.46.5/machineroom.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      514 2024-04-24 20:06:28.000000 machineroom-0.46.5/machineroom.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-24 20:06:28.000000 machineroom-0.46.5/machineroom.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       28 2024-04-24 20:06:28.000000 machineroom-0.46.5/machineroom.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       12 2024-04-24 20:06:28.000000 machineroom-0.46.5/machineroom.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       79 2024-04-24 20:06:29.061826 machineroom-0.46.5/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     2620 2024-04-24 14:34:36.000000 machineroom-0.46.5/setup.py
+-rw-r--r--   0 root         (0) staff       (20)     1532 2024-04-15 07:27:18.000000 machineroom-0.46.5/update
+-rw-r--r--   0 root         (0) staff       (20)        7 2024-04-24 20:06:25.000000 machineroom-0.46.5/version
```

### Comparing `machineroom-0.46.4/.gitignore` & `machineroom-0.46.5/.gitignore`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.4/LICENSE` & `machineroom-0.46.5/LICENSE`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.4/PKG-INFO` & `machineroom-0.46.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.46.4
+Version: 0.46.5
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.46.4/README.md` & `machineroom-0.46.5/README.md`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.4/cmdbin/connect` & `machineroom-0.46.5/cmdbin/connect`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.4/machineroom/__init__.py` & `machineroom-0.46.5/machineroom/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 logger5 = logging.getLogger("invoke")
 logger2.setLevel(logging.ERROR)
 logger1.setLevel(logging.ERROR)
 logger3.setLevel(logging.ERROR)
 logger4.setLevel(logging.ERROR)
 logger5.setLevel(logging.ERROR)
 
-__version__ = '0.46.4'
+__version__ = '0.46.5'
```

### Comparing `machineroom-0.46.4/machineroom/const.py` & `machineroom-0.46.5/machineroom/const.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.4/machineroom/infra.py` & `machineroom-0.46.5/machineroom/infra.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class Infra1(tb.DeploymentBotFoundation):
     def __init__(self, x):
         super().__init__(x)
         self.db = ServerRoom()
 
-    def __run_connect(self, callback_x=None):
+    def run_conn(self, callback_x=None):
         k = self.start_server_from
         if self.srv.serv_count < k:
             print("cannot start from out of range server number")
             return
         if self.run_tunnel_detection():
             self.srv.use_next_node()
             k += 1
@@ -40,15 +40,15 @@
                 self.connection_err(e, True)
             except Exception as e:
                 self.connection_err(e, False)
             self.srv.use_next_node()
             k += 1
         self.run_tunnel_detection_off()
 
-    def __run_offline(self, call_job=None):
+    def run_offline(self, call_job=None):
         k = self.start_server_from
         if self.srv.serv_count < k:
             print("cannot start from out of range server number")
             return
         while k < self.srv.serv_count:
             self.db.set_server_id(self.srv.current_id)
             self.stage_0()
```

### Comparing `machineroom-0.46.4/machineroom/schema.json` & `machineroom-0.46.5/machineroom/schema.json`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.4/machineroom/sql.py` & `machineroom-0.46.5/machineroom/sql.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.4/machineroom/taskbase.py` & `machineroom-0.46.5/machineroom/taskbase.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.4/machineroom/tunnels/conn.py` & `machineroom-0.46.5/machineroom/tunnels/conn.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.4/machineroom/util.py` & `machineroom-0.46.5/machineroom/util.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.4/machineroom/worker.py` & `machineroom-0.46.5/machineroom/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,35 +12,35 @@
 
 execute_path = os.path.dirname(__file__)
 
 
 class ServerDoorJob(Infra1):
 
     def action_import(self):
-        self.__run_connect()
+        self.run_conn()
 
     def action_retire(self):
-        self.__run_offline(self._retire_on_each_server)
+        self.run_offline(self._retire_on_each_server)
 
     def action_off_cert(self):
-        self.__run_offline(self._action_off_cert)
+        self.run_offline(self._action_off_cert)
 
     def _retire_on_each_server(self):
         self.db.update_res_kv("retired", True)
 
     def _action_off_cert(self):
         self.db.delete_res_kv("identity_cert_installed")
 
     def action_add_custom_cert(self, name, pubkey_path):
         def add_certification(x):
             if tb.detect_cert_signature(x, name) is False:
                 tb.copy_id(x, pubkey_path)
                 self.db.update_res_kv(f"custom_cert_{name}", True)
 
-        self.__run_connect(add_certification)
+        self.run_conn(add_certification)
 
 
 def internal_work():
     """
     This is the cmd console use functions
     alpha stage now.
     """
```

### Comparing `machineroom-0.46.4/machineroom.egg-info/PKG-INFO` & `machineroom-0.46.5/machineroom.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.46.4
+Version: 0.46.5
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.46.4/machineroom.egg-info/SOURCES.txt` & `machineroom-0.46.5/machineroom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.4/setup.py` & `machineroom-0.46.5/setup.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.4/update` & `machineroom-0.46.5/update`

 * *Files identical despite different names*

