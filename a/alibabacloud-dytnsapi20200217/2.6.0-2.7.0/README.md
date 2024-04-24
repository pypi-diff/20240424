# Comparing `tmp/alibabacloud_dytnsapi20200217-2.6.0.tar.gz` & `tmp/alibabacloud_dytnsapi20200217-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dytnsapi20200217-2.6.0.tar", last modified: Fri Feb  2 09:02:39 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dytnsapi20200217-2.7.0.tar", last modified: Wed Apr 24 07:23:50 2024, max compression
```

## Comparing `alibabacloud_dytnsapi20200217-2.6.0.tar` & `alibabacloud_dytnsapi20200217-2.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 09:02:39.000000 alibabacloud_dytnsapi20200217-2.6.0/
--rw-r--r--   0 root         (0) root         (0)     2880 2024-02-02 09:02:39.000000 alibabacloud_dytnsapi20200217-2.6.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-02-02 09:02:39.000000 alibabacloud_dytnsapi20200217-2.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-02 09:02:39.000000 alibabacloud_dytnsapi20200217-2.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2436 2024-02-02 09:02:39.000000 alibabacloud_dytnsapi20200217-2.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2024-02-02 09:02:39.000000 alibabacloud_dytnsapi20200217-2.6.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1200 2024-02-02 09:02:39.000000 alibabacloud_dytnsapi20200217-2.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 09:02:39.000000 alibabacloud_dytnsapi20200217-2.6.0/alibabacloud_dytnsapi20200217/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-02 09:02:39.000000 alibabacloud_dytnsapi20200217-2.6.0/alibabacloud_dytnsapi20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)   218847 2024-02-02 09:02:39.000000 alibabacloud_dytnsapi20200217-2.6.0/alibabacloud_dytnsapi20200217/client.py
--rw-r--r--   0 root         (0) root         (0)   255886 2024-02-02 09:02:39.000000 alibabacloud_dytnsapi20200217-2.6.0/alibabacloud_dytnsapi20200217/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 09:02:39.000000 alibabacloud_dytnsapi20200217-2.6.0/alibabacloud_dytnsapi20200217.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2436 2024-02-02 09:02:39.000000 alibabacloud_dytnsapi20200217-2.6.0/alibabacloud_dytnsapi20200217.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2024-02-02 09:02:39.000000 alibabacloud_dytnsapi20200217-2.6.0/alibabacloud_dytnsapi20200217.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-02 09:02:39.000000 alibabacloud_dytnsapi20200217-2.6.0/alibabacloud_dytnsapi20200217.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-02-02 09:02:39.000000 alibabacloud_dytnsapi20200217-2.6.0/alibabacloud_dytnsapi20200217.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-02-02 09:02:39.000000 alibabacloud_dytnsapi20200217-2.6.0/alibabacloud_dytnsapi20200217.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-02 09:02:39.000000 alibabacloud_dytnsapi20200217-2.6.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2636 2024-02-02 09:02:39.000000 alibabacloud_dytnsapi20200217-2.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:23:50.000000 alibabacloud_dytnsapi20200217-2.7.0/
+-rw-r--r--   0 root         (0) root         (0)     2950 2024-04-24 07:23:50.000000 alibabacloud_dytnsapi20200217-2.7.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-24 07:23:50.000000 alibabacloud_dytnsapi20200217-2.7.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-24 07:23:50.000000 alibabacloud_dytnsapi20200217-2.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-04-24 07:23:50.000000 alibabacloud_dytnsapi20200217-2.7.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-04-24 07:23:50.000000 alibabacloud_dytnsapi20200217-2.7.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-04-24 07:23:50.000000 alibabacloud_dytnsapi20200217-2.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:23:50.000000 alibabacloud_dytnsapi20200217-2.7.0/alibabacloud_dytnsapi20200217/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-24 07:23:50.000000 alibabacloud_dytnsapi20200217-2.7.0/alibabacloud_dytnsapi20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   222963 2024-04-24 07:23:50.000000 alibabacloud_dytnsapi20200217-2.7.0/alibabacloud_dytnsapi20200217/client.py
+-rw-r--r--   0 root         (0) root         (0)   262034 2024-04-24 07:23:50.000000 alibabacloud_dytnsapi20200217-2.7.0/alibabacloud_dytnsapi20200217/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:23:50.000000 alibabacloud_dytnsapi20200217-2.7.0/alibabacloud_dytnsapi20200217.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-04-24 07:23:50.000000 alibabacloud_dytnsapi20200217-2.7.0/alibabacloud_dytnsapi20200217.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-04-24 07:23:50.000000 alibabacloud_dytnsapi20200217-2.7.0/alibabacloud_dytnsapi20200217.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 07:23:50.000000 alibabacloud_dytnsapi20200217-2.7.0/alibabacloud_dytnsapi20200217.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-24 07:23:50.000000 alibabacloud_dytnsapi20200217-2.7.0/alibabacloud_dytnsapi20200217.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-24 07:23:50.000000 alibabacloud_dytnsapi20200217-2.7.0/alibabacloud_dytnsapi20200217.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-24 07:23:50.000000 alibabacloud_dytnsapi20200217-2.7.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-04-24 07:23:50.000000 alibabacloud_dytnsapi20200217-2.7.0/setup.py
```

### Comparing `alibabacloud_dytnsapi20200217-2.6.0/ChangeLog.md` & `alibabacloud_dytnsapi20200217-2.7.0/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-02-02 Version: 2.6.0
+- Support API QueryPhoneNumberOnlineTime.
+
+
 2024-01-12 Version: 2.5.2
 - Generated python 2020-02-17 for Dytnsapi.
 
 2023-12-29 Version: 2.5.1
 - Generated python 2020-02-17 for Dytnsapi.
 
 2023-12-28 Version: 2.5.0
```

### Comparing `alibabacloud_dytnsapi20200217-2.6.0/LICENSE` & `alibabacloud_dytnsapi20200217-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dytnsapi20200217-2.6.0/PKG-INFO` & `alibabacloud_dytnsapi20200217-2.7.0/alibabacloud_dytnsapi20200217.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_dytnsapi20200217
-Version: 2.6.0
+Name: alibabacloud-dytnsapi20200217
+Version: 2.7.0
 Summary: Alibaba Cloud Dytnsapi (20200217) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dytnsapi20200217-2.6.0/README-CN.md` & `alibabacloud_dytnsapi20200217-2.7.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dytnsapi20200217-2.6.0/README.md` & `alibabacloud_dytnsapi20200217-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dytnsapi20200217-2.6.0/alibabacloud_dytnsapi20200217/client.py` & `alibabacloud_dytnsapi20200217-2.7.0/alibabacloud_dytnsapi20200217/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -3005,14 +3005,108 @@
     async def query_phone_number_online_time_async(
         self,
         request: dytnsapi_20200217_models.QueryPhoneNumberOnlineTimeRequest,
     ) -> dytnsapi_20200217_models.QueryPhoneNumberOnlineTimeResponse:
         runtime = util_models.RuntimeOptions()
         return await self.query_phone_number_online_time_with_options_async(request, runtime)
 
+    def query_phone_twice_tel_verify_with_options(
+        self,
+        request: dytnsapi_20200217_models.QueryPhoneTwiceTelVerifyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dytnsapi_20200217_models.QueryPhoneTwiceTelVerifyResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.auth_code):
+            query['AuthCode'] = request.auth_code
+        if not UtilClient.is_unset(request.input_number):
+            query['InputNumber'] = request.input_number
+        if not UtilClient.is_unset(request.mask):
+            query['Mask'] = request.mask
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='QueryPhoneTwiceTelVerify',
+            version='2020-02-17',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dytnsapi_20200217_models.QueryPhoneTwiceTelVerifyResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def query_phone_twice_tel_verify_with_options_async(
+        self,
+        request: dytnsapi_20200217_models.QueryPhoneTwiceTelVerifyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dytnsapi_20200217_models.QueryPhoneTwiceTelVerifyResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.auth_code):
+            query['AuthCode'] = request.auth_code
+        if not UtilClient.is_unset(request.input_number):
+            query['InputNumber'] = request.input_number
+        if not UtilClient.is_unset(request.mask):
+            query['Mask'] = request.mask
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='QueryPhoneTwiceTelVerify',
+            version='2020-02-17',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dytnsapi_20200217_models.QueryPhoneTwiceTelVerifyResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def query_phone_twice_tel_verify(
+        self,
+        request: dytnsapi_20200217_models.QueryPhoneTwiceTelVerifyRequest,
+    ) -> dytnsapi_20200217_models.QueryPhoneTwiceTelVerifyResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.query_phone_twice_tel_verify_with_options(request, runtime)
+
+    async def query_phone_twice_tel_verify_async(
+        self,
+        request: dytnsapi_20200217_models.QueryPhoneTwiceTelVerifyRequest,
+    ) -> dytnsapi_20200217_models.QueryPhoneTwiceTelVerifyResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.query_phone_twice_tel_verify_with_options_async(request, runtime)
+
     def query_tag_apply_rule_with_options(
         self,
         request: dytnsapi_20200217_models.QueryTagApplyRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dytnsapi_20200217_models.QueryTagApplyRuleResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_dytnsapi20200217-2.6.0/alibabacloud_dytnsapi20200217/models.py` & `alibabacloud_dytnsapi20200217-2.7.0/alibabacloud_dytnsapi20200217/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5387,14 +5387,204 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = QueryPhoneNumberOnlineTimeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class QueryPhoneTwiceTelVerifyRequest(TeaModel):
+    def __init__(
+        self,
+        auth_code: str = None,
+        input_number: str = None,
+        mask: str = None,
+        owner_id: int = None,
+        resource_owner_account: str = None,
+        resource_owner_id: int = None,
+        start_time: str = None,
+    ):
+        self.auth_code = auth_code
+        self.input_number = input_number
+        self.mask = mask
+        self.owner_id = owner_id
+        self.resource_owner_account = resource_owner_account
+        self.resource_owner_id = resource_owner_id
+        self.start_time = start_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_code is not None:
+            result['AuthCode'] = self.auth_code
+        if self.input_number is not None:
+            result['InputNumber'] = self.input_number
+        if self.mask is not None:
+            result['Mask'] = self.mask
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.resource_owner_account is not None:
+            result['ResourceOwnerAccount'] = self.resource_owner_account
+        if self.resource_owner_id is not None:
+            result['ResourceOwnerId'] = self.resource_owner_id
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AuthCode') is not None:
+            self.auth_code = m.get('AuthCode')
+        if m.get('InputNumber') is not None:
+            self.input_number = m.get('InputNumber')
+        if m.get('Mask') is not None:
+            self.mask = m.get('Mask')
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('ResourceOwnerAccount') is not None:
+            self.resource_owner_account = m.get('ResourceOwnerAccount')
+        if m.get('ResourceOwnerId') is not None:
+            self.resource_owner_id = m.get('ResourceOwnerId')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
+class QueryPhoneTwiceTelVerifyResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        carrier_code: str = None,
+        verify_result: int = None,
+    ):
+        self.carrier_code = carrier_code
+        self.verify_result = verify_result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.carrier_code is not None:
+            result['CarrierCode'] = self.carrier_code
+        if self.verify_result is not None:
+            result['VerifyResult'] = self.verify_result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CarrierCode') is not None:
+            self.carrier_code = m.get('CarrierCode')
+        if m.get('VerifyResult') is not None:
+            self.verify_result = m.get('VerifyResult')
+        return self
+
+
+class QueryPhoneTwiceTelVerifyResponseBody(TeaModel):
+    def __init__(
+        self,
+        access_denied_detail: str = None,
+        code: str = None,
+        data: QueryPhoneTwiceTelVerifyResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.access_denied_detail = access_denied_detail
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_denied_detail is not None:
+            result['AccessDeniedDetail'] = self.access_denied_detail
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccessDeniedDetail') is not None:
+            self.access_denied_detail = m.get('AccessDeniedDetail')
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = QueryPhoneTwiceTelVerifyResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class QueryPhoneTwiceTelVerifyResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: QueryPhoneTwiceTelVerifyResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = QueryPhoneTwiceTelVerifyResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class QueryTagApplyRuleRequest(TeaModel):
     def __init__(
         self,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         tag_id: int = None,
```

### Comparing `alibabacloud_dytnsapi20200217-2.6.0/alibabacloud_dytnsapi20200217.egg-info/PKG-INFO` & `alibabacloud_dytnsapi20200217-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-dytnsapi20200217
-Version: 2.6.0
+Name: alibabacloud_dytnsapi20200217
+Version: 2.7.0
 Summary: Alibaba Cloud Dytnsapi (20200217) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dytnsapi20200217-2.6.0/setup.py` & `alibabacloud_dytnsapi20200217-2.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dytnsapi20200217.
 
-Created on 02/02/2024
+Created on 24/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dytnsapi20200217"
 NAME = "alibabacloud_dytnsapi20200217" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dytnsapi (20200217) SDK Library for Python"
```

