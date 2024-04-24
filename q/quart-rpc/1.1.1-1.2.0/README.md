# Comparing `tmp/quart_rpc-1.1.1.tar.gz` & `tmp/quart_rpc-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quart_rpc-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "quart_rpc-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `quart_rpc-1.1.1.tar` & `quart_rpc-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3104 2024-04-17 12:02:54.084518 quart_rpc-1.1.1/.gitignore
--rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 quart_rpc-1.1.1/LICENSE
--rw-r--r--   0        0        0     3473 2024-04-18 11:12:50.630490 quart_rpc-1.1.1/README.md
--rw-r--r--   0        0        0     1024 2024-04-18 09:57:23.895002 quart_rpc-1.1.1/app/__init__.py
--rw-r--r--   0        0        0     1856 2024-04-18 11:05:10.605491 quart_rpc-1.1.1/app/templates/index.html
--rw-r--r--   0        0        0      741 2024-04-16 14:38:49.181823 quart_rpc-1.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-18 11:13:21.094535 quart_rpc-1.1.1/quart_rpc/__init__.py
--rw-r--r--   0        0        0      164 2024-04-18 09:17:46.763194 quart_rpc-1.1.1/quart_rpc/latest.py
--rw-r--r--   0        0        0      244 2024-04-18 09:27:36.641998 quart_rpc-1.1.1/quart_rpc/version_1_0/__init__.py
--rw-r--r--   0        0        0      160 2024-04-18 09:56:48.552074 quart_rpc-1.1.1/quart_rpc/version_1_0/_protocols.py
--rw-r--r--   0        0        0      395 2024-04-18 09:21:53.897194 quart_rpc-1.1.1/quart_rpc/version_1_0/auth_session_key.py
--rw-r--r--   0        0        0      130 2024-04-18 11:05:19.979675 quart_rpc-1.1.1/quart_rpc/version_1_0/model.py
--rw-r--r--   0        0        0      480 2024-04-18 11:05:19.992185 quart_rpc-1.1.1/quart_rpc/version_1_0/request.py
--rw-r--r--   0        0        0     1099 2024-04-18 11:05:19.986245 quart_rpc-1.1.1/quart_rpc/version_1_0/response.py
--rw-r--r--   0        0        0     5484 2024-04-18 11:05:19.972570 quart_rpc-1.1.1/quart_rpc/version_1_0/rpc.py
--rw-r--r--   0        0        0      547 2024-04-18 10:08:33.791808 quart_rpc-1.1.1/quart_rpc/version_1_0/utilities.py
--rw-r--r--   0        0        0       15 2024-04-16 14:40:40.344290 quart_rpc-1.1.1/requirements/development.txt
--rw-r--r--   0        0        0       24 2024-04-17 12:22:19.294586 quart_rpc-1.1.1/requirements/main.txt
--rw-r--r--   0        0        0      399 2024-04-17 12:21:49.711577 quart_rpc-1.1.1/test.py
--rw-r--r--   0        0        0     4112 1970-01-01 00:00:00.000000 quart_rpc-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3104 2024-04-17 12:02:54.084518 quart_rpc-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 quart_rpc-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3514 2024-04-18 12:51:57.562300 quart_rpc-1.2.0/README.md
+-rw-r--r--   0        0        0      989 2024-04-24 13:25:20.658274 quart_rpc-1.2.0/app/__init__.py
+-rw-r--r--   0        0        0     1856 2024-04-18 11:05:10.605491 quart_rpc-1.2.0/app/templates/index.html
+-rw-r--r--   0        0        0      741 2024-04-16 14:38:49.181823 quart_rpc-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-24 13:29:13.899912 quart_rpc-1.2.0/quart_rpc/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-18 09:17:46.763194 quart_rpc-1.2.0/quart_rpc/latest.py
+-rw-r--r--   0        0        0      244 2024-04-18 09:27:36.641998 quart_rpc-1.2.0/quart_rpc/version_1_0/__init__.py
+-rw-r--r--   0        0        0      160 2024-04-18 09:56:48.552074 quart_rpc-1.2.0/quart_rpc/version_1_0/_protocols.py
+-rw-r--r--   0        0        0      395 2024-04-18 09:21:53.897194 quart_rpc-1.2.0/quart_rpc/version_1_0/auth_session_key.py
+-rw-r--r--   0        0        0      130 2024-04-18 11:05:19.979675 quart_rpc-1.2.0/quart_rpc/version_1_0/model.py
+-rw-r--r--   0        0        0      480 2024-04-18 11:05:19.992185 quart_rpc-1.2.0/quart_rpc/version_1_0/request.py
+-rw-r--r--   0        0        0     1160 2024-04-24 13:27:28.287137 quart_rpc-1.2.0/quart_rpc/version_1_0/response.py
+-rw-r--r--   0        0        0     5484 2024-04-18 11:05:19.972570 quart_rpc-1.2.0/quart_rpc/version_1_0/rpc.py
+-rw-r--r--   0        0        0      547 2024-04-18 10:08:33.791808 quart_rpc-1.2.0/quart_rpc/version_1_0/utilities.py
+-rw-r--r--   0        0        0       15 2024-04-16 14:40:40.344290 quart_rpc-1.2.0/requirements/development.txt
+-rw-r--r--   0        0        0       24 2024-04-17 12:22:19.294586 quart_rpc-1.2.0/requirements/main.txt
+-rw-r--r--   0        0        0      366 2024-04-24 13:25:20.658005 quart_rpc-1.2.0/test.py
+-rw-r--r--   0        0        0     4153 1970-01-01 00:00:00.000000 quart_rpc-1.2.0/PKG-INFO
```

### Comparing `quart_rpc-1.1.1/.gitignore` & `quart_rpc-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `quart_rpc-1.1.1/LICENSE` & `quart_rpc-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quart_rpc-1.1.1/README.md` & `quart_rpc-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 pip install quart-rpc
 ```
 
 ---
 
 The Quart implementation of [Flask-RPC](https://github.com/CheeseCake87/flask-rpc)
 
-Quart-RPC uses wRPC (Wee RPC) as its protocol, which is a
-micro JSON-based protocol that allows for
+Quart-RPC uses [wRPC (Wee RPC)](https://github.com/CheeseCake87/wRPC) 
+as its protocol, which is a micro JSON-based protocol that allows for
 easy communication between the client and server.
 
 The typical request/response cycle is as follows:
 
 **Request**
 
 ```json
```

### Comparing `quart_rpc-1.1.1/app/__init__.py` & `quart_rpc-1.2.0/app/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 from quart import Quart, session, render_template
 
 from quart_rpc.latest import RPC, RPCResponse, RPCAuthSessionKey
 
 
 def add_numbers(data: list) -> int:
-    return RPCResponse.success(
-        sum(data)
-    )
+    return RPCResponse.success(sum(data))
 
 
 def create_app():
     app = Quart(__name__)
     app.secret_key = "secret"
 
     RPC(
         app,
         url_prefix="/rpc",
         # session_auth=RPCAuthSessionKey("logged_in", [True]),
         host_auth=["127.0.0.1:5001"],
-        functions={
-            "add_numbers": add_numbers
-        }
+        functions={"add_numbers": add_numbers},
     )
 
     @app.before_request
     async def before_request():
         if "logged_in" not in session:
             session["logged_in"] = False
```

### Comparing `quart_rpc-1.1.1/app/templates/index.html` & `quart_rpc-1.2.0/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `quart_rpc-1.1.1/pyproject.toml` & `quart_rpc-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quart_rpc-1.1.1/quart_rpc/version_1_0/rpc.py` & `quart_rpc-1.2.0/quart_rpc/version_1_0/rpc.py`

 * *Files identical despite different names*

### Comparing `quart_rpc-1.1.1/quart_rpc/version_1_0/utilities.py` & `quart_rpc-1.2.0/quart_rpc/version_1_0/utilities.py`

 * *Files identical despite different names*

### Comparing `quart_rpc-1.1.1/PKG-INFO` & `quart_rpc-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quart-rpc
-Version: 1.1.1
+Version: 1.2.0
 Summary: Turn Quart into a simple RPC server
 Author-email: David Carmichael <david@uilix.com>
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -21,16 +21,16 @@
 pip install quart-rpc
 ```
 
 ---
 
 The Quart implementation of [Flask-RPC](https://github.com/CheeseCake87/flask-rpc)
 
-Quart-RPC uses wRPC (Wee RPC) as its protocol, which is a
-micro JSON-based protocol that allows for
+Quart-RPC uses [wRPC (Wee RPC)](https://github.com/CheeseCake87/wRPC) 
+as its protocol, which is a micro JSON-based protocol that allows for
 easy communication between the client and server.
 
 The typical request/response cycle is as follows:
 
 **Request**
 
 ```json
```

