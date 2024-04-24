# Comparing `tmp/dpack_py-0.2.1.tar.gz` & `tmp/dpack_py-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpack_py-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dpack_py-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dpack_py-0.2.1.tar` & `dpack_py-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       27 2024-04-22 18:27:21.236302 dpack_py-0.2.1/.gitignore
--rw-r--r--   0        0        0      100 2024-04-22 18:30:45.593747 dpack_py-0.2.1/Makefile
--rw-r--r--   0        0        0     7398 2024-04-23 13:10:17.896775 dpack_py-0.2.1/examples/uniswap-v3.dpack.json
--rw-r--r--   0        0        0     2555 2024-04-23 13:10:09.129746 dpack_py-0.2.1/examples/uniswap.py
--rw-r--r--   0        0        0      555 2024-04-23 13:15:40.662308 dpack_py-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4636 2024-04-22 22:21:26.863611 dpack_py-0.2.1/readme.md
--rw-r--r--   0        0        0       55 2024-04-22 16:49:07.422511 dpack_py-0.2.1/src/dpack/__init__.py
--rw-r--r--   0        0        0     1198 2024-04-22 22:09:39.235312 dpack_py-0.2.1/src/dpack/ape.py
--rw-r--r--   0        0        0     3006 2024-04-23 13:15:23.502221 dpack_py-0.2.1/src/dpack/dpack.py
--rw-r--r--   0        0        0     2452 2024-04-23 13:15:18.878780 dpack_py-0.2.1/tests/test_dpack.py
--rw-r--r--   0        0        0    10293 2024-04-22 10:38:52.852458 dpack_py-0.2.1/tests/weth-ropsten-artifact.json
--rw-r--r--   0        0        0      723 2024-04-21 07:13:55.705183 dpack_py-0.2.1/tests/weth_ropsten.dpack.json
--rw-r--r--   0        0        0     5206 1970-01-01 00:00:00.000000 dpack_py-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       27 2024-04-22 18:27:21.236302 dpack_py-0.2.2/.gitignore
+-rw-r--r--   0        0        0      100 2024-04-22 18:30:45.593747 dpack_py-0.2.2/Makefile
+-rw-r--r--   0        0        0     7398 2024-04-23 13:10:17.896775 dpack_py-0.2.2/examples/uniswap-v3.dpack.json
+-rw-r--r--   0        0        0     2555 2024-04-23 13:10:09.129746 dpack_py-0.2.2/examples/uniswap.py
+-rw-r--r--   0        0        0      555 2024-04-24 20:55:30.611314 dpack_py-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4641 2024-04-24 20:56:10.833132 dpack_py-0.2.2/readme.md
+-rw-r--r--   0        0        0       55 2024-04-22 16:49:07.422511 dpack_py-0.2.2/src/dpack/__init__.py
+-rw-r--r--   0        0        0     1198 2024-04-22 22:09:39.235312 dpack_py-0.2.2/src/dpack/ape.py
+-rw-r--r--   0        0        0     3255 2024-04-24 20:54:37.976520 dpack_py-0.2.2/src/dpack/dpack.py
+-rw-r--r--   0        0        0     2665 2024-04-24 20:55:22.497290 dpack_py-0.2.2/tests/test_dpack.py
+-rw-r--r--   0        0        0    10293 2024-04-22 10:38:52.852458 dpack_py-0.2.2/tests/weth-ropsten-artifact.json
+-rw-r--r--   0        0        0      723 2024-04-21 07:13:55.705183 dpack_py-0.2.2/tests/weth_ropsten.dpack.json
+-rw-r--r--   0        0        0     5211 1970-01-01 00:00:00.000000 dpack_py-0.2.2/PKG-INFO
```

### Comparing `dpack_py-0.2.1/examples/uniswap-v3.dpack.json` & `dpack_py-0.2.2/examples/uniswap-v3.dpack.json`

 * *Files identical despite different names*

### Comparing `dpack_py-0.2.1/examples/uniswap.py` & `dpack_py-0.2.2/examples/uniswap.py`

 * *Files identical despite different names*

### Comparing `dpack_py-0.2.1/pyproject.toml` & `dpack_py-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "dpack-py"
 authors = [{ name = "banteg" }]
 classifiers = ["License :: OSI Approved :: MIT License"]
-version = "0.2.1"
+version = "0.2.2"
 readme = "readme.md"
 description = "dpack is an evm artifact package format"
 requires-python = ">=3.9"
 dependencies = ["pydantic >=2", "httpx", "ethpm-types"]
 
 [tool.flit.module]
 name = "dpack"
```

### Comparing `dpack_py-0.2.1/readme.md` & `dpack_py-0.2.2/readme.md`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
 ## use dpack in ape
 
 this library also provides an easy wrapper that loads up objects as ape contract instances, so you can interact with them right away.
 
 `types` are exposed as a provider-aware wrapper [ContractContainer](https://github.com/ApeWorX/ape/blob/c2f1bc48c1afe3297a63e4e820dbfb751b90c932/src/ape/contracts/base.py#L1238). `objects` are ready-to-use [ContractInstance](https://github.com/ApeWorX/ape/blob/c2f1bc48c1afe3297a63e4e820dbfb751b90c932/src/ape/contracts/base.py#L815).
 
-types can be also accessed with a subscript shorthand like `pack["MyType"]`. you can an address to a type with `.at(address)`, which returns a `ContractInstance`.
+types can be also accessed with a subscript shorthand like `pack["MyType"]`. you can cast an address to a type with `.at(address)`, which returns a `ContractInstance`.
 
 objects can be also accessed with an attribute shorthand like `pack.my_contract`.
 
 ```python
 $ ape console --netwowrk ethereum:mainnet
 
 import dpack.ape
```

### Comparing `dpack_py-0.2.1/src/dpack/ape.py` & `dpack_py-0.2.2/src/dpack/ape.py`

 * *Files identical despite different names*

### Comparing `dpack_py-0.2.1/src/dpack/dpack.py` & `dpack_py-0.2.2/src/dpack/dpack.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from functools import cache
 from pathlib import Path
 from typing import Literal
 
 import httpx
 from ethpm_types import ContractInstance, ContractType
-from pydantic import BaseModel, constr
+from pydantic import BaseModel, constr, field_validator
 
 IPFS_RPC_URL = os.environ.get("IPFS_RPC_URL", "http://127.0.0.1:5001")
 IpfsCid = constr(pattern=r"[bB][aA][fF][yY]?\w{48,}")
 
 
 @cache
 def fetch_artifact(cid):
@@ -67,14 +67,21 @@
 
 class Dpack(BaseModel):
     format: Literal["dpack-1"] = "dpack-1"
     network: str
     types: dict[str, DpackType] = {}
     objects: dict[str, DpackObject] = {}
 
+    @field_validator("network")
+    @classmethod
+    def validate_network(cls, v: str):
+        if v == "mainnet":
+            raise ValueError(f'"{v}" is an ambiguous network name. perhaps you meant "ethereum".')
+        return v
+
     def __getattr__(self, name):
         if name in self.objects:
             return self.objects[name].contract_instance
         raise AttributeError()
 
     def __dir__(self):
         return super().__dir__() + sorted(self.objects.keys())
```

### Comparing `dpack_py-0.2.1/tests/test_dpack.py` & `dpack_py-0.2.2/tests/test_dpack.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,7 +80,13 @@
             typename="WETH9",
             path="tests/weth-ropsten-artifact.json",
             objectname="weth9",
             address="0xc778417E063141139Fce010982780140Aa0cD5Ab",
         )
     )
     assert built.model_dump() == pack.model_dump()
+
+
+def test_network_constraint():
+    # https://github.com/ricobank/dpack/blob/830ce46cc2cf6cc65888b6c9625e86d8cc9859d4/src/builder.ts#L19
+    with pytest.raises(ValueError):
+        dpack.Dpack(network="mainnet")
```

### Comparing `dpack_py-0.2.1/tests/weth-ropsten-artifact.json` & `dpack_py-0.2.2/tests/weth-ropsten-artifact.json`

 * *Files identical despite different names*

### Comparing `dpack_py-0.2.1/tests/weth_ropsten.dpack.json` & `dpack_py-0.2.2/tests/weth_ropsten.dpack.json`

 * *Files identical despite different names*

### Comparing `dpack_py-0.2.1/PKG-INFO` & `dpack_py-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpack-py
-Version: 0.2.1
+Version: 0.2.2
 Summary: dpack is an evm artifact package format
 Author: banteg
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pydantic >=2
 Requires-Dist: httpx
@@ -93,15 +93,15 @@
 
 ## use dpack in ape
 
 this library also provides an easy wrapper that loads up objects as ape contract instances, so you can interact with them right away.
 
 `types` are exposed as a provider-aware wrapper [ContractContainer](https://github.com/ApeWorX/ape/blob/c2f1bc48c1afe3297a63e4e820dbfb751b90c932/src/ape/contracts/base.py#L1238). `objects` are ready-to-use [ContractInstance](https://github.com/ApeWorX/ape/blob/c2f1bc48c1afe3297a63e4e820dbfb751b90c932/src/ape/contracts/base.py#L815).
 
-types can be also accessed with a subscript shorthand like `pack["MyType"]`. you can an address to a type with `.at(address)`, which returns a `ContractInstance`.
+types can be also accessed with a subscript shorthand like `pack["MyType"]`. you can cast an address to a type with `.at(address)`, which returns a `ContractInstance`.
 
 objects can be also accessed with an attribute shorthand like `pack.my_contract`.
 
 ```python
 $ ape console --netwowrk ethereum:mainnet
 
 import dpack.ape
```

