# Comparing `tmp/antchain_securitytech-1.2.3.tar.gz` & `tmp/antchain_securitytech-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_securitytech-1.2.3.tar", last modified: Fri Oct 27 03:21:12 2023, max compression
+gzip compressed data, was "dist/antchain_securitytech-1.2.9.tar", last modified: Mon Jan 22 01:47:26 2024, max compression
```

## Comparing `antchain_securitytech-1.2.3.tar` & `antchain_securitytech-1.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 03:21:12.000000 antchain_securitytech-1.2.3/
--rw-r--r--   0 root         (0) root         (0)      600 2023-10-27 03:21:12.000000 antchain_securitytech-1.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-10-27 03:21:12.000000 antchain_securitytech-1.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2216 2023-10-27 03:21:12.000000 antchain_securitytech-1.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      831 2023-10-27 03:21:12.000000 antchain_securitytech-1.2.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1017 2023-10-27 03:21:12.000000 antchain_securitytech-1.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 03:21:12.000000 antchain_securitytech-1.2.3/antchain_sdk_securitytech/
--rw-r--r--   0 root         (0) root         (0)       21 2023-10-27 03:21:12.000000 antchain_securitytech-1.2.3/antchain_sdk_securitytech/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62851 2023-10-27 03:21:12.000000 antchain_securitytech-1.2.3/antchain_sdk_securitytech/client.py
--rw-r--r--   0 root         (0) root         (0)   133666 2023-10-27 03:21:12.000000 antchain_securitytech-1.2.3/antchain_sdk_securitytech/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 03:21:12.000000 antchain_securitytech-1.2.3/antchain_securitytech.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2216 2023-10-27 03:21:12.000000 antchain_securitytech-1.2.3/antchain_securitytech.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      395 2023-10-27 03:21:12.000000 antchain_securitytech-1.2.3/antchain_securitytech.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-27 03:21:12.000000 antchain_securitytech-1.2.3/antchain_securitytech.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-10-27 03:21:12.000000 antchain_securitytech-1.2.3/antchain_securitytech.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-10-27 03:21:12.000000 antchain_securitytech-1.2.3/antchain_securitytech.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-10-27 03:21:12.000000 antchain_securitytech-1.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2534 2023-10-27 03:21:12.000000 antchain_securitytech-1.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 01:47:26.000000 antchain_securitytech-1.2.9/
+-rw-r--r--   0 root         (0) root         (0)      600 2024-01-22 01:47:26.000000 antchain_securitytech-1.2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-01-22 01:47:26.000000 antchain_securitytech-1.2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2216 2024-01-22 01:47:26.000000 antchain_securitytech-1.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      831 2024-01-22 01:47:26.000000 antchain_securitytech-1.2.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1017 2024-01-22 01:47:26.000000 antchain_securitytech-1.2.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 01:47:26.000000 antchain_securitytech-1.2.9/antchain_sdk_securitytech/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-01-22 01:47:26.000000 antchain_securitytech-1.2.9/antchain_sdk_securitytech/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    82535 2024-01-22 01:47:26.000000 antchain_securitytech-1.2.9/antchain_sdk_securitytech/client.py
+-rw-r--r--   0 root         (0) root         (0)   185040 2024-01-22 01:47:26.000000 antchain_securitytech-1.2.9/antchain_sdk_securitytech/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 01:47:26.000000 antchain_securitytech-1.2.9/antchain_securitytech.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2216 2024-01-22 01:47:26.000000 antchain_securitytech-1.2.9/antchain_securitytech.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      395 2024-01-22 01:47:26.000000 antchain_securitytech-1.2.9/antchain_securitytech.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-22 01:47:26.000000 antchain_securitytech-1.2.9/antchain_securitytech.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2024-01-22 01:47:26.000000 antchain_securitytech-1.2.9/antchain_securitytech.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-01-22 01:47:26.000000 antchain_securitytech-1.2.9/antchain_securitytech.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-01-22 01:47:26.000000 antchain_securitytech-1.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2534 2024-01-22 01:47:26.000000 antchain_securitytech-1.2.9/setup.py
```

### Comparing `antchain_securitytech-1.2.3/LICENSE` & `antchain_securitytech-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_securitytech-1.2.3/PKG-INFO` & `antchain_securitytech-1.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_securitytech
-Version: 1.2.3
+Version: 1.2.9
 Summary: Ant Chain SECURITYTECH SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_securitytech-1.2.3/README-CN.md` & `antchain_securitytech-1.2.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_securitytech-1.2.3/README.md` & `antchain_securitytech-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `antchain_securitytech-1.2.3/antchain_sdk_securitytech/client.py` & `antchain_securitytech-1.2.9/antchain_sdk_securitytech/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.2.3',
+                    'sdk_version': '1.2.9',
                     '_prod_code': 'SECURITYTECH',
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
-                    'sdk_version': '1.2.3',
+                    'sdk_version': '1.2.9',
                     '_prod_code': 'SECURITYTECH',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -1506,7 +1506,455 @@
         Summary: 申请设备设备密钥
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             securitytech_models.ApplyIifaaDevicekeyResponse(),
             await self.do_request_async('1.0', 'antsecuritytech.gateway.iifaa.devicekey.apply', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
+
+    def query_deviceplus_riskquery(
+        self,
+        request: securitytech_models.QueryDeviceplusRiskqueryRequest,
+    ) -> securitytech_models.QueryDeviceplusRiskqueryResponse:
+        """
+        Description: 设备风险咨询
+        Summary: 设备风险咨询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_deviceplus_riskquery_ex(request, headers, runtime)
+
+    async def query_deviceplus_riskquery_async(
+        self,
+        request: securitytech_models.QueryDeviceplusRiskqueryRequest,
+    ) -> securitytech_models.QueryDeviceplusRiskqueryResponse:
+        """
+        Description: 设备风险咨询
+        Summary: 设备风险咨询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_deviceplus_riskquery_ex_async(request, headers, runtime)
+
+    def query_deviceplus_riskquery_ex(
+        self,
+        request: securitytech_models.QueryDeviceplusRiskqueryRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> securitytech_models.QueryDeviceplusRiskqueryResponse:
+        """
+        Description: 设备风险咨询
+        Summary: 设备风险咨询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            securitytech_models.QueryDeviceplusRiskqueryResponse(),
+            self.do_request('1.0', 'antsecuritytech.gateway.deviceplus.riskquery.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_deviceplus_riskquery_ex_async(
+        self,
+        request: securitytech_models.QueryDeviceplusRiskqueryRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> securitytech_models.QueryDeviceplusRiskqueryResponse:
+        """
+        Description: 设备风险咨询
+        Summary: 设备风险咨询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            securitytech_models.QueryDeviceplusRiskqueryResponse(),
+            await self.do_request_async('1.0', 'antsecuritytech.gateway.deviceplus.riskquery.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_deviceplus_mpaas(
+        self,
+        request: securitytech_models.QueryDeviceplusMpaasRequest,
+    ) -> securitytech_models.QueryDeviceplusMpaasResponse:
+        """
+        Description: 设备风险咨询mpaas
+        Summary: 设备风险咨询mpaas
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_deviceplus_mpaas_ex(request, headers, runtime)
+
+    async def query_deviceplus_mpaas_async(
+        self,
+        request: securitytech_models.QueryDeviceplusMpaasRequest,
+    ) -> securitytech_models.QueryDeviceplusMpaasResponse:
+        """
+        Description: 设备风险咨询mpaas
+        Summary: 设备风险咨询mpaas
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_deviceplus_mpaas_ex_async(request, headers, runtime)
+
+    def query_deviceplus_mpaas_ex(
+        self,
+        request: securitytech_models.QueryDeviceplusMpaasRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> securitytech_models.QueryDeviceplusMpaasResponse:
+        """
+        Description: 设备风险咨询mpaas
+        Summary: 设备风险咨询mpaas
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            securitytech_models.QueryDeviceplusMpaasResponse(),
+            self.do_request('1.0', 'antsecuritytech.gateway.deviceplus.mpaas.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_deviceplus_mpaas_ex_async(
+        self,
+        request: securitytech_models.QueryDeviceplusMpaasRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> securitytech_models.QueryDeviceplusMpaasResponse:
+        """
+        Description: 设备风险咨询mpaas
+        Summary: 设备风险咨询mpaas
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            securitytech_models.QueryDeviceplusMpaasResponse(),
+            await self.do_request_async('1.0', 'antsecuritytech.gateway.deviceplus.mpaas.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def submit_ashield_periodhardeningtask(
+        self,
+        request: securitytech_models.SubmitAshieldPeriodhardeningtaskRequest,
+    ) -> securitytech_models.SubmitAshieldPeriodhardeningtaskResponse:
+        """
+        Description: 终端安全-Android应用加固-启动加固任务(包月)
+        Summary: 启动加固任务(包月)
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.submit_ashield_periodhardeningtask_ex(request, headers, runtime)
+
+    async def submit_ashield_periodhardeningtask_async(
+        self,
+        request: securitytech_models.SubmitAshieldPeriodhardeningtaskRequest,
+    ) -> securitytech_models.SubmitAshieldPeriodhardeningtaskResponse:
+        """
+        Description: 终端安全-Android应用加固-启动加固任务(包月)
+        Summary: 启动加固任务(包月)
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.submit_ashield_periodhardeningtask_ex_async(request, headers, runtime)
+
+    def submit_ashield_periodhardeningtask_ex(
+        self,
+        request: securitytech_models.SubmitAshieldPeriodhardeningtaskRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> securitytech_models.SubmitAshieldPeriodhardeningtaskResponse:
+        """
+        Description: 终端安全-Android应用加固-启动加固任务(包月)
+        Summary: 启动加固任务(包月)
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            securitytech_models.SubmitAshieldPeriodhardeningtaskResponse(),
+            self.do_request('1.0', 'antsecuritytech.gateway.ashield.periodhardeningtask.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def submit_ashield_periodhardeningtask_ex_async(
+        self,
+        request: securitytech_models.SubmitAshieldPeriodhardeningtaskRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> securitytech_models.SubmitAshieldPeriodhardeningtaskResponse:
+        """
+        Description: 终端安全-Android应用加固-启动加固任务(包月)
+        Summary: 启动加固任务(包月)
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            securitytech_models.SubmitAshieldPeriodhardeningtaskResponse(),
+            await self.do_request_async('1.0', 'antsecuritytech.gateway.ashield.periodhardeningtask.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def get_ashield_filetoken(
+        self,
+        request: securitytech_models.GetAshieldFiletokenRequest,
+    ) -> securitytech_models.GetAshieldFiletokenResponse:
+        """
+        Description: 终端安全-Android应用加固-获取上传文件的临时URL
+        Summary: 获取上传文件的临时URL
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_ashield_filetoken_ex(request, headers, runtime)
+
+    async def get_ashield_filetoken_async(
+        self,
+        request: securitytech_models.GetAshieldFiletokenRequest,
+    ) -> securitytech_models.GetAshieldFiletokenResponse:
+        """
+        Description: 终端安全-Android应用加固-获取上传文件的临时URL
+        Summary: 获取上传文件的临时URL
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_ashield_filetoken_ex_async(request, headers, runtime)
+
+    def get_ashield_filetoken_ex(
+        self,
+        request: securitytech_models.GetAshieldFiletokenRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> securitytech_models.GetAshieldFiletokenResponse:
+        """
+        Description: 终端安全-Android应用加固-获取上传文件的临时URL
+        Summary: 获取上传文件的临时URL
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            securitytech_models.GetAshieldFiletokenResponse(),
+            self.do_request('1.0', 'antsecuritytech.gateway.ashield.filetoken.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_ashield_filetoken_ex_async(
+        self,
+        request: securitytech_models.GetAshieldFiletokenRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> securitytech_models.GetAshieldFiletokenResponse:
+        """
+        Description: 终端安全-Android应用加固-获取上传文件的临时URL
+        Summary: 获取上传文件的临时URL
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            securitytech_models.GetAshieldFiletokenResponse(),
+            await self.do_request_async('1.0', 'antsecuritytech.gateway.ashield.filetoken.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def submit_ashield_hardeningtask(
+        self,
+        request: securitytech_models.SubmitAshieldHardeningtaskRequest,
+    ) -> securitytech_models.SubmitAshieldHardeningtaskResponse:
+        """
+        Description: 终端安全-Android应用加固-启动加固任务
+        Summary: 启动加固任务(按次计费)
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.submit_ashield_hardeningtask_ex(request, headers, runtime)
+
+    async def submit_ashield_hardeningtask_async(
+        self,
+        request: securitytech_models.SubmitAshieldHardeningtaskRequest,
+    ) -> securitytech_models.SubmitAshieldHardeningtaskResponse:
+        """
+        Description: 终端安全-Android应用加固-启动加固任务
+        Summary: 启动加固任务(按次计费)
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.submit_ashield_hardeningtask_ex_async(request, headers, runtime)
+
+    def submit_ashield_hardeningtask_ex(
+        self,
+        request: securitytech_models.SubmitAshieldHardeningtaskRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> securitytech_models.SubmitAshieldHardeningtaskResponse:
+        """
+        Description: 终端安全-Android应用加固-启动加固任务
+        Summary: 启动加固任务(按次计费)
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            securitytech_models.SubmitAshieldHardeningtaskResponse(),
+            self.do_request('1.0', 'antsecuritytech.gateway.ashield.hardeningtask.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def submit_ashield_hardeningtask_ex_async(
+        self,
+        request: securitytech_models.SubmitAshieldHardeningtaskRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> securitytech_models.SubmitAshieldHardeningtaskResponse:
+        """
+        Description: 终端安全-Android应用加固-启动加固任务
+        Summary: 启动加固任务(按次计费)
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            securitytech_models.SubmitAshieldHardeningtaskResponse(),
+            await self.do_request_async('1.0', 'antsecuritytech.gateway.ashield.hardeningtask.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def get_ashield_hardeningtaskprocess(
+        self,
+        request: securitytech_models.GetAshieldHardeningtaskprocessRequest,
+    ) -> securitytech_models.GetAshieldHardeningtaskprocessResponse:
+        """
+        Description: 终端安全-Android应用加固-查询加固任务进度
+        Summary: 查询加固任务进度
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_ashield_hardeningtaskprocess_ex(request, headers, runtime)
+
+    async def get_ashield_hardeningtaskprocess_async(
+        self,
+        request: securitytech_models.GetAshieldHardeningtaskprocessRequest,
+    ) -> securitytech_models.GetAshieldHardeningtaskprocessResponse:
+        """
+        Description: 终端安全-Android应用加固-查询加固任务进度
+        Summary: 查询加固任务进度
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_ashield_hardeningtaskprocess_ex_async(request, headers, runtime)
+
+    def get_ashield_hardeningtaskprocess_ex(
+        self,
+        request: securitytech_models.GetAshieldHardeningtaskprocessRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> securitytech_models.GetAshieldHardeningtaskprocessResponse:
+        """
+        Description: 终端安全-Android应用加固-查询加固任务进度
+        Summary: 查询加固任务进度
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            securitytech_models.GetAshieldHardeningtaskprocessResponse(),
+            self.do_request('1.0', 'antsecuritytech.gateway.ashield.hardeningtaskprocess.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_ashield_hardeningtaskprocess_ex_async(
+        self,
+        request: securitytech_models.GetAshieldHardeningtaskprocessRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> securitytech_models.GetAshieldHardeningtaskprocessResponse:
+        """
+        Description: 终端安全-Android应用加固-查询加固任务进度
+        Summary: 查询加固任务进度
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            securitytech_models.GetAshieldHardeningtaskprocessResponse(),
+            await self.do_request_async('1.0', 'antsecuritytech.gateway.ashield.hardeningtaskprocess.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def get_ashield_hardeningresult(
+        self,
+        request: securitytech_models.GetAshieldHardeningresultRequest,
+    ) -> securitytech_models.GetAshieldHardeningresultResponse:
+        """
+        Description: 终端安全-Android应用加固-查询加固后的产物下载链接
+        Summary: 查询加固后的产物下载链接
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_ashield_hardeningresult_ex(request, headers, runtime)
+
+    async def get_ashield_hardeningresult_async(
+        self,
+        request: securitytech_models.GetAshieldHardeningresultRequest,
+    ) -> securitytech_models.GetAshieldHardeningresultResponse:
+        """
+        Description: 终端安全-Android应用加固-查询加固后的产物下载链接
+        Summary: 查询加固后的产物下载链接
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_ashield_hardeningresult_ex_async(request, headers, runtime)
+
+    def get_ashield_hardeningresult_ex(
+        self,
+        request: securitytech_models.GetAshieldHardeningresultRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> securitytech_models.GetAshieldHardeningresultResponse:
+        """
+        Description: 终端安全-Android应用加固-查询加固后的产物下载链接
+        Summary: 查询加固后的产物下载链接
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            securitytech_models.GetAshieldHardeningresultResponse(),
+            self.do_request('1.0', 'antsecuritytech.gateway.ashield.hardeningresult.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_ashield_hardeningresult_ex_async(
+        self,
+        request: securitytech_models.GetAshieldHardeningresultRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> securitytech_models.GetAshieldHardeningresultResponse:
+        """
+        Description: 终端安全-Android应用加固-查询加固后的产物下载链接
+        Summary: 查询加固后的产物下载链接
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            securitytech_models.GetAshieldHardeningresultResponse(),
+            await self.do_request_async('1.0', 'antsecuritytech.gateway.ashield.hardeningresult.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def get_ashield_hardeninglog(
+        self,
+        request: securitytech_models.GetAshieldHardeninglogRequest,
+    ) -> securitytech_models.GetAshieldHardeninglogResponse:
+        """
+        Description: 终端安全-Android应用加固-查询加固后的日志下载链接
+        Summary: 查询加固后的日志下载链接
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_ashield_hardeninglog_ex(request, headers, runtime)
+
+    async def get_ashield_hardeninglog_async(
+        self,
+        request: securitytech_models.GetAshieldHardeninglogRequest,
+    ) -> securitytech_models.GetAshieldHardeninglogResponse:
+        """
+        Description: 终端安全-Android应用加固-查询加固后的日志下载链接
+        Summary: 查询加固后的日志下载链接
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_ashield_hardeninglog_ex_async(request, headers, runtime)
+
+    def get_ashield_hardeninglog_ex(
+        self,
+        request: securitytech_models.GetAshieldHardeninglogRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> securitytech_models.GetAshieldHardeninglogResponse:
+        """
+        Description: 终端安全-Android应用加固-查询加固后的日志下载链接
+        Summary: 查询加固后的日志下载链接
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            securitytech_models.GetAshieldHardeninglogResponse(),
+            self.do_request('1.0', 'antsecuritytech.gateway.ashield.hardeninglog.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_ashield_hardeninglog_ex_async(
+        self,
+        request: securitytech_models.GetAshieldHardeninglogRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> securitytech_models.GetAshieldHardeninglogResponse:
+        """
+        Description: 终端安全-Android应用加固-查询加固后的日志下载链接
+        Summary: 查询加固后的日志下载链接
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            securitytech_models.GetAshieldHardeninglogResponse(),
+            await self.do_request_async('1.0', 'antsecuritytech.gateway.ashield.hardeninglog.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
```

### Comparing `antchain_securitytech-1.2.3/antchain_sdk_securitytech/models.py` & `antchain_securitytech-1.2.9/antchain_sdk_securitytech/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -381,21 +381,24 @@
 
 class RequestHead(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         secret_id: str = None,
         product_code: str = None,
+        format_type: str = None,
     ):
         # 请求唯一标识
         self.request_id = request_id
         # 客户身份标识ID
         self.secret_id = secret_id
         # 客户签约产品code
         self.product_code = product_code
+        # response输出类型，默认json
+        self.format_type = format_type
 
     def validate(self):
         self.validate_required(self.request_id, 'request_id')
         self.validate_required(self.secret_id, 'secret_id')
         self.validate_required(self.product_code, 'product_code')
 
     def to_map(self):
@@ -406,24 +409,104 @@
         result = dict()
         if self.request_id is not None:
             result['request_id'] = self.request_id
         if self.secret_id is not None:
             result['secret_id'] = self.secret_id
         if self.product_code is not None:
             result['product_code'] = self.product_code
+        if self.format_type is not None:
+            result['format_type'] = self.format_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('request_id') is not None:
             self.request_id = m.get('request_id')
         if m.get('secret_id') is not None:
             self.secret_id = m.get('secret_id')
         if m.get('product_code') is not None:
             self.product_code = m.get('product_code')
+        if m.get('format_type') is not None:
+            self.format_type = m.get('format_type')
+        return self
+
+
+class RuntimeProtectConfig(TeaModel):
+    def __init__(
+        self,
+        anti_signature: int = None,
+        anti_debug: int = None,
+        anti_hook: int = None,
+        anti_inject: int = None,
+        anti_emulator: int = None,
+        anti_root: int = None,
+        anti_multi_app: int = None,
+    ):
+        # 重打包,签名校验,AndroidManifest防篡改,签名文件保护,0为检测到风险退出,1不处理
+        self.anti_signature = anti_signature
+        # 防调试,0为检测到风险退出,1不处理
+        self.anti_debug = anti_debug
+        # 防hook,0为检测到风险退出,1不处理
+        self.anti_hook = anti_hook
+        # 防注入,防内存dump,防内存数据修改,读取,0为检测到风险退出,1不处理
+        self.anti_inject = anti_inject
+        # 模拟器检查,0为检测到风险退出,1不处理
+        self.anti_emulator = anti_emulator
+        # 防root,0为检测到风险退出,1不处理
+        self.anti_root = anti_root
+        # 防多开软件运行,0为检测到风险退出,1不处理
+        self.anti_multi_app = anti_multi_app
+
+    def validate(self):
+        self.validate_required(self.anti_signature, 'anti_signature')
+        self.validate_required(self.anti_debug, 'anti_debug')
+        self.validate_required(self.anti_hook, 'anti_hook')
+        self.validate_required(self.anti_inject, 'anti_inject')
+        self.validate_required(self.anti_emulator, 'anti_emulator')
+        self.validate_required(self.anti_root, 'anti_root')
+        self.validate_required(self.anti_multi_app, 'anti_multi_app')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.anti_signature is not None:
+            result['anti_signature'] = self.anti_signature
+        if self.anti_debug is not None:
+            result['anti_debug'] = self.anti_debug
+        if self.anti_hook is not None:
+            result['anti_hook'] = self.anti_hook
+        if self.anti_inject is not None:
+            result['anti_inject'] = self.anti_inject
+        if self.anti_emulator is not None:
+            result['anti_emulator'] = self.anti_emulator
+        if self.anti_root is not None:
+            result['anti_root'] = self.anti_root
+        if self.anti_multi_app is not None:
+            result['anti_multi_app'] = self.anti_multi_app
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('anti_signature') is not None:
+            self.anti_signature = m.get('anti_signature')
+        if m.get('anti_debug') is not None:
+            self.anti_debug = m.get('anti_debug')
+        if m.get('anti_hook') is not None:
+            self.anti_hook = m.get('anti_hook')
+        if m.get('anti_inject') is not None:
+            self.anti_inject = m.get('anti_inject')
+        if m.get('anti_emulator') is not None:
+            self.anti_emulator = m.get('anti_emulator')
+        if m.get('anti_root') is not None:
+            self.anti_root = m.get('anti_root')
+        if m.get('anti_multi_app') is not None:
+            self.anti_multi_app = m.get('anti_multi_app')
         return self
 
 
 class FaceShieldResult(TeaModel):
     def __init__(
         self,
         apdid_token: str = None,
@@ -471,14 +554,82 @@
         if m.get('risk_desc') is not None:
             self.risk_desc = m.get('risk_desc')
         if m.get('sug_action') is not None:
             self.sug_action = m.get('sug_action')
         return self
 
 
+class FileTokenForUpload(TeaModel):
+    def __init__(
+        self,
+        access_id: str = None,
+        dir: str = None,
+        expire: str = None,
+        host: str = None,
+        policy: str = None,
+        signature: str = None,
+    ):
+        # .
+        self.access_id = access_id
+        # dir
+        self.dir = dir
+        # expire
+        self.expire = expire
+        # host
+        self.host = host
+        # policy
+        self.policy = policy
+        # signature
+        self.signature = signature
+
+    def validate(self):
+        self.validate_required(self.access_id, 'access_id')
+        self.validate_required(self.dir, 'dir')
+        self.validate_required(self.expire, 'expire')
+        self.validate_required(self.host, 'host')
+        self.validate_required(self.policy, 'policy')
+        self.validate_required(self.signature, 'signature')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_id is not None:
+            result['access_id'] = self.access_id
+        if self.dir is not None:
+            result['dir'] = self.dir
+        if self.expire is not None:
+            result['expire'] = self.expire
+        if self.host is not None:
+            result['host'] = self.host
+        if self.policy is not None:
+            result['policy'] = self.policy
+        if self.signature is not None:
+            result['signature'] = self.signature
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('access_id') is not None:
+            self.access_id = m.get('access_id')
+        if m.get('dir') is not None:
+            self.dir = m.get('dir')
+        if m.get('expire') is not None:
+            self.expire = m.get('expire')
+        if m.get('host') is not None:
+            self.host = m.get('host')
+        if m.get('policy') is not None:
+            self.policy = m.get('policy')
+        if m.get('signature') is not None:
+            self.signature = m.get('signature')
+        return self
+
+
 class DeviceRiskReportResultData(TeaModel):
     def __init__(
         self,
         webrtc_url: str = None,
         a_dynamic_swi: str = None,
         dynamic_interval: str = None,
         color: str = None,
@@ -671,14 +822,102 @@
         if m.get('operate_type') is not None:
             self.operate_type = m.get('operate_type')
         if m.get('insure_comp_credit_no') is not None:
             self.insure_comp_credit_no = m.get('insure_comp_credit_no')
         return self
 
 
+class RiskQueryData(TeaModel):
+    def __init__(
+        self,
+        risk_score: str = None,
+        risk_labels: List[str] = None,
+    ):
+        # 风险评分
+        self.risk_score = risk_score
+        # 风险标签
+        self.risk_labels = risk_labels
+
+    def validate(self):
+        self.validate_required(self.risk_score, 'risk_score')
+        self.validate_required(self.risk_labels, 'risk_labels')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.risk_score is not None:
+            result['risk_score'] = self.risk_score
+        if self.risk_labels is not None:
+            result['risk_labels'] = self.risk_labels
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('risk_score') is not None:
+            self.risk_score = m.get('risk_score')
+        if m.get('risk_labels') is not None:
+            self.risk_labels = m.get('risk_labels')
+        return self
+
+
+class HardeningTaskResponse(TeaModel):
+    def __init__(
+        self,
+        task_id: str = None,
+        status: int = None,
+        after_md_five: str = None,
+        after_size: int = None,
+    ):
+        # 加固任务的 ID，后续用来轮询调用
+        self.task_id = task_id
+        # 加固任务的状态
+        self.status = status
+        # 加固后 APK/ABB 的 MD5
+        self.after_md_five = after_md_five
+        # 加固后 APK/ABB 的大小
+        self.after_size = after_size
+
+    def validate(self):
+        self.validate_required(self.task_id, 'task_id')
+        self.validate_required(self.status, 'status')
+        self.validate_required(self.after_md_five, 'after_md_five')
+        self.validate_required(self.after_size, 'after_size')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.task_id is not None:
+            result['task_id'] = self.task_id
+        if self.status is not None:
+            result['status'] = self.status
+        if self.after_md_five is not None:
+            result['after_md_five'] = self.after_md_five
+        if self.after_size is not None:
+            result['after_size'] = self.after_size
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('task_id') is not None:
+            self.task_id = m.get('task_id')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('after_md_five') is not None:
+            self.after_md_five = m.get('after_md_five')
+        if m.get('after_size') is not None:
+            self.after_size = m.get('after_size')
+        return self
+
+
 class DeviceRiskResp(TeaModel):
     def __init__(
         self,
         apdid: str = None,
         apdid_token: str = None,
         risk_level: int = None,
         risk_desc: str = None,
@@ -850,14 +1089,50 @@
         if m.get('biz_params') is not None:
             for k in m.get('biz_params'):
                 temp_model = BizParam()
                 self.biz_params.append(temp_model.from_map(k))
         return self
 
 
+class ClassMethodConfig(TeaModel):
+    def __init__(
+        self,
+        class_name: str = None,
+        methods: str = None,
+    ):
+        # 加固类名
+        self.class_name = class_name
+        # 方法集合，使用英文逗号分隔
+        self.methods = methods
+
+    def validate(self):
+        self.validate_required(self.class_name, 'class_name')
+        self.validate_required(self.methods, 'methods')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.class_name is not None:
+            result['class_name'] = self.class_name
+        if self.methods is not None:
+            result['methods'] = self.methods
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('class_name') is not None:
+            self.class_name = m.get('class_name')
+        if m.get('methods') is not None:
+            self.methods = m.get('methods')
+        return self
+
+
 class RiskAssessResult(TeaModel):
     def __init__(
         self,
         risk_value: str = None,
         risk_score: str = None,
         model_infos: RiskModel = None,
     ):
@@ -1936,29 +2211,36 @@
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         corp_code: str = None,
         device_type: str = None,
         device_info: str = None,
+        product_code: str = None,
+        pub_key: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 产商code
         self.corp_code = corp_code
         # 设备类型
         self.device_type = device_type
         # 设备信息
         self.device_info = device_info
+        # 产品code
+        self.product_code = product_code
+        # 用于加密回传数据的公钥
+        self.pub_key = pub_key
 
     def validate(self):
         self.validate_required(self.corp_code, 'corp_code')
         self.validate_required(self.device_type, 'device_type')
         self.validate_required(self.device_info, 'device_info')
+        self.validate_required(self.product_code, 'product_code')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -1968,28 +2250,36 @@
             result['product_instance_id'] = self.product_instance_id
         if self.corp_code is not None:
             result['corp_code'] = self.corp_code
         if self.device_type is not None:
             result['device_type'] = self.device_type
         if self.device_info is not None:
             result['device_info'] = self.device_info
+        if self.product_code is not None:
+            result['product_code'] = self.product_code
+        if self.pub_key is not None:
+            result['pub_key'] = self.pub_key
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
         if m.get('corp_code') is not None:
             self.corp_code = m.get('corp_code')
         if m.get('device_type') is not None:
             self.device_type = m.get('device_type')
         if m.get('device_info') is not None:
             self.device_info = m.get('device_info')
+        if m.get('product_code') is not None:
+            self.product_code = m.get('product_code')
+        if m.get('pub_key') is not None:
+            self.pub_key = m.get('pub_key')
         return self
 
 
 class InitIifaaDeviceResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -3890,7 +4180,1140 @@
             self.message = m.get('message')
         if m.get('data') is not None:
             temp_model = IifaaEkytResponse()
             self.data = temp_model.from_map(m['data'])
         return self
 
 
+class QueryDeviceplusRiskqueryRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        client_id: str = None,
+        request_id: str = None,
+        scene_code: str = None,
+        phone_number: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 客户id
+        self.client_id = client_id
+        # 请求id
+        self.request_id = request_id
+        # 场景码
+        self.scene_code = scene_code
+        # 加密电话号码
+        self.phone_number = phone_number
+
+    def validate(self):
+        self.validate_required(self.client_id, 'client_id')
+        self.validate_required(self.request_id, 'request_id')
+        self.validate_required(self.scene_code, 'scene_code')
+        self.validate_required(self.phone_number, 'phone_number')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.client_id is not None:
+            result['client_id'] = self.client_id
+        if self.request_id is not None:
+            result['request_id'] = self.request_id
+        if self.scene_code is not None:
+            result['scene_code'] = self.scene_code
+        if self.phone_number is not None:
+            result['phone_number'] = self.phone_number
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('client_id') is not None:
+            self.client_id = m.get('client_id')
+        if m.get('request_id') is not None:
+            self.request_id = m.get('request_id')
+        if m.get('scene_code') is not None:
+            self.scene_code = m.get('scene_code')
+        if m.get('phone_number') is not None:
+            self.phone_number = m.get('phone_number')
+        return self
+
+
+class QueryDeviceplusRiskqueryResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+        code: int = None,
+        message: str = None,
+        request_id: str = None,
+        data: RiskQueryData = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否成功
+        self.success = success
+        # 返回码
+        self.code = code
+        # 返回信息
+        self.message = message
+        # 供nearx排查的链路业务请求id
+        self.request_id = request_id
+        # 风险咨询信息
+        self.data = data
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        if self.code is not None:
+            result['code'] = self.code
+        if self.message is not None:
+            result['message'] = self.message
+        if self.request_id is not None:
+            result['request_id'] = self.request_id
+        if self.data is not None:
+            result['data'] = self.data.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('code') is not None:
+            self.code = m.get('code')
+        if m.get('message') is not None:
+            self.message = m.get('message')
+        if m.get('request_id') is not None:
+            self.request_id = m.get('request_id')
+        if m.get('data') is not None:
+            temp_model = RiskQueryData()
+            self.data = temp_model.from_map(m['data'])
+        return self
+
+
+class QueryDeviceplusMpaasRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        workspace_id: str = None,
+        app_id: str = None,
+        scene_code: str = None,
+        phone_number: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # mpaas环境id
+        self.workspace_id = workspace_id
+        # mpaas应用id
+        self.app_id = app_id
+        # 场景码
+        self.scene_code = scene_code
+        # 加密电话号码
+        self.phone_number = phone_number
+
+    def validate(self):
+        self.validate_required(self.workspace_id, 'workspace_id')
+        self.validate_required(self.app_id, 'app_id')
+        self.validate_required(self.scene_code, 'scene_code')
+        self.validate_required(self.phone_number, 'phone_number')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.workspace_id is not None:
+            result['workspace_id'] = self.workspace_id
+        if self.app_id is not None:
+            result['app_id'] = self.app_id
+        if self.scene_code is not None:
+            result['scene_code'] = self.scene_code
+        if self.phone_number is not None:
+            result['phone_number'] = self.phone_number
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('workspace_id') is not None:
+            self.workspace_id = m.get('workspace_id')
+        if m.get('app_id') is not None:
+            self.app_id = m.get('app_id')
+        if m.get('scene_code') is not None:
+            self.scene_code = m.get('scene_code')
+        if m.get('phone_number') is not None:
+            self.phone_number = m.get('phone_number')
+        return self
+
+
+class QueryDeviceplusMpaasResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+        code: int = None,
+        message: str = None,
+        request_id: str = None,
+        data: RiskQueryData = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 是否成功
+        self.success = success
+        # 返回码
+        self.code = code
+        # 返回信息
+        self.message = message
+        # 供nearx排查的链路业务请求id
+        self.request_id = request_id
+        # 风险咨询信息
+        self.data = data
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        if self.code is not None:
+            result['code'] = self.code
+        if self.message is not None:
+            result['message'] = self.message
+        if self.request_id is not None:
+            result['request_id'] = self.request_id
+        if self.data is not None:
+            result['data'] = self.data.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('code') is not None:
+            self.code = m.get('code')
+        if m.get('message') is not None:
+            self.message = m.get('message')
+        if m.get('request_id') is not None:
+            self.request_id = m.get('request_id')
+        if m.get('data') is not None:
+            temp_model = RiskQueryData()
+            self.data = temp_model.from_map(m['data'])
+        return self
+
+
+class SubmitAshieldPeriodhardeningtaskRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        file_url: str = None,
+        so_protect: str = None,
+        so_protect_config: str = None,
+        assets_protect: str = None,
+        assets_protect_confing: str = None,
+        runtime_protect_config: RuntimeProtectConfig = None,
+        enable_life_func: str = None,
+        javatoc_jni_config: List[ClassMethodConfig] = None,
+        ext_info: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # APK,ABB 上传后的地址
+        self.file_url = file_url
+        # 开启so加固
+        self.so_protect = so_protect
+        # 开启so加固后,设置的so加固配置文件,默认对apk中libs目录下所有so进行加固,以逗号分隔
+        self.so_protect_config = so_protect_config
+        # 开启对assets下的资源文件进行加固
+        self.assets_protect = assets_protect
+        # 开启assets加固后,指定要对apk中assets目录下的哪些文件做加固,默认对assets下所有的文件进行保护,以逗号分隔
+        self.assets_protect_confing = assets_protect_confing
+        # 开启运行时保护,需要填写的参数,具体参数见下方,json格式
+        self.runtime_protect_config = runtime_protect_config
+        # 对生命周期函数进行java2jni保护
+        self.enable_life_func = enable_life_func
+        # java2jni配置文件
+        self.javatoc_jni_config = javatoc_jni_config
+        # 扩展信息,json字符串,暂不使用
+        self.ext_info = ext_info
+
+    def validate(self):
+        self.validate_required(self.file_url, 'file_url')
+        if self.runtime_protect_config:
+            self.runtime_protect_config.validate()
+        if self.javatoc_jni_config:
+            for k in self.javatoc_jni_config:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.file_url is not None:
+            result['file_url'] = self.file_url
+        if self.so_protect is not None:
+            result['so_protect'] = self.so_protect
+        if self.so_protect_config is not None:
+            result['so_protect_config'] = self.so_protect_config
+        if self.assets_protect is not None:
+            result['assets_protect'] = self.assets_protect
+        if self.assets_protect_confing is not None:
+            result['assets_protect_confing'] = self.assets_protect_confing
+        if self.runtime_protect_config is not None:
+            result['runtime_protect_config'] = self.runtime_protect_config.to_map()
+        if self.enable_life_func is not None:
+            result['enable_life_func'] = self.enable_life_func
+        result['javatoc_jni_config'] = []
+        if self.javatoc_jni_config is not None:
+            for k in self.javatoc_jni_config:
+                result['javatoc_jni_config'].append(k.to_map() if k else None)
+        if self.ext_info is not None:
+            result['ext_info'] = self.ext_info
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('file_url') is not None:
+            self.file_url = m.get('file_url')
+        if m.get('so_protect') is not None:
+            self.so_protect = m.get('so_protect')
+        if m.get('so_protect_config') is not None:
+            self.so_protect_config = m.get('so_protect_config')
+        if m.get('assets_protect') is not None:
+            self.assets_protect = m.get('assets_protect')
+        if m.get('assets_protect_confing') is not None:
+            self.assets_protect_confing = m.get('assets_protect_confing')
+        if m.get('runtime_protect_config') is not None:
+            temp_model = RuntimeProtectConfig()
+            self.runtime_protect_config = temp_model.from_map(m['runtime_protect_config'])
+        if m.get('enable_life_func') is not None:
+            self.enable_life_func = m.get('enable_life_func')
+        self.javatoc_jni_config = []
+        if m.get('javatoc_jni_config') is not None:
+            for k in m.get('javatoc_jni_config'):
+                temp_model = ClassMethodConfig()
+                self.javatoc_jni_config.append(temp_model.from_map(k))
+        if m.get('ext_info') is not None:
+            self.ext_info = m.get('ext_info')
+        return self
+
+
+class SubmitAshieldPeriodhardeningtaskResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        request_id: str = None,
+        res_success: bool = None,
+        res_code: str = None,
+        res_message: str = None,
+        res_data: HardeningTaskResponse = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 请求id
+        self.request_id = request_id
+        # 查询是否成功
+        self.res_success = res_success
+        # SUCCESS为成功,其他为失败
+        self.res_code = res_code
+        # 返回信息描述
+        self.res_message = res_message
+        # 返回的具体对象
+        self.res_data = res_data
+
+    def validate(self):
+        if self.res_data:
+            self.res_data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.request_id is not None:
+            result['request_id'] = self.request_id
+        if self.res_success is not None:
+            result['res_success'] = self.res_success
+        if self.res_code is not None:
+            result['res_code'] = self.res_code
+        if self.res_message is not None:
+            result['res_message'] = self.res_message
+        if self.res_data is not None:
+            result['res_data'] = self.res_data.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('request_id') is not None:
+            self.request_id = m.get('request_id')
+        if m.get('res_success') is not None:
+            self.res_success = m.get('res_success')
+        if m.get('res_code') is not None:
+            self.res_code = m.get('res_code')
+        if m.get('res_message') is not None:
+            self.res_message = m.get('res_message')
+        if m.get('res_data') is not None:
+            temp_model = HardeningTaskResponse()
+            self.res_data = temp_model.from_map(m['res_data'])
+        return self
+
+
+class GetAshieldFiletokenRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
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
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        return self
+
+
+class GetAshieldFiletokenResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        request_id: str = None,
+        res_success: bool = None,
+        res_code: str = None,
+        res_message: str = None,
+        res_data: FileTokenForUpload = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # .
+        self.request_id = request_id
+        # res_success
+        self.res_success = res_success
+        # res_code
+        self.res_code = res_code
+        # res_message
+        self.res_message = res_message
+        # .
+        self.res_data = res_data
+
+    def validate(self):
+        if self.res_data:
+            self.res_data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.request_id is not None:
+            result['request_id'] = self.request_id
+        if self.res_success is not None:
+            result['res_success'] = self.res_success
+        if self.res_code is not None:
+            result['res_code'] = self.res_code
+        if self.res_message is not None:
+            result['res_message'] = self.res_message
+        if self.res_data is not None:
+            result['res_data'] = self.res_data.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('request_id') is not None:
+            self.request_id = m.get('request_id')
+        if m.get('res_success') is not None:
+            self.res_success = m.get('res_success')
+        if m.get('res_code') is not None:
+            self.res_code = m.get('res_code')
+        if m.get('res_message') is not None:
+            self.res_message = m.get('res_message')
+        if m.get('res_data') is not None:
+            temp_model = FileTokenForUpload()
+            self.res_data = temp_model.from_map(m['res_data'])
+        return self
+
+
+class SubmitAshieldHardeningtaskRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        file_url: str = None,
+        so_protect: str = None,
+        so_protect_config: str = None,
+        assets_protect: str = None,
+        assets_protect_confing: str = None,
+        runtime_protect_config: RuntimeProtectConfig = None,
+        enable_life_func: str = None,
+        javatoc_jni_config: List[ClassMethodConfig] = None,
+        ext_info: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # APK,ABB 上传后的地址
+        self.file_url = file_url
+        # 开启so加固
+        self.so_protect = so_protect
+        # 开启so加固后,设置的so加固配置文件,默认对apk中libs目录下所有so进行加固,以逗号分隔
+        self.so_protect_config = so_protect_config
+        # 开启对assets下的资源文件进行加固
+        self.assets_protect = assets_protect
+        # 开启assets加固后,指定要对apk中assets目录下的哪些文件做加固,默认对assets下所有的文件进行保护,以逗号分隔
+        self.assets_protect_confing = assets_protect_confing
+        # 开启运行时保护,需要填写的参数,具体参数见下方,json格式
+        self.runtime_protect_config = runtime_protect_config
+        # 对生命周期函数进行java2jni保护
+        self.enable_life_func = enable_life_func
+        # java2jni配置文件
+        self.javatoc_jni_config = javatoc_jni_config
+        # 扩展信息,json字符串,暂不使用
+        self.ext_info = ext_info
+
+    def validate(self):
+        self.validate_required(self.file_url, 'file_url')
+        if self.runtime_protect_config:
+            self.runtime_protect_config.validate()
+        if self.javatoc_jni_config:
+            for k in self.javatoc_jni_config:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.file_url is not None:
+            result['file_url'] = self.file_url
+        if self.so_protect is not None:
+            result['so_protect'] = self.so_protect
+        if self.so_protect_config is not None:
+            result['so_protect_config'] = self.so_protect_config
+        if self.assets_protect is not None:
+            result['assets_protect'] = self.assets_protect
+        if self.assets_protect_confing is not None:
+            result['assets_protect_confing'] = self.assets_protect_confing
+        if self.runtime_protect_config is not None:
+            result['runtime_protect_config'] = self.runtime_protect_config.to_map()
+        if self.enable_life_func is not None:
+            result['enable_life_func'] = self.enable_life_func
+        result['javatoc_jni_config'] = []
+        if self.javatoc_jni_config is not None:
+            for k in self.javatoc_jni_config:
+                result['javatoc_jni_config'].append(k.to_map() if k else None)
+        if self.ext_info is not None:
+            result['ext_info'] = self.ext_info
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('file_url') is not None:
+            self.file_url = m.get('file_url')
+        if m.get('so_protect') is not None:
+            self.so_protect = m.get('so_protect')
+        if m.get('so_protect_config') is not None:
+            self.so_protect_config = m.get('so_protect_config')
+        if m.get('assets_protect') is not None:
+            self.assets_protect = m.get('assets_protect')
+        if m.get('assets_protect_confing') is not None:
+            self.assets_protect_confing = m.get('assets_protect_confing')
+        if m.get('runtime_protect_config') is not None:
+            temp_model = RuntimeProtectConfig()
+            self.runtime_protect_config = temp_model.from_map(m['runtime_protect_config'])
+        if m.get('enable_life_func') is not None:
+            self.enable_life_func = m.get('enable_life_func')
+        self.javatoc_jni_config = []
+        if m.get('javatoc_jni_config') is not None:
+            for k in m.get('javatoc_jni_config'):
+                temp_model = ClassMethodConfig()
+                self.javatoc_jni_config.append(temp_model.from_map(k))
+        if m.get('ext_info') is not None:
+            self.ext_info = m.get('ext_info')
+        return self
+
+
+class SubmitAshieldHardeningtaskResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        request_id: str = None,
+        res_success: bool = None,
+        res_code: str = None,
+        res_message: str = None,
+        res_data: HardeningTaskResponse = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 请求id
+        self.request_id = request_id
+        # 查询是否成功
+        self.res_success = res_success
+        # SUCCESS为成功,其他为失败
+        self.res_code = res_code
+        # 返回信息描述
+        self.res_message = res_message
+        # 返回的具体对象
+        self.res_data = res_data
+
+    def validate(self):
+        if self.res_data:
+            self.res_data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.request_id is not None:
+            result['request_id'] = self.request_id
+        if self.res_success is not None:
+            result['res_success'] = self.res_success
+        if self.res_code is not None:
+            result['res_code'] = self.res_code
+        if self.res_message is not None:
+            result['res_message'] = self.res_message
+        if self.res_data is not None:
+            result['res_data'] = self.res_data.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('request_id') is not None:
+            self.request_id = m.get('request_id')
+        if m.get('res_success') is not None:
+            self.res_success = m.get('res_success')
+        if m.get('res_code') is not None:
+            self.res_code = m.get('res_code')
+        if m.get('res_message') is not None:
+            self.res_message = m.get('res_message')
+        if m.get('res_data') is not None:
+            temp_model = HardeningTaskResponse()
+            self.res_data = temp_model.from_map(m['res_data'])
+        return self
+
+
+class GetAshieldHardeningtaskprocessRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        task_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 加固任务 ID
+        self.task_id = task_id
+
+    def validate(self):
+        self.validate_required(self.task_id, 'task_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.task_id is not None:
+            result['task_id'] = self.task_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('task_id') is not None:
+            self.task_id = m.get('task_id')
+        return self
+
+
+class GetAshieldHardeningtaskprocessResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        request_id: str = None,
+        res_success: bool = None,
+        res_code: str = None,
+        res_message: str = None,
+        res_data: HardeningTaskResponse = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 请求id
+        self.request_id = request_id
+        # 查询是否成功
+        self.res_success = res_success
+        # SUCCESS为成功，其他为失败
+        self.res_code = res_code
+        # 返回信息描述
+        self.res_message = res_message
+        # 返回的具体对象
+        self.res_data = res_data
+
+    def validate(self):
+        if self.res_data:
+            self.res_data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.request_id is not None:
+            result['request_id'] = self.request_id
+        if self.res_success is not None:
+            result['res_success'] = self.res_success
+        if self.res_code is not None:
+            result['res_code'] = self.res_code
+        if self.res_message is not None:
+            result['res_message'] = self.res_message
+        if self.res_data is not None:
+            result['res_data'] = self.res_data.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('request_id') is not None:
+            self.request_id = m.get('request_id')
+        if m.get('res_success') is not None:
+            self.res_success = m.get('res_success')
+        if m.get('res_code') is not None:
+            self.res_code = m.get('res_code')
+        if m.get('res_message') is not None:
+            self.res_message = m.get('res_message')
+        if m.get('res_data') is not None:
+            temp_model = HardeningTaskResponse()
+            self.res_data = temp_model.from_map(m['res_data'])
+        return self
+
+
+class GetAshieldHardeningresultRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        task_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 加固任务 ID
+        self.task_id = task_id
+
+    def validate(self):
+        self.validate_required(self.task_id, 'task_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.task_id is not None:
+            result['task_id'] = self.task_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('task_id') is not None:
+            self.task_id = m.get('task_id')
+        return self
+
+
+class GetAshieldHardeningresultResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        request_id: str = None,
+        res_success: bool = None,
+        res_code: str = None,
+        res_message: str = None,
+        res_data: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 请求id
+        self.request_id = request_id
+        # 查询是否成功
+        self.res_success = res_success
+        # SUCCESS为成功，其他为失败
+        self.res_code = res_code
+        # 返回信息描述
+        self.res_message = res_message
+        # 返回的下载链接
+        self.res_data = res_data
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.request_id is not None:
+            result['request_id'] = self.request_id
+        if self.res_success is not None:
+            result['res_success'] = self.res_success
+        if self.res_code is not None:
+            result['res_code'] = self.res_code
+        if self.res_message is not None:
+            result['res_message'] = self.res_message
+        if self.res_data is not None:
+            result['res_data'] = self.res_data
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('request_id') is not None:
+            self.request_id = m.get('request_id')
+        if m.get('res_success') is not None:
+            self.res_success = m.get('res_success')
+        if m.get('res_code') is not None:
+            self.res_code = m.get('res_code')
+        if m.get('res_message') is not None:
+            self.res_message = m.get('res_message')
+        if m.get('res_data') is not None:
+            self.res_data = m.get('res_data')
+        return self
+
+
+class GetAshieldHardeninglogRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        task_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 加固任务 ID
+        self.task_id = task_id
+
+    def validate(self):
+        self.validate_required(self.task_id, 'task_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.task_id is not None:
+            result['task_id'] = self.task_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('task_id') is not None:
+            self.task_id = m.get('task_id')
+        return self
+
+
+class GetAshieldHardeninglogResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        request_id: str = None,
+        res_success: bool = None,
+        res_code: str = None,
+        res_message: str = None,
+        res_data: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 请求id
+        self.request_id = request_id
+        # 查询是否成功
+        self.res_success = res_success
+        # SUCCESS为成功，其他为失败
+        self.res_code = res_code
+        # 返回信息描述
+        self.res_message = res_message
+        # 返回的下载链接
+        self.res_data = res_data
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.request_id is not None:
+            result['request_id'] = self.request_id
+        if self.res_success is not None:
+            result['res_success'] = self.res_success
+        if self.res_code is not None:
+            result['res_code'] = self.res_code
+        if self.res_message is not None:
+            result['res_message'] = self.res_message
+        if self.res_data is not None:
+            result['res_data'] = self.res_data
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('request_id') is not None:
+            self.request_id = m.get('request_id')
+        if m.get('res_success') is not None:
+            self.res_success = m.get('res_success')
+        if m.get('res_code') is not None:
+            self.res_code = m.get('res_code')
+        if m.get('res_message') is not None:
+            self.res_message = m.get('res_message')
+        if m.get('res_data') is not None:
+            self.res_data = m.get('res_data')
+        return self
+
+
```

### Comparing `antchain_securitytech-1.2.3/antchain_securitytech.egg-info/PKG-INFO` & `antchain_securitytech-1.2.9/antchain_securitytech.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-securitytech
-Version: 1.2.3
+Version: 1.2.9
 Summary: Ant Chain SECURITYTECH SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_securitytech-1.2.3/setup.py` & `antchain_securitytech-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_securitytech.
 
-Created on 27/10/2023
+Created on 22/01/2024
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_securitytech"
 NAME = "antchain_securitytech" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain SECURITYTECH SDK Library for Python"
```

