# Comparing `tmp/ithaca_py-0.2.2.tar.gz` & `tmp/ithaca_py-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ithaca_py-0.2.2.tar", max compression
+gzip compressed data, was "ithaca_py-0.2.3.tar", max compression
```

## Comparing `ithaca_py-0.2.2.tar` & `ithaca_py-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      983 2024-04-19 12:36:32.426024 ithaca_py-0.2.2/README.md
--rw-r--r--   0        0        0     5147 2024-04-19 12:36:32.426024 ithaca_py-0.2.2/ithaca/__init__.py
--rw-r--r--   0        0        0     3656 2024-04-19 12:36:32.426024 ithaca_py-0.2.2/ithaca/analytics.py
--rw-r--r--   0        0        0    10809 2024-04-19 12:36:32.426024 ithaca_py-0.2.2/ithaca/auth.py
--rw-r--r--   0        0        0     5589 2024-04-19 12:36:32.426024 ithaca_py-0.2.2/ithaca/calculation.py
--rw-r--r--   0        0        0     3206 2024-04-19 12:36:32.426024 ithaca_py-0.2.2/ithaca/client.py
--rw-r--r--   0        0        0     1846 2024-04-19 12:36:32.426024 ithaca_py-0.2.2/ithaca/constants.py
--rw-r--r--   0        0        0    12592 2024-04-19 12:36:32.426024 ithaca_py-0.2.2/ithaca/fundlock.py
--rw-r--r--   0        0        0      603 2024-04-19 12:36:32.426024 ithaca_py-0.2.2/ithaca/market.py
--rw-r--r--   0        0        0     7370 2024-04-19 12:36:32.426024 ithaca_py-0.2.2/ithaca/orders.py
--rw-r--r--   0        0        0     1373 2024-04-19 12:36:32.426024 ithaca_py-0.2.2/ithaca/protocol.py
--rw-r--r--   0        0        0     2210 2024-04-19 12:36:32.430024 ithaca_py-0.2.2/ithaca/socket.py
--rw-r--r--   0        0        0      929 2024-04-19 12:36:32.430024 ithaca_py-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 ithaca_py-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      983 2024-04-24 03:55:39.458822 ithaca_py-0.2.3/README.md
+-rw-r--r--   0        0        0     5147 2024-04-24 03:55:39.458822 ithaca_py-0.2.3/ithaca/__init__.py
+-rw-r--r--   0        0        0     3656 2024-04-24 03:55:39.458822 ithaca_py-0.2.3/ithaca/analytics.py
+-rw-r--r--   0        0        0    10809 2024-04-24 03:55:39.458822 ithaca_py-0.2.3/ithaca/auth.py
+-rw-r--r--   0        0        0     5589 2024-04-24 03:55:39.458822 ithaca_py-0.2.3/ithaca/calculation.py
+-rw-r--r--   0        0        0     3206 2024-04-24 03:55:39.462822 ithaca_py-0.2.3/ithaca/client.py
+-rw-r--r--   0        0        0     1846 2024-04-24 03:55:39.462822 ithaca_py-0.2.3/ithaca/constants.py
+-rw-r--r--   0        0        0    12592 2024-04-24 03:55:39.462822 ithaca_py-0.2.3/ithaca/fundlock.py
+-rw-r--r--   0        0        0      603 2024-04-24 03:55:39.462822 ithaca_py-0.2.3/ithaca/market.py
+-rw-r--r--   0        0        0     7370 2024-04-24 03:55:39.462822 ithaca_py-0.2.3/ithaca/orders.py
+-rw-r--r--   0        0        0     1373 2024-04-24 03:55:39.462822 ithaca_py-0.2.3/ithaca/protocol.py
+-rw-r--r--   0        0        0     2534 2024-04-24 03:55:39.462822 ithaca_py-0.2.3/ithaca/socket.py
+-rw-r--r--   0        0        0      929 2024-04-24 03:55:39.462822 ithaca_py-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 ithaca_py-0.2.3/PKG-INFO
```

### Comparing `ithaca_py-0.2.2/README.md` & `ithaca_py-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.2/ithaca/__init__.py` & `ithaca_py-0.2.3/ithaca/__init__.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.2/ithaca/analytics.py` & `ithaca_py-0.2.3/ithaca/analytics.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.2/ithaca/auth.py` & `ithaca_py-0.2.3/ithaca/auth.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.2/ithaca/calculation.py` & `ithaca_py-0.2.3/ithaca/calculation.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.2/ithaca/client.py` & `ithaca_py-0.2.3/ithaca/client.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.2/ithaca/constants.py` & `ithaca_py-0.2.3/ithaca/constants.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.2/ithaca/fundlock.py` & `ithaca_py-0.2.3/ithaca/fundlock.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.2/ithaca/market.py` & `ithaca_py-0.2.3/ithaca/market.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.2/ithaca/orders.py` & `ithaca_py-0.2.3/ithaca/orders.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.2/ithaca/protocol.py` & `ithaca_py-0.2.3/ithaca/protocol.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.2/ithaca/socket.py` & `ithaca_py-0.2.3/ithaca/socket.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,18 @@
     def __on_open(self, ws):
         print("socket connection open...\n")
         params = {
             "action": "VALIDATE_AUTH_TOKEN",
             "payload": self.parent.user.get("authToken"),
         }
         ws.send(dumps(params))
+        params = {
+            "action": "SUBSCRIBE_ORDER_BOOK",
+        }
+        ws.send(dumps(params))
         print(params)
 
     def __on_error(self, ws, error):
         print(error)
 
     def __on_close(self, wsapp, close_status_code, close_msg):
         print("on_close args:")
@@ -48,22 +52,29 @@
             #         quantity = leg["originalQty"]
             #         print(
             #             f"       {side} {quantity} {payoff} @ {strike} for {expiry}",
             #         )
         else:
             print(data)
 
-    def connect(self):
+    def connect(self, on_message = None):
         """Attempt to connect to the websocket endpoint."""
+        print("connect: start: " + self.parent.ws_url)
+        print("auth: " + self.parent.user.get("authToken"))
+
+        if on_message is None:
+            on_message = self.__on_message
+
         ws = websocket.WebSocketApp(
             url=self.parent.ws_url,
-            on_message=self.__on_message,
+            on_message=on_message,
             on_error=self.__on_error,
             on_close=self.__on_close,
             on_open=self.__on_open,
         )
         sslopt = (
             {"cert_reqs": ssl.CERT_NONE}
             if "localhost" in self.parent.base_url
             else None
         )
-        ws.run_forever(ping_interval=14, sslopt=sslopt)
+
+        ws.run_forever(ping_interval=14, sslopt=sslopt, reconnect=10)
```

### Comparing `ithaca_py-0.2.2/pyproject.toml` & `ithaca_py-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ithaca_py"
-version = "0.2.2"
+version = "0.2.3"
 description = "Ithaca Protocol SDK"
 authors = ["nhaga <nhaga5@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ithaca"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `ithaca_py-0.2.2/PKG-INFO` & `ithaca_py-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ithaca_py
-Version: 0.2.2
+Version: 0.2.3
 Summary: Ithaca Protocol SDK
 Author: nhaga
 Author-email: nhaga5@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

