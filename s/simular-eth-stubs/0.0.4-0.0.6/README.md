# Comparing `tmp/simular-eth-stubs-0.0.4.tar.gz` & `tmp/simular-eth-stubs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simular-eth-stubs-0.0.4.tar", last modified: Wed Apr 24 02:35:36 2024, max compression
+gzip compressed data, was "simular-eth-stubs-0.0.6.tar", last modified: Wed Apr 24 03:36:52 2024, max compression
```

## Comparing `simular-eth-stubs-0.0.4.tar` & `simular-eth-stubs-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-24 02:35:36.210000 simular-eth-stubs-0.0.4/
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)     5314 2024-04-24 02:35:36.210000 simular-eth-stubs-0.0.4/PKG-INFO
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)     3980 2024-04-24 02:33:35.000000 simular-eth-stubs-0.0.4/README.md
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)       38 2024-04-24 02:35:36.210000 simular-eth-stubs-0.0.4/setup.cfg
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)      464 2024-04-24 02:34:24.000000 simular-eth-stubs-0.0.4/setup.py
-drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-24 02:35:36.210000 simular-eth-stubs-0.0.4/simular_eth_stubs.egg-info/
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)     5314 2024-04-24 02:35:35.000000 simular-eth-stubs-0.0.4/simular_eth_stubs.egg-info/PKG-INFO
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)      222 2024-04-24 02:35:36.000000 simular-eth-stubs-0.0.4/simular_eth_stubs.egg-info/SOURCES.txt
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)        1 2024-04-24 02:35:35.000000 simular-eth-stubs-0.0.4/simular_eth_stubs.egg-info/dependency_links.txt
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)       12 2024-04-24 02:35:35.000000 simular-eth-stubs-0.0.4/simular_eth_stubs.egg-info/requires.txt
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)       14 2024-04-24 02:35:35.000000 simular-eth-stubs-0.0.4/simular_eth_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-24 03:36:52.420000 simular-eth-stubs-0.0.6/
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)     5333 2024-04-24 03:36:52.420000 simular-eth-stubs-0.0.6/PKG-INFO
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)     3991 2024-04-24 02:50:14.000000 simular-eth-stubs-0.0.6/README.md
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)       38 2024-04-24 03:36:52.420000 simular-eth-stubs-0.0.6/setup.cfg
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)      512 2024-04-24 03:21:01.000000 simular-eth-stubs-0.0.6/setup.py
+drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-24 03:36:52.420000 simular-eth-stubs-0.0.6/simular-stubs/
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)      116 2024-04-24 03:25:40.000000 simular-eth-stubs-0.0.6/simular-stubs/__init__.pyi
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)      791 2024-04-24 03:30:26.000000 simular-eth-stubs-0.0.6/simular-stubs/contract.pyi
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)     3840 2024-04-24 03:00:08.000000 simular-eth-stubs-0.0.6/simular-stubs/simular.pyi
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)      583 2024-04-24 03:20:31.000000 simular-eth-stubs-0.0.6/simular-stubs/utils.pyi
+drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-24 03:36:52.420000 simular-eth-stubs-0.0.6/simular_eth_stubs.egg-info/
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)     5333 2024-04-24 03:36:52.000000 simular-eth-stubs-0.0.6/simular_eth_stubs.egg-info/PKG-INFO
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)      286 2024-04-24 03:36:52.000000 simular-eth-stubs-0.0.6/simular_eth_stubs.egg-info/SOURCES.txt
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)        1 2024-04-24 03:36:52.000000 simular-eth-stubs-0.0.6/simular_eth_stubs.egg-info/dependency_links.txt
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)       14 2024-04-24 03:36:52.000000 simular-eth-stubs-0.0.6/simular_eth_stubs.egg-info/top_level.txt
```

### Comparing `simular-eth-stubs-0.0.4/PKG-INFO` & `simular-eth-stubs-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simular-eth-stubs
-Version: 0.0.4
+Version: 0.0.6
 Summary: Type stubs for simular-evm
 Home-page: https://github.com/james4ever0/simular-eth-stubs
 License: UNKNOWN
 Description: # Type stubs for simular-evm
         
         Fully documented type annotations for `PyEvm` and `PyAbi` in [simular-evm](https://pypi.org/project/simular-evm)
         
@@ -24,15 +24,15 @@
         
             def call(
                 self,
                 fn_name: str,
                 args: str,
                 to: str,
                 abi: PyAbi,
-            ):
+            ) -> object:
                 """
                 Transaction (read) operation to a contract at the given address `to`.
                 This will NOT change state in the EVM.
                 """
         
             def simulate(
                 self,
@@ -137,9 +137,10 @@
         
             def has_function(self, name: str) -> bool:
                 """Does the ABI contain the function `name`?"""
         
             def has_receive(self) -> bool:
                 """Does the contract have a receive function?"""
         ```
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `simular-eth-stubs-0.0.4/README.md` & `simular-eth-stubs-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     def call(
         self,
         fn_name: str,
         args: str,
         to: str,
         abi: PyAbi,
-    ):
+    ) -> object:
         """
         Transaction (read) operation to a contract at the given address `to`.
         This will NOT change state in the EVM.
         """
 
     def simulate(
         self,
@@ -130,8 +130,8 @@
         """Does the Contract have a fallback function?"""
 
     def has_function(self, name: str) -> bool:
         """Does the ABI contain the function `name`?"""
 
     def has_receive(self) -> bool:
         """Does the contract have a receive function?"""
-```
+```
```

### Comparing `simular-eth-stubs-0.0.4/simular_eth_stubs.egg-info/PKG-INFO` & `simular-eth-stubs-0.0.6/simular_eth_stubs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simular-eth-stubs
-Version: 0.0.4
+Version: 0.0.6
 Summary: Type stubs for simular-evm
 Home-page: https://github.com/james4ever0/simular-eth-stubs
 License: UNKNOWN
 Description: # Type stubs for simular-evm
         
         Fully documented type annotations for `PyEvm` and `PyAbi` in [simular-evm](https://pypi.org/project/simular-evm)
         
@@ -24,15 +24,15 @@
         
             def call(
                 self,
                 fn_name: str,
                 args: str,
                 to: str,
                 abi: PyAbi,
-            ):
+            ) -> object:
                 """
                 Transaction (read) operation to a contract at the given address `to`.
                 This will NOT change state in the EVM.
                 """
         
             def simulate(
                 self,
@@ -137,9 +137,10 @@
         
             def has_function(self, name: str) -> bool:
                 """Does the ABI contain the function `name`?"""
         
             def has_receive(self) -> bool:
                 """Does the contract have a receive function?"""
         ```
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

