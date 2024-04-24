# Comparing `tmp/machineroom-0.45.7.tar.gz` & `tmp/machineroom-0.45.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machineroom-0.45.7.tar", last modified: Wed Apr 24 18:48:57 2024, max compression
+gzip compressed data, was "machineroom-0.45.8.tar", last modified: Wed Apr 24 18:58:30 2024, max compression
```

## Comparing `machineroom-0.45.7.tar` & `machineroom-0.45.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 18:48:57.273468 machineroom-0.45.7/
--rw-r--r--   0 root         (0) staff       (20)     2365 2024-04-24 18:48:26.000000 machineroom-0.45.7/.gitignore
--rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.45.7/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     4714 2024-04-24 18:48:57.273200 machineroom-0.45.7/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     3597 2024-02-29 11:21:25.000000 machineroom-0.45.7/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 18:48:57.263947 machineroom-0.45.7/cmdbin/
--rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.45.7/cmdbin/connect
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 18:48:57.267684 machineroom-0.45.7/machineroom/
--rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-24 18:48:56.000000 machineroom-0.45.7/machineroom/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     9410 2024-04-24 17:40:53.000000 machineroom-0.45.7/machineroom/const.py
--rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.45.7/machineroom/schema.json
--rw-r--r--   0 root         (0) staff       (20)    14669 2024-04-24 18:22:06.000000 machineroom-0.45.7/machineroom/sql.py
--rw-r--r--   0 root         (0) staff       (20)    28485 2024-04-24 18:48:01.000000 machineroom-0.45.7/machineroom/taskbase.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 18:48:57.271628 machineroom-0.45.7/machineroom/tunnels/
--rw-r--r--   0 root         (0) staff       (20)       23 2024-04-24 17:37:19.000000 machineroom-0.45.7/machineroom/tunnels/__init__.py
--rwxr-xr-x   0 root         (0) staff       (20)     8069 2024-04-24 17:12:31.000000 machineroom-0.45.7/machineroom/tunnels/conn.py
--rw-r--r--   0 root         (0) staff       (20)      468 2024-04-24 17:12:31.000000 machineroom-0.45.7/machineroom/tunnels/fork.py
--rw-r--r--   0 root         (0) staff       (20)    15171 2024-04-24 18:22:06.000000 machineroom-0.45.7/machineroom/util.py
--rw-r--r--   0 root         (0) staff       (20)     5230 2024-04-24 18:48:01.000000 machineroom-0.45.7/machineroom/worker.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 18:48:57.272556 machineroom-0.45.7/machineroom.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     4714 2024-04-24 18:48:57.000000 machineroom-0.45.7/machineroom.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      493 2024-04-24 18:48:57.000000 machineroom-0.45.7/machineroom.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-04-24 18:48:57.000000 machineroom-0.45.7/machineroom.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       28 2024-04-24 18:48:57.000000 machineroom-0.45.7/machineroom.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       12 2024-04-24 18:48:57.000000 machineroom-0.45.7/machineroom.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       79 2024-04-24 18:48:57.274063 machineroom-0.45.7/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     2620 2024-04-24 14:34:36.000000 machineroom-0.45.7/setup.py
--rw-r--r--   0 root         (0) staff       (20)     1532 2024-04-15 07:27:18.000000 machineroom-0.45.7/update
--rw-r--r--   0 root         (0) staff       (20)        7 2024-04-24 18:48:47.000000 machineroom-0.45.7/version
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 18:58:30.689029 machineroom-0.45.8/
+-rw-r--r--   0 root         (0) staff       (20)     2365 2024-04-24 18:48:26.000000 machineroom-0.45.8/.gitignore
+-rw-r--r--   0 root         (0) staff       (20)     1068 2021-11-08 07:40:45.000000 machineroom-0.45.8/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     4714 2024-04-24 18:58:30.688867 machineroom-0.45.8/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     3597 2024-02-29 11:21:25.000000 machineroom-0.45.8/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 18:58:30.681754 machineroom-0.45.8/cmdbin/
+-rw-r--r--   0 root         (0) staff       (20)      586 2024-02-29 11:48:22.000000 machineroom-0.45.8/cmdbin/connect
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 18:58:30.684641 machineroom-0.45.8/machineroom/
+-rw-r--r--   0 root         (0) staff       (20)     1301 2024-04-24 18:58:30.000000 machineroom-0.45.8/machineroom/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     9410 2024-04-24 17:40:53.000000 machineroom-0.45.8/machineroom/const.py
+-rw-r--r--   0 root         (0) staff       (20)      996 2024-03-01 05:35:23.000000 machineroom-0.45.8/machineroom/schema.json
+-rw-r--r--   0 root         (0) staff       (20)    14669 2024-04-24 18:22:06.000000 machineroom-0.45.8/machineroom/sql.py
+-rw-r--r--   0 root         (0) staff       (20)    28485 2024-04-24 18:48:01.000000 machineroom-0.45.8/machineroom/taskbase.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 18:58:30.687803 machineroom-0.45.8/machineroom/tunnels/
+-rw-r--r--   0 root         (0) staff       (20)       23 2024-04-24 17:37:19.000000 machineroom-0.45.8/machineroom/tunnels/__init__.py
+-rwxr-xr-x   0 root         (0) staff       (20)     8069 2024-04-24 17:12:31.000000 machineroom-0.45.8/machineroom/tunnels/conn.py
+-rw-r--r--   0 root         (0) staff       (20)      468 2024-04-24 17:12:31.000000 machineroom-0.45.8/machineroom/tunnels/fork.py
+-rw-r--r--   0 root         (0) staff       (20)    15246 2024-04-24 18:58:01.000000 machineroom-0.45.8/machineroom/util.py
+-rw-r--r--   0 root         (0) staff       (20)     5230 2024-04-24 18:48:01.000000 machineroom-0.45.8/machineroom/worker.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-24 18:58:30.688301 machineroom-0.45.8/machineroom.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     4714 2024-04-24 18:58:30.000000 machineroom-0.45.8/machineroom.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      493 2024-04-24 18:58:30.000000 machineroom-0.45.8/machineroom.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-24 18:58:30.000000 machineroom-0.45.8/machineroom.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       28 2024-04-24 18:58:30.000000 machineroom-0.45.8/machineroom.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       12 2024-04-24 18:58:30.000000 machineroom-0.45.8/machineroom.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       79 2024-04-24 18:58:30.689566 machineroom-0.45.8/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     2620 2024-04-24 14:34:36.000000 machineroom-0.45.8/setup.py
+-rw-r--r--   0 root         (0) staff       (20)     1532 2024-04-15 07:27:18.000000 machineroom-0.45.8/update
+-rw-r--r--   0 root         (0) staff       (20)        7 2024-04-24 18:58:25.000000 machineroom-0.45.8/version
```

### Comparing `machineroom-0.45.7/.gitignore` & `machineroom-0.45.8/.gitignore`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.7/LICENSE` & `machineroom-0.45.8/LICENSE`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.7/PKG-INFO` & `machineroom-0.45.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.45.7
+Version: 0.45.8
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.45.7/README.md` & `machineroom-0.45.8/README.md`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.7/cmdbin/connect` & `machineroom-0.45.8/cmdbin/connect`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.7/machineroom/__init__.py` & `machineroom-0.45.8/machineroom/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 logger5 = logging.getLogger("invoke")
 logger2.setLevel(logging.ERROR)
 logger1.setLevel(logging.ERROR)
 logger3.setLevel(logging.ERROR)
 logger4.setLevel(logging.ERROR)
 logger5.setLevel(logging.ERROR)
 
-__version__ = '0.45.7'
+__version__ = '0.45.8'
```

### Comparing `machineroom-0.45.7/machineroom/const.py` & `machineroom-0.45.8/machineroom/const.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.7/machineroom/schema.json` & `machineroom-0.45.8/machineroom/schema.json`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.7/machineroom/sql.py` & `machineroom-0.45.8/machineroom/sql.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.7/machineroom/taskbase.py` & `machineroom-0.45.8/machineroom/taskbase.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.7/machineroom/tunnels/conn.py` & `machineroom-0.45.8/machineroom/tunnels/conn.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.7/machineroom/util.py` & `machineroom-0.45.8/machineroom/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -429,15 +429,15 @@
 
     def detect_servers(self):
         self.serv_count = read_file_total_lines(self.path_file)
         try:
             self.read_serv_at(0)
             self._on_detect = False
         except FoundVPNTunnel:
-            self.serv_count -= 1
+            ...
 
     def read_serv_at(self, index: int) -> dict:
         n = index % self.serv_count
         line = read_file_at_line(self.path_file, n)
         if "----" in line:
             line = line.split("----")
         elif "---" in line:
@@ -469,14 +469,17 @@
         self.current_host = line[1]
         self.current_user = line[2]
         self.current_pass = line[3]
         if self._on_detect is False:
             print(f"## ☎️ Now enter network ID#{n}: {line[0]} {line[1]}")
         return tmp
 
+    def has_tunnel(self) -> bool:
+        return self._tunnel_type != TunnelType.NO_TUNNEL
+
     def use_next_node(self, x: int = 1) -> dict:
         self._srv_index = self._srv_index + x
         return self.read_serv_at(self._srv_index)
 
 
 class InfrastructurePlannerFoundation:
     # total running nodes on this KVM
```

### Comparing `machineroom-0.45.7/machineroom/worker.py` & `machineroom-0.45.8/machineroom/worker.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.7/machineroom.egg-info/PKG-INFO` & `machineroom-0.45.8/machineroom.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machineroom
-Version: 0.45.7
+Version: 0.45.8
 Summary: A Python package to manage all my machines in the fingertip.
 Home-page: https://github.com/jjhesk/mymachineroom/
 Author: Jun-You Liu & Heskemo
 Author-email: meowmeow@gmail.com
 License: MIT
 Keywords: ssh machine room
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `machineroom-0.45.7/setup.py` & `machineroom-0.45.8/setup.py`

 * *Files identical despite different names*

### Comparing `machineroom-0.45.7/update` & `machineroom-0.45.8/update`

 * *Files identical despite different names*

