# Comparing `tmp/machineroom-0.46.3.tar.gz` & `tmp/machineroom-0.46.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machineroom-0.46.3.tar", last modified: Wed Apr 24 19:37:45 2024, max compression
+gzip compressed data, was "machineroom-0.46.4.tar", last modified: Wed Apr 24 20:04:07 2024, max compression
```

## Comparing `machineroom-0.46.3.tar` & `machineroom-0.46.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:37:45.633937 machineroom-0.46.3/
--rw-r--r--   0 root         (0) staff       (20)     2365 2024-04-24 18:48:26.000000 machineroom-0.46.3/.gitignore
--rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.46.3/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     4714 2024-04-24 19:37:45.633771 machineroom-0.46.3/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     3597 2024-02-29 11:21:25.000000 machineroom-0.46.3/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:37:45.625885 machineroom-0.46.3/cmdbin/
--rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.46.3/cmdbin/connect
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:37:45.629452 machineroom-0.46.3/machineroom/
--rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-24 19:37:45.000000 machineroom-0.46.3/machineroom/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     9410 2024-04-24 17:40:53.000000 machineroom-0.46.3/machineroom/const.py
--rw-r--r--   0 root         (0) staff       (20)     1924 2024-04-24 19:33:31.000000 machineroom-0.46.3/machineroom/infra.py
--rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.46.3/machineroom/schema.json
--rw-r--r--   0 root         (0) staff       (20)    14812 2024-04-24 19:05:42.000000 machineroom-0.46.3/machineroom/sql.py
--rw-r--r--   0 root         (0) staff       (20)    28511 2024-04-24 19:27:24.000000 machineroom-0.46.3/machineroom/taskbase.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:37:45.632670 machineroom-0.46.3/machineroom/tunnels/
--rw-r--r--   0 root         (0) staff       (20)       23 2024-04-24 17:37:19.000000 machineroom-0.46.3/machineroom/tunnels/__init__.py
--rwxr-xr-x   0 root         (0) staff       (20)     8069 2024-04-24 17:12:31.000000 machineroom-0.46.3/machineroom/tunnels/conn.py
--rw-r--r--   0 root         (0) staff       (20)      468 2024-04-24 17:12:31.000000 machineroom-0.46.3/machineroom/tunnels/fork.py
--rw-r--r--   0 root         (0) staff       (20)    15343 2024-04-24 19:09:16.000000 machineroom-0.46.3/machineroom/util.py
--rw-r--r--   0 root         (0) staff       (20)     4454 2024-04-24 19:36:33.000000 machineroom-0.46.3/machineroom/worker.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 19:37:45.633221 machineroom-0.46.3/machineroom.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     4714 2024-04-24 19:37:45.000000 machineroom-0.46.3/machineroom.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      514 2024-04-24 19:37:45.000000 machineroom-0.46.3/machineroom.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-04-24 19:37:45.000000 machineroom-0.46.3/machineroom.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       28 2024-04-24 19:37:45.000000 machineroom-0.46.3/machineroom.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       12 2024-04-24 19:37:45.000000 machineroom-0.46.3/machineroom.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       79 2024-04-24 19:37:45.634497 machineroom-0.46.3/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     2620 2024-04-24 14:34:36.000000 machineroom-0.46.3/setup.py
--rw-r--r--   0 root         (0) staff       (20)     1532 2024-04-15 07:27:18.000000 machineroom-0.46.3/update
--rw-r--r--   0 root         (0) staff       (20)        7 2024-04-24 19:37:39.000000 machineroom-0.46.3/version
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 20:04:07.938494 machineroom-0.46.4/
+-rw-r--r--   0 root         (0) staff       (20)     2365 2024-04-24 18:48:26.000000 machineroom-0.46.4/.gitignore
+-rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.46.4/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     4714 2024-04-24 20:04:07.938222 machineroom-0.46.4/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     3597 2024-02-29 11:21:25.000000 machineroom-0.46.4/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 20:04:07.927775 machineroom-0.46.4/cmdbin/
+-rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.46.4/cmdbin/connect
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 20:04:07.931692 machineroom-0.46.4/machineroom/
+-rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-24 20:04:07.000000 machineroom-0.46.4/machineroom/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     9410 2024-04-24 17:40:53.000000 machineroom-0.46.4/machineroom/const.py
+-rw-r--r--   0 root         (0) staff       (20)     1924 2024-04-24 19:33:31.000000 machineroom-0.46.4/machineroom/infra.py
+-rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.46.4/machineroom/schema.json
+-rw-r--r--   0 root         (0) staff       (20)    14903 2024-04-24 19:55:52.000000 machineroom-0.46.4/machineroom/sql.py
+-rw-r--r--   0 root         (0) staff       (20)    28511 2024-04-24 19:27:24.000000 machineroom-0.46.4/machineroom/taskbase.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 20:04:07.936651 machineroom-0.46.4/machineroom/tunnels/
+-rw-r--r--   0 root         (0) staff       (20)       23 2024-04-24 17:37:19.000000 machineroom-0.46.4/machineroom/tunnels/__init__.py
+-rwxr-xr-x   0 root         (0) staff       (20)     8069 2024-04-24 17:12:31.000000 machineroom-0.46.4/machineroom/tunnels/conn.py
+-rw-r--r--   0 root         (0) staff       (20)      468 2024-04-24 17:12:31.000000 machineroom-0.46.4/machineroom/tunnels/fork.py
+-rw-r--r--   0 root         (0) staff       (20)    15337 2024-04-24 20:03:00.000000 machineroom-0.46.4/machineroom/util.py
+-rw-r--r--   0 root         (0) staff       (20)     4489 2024-04-24 19:57:32.000000 machineroom-0.46.4/machineroom/worker.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 20:04:07.937529 machineroom-0.46.4/machineroom.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     4714 2024-04-24 20:04:07.000000 machineroom-0.46.4/machineroom.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      514 2024-04-24 20:04:07.000000 machineroom-0.46.4/machineroom.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-24 20:04:07.000000 machineroom-0.46.4/machineroom.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       28 2024-04-24 20:04:07.000000 machineroom-0.46.4/machineroom.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       12 2024-04-24 20:04:07.000000 machineroom-0.46.4/machineroom.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       79 2024-04-24 20:04:07.939200 machineroom-0.46.4/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     2620 2024-04-24 14:34:36.000000 machineroom-0.46.4/setup.py
+-rw-r--r--   0 root         (0) staff       (20)     1532 2024-04-15 07:27:18.000000 machineroom-0.46.4/update
+-rw-r--r--   0 root         (0) staff       (20)        7 2024-04-24 20:04:01.000000 machineroom-0.46.4/version
```

### Comparing `machineroom-0.46.3/.gitignore` & `machineroom-0.46.4/.gitignore`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.3/LICENSE` & `machineroom-0.46.4/LICENSE`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.3/PKG-INFO` & `machineroom-0.46.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.46.3
+Version: 0.46.4
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.46.3/README.md` & `machineroom-0.46.4/README.md`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.3/cmdbin/connect` & `machineroom-0.46.4/cmdbin/connect`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.3/machineroom/__init__.py` & `machineroom-0.46.4/machineroom/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 logger5 = logging.getLogger("invoke")
 logger2.setLevel(logging.ERROR)
 logger1.setLevel(logging.ERROR)
 logger3.setLevel(logging.ERROR)
 logger4.setLevel(logging.ERROR)
 logger5.setLevel(logging.ERROR)
 
-__version__ = '0.46.3'
+__version__ = '0.46.4'
```

### Comparing `machineroom-0.46.3/machineroom/const.py` & `machineroom-0.46.4/machineroom/const.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.3/machineroom/infra.py` & `machineroom-0.46.4/machineroom/infra.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.3/machineroom/schema.json` & `machineroom-0.46.4/machineroom/schema.json`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.3/machineroom/sql.py` & `machineroom-0.46.4/machineroom/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,22 +131,21 @@
             return False
         return True
 
     def get_member_res(self, tbl: str, server_id: str) -> dict:
         cursor = self.conn.cursor()
         _da = {}
         try:
-            cursor.execute(f'SELECT res FROM {tbl} WHERE id = ?',
-                           (server_id,))
+            cursor.execute(f'SELECT res FROM {tbl} WHERE id = ?', (server_id,))
             (res_01,) = cursor.fetchone()
             _da = json.loads(res_01)
         except json.JSONDecodeError as e:
             db_logger.error(e)
         except Exception as E:
-            db_logger.error('Data Insert Error : ', E)
+            db_logger.warn('Data READ:', E)
         return _da
 
     def get_host_info(self, tbl: str, server_id: str) -> Tuple[str, str, int]:
         cursor = self.conn.cursor()
         try:
             cursor.execute(f'SELECT host, user, port FROM {tbl} WHERE id = ?',
                            (server_id,))
@@ -330,19 +329,24 @@
             "next_action": "{}",
             "description": "",
             "res": json.dumps(file)
         }
         return self.insert_new(p)
 
     def get_res_kv(self, k: str):
-        da = self.get_member_res(self._tblembr, self.server_id)
-        if k in da:
-            return da[k]
-        else:
+        try:
+            da = self.get_member_res(self._tblembr, self.server_id)
+            if k in da:
+                return da[k]
+            else:
+                return ""
+        except TypeError:
             return ""
+        except Exception:
+            return ''
 
     def total_count(self, tbl: str) -> int:
         cursor = self.conn.cursor()
         cursor.execute(f"SELECT COUNT(*) as count FROM {tbl}")
         (count,) = cursor.fetchone()
         cursor.close()
         if count > 0:
```

### Comparing `machineroom-0.46.3/machineroom/taskbase.py` & `machineroom-0.46.4/machineroom/taskbase.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.3/machineroom/tunnels/conn.py` & `machineroom-0.46.4/machineroom/tunnels/conn.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.3/machineroom/util.py` & `machineroom-0.46.4/machineroom/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 from .const import *
 
 CMD_LIST1 = ["ls", "show", "list", "tell"]
 CMD_LIST2 = ["scan", "check", "validation", "valid"]
 
 
 def use_args() -> Tuple[str, str, str]:
-    opt1 = None
-    opt2 = None
-    opt3 = None
+    opt1 = ""
+    opt2 = ""
+    opt3 = ""
     cmd = "ls"
 
     if len(sys.argv) >= 2:
         opt1 = sys.argv[1]
         if len(sys.argv) >= 3:
             opt2 = sys.argv[2]
             if len(sys.argv) >= 4:
```

### Comparing `machineroom-0.46.3/machineroom/worker.py` & `machineroom-0.46.4/machineroom/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,18 +46,20 @@
     """
     (a, b, c) = use_args()
     local = ServerRoom()
     if a == "ls":
         print("Here is my machine room...")
         gh = local.show_all_serv()
         for (id, host, res) in gh:
+            local.set_server_id(id)
             y = FieldConstruct()
             y.add_icon(f"{id}  -> {host}     ")
-            if local.get_tunnel_profile() != "":
-                y.add_icon(f"TUNNEL PROFILE: {local.get_tunnel_profile()}")
+            tun = local.get_tunnel_profile()
+            if tun != "":
+                y.add_icon(f"TUNNEL PROFILE: {tun}")
             y.add_icon("EXPIRED" if local.is_what_installed_full("retire", id) else "")
             y.add_icon("CERT" if local.is_what_installed_full("identity_cert_installed", id) else "")
             y.add_icon("DOCKER" if local.is_what_installed_full("docker_compose_installed", id) else "")
             y.add_icon("DEAD" if local.is_what_installed_full("daed_installed", id) else "")
             y.add_icon("YACHT" if local.is_what_installed_full("yacht_installed", id) else "")
             y.add_icon("PY" if local.is_what_installed_full("python3_installed", id) else "")
             print(y.output())
```

### Comparing `machineroom-0.46.3/machineroom.egg-info/PKG-INFO` & `machineroom-0.46.4/machineroom.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.46.3
+Version: 0.46.4
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.46.3/machineroom.egg-info/SOURCES.txt` & `machineroom-0.46.4/machineroom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.3/setup.py` & `machineroom-0.46.4/setup.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.46.3/update` & `machineroom-0.46.4/update`

 * *Files identical despite different names*

