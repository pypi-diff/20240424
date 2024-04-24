# Comparing `tmp/antchain_duanka-1.0.6.tar.gz` & `tmp/antchain_duanka-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_duanka-1.0.6.tar", last modified: Wed Apr 10 07:18:07 2024, max compression
+gzip compressed data, was "dist/antchain_duanka-1.0.7.tar", last modified: Wed Apr 24 03:12:46 2024, max compression
```

## Comparing `antchain_duanka-1.0.6.tar` & `antchain_duanka-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2180 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      813 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      999 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/antchain_duanka.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2180 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/antchain_duanka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      347 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/antchain_duanka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/antchain_duanka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/antchain_duanka.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/antchain_duanka.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/antchain_sdk_duanka/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/antchain_sdk_duanka/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23083 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/antchain_sdk_duanka/client.py
--rw-r--r--   0 root         (0) root         (0)    35333 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/antchain_sdk_duanka/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2504 2024-04-10 07:18:07.000000 antchain_duanka-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 03:12:46.000000 antchain_duanka-1.0.7/
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-24 03:12:46.000000 antchain_duanka-1.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-24 03:12:46.000000 antchain_duanka-1.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2180 2024-04-24 03:12:46.000000 antchain_duanka-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      813 2024-04-24 03:12:46.000000 antchain_duanka-1.0.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      999 2024-04-24 03:12:46.000000 antchain_duanka-1.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 03:12:46.000000 antchain_duanka-1.0.7/antchain_duanka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2180 2024-04-24 03:12:46.000000 antchain_duanka-1.0.7/antchain_duanka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      347 2024-04-24 03:12:46.000000 antchain_duanka-1.0.7/antchain_duanka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 03:12:46.000000 antchain_duanka-1.0.7/antchain_duanka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2024-04-24 03:12:46.000000 antchain_duanka-1.0.7/antchain_duanka.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-24 03:12:46.000000 antchain_duanka-1.0.7/antchain_duanka.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 03:12:46.000000 antchain_duanka-1.0.7/antchain_sdk_duanka/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-24 03:12:46.000000 antchain_duanka-1.0.7/antchain_sdk_duanka/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23083 2024-04-24 03:12:46.000000 antchain_duanka-1.0.7/antchain_sdk_duanka/client.py
+-rw-r--r--   0 root         (0) root         (0)    35679 2024-04-24 03:12:46.000000 antchain_duanka-1.0.7/antchain_sdk_duanka/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-24 03:12:46.000000 antchain_duanka-1.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2504 2024-04-24 03:12:46.000000 antchain_duanka-1.0.7/setup.py
```

### Comparing `antchain_duanka-1.0.6/LICENSE` & `antchain_duanka-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_duanka-1.0.6/PKG-INFO` & `antchain_duanka-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_duanka
-Version: 1.0.6
+Version: 1.0.7
 Summary: Ant Chain DUANKA SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_duanka-1.0.6/README-CN.md` & `antchain_duanka-1.0.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_duanka-1.0.6/README.md` & `antchain_duanka-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `antchain_duanka-1.0.6/antchain_duanka.egg-info/PKG-INFO` & `antchain_duanka-1.0.7/antchain_duanka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-duanka
-Version: 1.0.6
+Version: 1.0.7
 Summary: Ant Chain DUANKA SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_duanka-1.0.6/antchain_sdk_duanka/client.py` & `antchain_duanka-1.0.7/antchain_sdk_duanka/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.6',
+                    'sdk_version': '1.0.7',
                     '_prod_code': 'DUANKA',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.6',
+                    'sdk_version': '1.0.7',
                     '_prod_code': 'DUANKA',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_duanka-1.0.6/antchain_sdk_duanka/models.py` & `antchain_duanka-1.0.7/antchain_sdk_duanka/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -634,28 +634,32 @@
 class QuerySkyholdResRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         biz_code: str = None,
         key_id: str = None,
         channel_code: str = None,
+        customer_id: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         # 业务biz_code
         self.biz_code = biz_code
         # 查询key
         self.key_id = key_id
         # 渠道code
         self.channel_code = channel_code
+        # 客户id
+        self.customer_id = customer_id
 
     def validate(self):
         self.validate_required(self.biz_code, 'biz_code')
         self.validate_required(self.key_id, 'key_id')
         self.validate_required(self.channel_code, 'channel_code')
+        self.validate_required(self.customer_id, 'customer_id')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -663,26 +667,30 @@
             result['auth_token'] = self.auth_token
         if self.biz_code is not None:
             result['biz_code'] = self.biz_code
         if self.key_id is not None:
             result['key_id'] = self.key_id
         if self.channel_code is not None:
             result['channel_code'] = self.channel_code
+        if self.customer_id is not None:
+            result['customer_id'] = self.customer_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('biz_code') is not None:
             self.biz_code = m.get('biz_code')
         if m.get('key_id') is not None:
             self.key_id = m.get('key_id')
         if m.get('channel_code') is not None:
             self.channel_code = m.get('channel_code')
+        if m.get('customer_id') is not None:
+            self.customer_id = m.get('customer_id')
         return self
 
 
 class QuerySkyholdResResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
```

### Comparing `antchain_duanka-1.0.6/setup.py` & `antchain_duanka-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_duanka.
 
-Created on 10/04/2024
+Created on 24/04/2024
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_duanka"
 NAME = "antchain_duanka" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain DUANKA SDK Library for Python"
```

