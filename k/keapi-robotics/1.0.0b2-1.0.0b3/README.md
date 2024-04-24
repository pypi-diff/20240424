# Comparing `tmp/keapi-robotics-1.0.0b2.tar.gz` & `tmp/keapi-robotics-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keapi-robotics-1.0.0b2.tar", last modified: Mon Nov  7 15:38:10 2022, max compression
+gzip compressed data, was "keapi-robotics-1.0.0b3.tar", last modified: Wed Sep  6 11:46:59 2023, max compression
```

## Comparing `keapi-robotics-1.0.0b2.tar` & `keapi-robotics-1.0.0b3.tar`

### file list

```diff
@@ -1,22 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 15:38:10.575531 keapi-robotics-1.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-11-07 15:37:51.000000 keapi-robotics-1.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3064 2022-11-07 15:38:10.575531 keapi-robotics-1.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2264 2022-11-07 15:37:51.000000 keapi-robotics-1.0.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 15:38:10.575531 keapi-robotics-1.0.0b2/keapi/
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-11-07 15:37:51.000000 keapi-robotics-1.0.0b2/keapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6694 2022-11-07 15:37:51.000000 keapi-robotics-1.0.0b2/keapi/_command_server.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-11-07 15:37:51.000000 keapi-robotics-1.0.0b2/keapi/_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     2539 2022-11-07 15:37:51.000000 keapi-robotics-1.0.0b2/keapi/_ke_var.py
--rw-r--r--   0 runner    (1001) docker     (121)     4992 2022-11-07 15:37:51.000000 keapi-robotics-1.0.0b2/keapi/_subscribe_server.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 15:38:10.575531 keapi-robotics-1.0.0b2/keapi/compat/
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-11-07 15:37:51.000000 keapi-robotics-1.0.0b2/keapi/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7936 2022-11-07 15:37:51.000000 keapi-robotics-1.0.0b2/keapi/compat/_tc_prog.py
--rw-r--r--   0 runner    (1001) docker     (121)     2629 2022-11-07 15:37:51.000000 keapi-robotics-1.0.0b2/keapi/compat/_tc_var.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 15:38:10.575531 keapi-robotics-1.0.0b2/keapi_robotics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3064 2022-11-07 15:38:10.000000 keapi-robotics-1.0.0b2/keapi_robotics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-11-07 15:38:10.000000 keapi-robotics-1.0.0b2/keapi_robotics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 15:38:10.000000 keapi-robotics-1.0.0b2/keapi_robotics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-07 15:38:10.000000 keapi-robotics-1.0.0b2/keapi_robotics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-07 15:38:10.000000 keapi-robotics-1.0.0b2/keapi_robotics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-07 15:38:10.575531 keapi-robotics-1.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-11-07 15:37:51.000000 keapi-robotics-1.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 11:46:59.453630 keapi-robotics-1.0.0b3/
+-rw-r--r--   0 runner    (1001) docker     (999)     1075 2023-09-06 11:46:44.000000 keapi-robotics-1.0.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)     3064 2023-09-06 11:46:59.453630 keapi-robotics-1.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     2264 2023-09-06 11:46:44.000000 keapi-robotics-1.0.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 11:46:59.453630 keapi-robotics-1.0.0b3/keapi/
+-rw-r--r--   0 runner    (1001) docker     (999)      400 2023-09-06 11:46:44.000000 keapi-robotics-1.0.0b3/keapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1737 2023-09-06 11:46:44.000000 keapi-robotics-1.0.0b3/keapi/_auth_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7064 2023-09-06 11:46:44.000000 keapi-robotics-1.0.0b3/keapi/_command_server.py
+-rw-r--r--   0 runner    (1001) docker     (999)      384 2023-09-06 11:46:44.000000 keapi-robotics-1.0.0b3/keapi/_error.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2539 2023-09-06 11:46:44.000000 keapi-robotics-1.0.0b3/keapi/_ke_var.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5482 2023-09-06 11:46:44.000000 keapi-robotics-1.0.0b3/keapi/_subscribe_server.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 11:46:59.453630 keapi-robotics-1.0.0b3/keapi_robotics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)     3064 2023-09-06 11:46:59.000000 keapi-robotics-1.0.0b3/keapi_robotics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      337 2023-09-06 11:46:59.000000 keapi-robotics-1.0.0b3/keapi_robotics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-06 11:46:59.000000 keapi-robotics-1.0.0b3/keapi_robotics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       66 2023-09-06 11:46:59.000000 keapi-robotics-1.0.0b3/keapi_robotics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        6 2023-09-06 11:46:59.000000 keapi-robotics-1.0.0b3/keapi_robotics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-06 11:46:59.453630 keapi-robotics-1.0.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1261 2023-09-06 11:46:44.000000 keapi-robotics-1.0.0b3/setup.py
```

### Comparing `keapi-robotics-1.0.0b2/LICENSE` & `keapi-robotics-1.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `keapi-robotics-1.0.0b2/PKG-INFO` & `keapi-robotics-1.0.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keapi-robotics
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: A API to communicate with a KEBA PLC via WebSockets
 Author: Sebastian Redinger
 Author-email: sebastian.redinger@fsbondtec.at
 License: MIT
 Keywords: keapi
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `keapi-robotics-1.0.0b2/README.md` & `keapi-robotics-1.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `keapi-robotics-1.0.0b2/keapi/_command_server.py` & `keapi-robotics-1.0.0b3/keapi/_command_server.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from ._error import KebaError, HttpError
+from ._error import KebaError, HttpError, SocketError
+from ._auth_mgr import AuthMgr
 import json
 import websocket
 from enum import Enum
 from typing import Any
 from threading import Thread, Lock, Condition
 
 
@@ -99,27 +100,26 @@
                 self._state = self.State.KEBA_ERROR
             self._response = j_ans
             return True
         else:
             return False
 
 
-def connect_commands(url: str):
+def connect_commands(auth_mgr: AuthMgr):
     """Establishes a connection to the RcWebApi Commands
     Socket and returns CommandServer object which can
     be used to interact with the socket.
 
-    :param url: Full URL to socket
-        (e.g. ws://IP:PORT/Robot/websocket-command)
-    :type url: str
+    :param auth_mgr: Instance of AuthMgr
+    :type auth_mgr: AuthMgr
     :return: CommandServer object
     :rtype: CommandServer
     """
     srv = CommandServer()
-    srv._connect(url)
+    srv._connect(auth_mgr)
     return srv
 
 
 class CommandServer:
     """Holds the connection to the RcWebApi's command
     socket. Provides a low level API to execute or start
     commands on the KEBA PLC
@@ -188,23 +188,28 @@
         :type cmd: str
         :return: Command result
         :rtype: Any
         """
         t = self.start(cmd, **kwargs)
         return t.wait()
 
-    def _connect(self, url):
+    def _connect(self, auth_mgr: AuthMgr):
+        url = (f"ws://{auth_mgr.host_ip()}/api/v4"
+               f"/rc/robots/{auth_mgr.robot_name()}"
+               f"/websocket-command?auth_token={auth_mgr.auth_token()}")
+        if auth_mgr.is_client_id_set():
+            url = f"{url}&client_id={auth_mgr.client_id()}"
         self._rec_id_counter = 0
         self._ws = websocket.WebSocket()
-        self._ws.connect(url, subprotocols=['RcWebApi.v1.json'])
+        self._ws.connect(url)
         ret = json.loads(self._ws.recv())
-        if ret['status'] != 200:
-            raise HttpError(
-                'Connection to Keba Socket could not be esablished.'
-                )
+        if ret['data']['status'] != 200:
+            raise SocketError('Connection to Keba Socket could not be esablished.')
+        if not auth_mgr.is_client_id_set():
+            auth_mgr.set_client_id(ret['data']['greeting']['client_id'])
         self._receiver_thread_stop = False
         self._receiver_thread = Thread(target=self._thread_fun)
         self._receiver_thread.start()
 
     def _thread_fun(self):
         while not self._receiver_thread_stop:
             ret = self._ws.recv()
```

### Comparing `keapi-robotics-1.0.0b2/keapi/_ke_var.py` & `keapi-robotics-1.0.0b3/keapi/_ke_var.py`

 * *Files identical despite different names*

### Comparing `keapi-robotics-1.0.0b2/keapi/_subscribe_server.py` & `keapi-robotics-1.0.0b3/keapi/_subscribe_server.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from ._error import SocketError
+from ._auth_mgr import AuthMgr
 import json
 import websocket
 from threading import Thread, Lock
 
 
-def connect_subscriber(url: str):
+def connect_subscriber(auth_mgr: AuthMgr):
     """Establishes a connection to the RcWebApi Subscribe
     Socket and returns SubscribeServer object which can
     be used to interact with the socket.
 
-    :param url: Full URL to socket
-        (e.g. ws://IP:PORT/Robot/websocket-subscribe)
-    :type url: str
+    :param auth_mgr: Instance of AuthMgr
+    :type auth_mgr: AuthMgr
     :return: SubscribeServer object
     :rtype: SubscribeServer
     """
     srv = SubscribeServer()
-    srv._connect(url)
+    srv._connect(auth_mgr)
     return srv
 
 
 class SubscribeServer:
     """Holds the connection to the RcWebApi's subscribe
     socket. Provides a low level API to subscribe and
     unsubscribe to topics predefined by KEBA.
@@ -30,14 +30,15 @@
     """
     def __init__(self) -> None:
         self._ws = None
         self._receiver_thread = None
         self._is_connected = False
         self._subscription_dict = {}
         self._lock = Lock()
+        self._auth_mgr = None
 
     def disconnect(self):
         """Unsubscribes from all active subscriptions
         and closes the connection to the socket.
         """
         with self._lock:
             self._subscription_dict = {}
@@ -111,27 +112,38 @@
         with self._lock:
             if func is None or len(self._subscription_dict[topic]) == 1:
                 del self._subscription_dict[topic]
                 _unsub_req(self, topic)
             else:
                 self._subscription_dict[topic].remove(func)
 
-    def _connect(self, url):
+    def _connect(self, auth_mgr):
+        url = (f"ws://{auth_mgr.host_ip()}/api/v4"
+               f"/rc/robots/{auth_mgr.robot_name()}"
+               f"/websocket-subscribe?auth_token={auth_mgr.auth_token()}")
+
+        if auth_mgr.is_client_id_set():
+            url = f"{url}&client_id={auth_mgr.client_id()}"
+
+        self._auth_mgr = auth_mgr
         self._ws = websocket.WebSocketApp(url,
-                                          subprotocols=['RcWebApi.v1.json'],
                                           on_message=self._message_handler,
                                           on_error=self._error_handler,
                                           on_open=self._open_handler)
         self._receiver_thread = Thread(target=self._thread_fun)
         self._receiver_thread.start()
 
     def _message_handler(self, ws, message):
         json_msg = json.loads(message)
         if 'topic' in json_msg:
             topic = json_msg['topic']
+            if topic == 'connection':
+                if not self._auth_mgr.is_client_id_set():
+                    self._auth_mgr.set_client_id(json_msg['data']['greeting']['client_id'])
+                return
             if topic not in self._subscription_dict:
                 return
             with self._lock:
                 for func in self._subscription_dict[topic]:
                     func(json_msg)
 
     def _error_handler(self, ws, error):
```

### Comparing `keapi-robotics-1.0.0b2/keapi_robotics.egg-info/PKG-INFO` & `keapi-robotics-1.0.0b3/keapi_robotics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keapi-robotics
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: A API to communicate with a KEBA PLC via WebSockets
 Author: Sebastian Redinger
 Author-email: sebastian.redinger@fsbondtec.at
 License: MIT
 Keywords: keapi
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `keapi-robotics-1.0.0b2/setup.py` & `keapi-robotics-1.0.0b3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
-VERSION = "1.0.0.beta2"
+VERSION = "1.0.0.beta3"
 
 install_requires = ['websocket-client==1.4.1']
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="keapi-robotics",
```

