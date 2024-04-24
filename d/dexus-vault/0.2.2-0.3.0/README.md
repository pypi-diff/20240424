# Comparing `tmp/dexus_vault-0.2.2.tar.gz` & `tmp/dexus_vault-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexus_vault-0.2.2.tar", last modified: Wed Apr 17 10:05:58 2024, max compression
+gzip compressed data, was "dexus_vault-0.3.0.tar", last modified: Wed Apr 24 12:04:52 2024, max compression
```

## Comparing `dexus_vault-0.2.2.tar` & `dexus_vault-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:58.847855 dexus_vault-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-04-17 10:05:58.847855 dexus_vault-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8158 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:58.843855 dexus_vault-0.2.2/dexus_vault/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:58.843855 dexus_vault-0.2.2/dexus_vault/grpc_dexidp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/grpc_dexidp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:58.843855 dexus_vault-0.2.2/dexus_vault/grpc_dexidp/dexidp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/grpc_dexidp/dexidp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/grpc_dexidp/dexidp/api_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    19894 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/grpc_dexidp/dexidp/api_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:58.843855 dexus_vault-0.2.2/dexus_vault/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/src/dex_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/src/vault_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:58.847855 dexus_vault-0.2.2/dexus_vault/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/utils/client_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/dexus_vault/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:58.847855 dexus_vault-0.2.2/dexus_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-04-17 10:05:58.000000 dexus_vault-0.2.2/dexus_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-17 10:05:58.000000 dexus_vault-0.2.2/dexus_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 10:05:58.000000 dexus_vault-0.2.2/dexus_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 10:05:58.000000 dexus_vault-0.2.2/dexus_vault.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-17 10:05:58.000000 dexus_vault-0.2.2/dexus_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 10:05:58.000000 dexus_vault-0.2.2/dexus_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 10:05:58.847855 dexus_vault-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-17 10:05:37.000000 dexus_vault-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:04:52.481134 dexus_vault-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-04-24 12:04:52.481134 dexus_vault-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:04:52.477134 dexus_vault-0.3.0/dexus_vault/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:04:52.481134 dexus_vault-0.3.0/dexus_vault/grpc_dexidp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/grpc_dexidp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:04:52.481134 dexus_vault-0.3.0/dexus_vault/grpc_dexidp/dexidp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/grpc_dexidp/dexidp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/grpc_dexidp/dexidp/api_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19894 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/grpc_dexidp/dexidp/api_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:04:52.481134 dexus_vault-0.3.0/dexus_vault/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/src/dex_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/src/vault_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/syncer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:04:52.481134 dexus_vault-0.3.0/dexus_vault/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/dexus_vault/utils/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:04:52.481134 dexus_vault-0.3.0/dexus_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-04-24 12:04:52.000000 dexus_vault-0.3.0/dexus_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-24 12:04:52.000000 dexus_vault-0.3.0/dexus_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:04:52.000000 dexus_vault-0.3.0/dexus_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 12:04:52.000000 dexus_vault-0.3.0/dexus_vault.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-24 12:04:52.000000 dexus_vault-0.3.0/dexus_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 12:04:52.000000 dexus_vault-0.3.0/dexus_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 12:04:52.481134 dexus_vault-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-24 12:04:42.000000 dexus_vault-0.3.0/setup.py
```

### Comparing `dexus_vault-0.2.2/LICENSE` & `dexus_vault-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.2.2/PKG-INFO` & `dexus_vault-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexus-vault
-Version: 0.2.2
+Version: 0.3.0
 Summary: Synchronizer of Dex clients with secrets in Vault
 Home-page: https://github.com/ifurs/dexus-vault
 Author: ifurs
 License: Apache License 2.0
 Project-URL: Source, https://github.com/ifurs/dexus-vault
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -21,14 +21,16 @@
 License-File: LICENSE
 Requires-Dist: grpcio~=1.62.0
 Requires-Dist: grpcio-tools~=1.60.1
 Requires-Dist: googleapis-common-protos>=1.62.0
 Requires-Dist: protobuf~=4.25.3
 Requires-Dist: hvac~=2.1.0
 Requires-Dist: prometheus_client~=0.20.0
+Requires-Dist: pydantic-settings~=2.2.1
+Requires-Dist: pydantic>=2.7.0
 
 # DEXUS VAULT
 
 [![Latest Github release](https://img.shields.io/github/tag/ifurs/dexus-vault.svg)](https://github.com/ifurs/dexus-vault/releases/latest)
 ![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)
 ![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)
 
@@ -150,26 +152,33 @@
 
 There are several authentication methods available:
 
 - Token-based authentication
 - LDAP authentication
 - Certificate-based authentication
 - AppRole authentication: To use this method, set `VAULT_APPROLE` to `true`. The HVAC client will then log into Vault using the default file mounted by the Vault agent by default, also there is possible to specify approle id and secret via env vars too.
+- Kubernetes authentication: To use this method, set variable `VAULT_KUBERNETES_ROLE` with role name
 
 ### Metrics
 
 For now "dexus-vault" publish simplified metrics, like this:
 
 ```bash
 client_create{status="ok"} 1.0
+client_delete{status="failed"} 3.0
+client_update{status="failed"} 0.0
+client_skip 5.0
+incorrect_secrets 2.0
 ```
 
-for "status" could be values "ok" and "failed"
+- labeled metrics(status): `client_create`, `client_delete`, `client_update`
+- non labeled: `client_skip` and `incorrect_secrets`
+for "status" label could be values "ok" and "failed"
 
-> **NOTE:** We plan to redesign the metrics system in the near future. Any contributions to this effort are greatly appreciated.
+> **NOTE:** Metrics are still under discussion. Any contributions to this effort are greatly appreciated.
 
 ## 🔒 Vault secret structure
 
 This example demonstrates all the parameters available for a client, which align with the Dex gRPC protocol message.
 
 ```json
 {
@@ -203,16 +212,16 @@
 - All gRPC API methods dexus_vault use, defined in [api.proto](https://github.com/dexidp/dex/blob/v2.38.0/api/v2/api.proto)
 and compiled with `grpc_tools.protoc`
 
 ## Roadmap
 
 Plans for future:
 
-- [ ] Redesign metrics concept to make it more Prometheus friendly
-- [ ] Switch to pydantic
+- [x] Redesign metrics concept to make it more Prometheus friendly
+- [x] Switch to pydantic
 - [ ] Implement functionality that tracks current clients state in Dex
 - [ ] Make logs more Fluent
 - [ ] Redesign dexus-vault to work like cli and accepts params
 - [ ] Implement feature to use other storage options
 
 ## 🔥 Thanks
```

### Comparing `dexus_vault-0.2.2/README.md` & `dexus_vault-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -122,26 +122,33 @@
 
 There are several authentication methods available:
 
 - Token-based authentication
 - LDAP authentication
 - Certificate-based authentication
 - AppRole authentication: To use this method, set `VAULT_APPROLE` to `true`. The HVAC client will then log into Vault using the default file mounted by the Vault agent by default, also there is possible to specify approle id and secret via env vars too.
+- Kubernetes authentication: To use this method, set variable `VAULT_KUBERNETES_ROLE` with role name
 
 ### Metrics
 
 For now "dexus-vault" publish simplified metrics, like this:
 
 ```bash
 client_create{status="ok"} 1.0
+client_delete{status="failed"} 3.0
+client_update{status="failed"} 0.0
+client_skip 5.0
+incorrect_secrets 2.0
 ```
 
-for "status" could be values "ok" and "failed"
+- labeled metrics(status): `client_create`, `client_delete`, `client_update`
+- non labeled: `client_skip` and `incorrect_secrets`
+for "status" label could be values "ok" and "failed"
 
-> **NOTE:** We plan to redesign the metrics system in the near future. Any contributions to this effort are greatly appreciated.
+> **NOTE:** Metrics are still under discussion. Any contributions to this effort are greatly appreciated.
 
 ## 🔒 Vault secret structure
 
 This example demonstrates all the parameters available for a client, which align with the Dex gRPC protocol message.
 
 ```json
 {
@@ -175,16 +182,16 @@
 - All gRPC API methods dexus_vault use, defined in [api.proto](https://github.com/dexidp/dex/blob/v2.38.0/api/v2/api.proto)
 and compiled with `grpc_tools.protoc`
 
 ## Roadmap
 
 Plans for future:
 
-- [ ] Redesign metrics concept to make it more Prometheus friendly
-- [ ] Switch to pydantic
+- [x] Redesign metrics concept to make it more Prometheus friendly
+- [x] Switch to pydantic
 - [ ] Implement functionality that tracks current clients state in Dex
 - [ ] Make logs more Fluent
 - [ ] Redesign dexus-vault to work like cli and accepts params
 - [ ] Implement feature to use other storage options
 
 ## 🔥 Thanks
```

### Comparing `dexus_vault-0.2.2/dexus_vault/__main__.py` & `dexus_vault-0.3.0/dexus_vault/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import threading
 
-from dexus_vault.client import run
+from dexus_vault.syncer import run
 from dexus_vault.utils.logger import logger
+from dexus_vault.__version__ import __title__, __version__  # noqa: F401
 
 # Try to import dotenv, if it's installed
 try:
     from dotenv import load_dotenv, find_dotenv
 
     load_dotenv(find_dotenv())
 except ImportError:
-    logger.debug(f"if you want to use .env file, please install python-dotenv")
+    logger.debug(f"If you want to use .env file, please install python-dotenv")
 
 
 def main():
     """
     Start a new thread to run the synchronization process.
     """
     try:
@@ -23,9 +24,9 @@
     except (KeyboardInterrupt, SystemExit):
         logger.info("Interrupt received, stopping...")
     except Exception as e:
         logger.error(f"An error occurred: {e}")
 
 
 if __name__ == "__main__":
-    logger.info("Starting dexus_vault...")
+    logger.info(f"Starting {__title__}, version {__version__}...")
     main()
```

### Comparing `dexus_vault-0.2.2/dexus_vault/grpc_dexidp/dexidp/api_pb2.py` & `dexus_vault-0.3.0/dexus_vault/grpc_dexidp/dexidp/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.2.2/dexus_vault/grpc_dexidp/dexidp/api_pb2_grpc.py` & `dexus_vault-0.3.0/dexus_vault/grpc_dexidp/dexidp/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dexus_vault-0.2.2/dexus_vault/src/dex_processor.py` & `dexus_vault-0.3.0/dexus_vault/src/dex_processor.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,152 +5,202 @@
 from google.protobuf.json_format import MessageToDict
 
 # Load GRPC Stub and Methods from pb2 defined using protobuf builder
 from dexus_vault.grpc_dexidp.dexidp.api_pb2_grpc import DexStub
 import dexus_vault.grpc_dexidp.dexidp.api_pb2 as pb2
 
 from dexus_vault.utils.logger import logger
-from dexus_vault.utils.metrics import client_create_metric, client_delete_metric
 
 
 class DexClient:
     """
     This class defines all logic for operating with Dex gRPC API
     """
 
     def __init__(self, config):
         # credentials used for Dex connection including GRPC URL
         self.config = config
-
         # channel credentials obj placeholder
         self.channel = self.dex_grpc_connect()
 
     # crete grpc connection to Dex
     def dex_grpc_connect(self) -> object:
         """
         Open connection to Dex gRPC
         """
 
-        if self.config["CLIENT_CRT"]:
-            self.creds = grpc.ssl_channel_credentials(
-                root_certificates=self.config["CA_CRT"],
-                private_key=self.config["CLIENT_KEY"],
-                certificate_chain=self.config["CLIENT_CRT"],
-            )
+        if self.config.client_crt and self.config.client_key:
+            # load credentials from files
+            with open(self.config.ca_crt, "r") as ca, open(
+                self.config.client_key, "r"
+            ) as key, open(self.config.client_crt, "r") as crt:
+
+                # define secure channel with credentials
+                self.creds = grpc.ssl_channel_credentials(
+                    root_certificates=ca.read(),
+                    private_key=key.read(),
+                    certificate_chain=crt.read(),
+                )
             return grpc.secure_channel(
-                target=self.config["DEX_GRPC_URL"], credentials=self.creds
+                target=self.config.dex_grpc_url, credentials=self.creds
             )
+
         else:
+            # insecure channel
             logger.debug(f"Dex client started in insecure channel")
-            return grpc.insecure_channel(target=self.config["DEX_GRPC_URL"])
+            return grpc.insecure_channel(target=self.config.dex_grpc_url)
 
     def dex_grpc_close_connection(self):
         """
         Close connection to Dex gRPC
         """
         if self.channel:
             self.channel.close()
 
+    # TODO: research more clean way for retrying connection
     def dex_waiter(self) -> bool:
         """
         Ensure connection to Dex gRPC
         """
         _retry = 0
         while True:
             try:
                 logger.info(f"Dex server version {self.get_dex_version()}")
                 return True
             except Exception as error:
-                if _retry >= self.config["DEX_MAX_RETRIES"]:
+                if _retry >= self.config.dex_max_retries:
                     raise RuntimeError(f"Could not connect to Dex gRPC server: {error}")
                 else:
                     _retry += 1
                     logger.debug(f"Dex gRPC is unavailable, retying...")
-                    time.sleep(self.config["DEX_RETRY_WAIT"])
+                    time.sleep(self.config.dex_retry_wait)
 
     def get_dex_version(self) -> dict:
         """
         Get Dex version
         """
         dex_request = pb2.VersionReq()
         response = DexStub(self.channel).GetVersion(dex_request)
-
         return MessageToDict(response)
 
     def get_dex_client(self, client_id: str) -> dict | None:
         """
-        Call Get Dex Client with by client id
+        Get Dex Client by id
         """
         dex_request = pb2.GetClientReq()
         dex_request.id = client_id
 
         try:
             response = DexStub(self.channel).GetClient(dex_request)
-            return MessageToDict(response)
+            return MessageToDict(response).get("client")
 
         except grpc.RpcError as rpc_error:
             if rpc_error.code() == grpc.StatusCode.UNKNOWN:
                 logger.debug(
-                    f"RESPONSE FROM GRPC: {rpc_error.details()}, client {client_id}"
+                    f"Dex gRPC response: {rpc_error.details()}, client {client_id}"
                 )
             else:
                 logger.warning(
-                    f"GRPC CALL CODE: {rpc_error.code()} with details {rpc_error.details()}"
+                    f"Dex gRPC error code: {rpc_error.code()} with details {rpc_error.details()}"
                 )
 
     def create_dex_client(self, client: dict) -> dict | None:
         """
         Create OIDC client in Dex
         """
         try:
+            # define MessageReq parameter for gRPC
             request = pb2.CreateClientReq()
-            request.client.id = client.get("id")
-            request.client.secret = client.get("secret")
-            request.client.redirect_uris.extend(client.get("redirect_uris", ""))
-            request.client.trusted_peers.extend(client.get("trusted_peers", ""))
-            request.client.public = client.get("public", 0)
-            request.client.name = client.get("name", "")
-            request.client.logo_url = client.get("logo_url", "")
-
+            request.client.id = client.id
+            request.client.secret = client.secret
+            request.client.redirect_uris.extend(client.redirect_uris)
+            request.client.trusted_peers.extend(client.trusted_peers)
+            request.client.public = client.public
+            request.client.name = client.name
+            request.client.logo_url = client.logo_url
+            # send request to Dex gRPC and store response
             response = MessageToDict(DexStub(self.channel).CreateClient(request))
+            # check if client was created
             if response.get("client", None) is not None:
                 client_id = response.get("client").get("id")
-                client_create_metric.labels(status="ok").inc()
                 logger.info(f"Created new Dex client '{client_id}'")
-                return client_id
+                return {
+                    "client": client_id,
+                    "operation": "create",
+                    "status": "ok",
+                    "response": response,
+                }
+            # check if client already exists returned from Dex
+            elif response.get("alreadyExists", None) is not None:
+                logger.info(
+                    f"Client {client.id} already exists, check Vault configs for duplicates"
+                )
+                return {
+                    "client": client.id,
+                    "operation": "create",
+                    "status": "skipped",
+                    "response": response,
+                }
+            # check if there was an error in response
             else:
-                logger.warning(f"RESPONSE FROM GRPC: {response}")
-
+                logger.warning(f"Dex gRPC response: {response}")
+                return {
+                    "client": client.id,
+                    "operation": "delete",
+                    "status": "failed",
+                    "response": response,
+                }
+        # catch any exception and log it
         except Exception as error:
-            client_create_metric.labels(status="failed").inc()
-            logger.error(f"Failed to create client {client.get('id')}")
-            logger.error(f"RESPONSE FROM GRPC: {error}")
+            logger.error(f"Failed to create client {client.id}")
+            logger.error(f"Dex gRPC response: {error}")
+            return {
+                "client": client.id,
+                "operation": "delete",
+                "status": "failed",
+                "response": error,
+            }
 
     def delete_dex_client(self, client_id: str) -> None:
         """
         Delete OIDC client in Dex
         """
         try:
             dex_request = pb2.DeleteClientReq()
             dex_request.id = client_id
 
-            # Because of Dex implementation, this request returns None
-            # Or simple dict {'notFound': True} so it need to be processed
+            # Returns None(means deleted) or {'notFound': True}, in other case it will raise an exception
             response = MessageToDict(DexStub(self.channel).DeleteClient(dex_request))
-
             if response.get("notFound", None) is not None:
-                client_delete_metric.labels(status="failed").inc()
                 logger.warning(f"Client '{client_id}' not found")
+                return {
+                    "client": client_id,
+                    "operation": "delete",
+                    "status": "skipped",
+                    "response": response,
+                }
+
             else:
-                client_create_metric.labels(status="ok").inc()
                 logger.info(f"client {client_id} was deleted")
+                return {
+                    "client": client_id,
+                    "operation": "delete",
+                    "status": "ok",
+                    "response": response,
+                }
+
         except Exception as error:
-            client_delete_metric.labels(status="failed").inc()
             logger.error(f"Failed to delete client {client_id}")
-            logger.error(f"RESPONSE FROM GRPC: {error}")
+            logger.error(f"Dex gRPC response: {error}")
+            return {
+                "client": client_id,
+                "operation": "delete",
+                "status": "failed",
+                "response": error,
+            }
 
     def __del__(self):
         """
         Every time DexClient object deletes, this will close gRPC connection
         """
         self.dex_grpc_close_connection()
         logger.debug(f"Dex connection closed")
```

### Comparing `dexus_vault-0.2.2/dexus_vault.egg-info/PKG-INFO` & `dexus_vault-0.3.0/dexus_vault.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexus-vault
-Version: 0.2.2
+Version: 0.3.0
 Summary: Synchronizer of Dex clients with secrets in Vault
 Home-page: https://github.com/ifurs/dexus-vault
 Author: ifurs
 License: Apache License 2.0
 Project-URL: Source, https://github.com/ifurs/dexus-vault
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -21,14 +21,16 @@
 License-File: LICENSE
 Requires-Dist: grpcio~=1.62.0
 Requires-Dist: grpcio-tools~=1.60.1
 Requires-Dist: googleapis-common-protos>=1.62.0
 Requires-Dist: protobuf~=4.25.3
 Requires-Dist: hvac~=2.1.0
 Requires-Dist: prometheus_client~=0.20.0
+Requires-Dist: pydantic-settings~=2.2.1
+Requires-Dist: pydantic>=2.7.0
 
 # DEXUS VAULT
 
 [![Latest Github release](https://img.shields.io/github/tag/ifurs/dexus-vault.svg)](https://github.com/ifurs/dexus-vault/releases/latest)
 ![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)
 ![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)
 
@@ -150,26 +152,33 @@
 
 There are several authentication methods available:
 
 - Token-based authentication
 - LDAP authentication
 - Certificate-based authentication
 - AppRole authentication: To use this method, set `VAULT_APPROLE` to `true`. The HVAC client will then log into Vault using the default file mounted by the Vault agent by default, also there is possible to specify approle id and secret via env vars too.
+- Kubernetes authentication: To use this method, set variable `VAULT_KUBERNETES_ROLE` with role name
 
 ### Metrics
 
 For now "dexus-vault" publish simplified metrics, like this:
 
 ```bash
 client_create{status="ok"} 1.0
+client_delete{status="failed"} 3.0
+client_update{status="failed"} 0.0
+client_skip 5.0
+incorrect_secrets 2.0
 ```
 
-for "status" could be values "ok" and "failed"
+- labeled metrics(status): `client_create`, `client_delete`, `client_update`
+- non labeled: `client_skip` and `incorrect_secrets`
+for "status" label could be values "ok" and "failed"
 
-> **NOTE:** We plan to redesign the metrics system in the near future. Any contributions to this effort are greatly appreciated.
+> **NOTE:** Metrics are still under discussion. Any contributions to this effort are greatly appreciated.
 
 ## 🔒 Vault secret structure
 
 This example demonstrates all the parameters available for a client, which align with the Dex gRPC protocol message.
 
 ```json
 {
@@ -203,16 +212,16 @@
 - All gRPC API methods dexus_vault use, defined in [api.proto](https://github.com/dexidp/dex/blob/v2.38.0/api/v2/api.proto)
 and compiled with `grpc_tools.protoc`
 
 ## Roadmap
 
 Plans for future:
 
-- [ ] Redesign metrics concept to make it more Prometheus friendly
-- [ ] Switch to pydantic
+- [x] Redesign metrics concept to make it more Prometheus friendly
+- [x] Switch to pydantic
 - [ ] Implement functionality that tracks current clients state in Dex
 - [ ] Make logs more Fluent
 - [ ] Redesign dexus-vault to work like cli and accepts params
 - [ ] Implement feature to use other storage options
 
 ## 🔥 Thanks
```

### Comparing `dexus_vault-0.2.2/dexus_vault.egg-info/SOURCES.txt` & `dexus_vault-0.3.0/dexus_vault.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 LICENSE
 README.md
 setup.py
 dexus_vault/__init__.py
 dexus_vault/__main__.py
 dexus_vault/__version__.py
-dexus_vault/client.py
+dexus_vault/syncer.py
 dexus_vault.egg-info/PKG-INFO
 dexus_vault.egg-info/SOURCES.txt
 dexus_vault.egg-info/dependency_links.txt
 dexus_vault.egg-info/entry_points.txt
 dexus_vault.egg-info/requires.txt
 dexus_vault.egg-info/top_level.txt
 dexus_vault/grpc_dexidp/__init__.py
 dexus_vault/grpc_dexidp/dexidp/__init__.py
 dexus_vault/grpc_dexidp/dexidp/api_pb2.py
 dexus_vault/grpc_dexidp/dexidp/api_pb2_grpc.py
 dexus_vault/src/__init__.py
 dexus_vault/src/dex_processor.py
 dexus_vault/src/vault_processor.py
 dexus_vault/utils/__init__.py
-dexus_vault/utils/client_parser.py
 dexus_vault/utils/config.py
-dexus_vault/utils/files.py
 dexus_vault/utils/logger.py
-dexus_vault/utils/metrics.py
-dexus_vault/utils/types.py
+dexus_vault/utils/metrics.py
```

### Comparing `dexus_vault-0.2.2/setup.py` & `dexus_vault-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,16 @@
     install_requires=[
         "grpcio~=1.62.0",
         "grpcio-tools~=1.60.1",
         "googleapis-common-protos>=1.62.0",
         "protobuf~=4.25.3",
         "hvac~=2.1.0",
         "prometheus_client~=0.20.0",
+        "pydantic-settings~=2.2.1",
+        "pydantic>=2.7.0",
     ],
     python_requires=">=3.8",
     project_urls={"Source": about["__url__"]},
     entry_points={
         "console_scripts": [f"{about['__title__']} = dexus_vault.__main__:main"]
     },
 )
```

