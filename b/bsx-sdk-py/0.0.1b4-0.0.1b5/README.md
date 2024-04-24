# Comparing `tmp/bsx_sdk_py-0.0.1b4.tar.gz` & `tmp/bsx_sdk_py-0.0.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsx_sdk_py-0.0.1b4.tar", max compression
+gzip compressed data, was "bsx_sdk_py-0.0.1b5.tar", max compression
```

## Comparing `bsx_sdk_py-0.0.1b4.tar` & `bsx_sdk_py-0.0.1b5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2170 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/README.md
--rw-r--r--   0        0        0       89 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/client/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/client/rest/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/client/rest/account/__init__.py
--rw-r--r--   0        0        0     1797 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/client/rest/account/client.py
--rw-r--r--   0        0        0      176 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/client/rest/account/types.py
--rw-r--r--   0        0        0        0 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/client/rest/auth/__init__.py
--rw-r--r--   0        0        0     2453 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/client/rest/auth/client.py
--rw-r--r--   0        0        0      214 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/client/rest/auth/types.py
--rw-r--r--   0        0        0     3254 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/client/rest/base.py
--rw-r--r--   0        0        0        0 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/client/rest/market/__init__.py
--rw-r--r--   0        0        0     4250 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/client/rest/market/client.py
--rw-r--r--   0        0        0      224 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/client/rest/market/types.py
--rw-r--r--   0        0        0       24 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/common/__init__.py
--rw-r--r--   0        0        0      481 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/common/acc_info.py
--rw-r--r--   0        0        0     1167 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/common/exception.py
--rw-r--r--   0        0        0     1882 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/common/lock.py
--rw-r--r--   0        0        0        0 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/common/types/__init__.py
--rw-r--r--   0        0        0     6955 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/common/types/account.py
--rw-r--r--   0        0        0     1470 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/common/types/auth.py
--rw-r--r--   0        0        0      234 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/common/types/base.py
--rw-r--r--   0        0        0     8443 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/common/types/market.py
--rw-r--r--   0        0        0       62 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/helper/__init__.py
--rw-r--r--   0        0        0     1292 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/helper/acc_storage.py
--rw-r--r--   0        0        0     1871 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/helper/api_key_base_manager.py
--rw-r--r--   0        0        0     1563 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/helper/base.py
--rw-r--r--   0        0        0     1417 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/helper/secret_base_manager.py
--rw-r--r--   0        0        0     8631 2024-04-01 04:47:05.969832 bsx_sdk_py-0.0.1b4/bsx_py/instance.py
--rw-r--r--   0        0        0      556 2024-04-01 04:47:05.993832 bsx_sdk_py-0.0.1b4/pyproject.toml
--rw-r--r--   0        0        0     2838 1970-01-01 00:00:00.000000 bsx_sdk_py-0.0.1b4/PKG-INFO
+-rw-r--r--   0        0        0     2170 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/README.md
+-rw-r--r--   0        0        0       89 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/rest/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/rest/account/__init__.py
+-rw-r--r--   0        0        0     1797 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/rest/account/client.py
+-rw-r--r--   0        0        0      176 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/rest/account/types.py
+-rw-r--r--   0        0        0        0 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/rest/auth/__init__.py
+-rw-r--r--   0        0        0     2453 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/rest/auth/client.py
+-rw-r--r--   0        0        0      214 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/rest/auth/types.py
+-rw-r--r--   0        0        0     3254 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/rest/base.py
+-rw-r--r--   0        0        0        0 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/rest/market/__init__.py
+-rw-r--r--   0        0        0     4250 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/rest/market/client.py
+-rw-r--r--   0        0        0      224 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/client/rest/market/types.py
+-rw-r--r--   0        0        0       24 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/common/__init__.py
+-rw-r--r--   0        0        0      481 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/common/acc_info.py
+-rw-r--r--   0        0        0     1167 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/common/exception.py
+-rw-r--r--   0        0        0     1882 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/common/lock.py
+-rw-r--r--   0        0        0        0 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/common/types/__init__.py
+-rw-r--r--   0        0        0     6955 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/common/types/account.py
+-rw-r--r--   0        0        0     1470 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/common/types/auth.py
+-rw-r--r--   0        0        0      234 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/common/types/base.py
+-rw-r--r--   0        0        0     8455 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/common/types/market.py
+-rw-r--r--   0        0        0       62 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/helper/__init__.py
+-rw-r--r--   0        0        0     1292 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/helper/acc_storage.py
+-rw-r--r--   0        0        0     1871 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/helper/api_key_base_manager.py
+-rw-r--r--   0        0        0     1563 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/helper/base.py
+-rw-r--r--   0        0        0     1417 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/helper/secret_base_manager.py
+-rw-r--r--   0        0        0     8631 2024-04-24 10:12:45.780298 bsx_sdk_py-0.0.1b5/bsx_py/instance.py
+-rw-r--r--   0        0        0      556 2024-04-24 10:12:45.800298 bsx_sdk_py-0.0.1b5/pyproject.toml
+-rw-r--r--   0        0        0     2838 1970-01-01 00:00:00.000000 bsx_sdk_py-0.0.1b5/PKG-INFO
```

### Comparing `bsx_sdk_py-0.0.1b4/README.md` & `bsx_sdk_py-0.0.1b5/README.md`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b4/bsx_py/client/rest/account/client.py` & `bsx_sdk_py-0.0.1b5/bsx_py/client/rest/account/client.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b4/bsx_py/client/rest/auth/client.py` & `bsx_sdk_py-0.0.1b5/bsx_py/client/rest/auth/client.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b4/bsx_py/client/rest/base.py` & `bsx_sdk_py-0.0.1b5/bsx_py/client/rest/base.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b4/bsx_py/client/rest/market/client.py` & `bsx_sdk_py-0.0.1b5/bsx_py/client/rest/market/client.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b4/bsx_py/common/exception.py` & `bsx_sdk_py-0.0.1b5/bsx_py/common/exception.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b4/bsx_py/common/lock.py` & `bsx_sdk_py-0.0.1b5/bsx_py/common/lock.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b4/bsx_py/common/types/account.py` & `bsx_sdk_py-0.0.1b5/bsx_py/common/types/account.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b4/bsx_py/common/types/auth.py` & `bsx_sdk_py-0.0.1b5/bsx_py/common/types/auth.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b4/bsx_py/common/types/market.py` & `bsx_sdk_py-0.0.1b5/bsx_py/common/types/market.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,18 +88,18 @@
         reduce_only (bool): optional; default is false
     """
     side: Side
     type: OrderType
     product_index: int
     price: Decimal
     size: Decimal
-    post_only = False
-    reduce_only = False
     time_in_force: str
     nonce: int
+    post_only: bool = False
+    reduce_only: bool = False
 
 
 @dataclass
 class Trade(metaclass=DataClassMeta):
     id: str
     price: Decimal
     size: Decimal
```

### Comparing `bsx_sdk_py-0.0.1b4/bsx_py/helper/acc_storage.py` & `bsx_sdk_py-0.0.1b5/bsx_py/helper/acc_storage.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b4/bsx_py/helper/api_key_base_manager.py` & `bsx_sdk_py-0.0.1b5/bsx_py/helper/api_key_base_manager.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b4/bsx_py/helper/base.py` & `bsx_sdk_py-0.0.1b5/bsx_py/helper/base.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b4/bsx_py/helper/secret_base_manager.py` & `bsx_sdk_py-0.0.1b5/bsx_py/helper/secret_base_manager.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b4/bsx_py/instance.py` & `bsx_sdk_py-0.0.1b5/bsx_py/instance.py`

 * *Files identical despite different names*

### Comparing `bsx_sdk_py-0.0.1b4/pyproject.toml` & `bsx_sdk_py-0.0.1b5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bsx-sdk-py"
-version = "0.0.1beta4"
+version = "0.0.1beta5"
 description = ""
 authors = ["bsx-engineering <dev@bsx.exchange>"]
 readme = "README.md"
 packages = [
     { include = "bsx_py" }
 ]
```

### Comparing `bsx_sdk_py-0.0.1b4/PKG-INFO` & `bsx_sdk_py-0.0.1b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsx-sdk-py
-Version: 0.0.1b4
+Version: 0.0.1b5
 Summary: 
 Author: bsx-engineering
 Author-email: dev@bsx.exchange
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

