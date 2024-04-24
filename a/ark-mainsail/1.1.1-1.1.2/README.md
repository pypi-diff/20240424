# Comparing `tmp/ark-mainsail-1.1.1.tar.gz` & `tmp/ark-mainsail-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ark-mainsail-1.1.1.tar", last modified: Sun Apr 21 16:02:58 2024, max compression
+gzip compressed data, was "ark-mainsail-1.1.2.tar", last modified: Wed Apr 24 18:09:41 2024, max compression
```

## Comparing `ark-mainsail-1.1.1.tar` & `ark-mainsail-1.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 16:02:58.104925 ark-mainsail-1.1.1/
--rw-rw-rw-   0        0        0     1063 2024-03-31 14:12:30.000000 ark-mainsail-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     4263 2024-04-21 16:02:58.099959 ark-mainsail-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-21 16:02:58.095949 ark-mainsail-1.1.1/ark_mainsail.egg-info/
--rw-rw-rw-   0        0        0     4263 2024-04-21 16:02:57.000000 ark-mainsail-1.1.1/ark_mainsail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      936 2024-04-21 16:02:57.000000 ark-mainsail-1.1.1/ark_mainsail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 16:02:57.000000 ark-mainsail-1.1.1/ark_mainsail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-21 16:02:57.000000 ark-mainsail-1.1.1/ark_mainsail.egg-info/requires.txt
--rw-rw-rw-   0        0        0       40 2024-04-21 16:02:57.000000 ark-mainsail-1.1.1/ark_mainsail.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-21 16:02:58.003199 ark-mainsail-1.1.1/mainsail/
--rw-rw-rw-   0        0        0     1924 2024-04-13 21:52:02.000000 ark-mainsail-1.1.1/mainsail/__init__.py
--rw-rw-rw-   0        0        0      961 2024-04-07 19:01:11.000000 ark-mainsail-1.1.1/mainsail/config.py
--rw-rw-rw-   0        0        0     1585 2024-03-31 14:12:31.000000 ark-mainsail-1.1.1/mainsail/deserializer.py
--rw-rw-rw-   0        0        0     9663 2024-04-07 05:49:52.000000 ark-mainsail-1.1.1/mainsail/identity.py
--rw-rw-rw-   0        0        0     5204 2024-04-21 15:46:24.000000 ark-mainsail-1.1.1/mainsail/rest.py
--rw-rw-rw-   0        0        0     1884 2024-03-31 14:12:31.000000 ark-mainsail-1.1.1/mainsail/serializer.py
--rw-rw-rw-   0        0        0     9397 2024-04-21 10:35:01.000000 ark-mainsail-1.1.1/mainsail/transaction.py
-drwxrwxrwx   0        0        0        0 2024-04-21 16:02:58.029128 ark-mainsail-1.1.1/mainsail/tx/
--rw-rw-rw-   0        0        0     1424 2024-04-07 15:25:42.000000 ark-mainsail-1.1.1/mainsail/tx/__init__.py
--rw-rw-rw-   0        0        0     7080 2024-04-13 15:44:25.000000 ark-mainsail-1.1.1/mainsail/tx/v1.py
--rw-rw-rw-   0        0        0     5013 2024-04-21 15:08:34.000000 ark-mainsail-1.1.1/mainsail/webhook.py
-drwxrwxrwx   0        0        0        0 2024-04-21 16:02:58.068027 ark-mainsail-1.1.1/pool/
--rw-rw-rw-   0        0        0     4758 2024-04-21 13:47:11.000000 ark-mainsail-1.1.1/pool/__init__.py
--rw-rw-rw-   0        0        0     5350 2024-04-21 12:14:16.000000 ark-mainsail-1.1.1/pool/__main__.py
--rw-rw-rw-   0        0        0      956 2024-04-21 10:42:43.000000 ark-mainsail-1.1.1/pool/api.py
--rw-rw-rw-   0        0        0     9545 2024-04-21 15:08:51.000000 ark-mainsail-1.1.1/pool/biom.py
--rw-rw-rw-   0        0        0     9370 2024-04-20 13:43:34.000000 ark-mainsail-1.1.1/pool/tbw.py
--rw-rw-rw-   0        0        0       42 2024-04-21 16:02:58.104925 ark-mainsail-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1599 2024-04-20 18:25:10.000000 ark-mainsail-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 16:02:58.093954 ark-mainsail-1.1.1/test/
--rw-rw-rw-   0        0        0       25 2024-04-01 18:54:30.000000 ark-mainsail-1.1.1/test/__init__.py
--rw-rw-rw-   0        0        0     1765 2024-04-06 14:10:01.000000 ark-mainsail-1.1.1/test/test_identity.py
--rw-rw-rw-   0        0        0     3635 2024-04-20 11:21:27.000000 ark-mainsail-1.1.1/test/test_v1_builders.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:09:41.944076 ark-mainsail-1.1.2/
+-rw-rw-rw-   0        0        0     1063 2024-03-31 14:12:30.000000 ark-mainsail-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     4281 2024-04-24 18:09:41.942081 ark-mainsail-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 18:09:41.940087 ark-mainsail-1.1.2/ark_mainsail.egg-info/
+-rw-rw-rw-   0        0        0     4281 2024-04-24 18:09:41.000000 ark-mainsail-1.1.2/ark_mainsail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      936 2024-04-24 18:09:41.000000 ark-mainsail-1.1.2/ark_mainsail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 18:09:41.000000 ark-mainsail-1.1.2/ark_mainsail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-24 18:09:41.000000 ark-mainsail-1.1.2/ark_mainsail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       40 2024-04-24 18:09:41.000000 ark-mainsail-1.1.2/ark_mainsail.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 18:09:41.907174 ark-mainsail-1.1.2/mainsail/
+-rw-rw-rw-   0        0        0     1924 2024-04-13 21:52:02.000000 ark-mainsail-1.1.2/mainsail/__init__.py
+-rw-rw-rw-   0        0        0      961 2024-04-07 19:01:11.000000 ark-mainsail-1.1.2/mainsail/config.py
+-rw-rw-rw-   0        0        0     1585 2024-03-31 14:12:31.000000 ark-mainsail-1.1.2/mainsail/deserializer.py
+-rw-rw-rw-   0        0        0     9663 2024-04-07 05:49:52.000000 ark-mainsail-1.1.2/mainsail/identity.py
+-rw-rw-rw-   0        0        0     5204 2024-04-21 15:46:24.000000 ark-mainsail-1.1.2/mainsail/rest.py
+-rw-rw-rw-   0        0        0     1884 2024-03-31 14:12:31.000000 ark-mainsail-1.1.2/mainsail/serializer.py
+-rw-rw-rw-   0        0        0     9397 2024-04-21 10:35:01.000000 ark-mainsail-1.1.2/mainsail/transaction.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:09:41.911163 ark-mainsail-1.1.2/mainsail/tx/
+-rw-rw-rw-   0        0        0     1424 2024-04-07 15:25:42.000000 ark-mainsail-1.1.2/mainsail/tx/__init__.py
+-rw-rw-rw-   0        0        0     7080 2024-04-13 15:44:25.000000 ark-mainsail-1.1.2/mainsail/tx/v1.py
+-rw-rw-rw-   0        0        0     5013 2024-04-21 15:08:34.000000 ark-mainsail-1.1.2/mainsail/webhook.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:09:41.929120 ark-mainsail-1.1.2/pool/
+-rw-rw-rw-   0        0        0     4840 2024-04-24 08:02:47.000000 ark-mainsail-1.1.2/pool/__init__.py
+-rw-rw-rw-   0        0        0     5358 2024-04-23 19:26:57.000000 ark-mainsail-1.1.2/pool/__main__.py
+-rw-rw-rw-   0        0        0     1251 2024-04-24 08:02:26.000000 ark-mainsail-1.1.2/pool/api.py
+-rw-rw-rw-   0        0        0    11508 2024-04-24 18:05:21.000000 ark-mainsail-1.1.2/pool/biom.py
+-rw-rw-rw-   0        0        0     9519 2024-04-24 05:58:10.000000 ark-mainsail-1.1.2/pool/tbw.py
+-rw-rw-rw-   0        0        0       42 2024-04-24 18:09:41.944076 ark-mainsail-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1599 2024-04-24 09:12:19.000000 ark-mainsail-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:09:41.937094 ark-mainsail-1.1.2/test/
+-rw-rw-rw-   0        0        0       25 2024-04-01 18:54:30.000000 ark-mainsail-1.1.2/test/__init__.py
+-rw-rw-rw-   0        0        0     1765 2024-04-06 14:10:01.000000 ark-mainsail-1.1.2/test/test_identity.py
+-rw-rw-rw-   0        0        0     3635 2024-04-20 11:21:27.000000 ark-mainsail-1.1.2/test/test_v1_builders.py
```

### Comparing `ark-mainsail-1.1.1/LICENSE` & `ark-mainsail-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.1.1/PKG-INFO` & `ark-mainsail-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ark-mainsail
-Version: 1.1.1
+Version: 1.1.2
 Summary: Interact with ARK blockchain and forks
 Home-page: https://github.com/Moustikitos/python-mainsail
 Author: Toons
 Author-email: moustikitos@gmail.com
 Maintainer: Toons
 Maintainer-email: moustikitos@gmail.com
 License: Copyright 2024, MIT licence
@@ -119,15 +119,15 @@
 * [x] MultiPayment
 * [x] ValidatorResignation
 * [x] UsernameRegistration
 * [x] UsernameResignation
 
 ## Features
 
-* [x] pool managment tools
+* [x] pool server with remote managment tool
 * [x] secured private keys storage
 * [x] secured webhook subscriptions storage
 * [x] offline network configuration available
 
 ## Support this project
 
 <!-- [![Liberapay receiving](https://img.shields.io/liberapay/goal/Toons?logo=liberapay)](https://liberapay.com/Toons/donate) -->
```

### Comparing `ark-mainsail-1.1.1/ark_mainsail.egg-info/PKG-INFO` & `ark-mainsail-1.1.2/ark_mainsail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ark-mainsail
-Version: 1.1.1
+Version: 1.1.2
 Summary: Interact with ARK blockchain and forks
 Home-page: https://github.com/Moustikitos/python-mainsail
 Author: Toons
 Author-email: moustikitos@gmail.com
 Maintainer: Toons
 Maintainer-email: moustikitos@gmail.com
 License: Copyright 2024, MIT licence
@@ -119,15 +119,15 @@
 * [x] MultiPayment
 * [x] ValidatorResignation
 * [x] UsernameRegistration
 * [x] UsernameResignation
 
 ## Features
 
-* [x] pool managment tools
+* [x] pool server with remote managment tool
 * [x] secured private keys storage
 * [x] secured webhook subscriptions storage
 * [x] offline network configuration available
 
 ## Support this project
 
 <!-- [![Liberapay receiving](https://img.shields.io/liberapay/goal/Toons?logo=liberapay)](https://liberapay.com/Toons/donate) -->
```

### Comparing `ark-mainsail-1.1.1/ark_mainsail.egg-info/SOURCES.txt` & `ark-mainsail-1.1.2/ark_mainsail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.1.1/mainsail/__init__.py` & `ark-mainsail-1.1.2/mainsail/__init__.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.1.1/mainsail/config.py` & `ark-mainsail-1.1.2/mainsail/config.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.1.1/mainsail/deserializer.py` & `ark-mainsail-1.1.2/mainsail/deserializer.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.1.1/mainsail/identity.py` & `ark-mainsail-1.1.2/mainsail/identity.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.1.1/mainsail/rest.py` & `ark-mainsail-1.1.2/mainsail/rest.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.1.1/mainsail/serializer.py` & `ark-mainsail-1.1.2/mainsail/serializer.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.1.1/mainsail/transaction.py` & `ark-mainsail-1.1.2/mainsail/transaction.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.1.1/mainsail/tx/__init__.py` & `ark-mainsail-1.1.2/mainsail/tx/__init__.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.1.1/mainsail/tx/v1.py` & `ark-mainsail-1.1.2/mainsail/tx/v1.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.1.1/mainsail/webhook.py` & `ark-mainsail-1.1.2/mainsail/webhook.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.1.1/pool/__init__.py` & `ark-mainsail-1.1.2/pool/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,20 +77,20 @@
             data = json.loads(flask.request.data).get("data", {})
             conf = dict(
                 loadJson(path), **dict(
                     [k, v] for k, v in data.items() if k in CONF_PARAMETERS
                 )
             )
             dumpJson(conf, path, ensure_ascii=False)
-            return flask.jsonify({"status": 204}), 204
+            return flask.jsonify({"status": 204}), 200
     else:
-        return flask.jsonify({"status": 403}), 403
+        return flask.jsonify({"status": 403}), 200
 
 
-@app.route("/configure/delegate/", methods=["POST", "GET"])
+@app.route("/configure/delegate", methods=["POST"])
 def configure_delegate() -> flask.Response:
     if biom.check_headers(flask.request.headers):
         puk = flask.request.headers["puk"]
         path = os.path.join(tbw.DATA, f"{puk}.json")
         data = json.loads(flask.request.data)
         info = dict(
             loadJson(path), **dict(
@@ -98,20 +98,17 @@
                 if k in biom.DELEGATE_PARAMETERS.keys()
             )
         )
         if flask.request.method == "POST":
             LOGGER.debug(f"---- received> {data}")
             LOGGER.info(f"updating {puk} info> {info}")
             dumpJson(info, path, ensure_ascii=False)
-            return flask.jsonify({"status": 204, "updated": data}), 204
-        else:
-            info.pop("prk", None)
-            return flask.jsonify(info), 200
+            return flask.jsonify({"status": 204, "updated": data}), 200
     else:
-        return flask.jsonify({"status": 403}), 403
+        return flask.jsonify({"status": 403}), 200
 
 
 @app.route("/block/forged", methods=["POST", "GET"])
 def block_forged() -> flask.Response:
     check = False
     if flask.request.method == "POST":
         check = webhook.verify(
@@ -121,18 +118,23 @@
         if check is True and flask.request.data != b'':
             data = json.loads(flask.request.data)
             block = data.get("data", {}).get("block", {}).get("data", {})
             LOGGER.debug("block received> %s", block)
             JOB.put(block)
         else:
             check = False
-    return flask.jsonify({"acknowledge": check}), 200 if check else 403
+    return flask.jsonify({"acknowledge": check}), 200
 
 
 def main():
+    """
+    Server main loop ran as a `threading.Thread` target. It gets block
+    passed by `block_forged` (`/block/forged` endpoint) and update forgery
+    of validator issuing the block.
+    """
     LOGGER.info("entering main loop")
     while True:
         block = JOB.get()
         if block not in [False, None]:
             lock = biom.acquireLock()
             try:
                 result = tbw.update_forgery(block)
```

### Comparing `ark-mainsail-1.1.1/pool/__main__.py` & `ark-mainsail-1.1.2/pool/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                 LOGGER.info(
                     f"{puk}: "
                     f"block delay<{block_delay}> - forged blocks<{blocks}>"
                 )
                 if blocks > block_delay:
                     lock = biom.acquireLock()
                     try:
-                        tbw.freeze_forgery(puk)
+                        tbw.freeze_forgery(puk, **info)
                     except Exception:
                         LOGGER.exception("---- error occured>")
                     else:
                         LOGGER.info(f"{puk} forgery frozen")
                     finally:
                         biom.releaseLock(lock)
                     tbw.bake_registry(puk)
```

### Comparing `ark-mainsail-1.1.1/pool/api.py` & `ark-mainsail-1.1.2/pool/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,23 +8,30 @@
 
 @app.route("/<string:puk>", methods=["GET"])
 def delegate(puk: str) -> flask.Response:
     info = loadJson(os.path.join(tbw.DATA, f"{puk}.json"))
     if len(info):
         info.pop("prk", False)
         return flask.jsonify(info), 200
-    return flask.jsonify({"status": 404}), 404
+    return flask.jsonify({"status": 404}), 200
 
 
 @app.route("/<string:puk>/forgery", methods=["GET"])
 def forgery(puk: str) -> flask.Response:
     path = os.path.join(tbw.DATA, puk, "forgery.json")
     if os.path.exists(path):
-        return flask.jsonify(loadJson(path)), 200
-    return flask.jsonify({"status": 404}), 404
+        forgery = loadJson(path)
+        forgery.pop("reward", False)
+        for k in forgery:
+            if k not in ["blocks", "contributions"]:
+                forgery[k] /= tbw.XTOSHI
+        for k in forgery.get("contributions", {}):
+            forgery["contributions"][k] /= tbw.XTOSHI
+        return flask.jsonify(forgery), 200
+    return flask.jsonify({"status": 404}), 200
 
 
 def run(debug: bool = True) -> flask.Flask:
     global app, MAIN
 
     MAIN = threading.Thread(target=main)
     MAIN.daemon = True
```

### Comparing `ark-mainsail-1.1.1/pool/biom.py` & `ark-mainsail-1.1.2/pool/biom.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 # -*- coding: utf-8 -*-
 
 import io
 import os
 import re
 import sys
-import json
+import math
+import time
 import base58
 import getpass
 import logging
+import datetime
 import requests
 
+from datetime import timezone
 from urllib import parse
 from pool import tbw
 from mainsail import identity, rest, webhook, dumpJson, loadJson
 from typing import Union, List
 
 # set basic logging
 logging.basicConfig()
 LOGGER = logging.getLogger(__name__)
-LOGGER.setLevel(logging.INFO)
+LOGGER.setLevel(logging.DEBUG)
 
 DELEGATE_PARAMETERS = {
     "share": float,
     "min_vote": float,
     "max_vote": float,
-    "peer": dict,
+    "min_share": float,
     "excludes": list,
     "block_delay": int,
     "message": str,
-    "chunck_size": int
+    "chunck_size": int,
+    "wallet": str
 }
 
 try:
     import fcntl
 
     def acquireLock():
         '''acquire exclusive lock file access'''
@@ -77,35 +81,53 @@
         LOGGER.info("global lock released")
 
 
 class IdentityError(Exception):
     pass
 
 
+def get_nonces():
+    base_time = math.ceil(time.time()/5) * 5
+    datetimes = [
+        datetime.datetime.fromtimestamp(base_time + n)
+        .astimezone(timezone.utc).strftime("%Y-%m-%H%m%S").encode("utf-8")
+        for n in [-5, 0]
+    ]
+    return [
+        identity.cSecp256k1.hash_sha256(dt).decode("utf-8")
+        for dt in datetimes
+    ]
+
+
 def secure_headers(
     headers: dict = {},
     prk: Union[identity.KeyRing, List[int], str, int] = None
 ) -> dict:
     if isinstance(prk, list):
         prk = identity.KeyRing.load(prk)
     elif not isinstance(prk, identity.KeyRing):
         prk = identity.KeyRing.create(prk)
-    nonce = os.urandom(64).hex()
+    nonce = get_nonces()[-1]
     headers.update(
         nonce=nonce,
         sig=prk.sign(nonce).raw(),
         puk=prk.puk().encode()
     )
     return headers
 
 
 def check_headers(headers: dict) -> bool:
     try:
         path = os.path.join(tbw.DATA, f"{headers['puk']}.json")
-        if os.path.exists(path):
+        valid_nonces = get_nonces()
+        LOGGER.debug(
+            f"---- received nonce {headers['nonce']} - "
+            f"valid nonces: {'|'.join(valid_nonces)}"
+        )
+        if os.path.exists(path) and headers["nonce"] in valid_nonces:
             return identity.get_signer().verify(
                 headers["puk"], headers["nonce"], headers["sig"]
             )
     except KeyError:
         pass
     return False
 
@@ -179,83 +201,103 @@
     for arg in [a for a in sys.argv if "=" in a]:
         key, value = arg.split("=")
         key = key.replace("--", "").replace("-", "_")
         options[key] = value
     # manage parameters
     params = {}
     for key, value in options.items():
-        if key == "excludes":
+        if key == "port":
+            try:
+                params[key] = int(value)
+            except Exception:
+                LOGGER.info(
+                    f"conversion into {type(0)} impossible for {value}"
+                )
+        elif key == "wallet":
+            try:
+                base58.b58decode_check(value)
+            except Exception:
+                LOGGER.info(f"{value} is not a valid wallet address")
+            else:
+                params[key] = value
+        elif key == "excludes":
             addresses = []
             for address in [
                 addr.strip() for addr in value.split(",") if addr != ""
             ]:
                 try:
                     base58.b58decode_check(address)
                 except Exception:
-                    pass
+                    LOGGER.info(f"{address} is not a valid wallet address")
                 else:
                     addresses.append(address)
             params[key] = addresses
-        elif key == "peer":
-            try:
-                value = json.loads(value)
-            except Exception:
-                pass
-            else:
-                params[key] = addresses
         elif key in DELEGATE_PARAMETERS.keys():
             try:
                 params[key] = DELEGATE_PARAMETERS[key](value)
             except Exception:
-                pass
+                LOGGER.info(
+                    f"conversion into {DELEGATE_PARAMETERS[key]} "
+                    f"impossible for {value}"
+                )
+        else:
+            params[key] = value
     LOGGER.info(f"grabed options: {params}")
     return params
 
 
 def add_delegate(puk: str, **kwargs) -> None:
     # check identity
-    prk = identity.KeyRing.create()
+    prk = identity.KeyRing.create(kwargs.pop("prk", None))
     if prk.puk().encode() != puk:
         raise IdentityError(f"private key does not match public key {puk}")
-    # save private key
+    # secure private key using a pincode
+    # it will give the possibility to mnsl-bg service to sign transactions
     answer = ""
     while re.match(r"^[0-9]+$", answer) is None:
-        answer = getpass.getpass("enter pin code to secure secret> ")
+        answer = getpass.getpass(
+            "enter pin code to secure secret (only figures)> "
+        )
     pincode = [int(e) for e in answer]
     prk.dump(pincode)
     # reach a network
     while not hasattr(rest.config, "nethash"):
         try:
-            rest.use_network(input("provide a valid network peer> "))
+            rest.use_network(
+                input("provide a network peer API [default=localhost:4003]> ")
+                or "http://127.0.0.1:4003"
+            )
         except KeyboardInterrupt:
             print("\n")
             break
         except Exception as error:
             LOGGER.info("%r", error)
             pass
     # reach a valid subscription node
     webhook_peer = None
     while webhook_peer is None:
-        webhook_peer = input("provide a valid webhook peer> ") \
-            or "http://127.0.0.1:4004"
+        webhook_peer = input(
+            "provide your webhook peer [default=localhost:4004]> "
+        ) or "http://127.0.0.1:4004"
         try:
             resp = requests.head(f"{webhook_peer}/api/webhooks", timeout=2)
             if resp.status_code != 200:
                 webhook_peer = None
         except KeyboardInterrupt:
             print("\n")
             break
         except Exception as error:
             LOGGER.info("%r", error)
             webhook_peer = None
     # reach a valid target endpoint
     target_endpoint = None
     while target_endpoint is None:
-        target_endpoint = input("provide a valid target server> ") \
-            or "http://127.0.0.1:5000"
+        target_endpoint = input(
+            "provide your target server [default=localhost:5000]> "
+        ) or "http://127.0.0.1:5000"
         try:
             resp = requests.post(f"{target_endpoint}/block/forged", timeout=2)
             if resp.status_code not in [200, 403]:
                 target_endpoint = None
         except KeyboardInterrupt:
             print("\n")
             break
@@ -277,20 +319,29 @@
     path = os.path.join(tbw.DATA, f"{puk}.json")
     dumpJson(dict(options, **loadJson(path)), path, ensure_ascii=False)
     os.makedirs(os.path.join(tbw.DATA, puk), exist_ok=True)
     LOGGER.info(f"delegate {puk} set")
 
 
 def set_delegate(**kwargs) -> requests.Response:
-    # update from command line
+    # `peer` is just to be used inside this function so we pop it from kwargs
+    # if # found there
+    peer = kwargs.pop("peer", {})
+    # merge kwargs with command line
     options = _merge_options(**kwargs)
-    # asc pincode if no one is given
+    # because `ip` and `port` of remote pool can be set using command line args
+    # we pop them from here
+    if peer == {}:
+        peer["ip"] = options.pop("ip", "127.0.0.1")
+        peer["ports"] = {"requests": options.pop("port", 5000)}
+    # ask pincode if no one is given
+    answer = options.pop("pincode", "")
     if "pincode" not in options:
-        answer = ""
         while re.match(r"^[0-9]+$", answer) is None:
-            answer = getpass.getpass("enter validator secret pincode> ")
-    pincode = [int(e) for e in options.pop("pincode", answer)]
+            answer = getpass.getpass("enter validator security pincode> ")
+    pincode = [int(e) for e in answer]
+    # only valid delegate parameters available in `options` from there
     # secure POST headers and send parameters
     return rest.POST.configure.delegate(
-        peer=options.get("peer", {}), **options,
+        peer=peer, **options,
         headers=secure_headers(rest.POST.headers, pincode)
     )
```

### Comparing `ark-mainsail-1.1.1/pool/tbw.py` & `ark-mainsail-1.1.2/pool/tbw.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 
     # 2. GET FEES AND REWARDS SINCE LAST FORGED BLOCK
     last_block = loadJson(os.path.join(DATA, publicKey, "last.block"))
     # If no block found save the first one and exit.
     if last_block == {}:
         dumpJson(block, os.path.join(DATA, publicKey, "last.block"))
         return False
-
     blocks = 1
     reward = int(block["reward"])
     fee = int(block["totalFee"])
     # get all unparsed blocks till the last forged
     unparsed_blocks, page, last_height = [], 1, last_block["height"]
     while page > 0:  # infinite loop
         resp = rest.GET.api.delegates(
@@ -114,36 +113,26 @@
             )
         )
     ] for address in voters_weight)
     forgery["reward"] = forgery.get("reward", 0) + generator_reward
     forgery["blocks"] = forgery.get("blocks", 0) + blocks
     forgery["fee"] = forgery.get("fee", 0) + fee
     forgery["contributions"] = new_contributions
-    # compute checksum to determine lost XTOSHI due to roundings
-    checksum = (sum(new_contributions.values()) + forgery["reward"]) / XTOSHI
-    checksum /= max(1, forgery["blocks"])
-    checksum *= XTOSHI
-    lost = float(rest.config.constants["reward"]) - checksum
-    LOGGER.info(f"checksum: {checksum:.3f} -> {lost:.3f} XTOSHI lost")
-    if lost >= len(voters):
-        for voter in forgery["contributions"]:
-            forgery["contributions"][voter] += 1
-        lost -= len(voters)
-        LOGGER.info(
-            f"redistribution of {lost:d} lost XTOSHI to {len(voters)} voters "
-            "done"
-        )
-    forgery["lost"] = round(lost, 3)
+    # compute checksum to determine XTOSHI
+    checksum = (sum(new_contributions.values()) + forgery["reward"])
+    checksum -= int(rest.config.constants["reward"]) * forgery["blocks"]
+    checksum -= forgery.get("undistributed", 0)
+    LOGGER.info(f"losed XTOSHI: {checksum}")
     # update true block weight state
     dumpJson(block, os.path.join(DATA, publicKey, "last.block"))
     dumpJson(forgery, os.path.join(DATA, publicKey, "forgery.json"))
     LOGGER.info(
         f"{shared_reward / XTOSHI} token distributed to {len(voters)} voters "
         f"- {generator_reward / XTOSHI} token plus {fee / XTOSHI} fee added "
-        f"to {identity.get_wallet(publicKey)} share"
+        f"to {info.get('wallet', identity.get_wallet(publicKey))} share"
     )
 
     # 5. PRINT VOTE CHANGES
     for downvoter in list(set(contributions.keys()) - set(voters.keys())):
         LOGGER.info(
             f"{downvoter} downvoted {publicKey} : "
             f"{contributions[downvoter] / XTOSHI:.8f} token leaved"
@@ -155,36 +144,41 @@
         )
 
     # Exit with True means 5 steps gone straight.
     return True
 
 
 def freeze_forgery(puk: str, **options) -> None:
-    min_share = options.get("min_share", 1) * XTOSHI
+    min_share = options.get("min_share", 1.0) * XTOSHI
     forgery = loadJson(os.path.join(DATA, puk, "forgery.json"))
     tbw = {
         "timestamp": f"{datetime.datetime.now()}",
         "validator-share": forgery.get("reward", 0) + forgery.get("fee", 0),
         "voter-shares": dict(
             [voter, amount]
             for voter, amount in forgery.get("contributions", {}).items()
             if amount >= min_share
         )
     }
     dumpJson(
         tbw, os.path.join(DATA, puk, f"{time.strftime('%Y%m%d-%H%M')}.forgery")
     )
-
     forgery.pop("blocks", 0)
     forgery.pop("reward", 0)
     forgery.pop("fee", 0)
-    forgery["contributions"] = dict(
+    contributions = dict(
         [voter, 0 if voter in tbw["voter-shares"] else amount]
         for voter, amount in forgery.get("contributions", {}).items()
     )
+    forgery["contributions"] = contributions
+    forgery["undistributed"] = sum(contributions.values())
+    LOGGER.info(
+        f"forgery frozen @ {time.strftime('%Y%m%d-%H%M')} - "
+        f"{forgery['undistributed']} XTOSHI undistributed"
+    )
     dumpJson(forgery, os.path.join(DATA, puk, "forgery.json"))
 
 
 def bake_registry(puk: str) -> None:
     info = loadJson(os.path.join(DATA, f"{puk}.json"))
     names = [
         name.split(".")[0] for name in os.listdir(os.path.join(DATA, puk))
@@ -192,24 +186,28 @@
     ]
     if len(names):
         prk = identity.KeyRing.load(info.get("prk", None))
         rest.load_network(info["nethash"])
         wallet = rest.GET.api.wallets(puk)
         nonce = int(wallet.get("nonce", 0)) + 1
         for name in names:
+            LOGGER.info(f"baking registry for {name} frozen forgery...")
             registry = []
             tbw = loadJson(os.path.join(DATA, puk, f"{name}.forgery"))
             share = Transfer(
-                tbw["validator-share"] / XTOSHI, wallet["address"],
-                f"{puk} reward"
+                tbw["validator-share"] / XTOSHI,
+                info.get("wallet", wallet["address"]),
+                f"\U0001f4b3 {wallet.get('username', puk)} reward"
             )
             share.sign(prk, nonce=nonce)
             registry.append(share.serialize())
 
-            message = info.get("message", "Voter share")
+            message = info.get(
+                "message", f"\U0001f4b3 {wallet.get('username', puk)} share"
+            )
             voter_shares = tbw.get("voter-shares", {})
             if len(voter_shares) <= 2:
                 for address, amount in voter_shares.items():
                     nonce += 1
                     transfer = Transfer(amount / XTOSHI, address, message)
                     transfer.sign(prk, nonce=nonce)
                     registry.append(transfer.serialize())
@@ -230,7 +228,8 @@
                 dumpJson(
                     tbw, os.path.join(DATA, puk, "forgery", f"{name}.forgery")
                 )
             except Exception:
                 pass
             else:
                 os.remove(os.path.join(DATA, puk, f"{name}.forgery"))
+            LOGGER.info(f"{len(registry)} transactions baked")
```

### Comparing `ark-mainsail-1.1.1/setup.py` & `ark-mainsail-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 
 with open("README.md") as f2:
     LONG_DESCRIPTION = f2.read()
 
 kw = {
-    "version": "1.1.1",
+    "version": "1.1.2",
     "name": "ark-mainsail",
     "keywords": ["api", "ark", "blockchain"],
     "author": "Toons",
     "author_email": "moustikitos@gmail.com",
     "maintainer": "Toons",
     "maintainer_email": "moustikitos@gmail.com",
     "url": "https://github.com/Moustikitos/python-mainsail",
```

### Comparing `ark-mainsail-1.1.1/test/test_identity.py` & `ark-mainsail-1.1.2/test/test_identity.py`

 * *Files identical despite different names*

### Comparing `ark-mainsail-1.1.1/test/test_v1_builders.py` & `ark-mainsail-1.1.2/test/test_v1_builders.py`

 * *Files identical despite different names*

