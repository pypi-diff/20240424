# Comparing `tmp/alibabacloud_waf-openapi20211001-3.3.0.tar.gz` & `tmp/alibabacloud_waf-openapi20211001-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_waf-openapi20211001-3.3.0.tar", last modified: Sun Apr  7 03:49:29 2024, max compression
+gzip compressed data, was "dist/alibabacloud_waf-openapi20211001-3.4.0.tar", last modified: Wed Apr 24 17:19:03 2024, max compression
```

## Comparing `alibabacloud_waf-openapi20211001-3.3.0.tar` & `alibabacloud_waf-openapi20211001-3.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 03:49:29.000000 alibabacloud_waf-openapi20211001-3.3.0/
--rw-r--r--   0 root         (0) root         (0)     1627 2024-04-07 03:49:28.000000 alibabacloud_waf-openapi20211001-3.3.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-07 03:49:28.000000 alibabacloud_waf-openapi20211001-3.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-07 03:49:28.000000 alibabacloud_waf-openapi20211001-3.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2457 2024-04-07 03:49:29.000000 alibabacloud_waf-openapi20211001-3.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1127 2024-04-07 03:49:28.000000 alibabacloud_waf-openapi20211001-3.3.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1212 2024-04-07 03:49:28.000000 alibabacloud_waf-openapi20211001-3.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 03:49:29.000000 alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-07 03:49:28.000000 alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001/__init__.py
--rw-r--r--   0 root         (0) root         (0)   294088 2024-04-07 03:49:28.000000 alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001/client.py
--rw-r--r--   0 root         (0) root         (0)   585958 2024-04-07 03:49:28.000000 alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 03:49:29.000000 alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2457 2024-04-07 03:49:29.000000 alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      484 2024-04-07 03:49:29.000000 alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 03:49:29.000000 alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-07 03:49:29.000000 alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-04-07 03:49:29.000000 alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-07 03:49:29.000000 alibabacloud_waf-openapi20211001-3.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2653 2024-04-07 03:49:28.000000 alibabacloud_waf-openapi20211001-3.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 17:19:03.000000 alibabacloud_waf-openapi20211001-3.4.0/
+-rw-r--r--   0 root         (0) root         (0)     2000 2024-04-24 17:19:02.000000 alibabacloud_waf-openapi20211001-3.4.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-24 17:19:02.000000 alibabacloud_waf-openapi20211001-3.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-24 17:19:02.000000 alibabacloud_waf-openapi20211001-3.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-24 17:19:03.000000 alibabacloud_waf-openapi20211001-3.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-04-24 17:19:02.000000 alibabacloud_waf-openapi20211001-3.4.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1212 2024-04-24 17:19:02.000000 alibabacloud_waf-openapi20211001-3.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 17:19:03.000000 alibabacloud_waf-openapi20211001-3.4.0/alibabacloud_waf_openapi20211001/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-24 17:19:02.000000 alibabacloud_waf-openapi20211001-3.4.0/alibabacloud_waf_openapi20211001/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   352002 2024-04-24 17:19:02.000000 alibabacloud_waf-openapi20211001-3.4.0/alibabacloud_waf_openapi20211001/client.py
+-rw-r--r--   0 root         (0) root         (0)   683975 2024-04-24 17:19:02.000000 alibabacloud_waf-openapi20211001-3.4.0/alibabacloud_waf_openapi20211001/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 17:19:03.000000 alibabacloud_waf-openapi20211001-3.4.0/alibabacloud_waf_openapi20211001.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-24 17:19:03.000000 alibabacloud_waf-openapi20211001-3.4.0/alibabacloud_waf_openapi20211001.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      484 2024-04-24 17:19:03.000000 alibabacloud_waf-openapi20211001-3.4.0/alibabacloud_waf_openapi20211001.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 17:19:03.000000 alibabacloud_waf-openapi20211001-3.4.0/alibabacloud_waf_openapi20211001.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-24 17:19:03.000000 alibabacloud_waf-openapi20211001-3.4.0/alibabacloud_waf_openapi20211001.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-24 17:19:03.000000 alibabacloud_waf-openapi20211001-3.4.0/alibabacloud_waf_openapi20211001.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-24 17:19:03.000000 alibabacloud_waf-openapi20211001-3.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2653 2024-04-24 17:19:02.000000 alibabacloud_waf-openapi20211001-3.4.0/setup.py
```

### Comparing `alibabacloud_waf-openapi20211001-3.3.0/ChangeLog.md` & `alibabacloud_waf-openapi20211001-3.4.0/ChangeLog.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+2024-04-07 Version: 3.3.0
+- Support API DescribeCerts.
+- Support API DescribeCloudResources.
+- Support API DescribeDomainDNSRecord.
+- Support API DescribeProductInstances.
+- Support API DescribeResourceRegionId.
+- Support API DescribeResourceSupportRegions.
+- Support API ModifyDefenseResourceXff.
+- Support API ModifyDefenseRuleCache.
+- Support API SyncProductInstance.
+
+
 2024-03-28 Version: 3.2.0
 - Support API DescribeCerts.
 - Support API DescribeDomainDNSRecord.
 - Support API DescribeResourceRegionId.
 - Support API DescribeResourceSupportRegions.
 - Support API ModifyDefenseResourceXff.
 - Support API ModifyDefenseRuleCache.
```

### Comparing `alibabacloud_waf-openapi20211001-3.3.0/LICENSE` & `alibabacloud_waf-openapi20211001-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_waf-openapi20211001-3.3.0/PKG-INFO` & `alibabacloud_waf-openapi20211001-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_waf-openapi20211001
-Version: 3.3.0
+Version: 3.4.0
 Summary: Alibaba Cloud waf-openapi (20211001) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_waf-openapi20211001-3.3.0/README-CN.md` & `alibabacloud_waf-openapi20211001-3.4.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_waf-openapi20211001-3.3.0/README.md` & `alibabacloud_waf-openapi20211001-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001/client.py` & `alibabacloud_waf-openapi20211001-3.4.0/alibabacloud_waf_openapi20211001/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -149,14 +149,96 @@
     async def clear_major_protection_black_ip_async(
         self,
         request: waf_openapi_20211001_models.ClearMajorProtectionBlackIpRequest,
     ) -> waf_openapi_20211001_models.ClearMajorProtectionBlackIpResponse:
         runtime = util_models.RuntimeOptions()
         return await self.clear_major_protection_black_ip_with_options_async(request, runtime)
 
+    def copy_defense_template_with_options(
+        self,
+        request: waf_openapi_20211001_models.CopyDefenseTemplateRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.CopyDefenseTemplateResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CopyDefenseTemplate',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.CopyDefenseTemplateResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def copy_defense_template_with_options_async(
+        self,
+        request: waf_openapi_20211001_models.CopyDefenseTemplateRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.CopyDefenseTemplateResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CopyDefenseTemplate',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.CopyDefenseTemplateResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def copy_defense_template(
+        self,
+        request: waf_openapi_20211001_models.CopyDefenseTemplateRequest,
+    ) -> waf_openapi_20211001_models.CopyDefenseTemplateResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.copy_defense_template_with_options(request, runtime)
+
+    async def copy_defense_template_async(
+        self,
+        request: waf_openapi_20211001_models.CopyDefenseTemplateRequest,
+    ) -> waf_openapi_20211001_models.CopyDefenseTemplateResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.copy_defense_template_with_options_async(request, runtime)
+
     def create_defense_resource_group_with_options(
         self,
         request: waf_openapi_20211001_models.CreateDefenseResourceGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.CreateDefenseResourceGroupResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -747,14 +829,88 @@
     async def create_member_accounts_async(
         self,
         request: waf_openapi_20211001_models.CreateMemberAccountsRequest,
     ) -> waf_openapi_20211001_models.CreateMemberAccountsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.create_member_accounts_with_options_async(request, runtime)
 
+    def create_postpaid_instance_with_options(
+        self,
+        request: waf_openapi_20211001_models.CreatePostpaidInstanceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.CreatePostpaidInstanceResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreatePostpaidInstance',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.CreatePostpaidInstanceResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_postpaid_instance_with_options_async(
+        self,
+        request: waf_openapi_20211001_models.CreatePostpaidInstanceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.CreatePostpaidInstanceResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreatePostpaidInstance',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.CreatePostpaidInstanceResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_postpaid_instance(
+        self,
+        request: waf_openapi_20211001_models.CreatePostpaidInstanceRequest,
+    ) -> waf_openapi_20211001_models.CreatePostpaidInstanceResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.create_postpaid_instance_with_options(request, runtime)
+
+    async def create_postpaid_instance_async(
+        self,
+        request: waf_openapi_20211001_models.CreatePostpaidInstanceRequest,
+    ) -> waf_openapi_20211001_models.CreatePostpaidInstanceResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.create_postpaid_instance_with_options_async(request, runtime)
+
     def delete_defense_resource_group_with_options(
         self,
         request: waf_openapi_20211001_models.DeleteDefenseResourceGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DeleteDefenseResourceGroupResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -1337,14 +1493,96 @@
     async def describe_account_delegated_status_async(
         self,
         request: waf_openapi_20211001_models.DescribeAccountDelegatedStatusRequest,
     ) -> waf_openapi_20211001_models.DescribeAccountDelegatedStatusResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_account_delegated_status_with_options_async(request, runtime)
 
+    def describe_cert_detail_with_options(
+        self,
+        request: waf_openapi_20211001_models.DescribeCertDetailRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeCertDetailResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.cert_identifier):
+            query['CertIdentifier'] = request.cert_identifier
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeCertDetail',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeCertDetailResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_cert_detail_with_options_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeCertDetailRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeCertDetailResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.cert_identifier):
+            query['CertIdentifier'] = request.cert_identifier
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeCertDetail',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeCertDetailResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_cert_detail(
+        self,
+        request: waf_openapi_20211001_models.DescribeCertDetailRequest,
+    ) -> waf_openapi_20211001_models.DescribeCertDetailResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_cert_detail_with_options(request, runtime)
+
+    async def describe_cert_detail_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeCertDetailRequest,
+    ) -> waf_openapi_20211001_models.DescribeCertDetailResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_cert_detail_with_options_async(request, runtime)
+
     def describe_certs_with_options(
         self,
         request: waf_openapi_20211001_models.DescribeCertsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DescribeCertsResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -1549,14 +1787,96 @@
     async def describe_cloud_resources_async(
         self,
         request: waf_openapi_20211001_models.DescribeCloudResourcesRequest,
     ) -> waf_openapi_20211001_models.DescribeCloudResourcesResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_cloud_resources_with_options_async(request, runtime)
 
+    def describe_defense_resource_with_options(
+        self,
+        request: waf_openapi_20211001_models.DescribeDefenseResourceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeDefenseResourceResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource):
+            query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeDefenseResource',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeDefenseResourceResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_defense_resource_with_options_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeDefenseResourceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeDefenseResourceResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource):
+            query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeDefenseResource',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeDefenseResourceResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_defense_resource(
+        self,
+        request: waf_openapi_20211001_models.DescribeDefenseResourceRequest,
+    ) -> waf_openapi_20211001_models.DescribeDefenseResourceResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_defense_resource_with_options(request, runtime)
+
+    async def describe_defense_resource_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeDefenseResourceRequest,
+    ) -> waf_openapi_20211001_models.DescribeDefenseResourceResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_defense_resource_with_options_async(request, runtime)
+
     def describe_defense_resource_group_with_options(
         self,
         request: waf_openapi_20211001_models.DescribeDefenseResourceGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DescribeDefenseResourceGroupResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -1631,14 +1951,288 @@
     async def describe_defense_resource_group_async(
         self,
         request: waf_openapi_20211001_models.DescribeDefenseResourceGroupRequest,
     ) -> waf_openapi_20211001_models.DescribeDefenseResourceGroupResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_defense_resource_group_with_options_async(request, runtime)
 
+    def describe_defense_resource_group_names_with_options(
+        self,
+        request: waf_openapi_20211001_models.DescribeDefenseResourceGroupNamesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeDefenseResourceGroupNamesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.group_name_like):
+            query['GroupNameLike'] = request.group_name_like
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeDefenseResourceGroupNames',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeDefenseResourceGroupNamesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_defense_resource_group_names_with_options_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeDefenseResourceGroupNamesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeDefenseResourceGroupNamesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.group_name_like):
+            query['GroupNameLike'] = request.group_name_like
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeDefenseResourceGroupNames',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeDefenseResourceGroupNamesResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_defense_resource_group_names(
+        self,
+        request: waf_openapi_20211001_models.DescribeDefenseResourceGroupNamesRequest,
+    ) -> waf_openapi_20211001_models.DescribeDefenseResourceGroupNamesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_defense_resource_group_names_with_options(request, runtime)
+
+    async def describe_defense_resource_group_names_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeDefenseResourceGroupNamesRequest,
+    ) -> waf_openapi_20211001_models.DescribeDefenseResourceGroupNamesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_defense_resource_group_names_with_options_async(request, runtime)
+
+    def describe_defense_resource_groups_with_options(
+        self,
+        request: waf_openapi_20211001_models.DescribeDefenseResourceGroupsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeDefenseResourceGroupsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.group_name_like):
+            query['GroupNameLike'] = request.group_name_like
+        if not UtilClient.is_unset(request.group_names):
+            query['GroupNames'] = request.group_names
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeDefenseResourceGroups',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeDefenseResourceGroupsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_defense_resource_groups_with_options_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeDefenseResourceGroupsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeDefenseResourceGroupsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.group_name_like):
+            query['GroupNameLike'] = request.group_name_like
+        if not UtilClient.is_unset(request.group_names):
+            query['GroupNames'] = request.group_names
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeDefenseResourceGroups',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeDefenseResourceGroupsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_defense_resource_groups(
+        self,
+        request: waf_openapi_20211001_models.DescribeDefenseResourceGroupsRequest,
+    ) -> waf_openapi_20211001_models.DescribeDefenseResourceGroupsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_defense_resource_groups_with_options(request, runtime)
+
+    async def describe_defense_resource_groups_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeDefenseResourceGroupsRequest,
+    ) -> waf_openapi_20211001_models.DescribeDefenseResourceGroupsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_defense_resource_groups_with_options_async(request, runtime)
+
+    def describe_defense_resource_names_with_options(
+        self,
+        request: waf_openapi_20211001_models.DescribeDefenseResourceNamesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeDefenseResourceNamesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource):
+            query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeDefenseResourceNames',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeDefenseResourceNamesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_defense_resource_names_with_options_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeDefenseResourceNamesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeDefenseResourceNamesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource):
+            query['Resource'] = request.resource
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeDefenseResourceNames',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeDefenseResourceNamesResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_defense_resource_names(
+        self,
+        request: waf_openapi_20211001_models.DescribeDefenseResourceNamesRequest,
+    ) -> waf_openapi_20211001_models.DescribeDefenseResourceNamesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_defense_resource_names_with_options(request, runtime)
+
+    async def describe_defense_resource_names_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeDefenseResourceNamesRequest,
+    ) -> waf_openapi_20211001_models.DescribeDefenseResourceNamesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_defense_resource_names_with_options_async(request, runtime)
+
     def describe_defense_resource_templates_with_options(
         self,
         request: waf_openapi_20211001_models.DescribeDefenseResourceTemplatesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DescribeDefenseResourceTemplatesResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -2081,14 +2675,112 @@
     async def describe_defense_template_async(
         self,
         request: waf_openapi_20211001_models.DescribeDefenseTemplateRequest,
     ) -> waf_openapi_20211001_models.DescribeDefenseTemplateResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_defense_template_with_options_async(request, runtime)
 
+    def describe_defense_template_valid_groups_with_options(
+        self,
+        request: waf_openapi_20211001_models.DescribeDefenseTemplateValidGroupsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeDefenseTemplateValidGroupsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.defense_scene):
+            query['DefenseScene'] = request.defense_scene
+        if not UtilClient.is_unset(request.group_name):
+            query['GroupName'] = request.group_name
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeDefenseTemplateValidGroups',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeDefenseTemplateValidGroupsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_defense_template_valid_groups_with_options_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeDefenseTemplateValidGroupsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeDefenseTemplateValidGroupsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.defense_scene):
+            query['DefenseScene'] = request.defense_scene
+        if not UtilClient.is_unset(request.group_name):
+            query['GroupName'] = request.group_name
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeDefenseTemplateValidGroups',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeDefenseTemplateValidGroupsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_defense_template_valid_groups(
+        self,
+        request: waf_openapi_20211001_models.DescribeDefenseTemplateValidGroupsRequest,
+    ) -> waf_openapi_20211001_models.DescribeDefenseTemplateValidGroupsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_defense_template_valid_groups_with_options(request, runtime)
+
+    async def describe_defense_template_valid_groups_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeDefenseTemplateValidGroupsRequest,
+    ) -> waf_openapi_20211001_models.DescribeDefenseTemplateValidGroupsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_defense_template_valid_groups_with_options_async(request, runtime)
+
     def describe_defense_templates_with_options(
         self,
         request: waf_openapi_20211001_models.DescribeDefenseTemplatesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DescribeDefenseTemplatesResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -3463,14 +4155,96 @@
     async def describe_product_instances_async(
         self,
         request: waf_openapi_20211001_models.DescribeProductInstancesRequest,
     ) -> waf_openapi_20211001_models.DescribeProductInstancesResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_product_instances_with_options_async(request, runtime)
 
+    def describe_punished_domains_with_options(
+        self,
+        request: waf_openapi_20211001_models.DescribePunishedDomainsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribePunishedDomainsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.domains):
+            query['Domains'] = request.domains
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribePunishedDomains',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribePunishedDomainsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_punished_domains_with_options_async(
+        self,
+        request: waf_openapi_20211001_models.DescribePunishedDomainsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribePunishedDomainsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.domains):
+            query['Domains'] = request.domains
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribePunishedDomains',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribePunishedDomainsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_punished_domains(
+        self,
+        request: waf_openapi_20211001_models.DescribePunishedDomainsRequest,
+    ) -> waf_openapi_20211001_models.DescribePunishedDomainsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_punished_domains_with_options(request, runtime)
+
+    async def describe_punished_domains_async(
+        self,
+        request: waf_openapi_20211001_models.DescribePunishedDomainsRequest,
+    ) -> waf_openapi_20211001_models.DescribePunishedDomainsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_punished_domains_with_options_async(request, runtime)
+
     def describe_resource_instance_certs_with_options(
         self,
         request: waf_openapi_20211001_models.DescribeResourceInstanceCertsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DescribeResourceInstanceCertsResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -4851,14 +5625,96 @@
     async def describe_sls_log_store_status_async(
         self,
         request: waf_openapi_20211001_models.DescribeSlsLogStoreStatusRequest,
     ) -> waf_openapi_20211001_models.DescribeSlsLogStoreStatusResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_sls_log_store_status_with_options_async(request, runtime)
 
+    def describe_template_resource_count_with_options(
+        self,
+        request: waf_openapi_20211001_models.DescribeTemplateResourceCountRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeTemplateResourceCountResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        if not UtilClient.is_unset(request.template_ids):
+            query['TemplateIds'] = request.template_ids
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeTemplateResourceCount',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeTemplateResourceCountResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_template_resource_count_with_options_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeTemplateResourceCountRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeTemplateResourceCountResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        if not UtilClient.is_unset(request.template_ids):
+            query['TemplateIds'] = request.template_ids
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeTemplateResourceCount',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeTemplateResourceCountResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_template_resource_count(
+        self,
+        request: waf_openapi_20211001_models.DescribeTemplateResourceCountRequest,
+    ) -> waf_openapi_20211001_models.DescribeTemplateResourceCountResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_template_resource_count_with_options(request, runtime)
+
+    async def describe_template_resource_count_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeTemplateResourceCountRequest,
+    ) -> waf_openapi_20211001_models.DescribeTemplateResourceCountResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_template_resource_count_with_options_async(request, runtime)
+
     def describe_template_resources_with_options(
         self,
         request: waf_openapi_20211001_models.DescribeTemplateResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DescribeTemplateResourcesResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -5347,14 +6203,264 @@
     async def describe_waf_source_ip_segment_async(
         self,
         request: waf_openapi_20211001_models.DescribeWafSourceIpSegmentRequest,
     ) -> waf_openapi_20211001_models.DescribeWafSourceIpSegmentResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_waf_source_ip_segment_with_options_async(request, runtime)
 
+    def list_tag_keys_with_options(
+        self,
+        request: waf_openapi_20211001_models.ListTagKeysRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.ListTagKeysResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListTagKeys',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.ListTagKeysResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_tag_keys_with_options_async(
+        self,
+        request: waf_openapi_20211001_models.ListTagKeysRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.ListTagKeysResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListTagKeys',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.ListTagKeysResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_tag_keys(
+        self,
+        request: waf_openapi_20211001_models.ListTagKeysRequest,
+    ) -> waf_openapi_20211001_models.ListTagKeysResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_tag_keys_with_options(request, runtime)
+
+    async def list_tag_keys_async(
+        self,
+        request: waf_openapi_20211001_models.ListTagKeysRequest,
+    ) -> waf_openapi_20211001_models.ListTagKeysResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_tag_keys_with_options_async(request, runtime)
+
+    def list_tag_resources_with_options(
+        self,
+        request: waf_openapi_20211001_models.ListTagResourcesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.ListTagResourcesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_id):
+            query['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListTagResources',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.ListTagResourcesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_tag_resources_with_options_async(
+        self,
+        request: waf_openapi_20211001_models.ListTagResourcesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.ListTagResourcesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_id):
+            query['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListTagResources',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.ListTagResourcesResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_tag_resources(
+        self,
+        request: waf_openapi_20211001_models.ListTagResourcesRequest,
+    ) -> waf_openapi_20211001_models.ListTagResourcesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_tag_resources_with_options(request, runtime)
+
+    async def list_tag_resources_async(
+        self,
+        request: waf_openapi_20211001_models.ListTagResourcesRequest,
+    ) -> waf_openapi_20211001_models.ListTagResourcesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_tag_resources_with_options_async(request, runtime)
+
+    def list_tag_values_with_options(
+        self,
+        request: waf_openapi_20211001_models.ListTagValuesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.ListTagValuesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.key):
+            query['Key'] = request.key
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListTagValues',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.ListTagValuesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_tag_values_with_options_async(
+        self,
+        request: waf_openapi_20211001_models.ListTagValuesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.ListTagValuesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.key):
+            query['Key'] = request.key
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListTagValues',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.ListTagValuesResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_tag_values(
+        self,
+        request: waf_openapi_20211001_models.ListTagValuesRequest,
+    ) -> waf_openapi_20211001_models.ListTagValuesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_tag_values_with_options(request, runtime)
+
+    async def list_tag_values_async(
+        self,
+        request: waf_openapi_20211001_models.ListTagValuesRequest,
+    ) -> waf_openapi_20211001_models.ListTagValuesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_tag_values_with_options_async(request, runtime)
+
     def modify_defense_resource_group_with_options(
         self,
         request: waf_openapi_20211001_models.ModifyDefenseResourceGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.ModifyDefenseResourceGroupResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -6087,14 +7193,96 @@
     async def modify_domain_async(
         self,
         request: waf_openapi_20211001_models.ModifyDomainRequest,
     ) -> waf_openapi_20211001_models.ModifyDomainResponse:
         runtime = util_models.RuntimeOptions()
         return await self.modify_domain_with_options_async(request, runtime)
 
+    def modify_domain_punish_status_with_options(
+        self,
+        request: waf_openapi_20211001_models.ModifyDomainPunishStatusRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.ModifyDomainPunishStatusResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.domain):
+            query['Domain'] = request.domain
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyDomainPunishStatus',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.ModifyDomainPunishStatusResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def modify_domain_punish_status_with_options_async(
+        self,
+        request: waf_openapi_20211001_models.ModifyDomainPunishStatusRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.ModifyDomainPunishStatusResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.domain):
+            query['Domain'] = request.domain
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyDomainPunishStatus',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.ModifyDomainPunishStatusResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def modify_domain_punish_status(
+        self,
+        request: waf_openapi_20211001_models.ModifyDomainPunishStatusRequest,
+    ) -> waf_openapi_20211001_models.ModifyDomainPunishStatusResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.modify_domain_punish_status_with_options(request, runtime)
+
+    async def modify_domain_punish_status_async(
+        self,
+        request: waf_openapi_20211001_models.ModifyDomainPunishStatusRequest,
+    ) -> waf_openapi_20211001_models.ModifyDomainPunishStatusResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.modify_domain_punish_status_with_options_async(request, runtime)
+
     def modify_hybrid_cloud_cluster_bypass_status_with_options(
         self,
         request: waf_openapi_20211001_models.ModifyHybridCloudClusterBypassStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.ModifyHybridCloudClusterBypassStatusResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -6640,7 +7828,175 @@
         SyncProductInstance is an asynchronous operation. You can call the [DescribeProductInstances](~~2743168~~) operation to query the status of the task.
         
         @param request: SyncProductInstanceRequest
         @return: SyncProductInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.sync_product_instance_with_options_async(request, runtime)
+
+    def tag_resources_with_options(
+        self,
+        request: waf_openapi_20211001_models.TagResourcesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.TagResourcesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_id):
+            query['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='TagResources',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.TagResourcesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def tag_resources_with_options_async(
+        self,
+        request: waf_openapi_20211001_models.TagResourcesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.TagResourcesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_id):
+            query['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='TagResources',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.TagResourcesResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def tag_resources(
+        self,
+        request: waf_openapi_20211001_models.TagResourcesRequest,
+    ) -> waf_openapi_20211001_models.TagResourcesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.tag_resources_with_options(request, runtime)
+
+    async def tag_resources_async(
+        self,
+        request: waf_openapi_20211001_models.TagResourcesRequest,
+    ) -> waf_openapi_20211001_models.TagResourcesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.tag_resources_with_options_async(request, runtime)
+
+    def untag_resources_with_options(
+        self,
+        request: waf_openapi_20211001_models.UntagResourcesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.UntagResourcesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.all):
+            query['All'] = request.all
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_id):
+            query['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.tag_key):
+            query['TagKey'] = request.tag_key
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UntagResources',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.UntagResourcesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def untag_resources_with_options_async(
+        self,
+        request: waf_openapi_20211001_models.UntagResourcesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.UntagResourcesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.all):
+            query['All'] = request.all
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_id):
+            query['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.tag_key):
+            query['TagKey'] = request.tag_key
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UntagResources',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.UntagResourcesResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def untag_resources(
+        self,
+        request: waf_openapi_20211001_models.UntagResourcesRequest,
+    ) -> waf_openapi_20211001_models.UntagResourcesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.untag_resources_with_options(request, runtime)
+
+    async def untag_resources_async(
+        self,
+        request: waf_openapi_20211001_models.UntagResourcesRequest,
+    ) -> waf_openapi_20211001_models.UntagResourcesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.untag_resources_with_options_async(request, runtime)
```

### Comparing `alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001/models.py` & `alibabacloud_waf-openapi20211001-3.4.0/alibabacloud_waf_openapi20211001/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -130,14 +130,144 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ClearMajorProtectionBlackIpResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CopyDefenseTemplateRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        region_id: str = None,
+        resource_manager_resource_group_id: str = None,
+        template_id: int = None,
+    ):
+        # The ID of the Web Application Firewall (WAF) instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id
+        # The ID of the protection template that you want to copy.
+        self.template_id = template_id
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
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_manager_resource_group_id is not None:
+            result['ResourceManagerResourceGroupId'] = self.resource_manager_resource_group_id
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceManagerResourceGroupId') is not None:
+            self.resource_manager_resource_group_id = m.get('ResourceManagerResourceGroupId')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        return self
+
+
+class CopyDefenseTemplateResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        template_id: int = None,
+    ):
+        # The request ID.
+        self.request_id = request_id
+        # The ID of the new protection template.
+        self.template_id = template_id
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
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        return self
+
+
+class CopyDefenseTemplateResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CopyDefenseTemplateResponseBody = None,
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
+            temp_model = CopyDefenseTemplateResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateDefenseResourceGroupRequest(TeaModel):
     def __init__(
         self,
         add_list: str = None,
         description: str = None,
         group_name: str = None,
         instance_id: str = None,
@@ -1405,18 +1535,28 @@
         self,
         instance_id: str = None,
         member_account_ids: List[str] = None,
         region_id: str = None,
         resource_manager_resource_group_id: str = None,
         source_ip: str = None,
     ):
+        # The ID of the WAF instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
         self.instance_id = instance_id
+        # The Alibaba Cloud account IDs of the members that you want to add. You can add up to 10 members at the same time.
         self.member_account_ids = member_account_ids
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
         self.region_id = region_id
+        # The ID of the Alibaba Cloud resource group.
         self.resource_manager_resource_group_id = resource_manager_resource_group_id
+        # The source IP address of the request. The system automatically obtains the value of this parameter.
         self.source_ip = source_ip
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1452,14 +1592,15 @@
 
 
 class CreateMemberAccountsResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1515,14 +1656,128 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateMemberAccountsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreatePostpaidInstanceRequest(TeaModel):
+    def __init__(
+        self,
+        region_id: str = None,
+        resource_manager_resource_group_id: str = None,
+    ):
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id
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
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_manager_resource_group_id is not None:
+            result['ResourceManagerResourceGroupId'] = self.resource_manager_resource_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceManagerResourceGroupId') is not None:
+            self.resource_manager_resource_group_id = m.get('ResourceManagerResourceGroupId')
+        return self
+
+
+class CreatePostpaidInstanceResponseBody(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        request_id: str = None,
+    ):
+        # The ID of the WAF instance.
+        self.instance_id = instance_id
+        # The ID of the request.
+        self.request_id = request_id
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
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CreatePostpaidInstanceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreatePostpaidInstanceResponseBody = None,
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
+            temp_model = CreatePostpaidInstanceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteDefenseResourceGroupRequest(TeaModel):
     def __init__(
         self,
         group_name: str = None,
         instance_id: str = None,
         region_id: str = None,
         resource_manager_resource_group_id: str = None,
@@ -2170,18 +2425,28 @@
         self,
         instance_id: str = None,
         member_account_id: str = None,
         region_id: str = None,
         resource_manager_resource_group_id: str = None,
         source_ip: str = None,
     ):
+        # The ID of the WAF instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
         self.instance_id = instance_id
+        # The Alibaba Cloud account ID of the managed member.
         self.member_account_id = member_account_id
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
         self.region_id = region_id
+        # The ID of the Alibaba Cloud resource group.
         self.resource_manager_resource_group_id = resource_manager_resource_group_id
+        # The source IP address of the request. The system automatically obtains the value of this parameter.
         self.source_ip = source_ip
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2217,14 +2482,15 @@
 
 
 class DeleteMemberAccountResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2287,16 +2553,24 @@
 class DescribeAccountDelegatedStatusRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         region_id: str = None,
         resource_manager_resource_group_id: str = None,
     ):
+        # The ID of the WAF instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
         self.instance_id = instance_id
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
         self.region_id = region_id
+        # The ID of the Alibaba Cloud resource group.
         self.resource_manager_resource_group_id = resource_manager_resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2327,17 +2601,24 @@
     def __init__(
         self,
         account_id: str = None,
         account_name: str = None,
         delegated_status: bool = None,
         request_id: str = None,
     ):
+        # The ID of the Alibaba Cloud account.
         self.account_id = account_id
+        # The name of the Alibaba Cloud account. This parameter is returned only if the account is the delegated administrator account.
         self.account_name = account_name
+        # Indicates whether the Alibaba Cloud account is the delegated administrator account of the WAF instance.
+        # 
+        # *   **true**\
+        # *   **false**\
         self.delegated_status = delegated_status
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2405,14 +2686,216 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeAccountDelegatedStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeCertDetailRequest(TeaModel):
+    def __init__(
+        self,
+        cert_identifier: str = None,
+        instance_id: str = None,
+        region_id: str = None,
+        resource_manager_resource_group_id: str = None,
+    ):
+        # The ID of the certificate.
+        self.cert_identifier = cert_identifier
+        # The ID of the WAF instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id
+        # The region in which the Web Application Firewall (WAF) instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id
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
+        if self.cert_identifier is not None:
+            result['CertIdentifier'] = self.cert_identifier
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_manager_resource_group_id is not None:
+            result['ResourceManagerResourceGroupId'] = self.resource_manager_resource_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CertIdentifier') is not None:
+            self.cert_identifier = m.get('CertIdentifier')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceManagerResourceGroupId') is not None:
+            self.resource_manager_resource_group_id = m.get('ResourceManagerResourceGroupId')
+        return self
+
+
+class DescribeCertDetailResponseBodyCertDetail(TeaModel):
+    def __init__(
+        self,
+        after_date: int = None,
+        before_date: int = None,
+        cert_identifier: str = None,
+        cert_name: str = None,
+        common_name: str = None,
+        domain: str = None,
+        sans: List[str] = None,
+    ):
+        # The time when the certificate expires. This value is a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
+        self.after_date = after_date
+        # The time when the certificate was issued. This value is a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
+        self.before_date = before_date
+        # The ID of the certificate.
+        self.cert_identifier = cert_identifier
+        # The name of the certificate.
+        self.cert_name = cert_name
+        # The primary domain name, which is a common name.
+        self.common_name = common_name
+        # The domain name that is associated with the certificate.
+        self.domain = domain
+        # The other domain names that are associated with the certificate.
+        self.sans = sans
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
+        if self.after_date is not None:
+            result['AfterDate'] = self.after_date
+        if self.before_date is not None:
+            result['BeforeDate'] = self.before_date
+        if self.cert_identifier is not None:
+            result['CertIdentifier'] = self.cert_identifier
+        if self.cert_name is not None:
+            result['CertName'] = self.cert_name
+        if self.common_name is not None:
+            result['CommonName'] = self.common_name
+        if self.domain is not None:
+            result['Domain'] = self.domain
+        if self.sans is not None:
+            result['Sans'] = self.sans
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AfterDate') is not None:
+            self.after_date = m.get('AfterDate')
+        if m.get('BeforeDate') is not None:
+            self.before_date = m.get('BeforeDate')
+        if m.get('CertIdentifier') is not None:
+            self.cert_identifier = m.get('CertIdentifier')
+        if m.get('CertName') is not None:
+            self.cert_name = m.get('CertName')
+        if m.get('CommonName') is not None:
+            self.common_name = m.get('CommonName')
+        if m.get('Domain') is not None:
+            self.domain = m.get('Domain')
+        if m.get('Sans') is not None:
+            self.sans = m.get('Sans')
+        return self
+
+
+class DescribeCertDetailResponseBody(TeaModel):
+    def __init__(
+        self,
+        cert_detail: DescribeCertDetailResponseBodyCertDetail = None,
+        request_id: str = None,
+    ):
+        # The details of the certificate.
+        self.cert_detail = cert_detail
+        # The ID of the request.
+        self.request_id = request_id
+
+    def validate(self):
+        if self.cert_detail:
+            self.cert_detail.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cert_detail is not None:
+            result['CertDetail'] = self.cert_detail.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CertDetail') is not None:
+            temp_model = DescribeCertDetailResponseBodyCertDetail()
+            self.cert_detail = temp_model.from_map(m['CertDetail'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeCertDetailResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeCertDetailResponseBody = None,
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
+            temp_model = DescribeCertDetailResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeCertsRequest(TeaModel):
     def __init__(
         self,
         algorithm: str = None,
         domain: str = None,
         instance_id: str = None,
         page_number: int = None,
@@ -2953,14 +3436,296 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeCloudResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeDefenseResourceRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        region_id: str = None,
+        resource: str = None,
+        resource_manager_resource_group_id: str = None,
+    ):
+        # The ID of the Web Application Firewall (WAF) instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id
+        # The name of the protected object that you want to query. Only exact queries are supported.
+        self.resource = resource
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id
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
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource is not None:
+            result['Resource'] = self.resource
+        if self.resource_manager_resource_group_id is not None:
+            result['ResourceManagerResourceGroupId'] = self.resource_manager_resource_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('Resource') is not None:
+            self.resource = m.get('Resource')
+        if m.get('ResourceManagerResourceGroupId') is not None:
+            self.resource_manager_resource_group_id = m.get('ResourceManagerResourceGroupId')
+        return self
+
+
+class DescribeDefenseResourceResponseBodyResource(TeaModel):
+    def __init__(
+        self,
+        acw_cookie_status: int = None,
+        acw_secure_status: int = None,
+        acw_v3secure_status: int = None,
+        custom_headers: List[str] = None,
+        description: str = None,
+        detail: Dict[str, Any] = None,
+        gmt_create: int = None,
+        gmt_modified: int = None,
+        owner_user_id: str = None,
+        pattern: str = None,
+        product: str = None,
+        resource: str = None,
+        resource_group: str = None,
+        resource_manager_resource_group_id: str = None,
+        resource_origin: str = None,
+        xff_status: int = None,
+    ):
+        # The status of the tracking cookie.
+        # 
+        # *   **0**: disabled.
+        # *   **1**: enabled.
+        self.acw_cookie_status = acw_cookie_status
+        # The status of the secure attribute of the tracking cookie.
+        # 
+        # *   **0**: disabled.
+        # *   **1**: enabled.
+        self.acw_secure_status = acw_secure_status
+        # The status of the secure attribute of the slider CAPTCHA cookie.
+        # 
+        # *   **0**: disabled.
+        # *   **1**: enabled.
+        self.acw_v3secure_status = acw_v3secure_status
+        # The custom header fields.
+        # 
+        # >  If the value of XffStatus is 1, the first IP address in the specified header field is used as the originating IP address of the client to prevent X-Forwarded-For (XFF) forgery. If you specify multiple header fields, WAF reads the values of the header fields in sequence until the originating IP address is obtained. If the originating IP address cannot be obtained, the first IP address in the XFF header field is used as the originating IP address of the client.
+        self.custom_headers = custom_headers
+        # The description of the protected object.
+        self.description = description
+        # The details of the protected object. Different key-value pairs indicate different attributes of the protected object.
+        self.detail = detail
+        # The time when the protected object was created. Unit: milliseconds.
+        self.gmt_create = gmt_create
+        # The time when the protected object was modified. Unit: milliseconds.
+        self.gmt_modified = gmt_modified
+        # The user ID (UID) of the Alibaba Cloud account to which the protected object belongs.
+        self.owner_user_id = owner_user_id
+        # The pattern used for the protected object.
+        self.pattern = pattern
+        # The name of the cloud service.
+        self.product = product
+        # The name of the protected object.
+        self.resource = resource
+        # The name of the protected object group to which the protected object belongs.
+        self.resource_group = resource_group
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id
+        # The origin of the protected object. Valid values:
+        # 
+        # *   **custom**\
+        # *   **access**\
+        self.resource_origin = resource_origin
+        # Indicates whether a Layer 7 proxy is deployed in front of WAF, such as Anti-DDoS Proxy and Alibaba Cloud CDN. Valid values:
+        # 
+        # *   **0**: No Layer 7 proxy is deployed.
+        # *   **1**: A Layer 7 proxy is deployed.
+        self.xff_status = xff_status
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
+        if self.acw_cookie_status is not None:
+            result['AcwCookieStatus'] = self.acw_cookie_status
+        if self.acw_secure_status is not None:
+            result['AcwSecureStatus'] = self.acw_secure_status
+        if self.acw_v3secure_status is not None:
+            result['AcwV3SecureStatus'] = self.acw_v3secure_status
+        if self.custom_headers is not None:
+            result['CustomHeaders'] = self.custom_headers
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.detail is not None:
+            result['Detail'] = self.detail
+        if self.gmt_create is not None:
+            result['GmtCreate'] = self.gmt_create
+        if self.gmt_modified is not None:
+            result['GmtModified'] = self.gmt_modified
+        if self.owner_user_id is not None:
+            result['OwnerUserId'] = self.owner_user_id
+        if self.pattern is not None:
+            result['Pattern'] = self.pattern
+        if self.product is not None:
+            result['Product'] = self.product
+        if self.resource is not None:
+            result['Resource'] = self.resource
+        if self.resource_group is not None:
+            result['ResourceGroup'] = self.resource_group
+        if self.resource_manager_resource_group_id is not None:
+            result['ResourceManagerResourceGroupId'] = self.resource_manager_resource_group_id
+        if self.resource_origin is not None:
+            result['ResourceOrigin'] = self.resource_origin
+        if self.xff_status is not None:
+            result['XffStatus'] = self.xff_status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AcwCookieStatus') is not None:
+            self.acw_cookie_status = m.get('AcwCookieStatus')
+        if m.get('AcwSecureStatus') is not None:
+            self.acw_secure_status = m.get('AcwSecureStatus')
+        if m.get('AcwV3SecureStatus') is not None:
+            self.acw_v3secure_status = m.get('AcwV3SecureStatus')
+        if m.get('CustomHeaders') is not None:
+            self.custom_headers = m.get('CustomHeaders')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('Detail') is not None:
+            self.detail = m.get('Detail')
+        if m.get('GmtCreate') is not None:
+            self.gmt_create = m.get('GmtCreate')
+        if m.get('GmtModified') is not None:
+            self.gmt_modified = m.get('GmtModified')
+        if m.get('OwnerUserId') is not None:
+            self.owner_user_id = m.get('OwnerUserId')
+        if m.get('Pattern') is not None:
+            self.pattern = m.get('Pattern')
+        if m.get('Product') is not None:
+            self.product = m.get('Product')
+        if m.get('Resource') is not None:
+            self.resource = m.get('Resource')
+        if m.get('ResourceGroup') is not None:
+            self.resource_group = m.get('ResourceGroup')
+        if m.get('ResourceManagerResourceGroupId') is not None:
+            self.resource_manager_resource_group_id = m.get('ResourceManagerResourceGroupId')
+        if m.get('ResourceOrigin') is not None:
+            self.resource_origin = m.get('ResourceOrigin')
+        if m.get('XffStatus') is not None:
+            self.xff_status = m.get('XffStatus')
+        return self
+
+
+class DescribeDefenseResourceResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        resource: DescribeDefenseResourceResponseBodyResource = None,
+    ):
+        # The request ID.
+        self.request_id = request_id
+        # The information about the protected object.
+        self.resource = resource
+
+    def validate(self):
+        if self.resource:
+            self.resource.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.resource is not None:
+            result['Resource'] = self.resource.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Resource') is not None:
+            temp_model = DescribeDefenseResourceResponseBodyResource()
+            self.resource = temp_model.from_map(m['Resource'])
+        return self
+
+
+class DescribeDefenseResourceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeDefenseResourceResponseBody = None,
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
+            temp_model = DescribeDefenseResourceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeDefenseResourceGroupRequest(TeaModel):
     def __init__(
         self,
         group_name: str = None,
         instance_id: str = None,
         region_id: str = None,
         resource_manager_resource_group_id: str = None,
@@ -3141,14 +3906,538 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeDefenseResourceGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeDefenseResourceGroupNamesRequest(TeaModel):
+    def __init__(
+        self,
+        group_name_like: str = None,
+        instance_id: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        region_id: str = None,
+        resource_manager_resource_group_id: str = None,
+    ):
+        # The name of the protected object group. Fuzzy queries are supported.
+        self.group_name_like = group_name_like
+        # The ID of the Web Application Firewall (WAF) instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id
+        # The page number. Default value: **1**.
+        self.page_number = page_number
+        # The number of entries per page. Default value: **20**.
+        self.page_size = page_size
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id
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
+        if self.group_name_like is not None:
+            result['GroupNameLike'] = self.group_name_like
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_manager_resource_group_id is not None:
+            result['ResourceManagerResourceGroupId'] = self.resource_manager_resource_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('GroupNameLike') is not None:
+            self.group_name_like = m.get('GroupNameLike')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceManagerResourceGroupId') is not None:
+            self.resource_manager_resource_group_id = m.get('ResourceManagerResourceGroupId')
+        return self
+
+
+class DescribeDefenseResourceGroupNamesResponseBody(TeaModel):
+    def __init__(
+        self,
+        group_names: List[str] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        # The names of the protected object groups.
+        self.group_names = group_names
+        # The request ID.
+        self.request_id = request_id
+        # The total number of entries returned.
+        self.total_count = total_count
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
+        if self.group_names is not None:
+            result['GroupNames'] = self.group_names
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('GroupNames') is not None:
+            self.group_names = m.get('GroupNames')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class DescribeDefenseResourceGroupNamesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeDefenseResourceGroupNamesResponseBody = None,
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
+            temp_model = DescribeDefenseResourceGroupNamesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeDefenseResourceGroupsRequest(TeaModel):
+    def __init__(
+        self,
+        group_name_like: str = None,
+        group_names: str = None,
+        instance_id: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        region_id: str = None,
+        resource_manager_resource_group_id: str = None,
+    ):
+        # The name of the protected object group that you want to query. Fuzzy queries are supported.
+        self.group_name_like = group_name_like
+        # The names of the protected object groups that you want to query. Separate multiple names with commas (,).
+        self.group_names = group_names
+        # The ID of the Web Application Firewall (WAF) instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id
+        # The page number. Default value: **1**.
+        self.page_number = page_number
+        # The number of entries per page. Default value: **20**.
+        self.page_size = page_size
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id
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
+        if self.group_name_like is not None:
+            result['GroupNameLike'] = self.group_name_like
+        if self.group_names is not None:
+            result['GroupNames'] = self.group_names
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_manager_resource_group_id is not None:
+            result['ResourceManagerResourceGroupId'] = self.resource_manager_resource_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('GroupNameLike') is not None:
+            self.group_name_like = m.get('GroupNameLike')
+        if m.get('GroupNames') is not None:
+            self.group_names = m.get('GroupNames')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceManagerResourceGroupId') is not None:
+            self.resource_manager_resource_group_id = m.get('ResourceManagerResourceGroupId')
+        return self
+
+
+class DescribeDefenseResourceGroupsResponseBodyGroups(TeaModel):
+    def __init__(
+        self,
+        description: str = None,
+        gmt_create: int = None,
+        gmt_modified: int = None,
+        group_name: str = None,
+        resource_list: str = None,
+    ):
+        # The description of the protected object group.
+        self.description = description
+        # The time when the protected object group was created. Unit: milliseconds.
+        self.gmt_create = gmt_create
+        # The most recent time when the protected object group was modified. Unit: milliseconds.
+        self.gmt_modified = gmt_modified
+        # The name of the protected object group.
+        self.group_name = group_name
+        # The names of the protected objects that are added to the protected object group. Separate multiple protected objects with commas (,).
+        self.resource_list = resource_list
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
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.gmt_create is not None:
+            result['GmtCreate'] = self.gmt_create
+        if self.gmt_modified is not None:
+            result['GmtModified'] = self.gmt_modified
+        if self.group_name is not None:
+            result['GroupName'] = self.group_name
+        if self.resource_list is not None:
+            result['ResourceList'] = self.resource_list
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('GmtCreate') is not None:
+            self.gmt_create = m.get('GmtCreate')
+        if m.get('GmtModified') is not None:
+            self.gmt_modified = m.get('GmtModified')
+        if m.get('GroupName') is not None:
+            self.group_name = m.get('GroupName')
+        if m.get('ResourceList') is not None:
+            self.resource_list = m.get('ResourceList')
+        return self
+
+
+class DescribeDefenseResourceGroupsResponseBody(TeaModel):
+    def __init__(
+        self,
+        groups: List[DescribeDefenseResourceGroupsResponseBodyGroups] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        # The list of protected object groups.
+        self.groups = groups
+        # The request ID.
+        self.request_id = request_id
+        # The total number of entries returned.
+        self.total_count = total_count
+
+    def validate(self):
+        if self.groups:
+            for k in self.groups:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Groups'] = []
+        if self.groups is not None:
+            for k in self.groups:
+                result['Groups'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.groups = []
+        if m.get('Groups') is not None:
+            for k in m.get('Groups'):
+                temp_model = DescribeDefenseResourceGroupsResponseBodyGroups()
+                self.groups.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class DescribeDefenseResourceGroupsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeDefenseResourceGroupsResponseBody = None,
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
+            temp_model = DescribeDefenseResourceGroupsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeDefenseResourceNamesRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        region_id: str = None,
+        resource: str = None,
+        resource_manager_resource_group_id: str = None,
+    ):
+        # The ID of the Web Application Firewall (WAF) instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id
+        # The page number. Default value: **1**.
+        self.page_number = page_number
+        # The number of entries per page. Default value: **20**.
+        self.page_size = page_size
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id
+        # The name of the protected object that you want to query.
+        self.resource = resource
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id
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
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource is not None:
+            result['Resource'] = self.resource
+        if self.resource_manager_resource_group_id is not None:
+            result['ResourceManagerResourceGroupId'] = self.resource_manager_resource_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('Resource') is not None:
+            self.resource = m.get('Resource')
+        if m.get('ResourceManagerResourceGroupId') is not None:
+            self.resource_manager_resource_group_id = m.get('ResourceManagerResourceGroupId')
+        return self
+
+
+class DescribeDefenseResourceNamesResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        resources: List[str] = None,
+        total_count: int = None,
+    ):
+        # The ID of the request.
+        self.request_id = request_id
+        # The names of the protected objects.
+        self.resources = resources
+        # The total number of entries returned.
+        self.total_count = total_count
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
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.resources is not None:
+            result['Resources'] = self.resources
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Resources') is not None:
+            self.resources = m.get('Resources')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class DescribeDefenseResourceNamesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeDefenseResourceNamesResponseBody = None,
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
+            temp_model = DescribeDefenseResourceNamesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeDefenseResourceTemplatesRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         region_id: str = None,
         resource: str = None,
         resource_manager_resource_group_id: str = None,
@@ -3561,15 +4850,15 @@
         # *   **1:** enabled.
         self.acw_cookie_status = acw_cookie_status
         # The status of the secure attribute in the tracking cookie.
         # 
         # *   **0:** disabled.
         # *   **1:** enabled.
         self.acw_secure_status = acw_secure_status
-        # The status of the slider CAPTCHA cookie.
+        # The status of the secure attribute in the slider CAPTCHA cookie.
         # 
         # *   **0:** disabled.
         # *   **1:** enabled.
         self.acw_v3secure_status = acw_v3secure_status
         # The custom XFF headers that are used to identify the originating IP addresses of clients. If the value of XffStatus is 1 and CustomHeaders is left empty, the first IP addresses in the XFF headers are used as the originating IP addresses of clients.
         self.custom_headers = custom_headers
         # The description of the protected object.
@@ -3590,15 +4879,15 @@
         self.resource = resource
         # The name of the protected object group to which the protected object belongs.
         self.resource_group = resource_group
         # The ID of the Alibaba Cloud resource group.
         self.resource_manager_resource_group_id = resource_manager_resource_group_id
         # The origin of the protected object.
         self.resource_origin = resource_origin
-        # Indicates whether the X-Forwarded-For (XFF) proxy feature is enabled for the protected object.
+        # Indicates whether the X-Forwarded-For (XFF) proxy is enabled.
         self.xff_status = xff_status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4466,14 +5755,190 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeDefenseTemplateResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeDefenseTemplateValidGroupsRequest(TeaModel):
+    def __init__(
+        self,
+        defense_scene: str = None,
+        group_name: str = None,
+        instance_id: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        region_id: str = None,
+        resource_manager_resource_group_id: str = None,
+        template_id: int = None,
+    ):
+        # The scenario in which the protection template is used.
+        # 
+        # *   **waf_group**: basic protection.
+        # *   **antiscan**: scan protection.
+        # *   **ip_blacklist**: IP address blacklist.
+        # *   **custom_acl**: custom rule.
+        # *   **whitelist**: whitelist.
+        # *   **region_block**: region blacklist.
+        # *   **custom_response**: custom response.
+        # *   **cc**: HTTP flood protection.
+        # *   **tamperproof**: website tamper-proofing.
+        # *   **dlp**: data leakage prevention.
+        self.defense_scene = defense_scene
+        # The name of the protected object group that you want to query.
+        self.group_name = group_name
+        # The ID of the Web Application Firewall (WAF) instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id
+        # The page number. Default value: **1**.
+        self.page_number = page_number
+        # The number of entries per page. Default value: **20**.
+        self.page_size = page_size
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id
+        # The ID of the protection template.
+        self.template_id = template_id
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
+        if self.defense_scene is not None:
+            result['DefenseScene'] = self.defense_scene
+        if self.group_name is not None:
+            result['GroupName'] = self.group_name
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_manager_resource_group_id is not None:
+            result['ResourceManagerResourceGroupId'] = self.resource_manager_resource_group_id
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DefenseScene') is not None:
+            self.defense_scene = m.get('DefenseScene')
+        if m.get('GroupName') is not None:
+            self.group_name = m.get('GroupName')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceManagerResourceGroupId') is not None:
+            self.resource_manager_resource_group_id = m.get('ResourceManagerResourceGroupId')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        return self
+
+
+class DescribeDefenseTemplateValidGroupsResponseBody(TeaModel):
+    def __init__(
+        self,
+        groups: List[str] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        # The names of the protected object groups.
+        self.groups = groups
+        # The ID of the request.
+        self.request_id = request_id
+        # The total number of entries returned.
+        self.total_count = total_count
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
+        if self.groups is not None:
+            result['Groups'] = self.groups
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Groups') is not None:
+            self.groups = m.get('Groups')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class DescribeDefenseTemplateValidGroupsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeDefenseTemplateValidGroupsResponseBody = None,
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
+            temp_model = DescribeDefenseTemplateValidGroupsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeDefenseTemplatesRequest(TeaModel):
     def __init__(
         self,
         defense_scene: str = None,
         defense_sub_scene: str = None,
         instance_id: str = None,
         page_number: int = None,
@@ -8732,18 +10197,32 @@
         self,
         account_status: str = None,
         instance_id: str = None,
         region_id: str = None,
         resource_manager_resource_group_id: str = None,
         source_ip: str = None,
     ):
+        # The status of the member that you want to query.
+        # 
+        # *   **enabled**: managed.
+        # *   **disabled**: not managed.
+        # *   **disabling**: being deleted.
         self.account_status = account_status
+        # The ID of the Web Application Firewall (WAF) instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
         self.instance_id = instance_id
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
         self.region_id = region_id
+        # The ID of the Alibaba Cloud resource group.
         self.resource_manager_resource_group_id = resource_manager_resource_group_id
+        # The source IP address of the request. The system specifies this parameter.
         self.source_ip = source_ip
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8783,18 +10262,27 @@
         self,
         account_id: str = None,
         account_name: str = None,
         account_status: str = None,
         description: str = None,
         gmt_create: int = None,
     ):
+        # The ID of the member.
         self.account_id = account_id
+        # The name of the member.
         self.account_name = account_name
+        # The status of the member.
+        # 
+        # *   **enabled**: managed.
+        # *   **disabled**: not managed.
+        # *   **disabling**: being deleted.
         self.account_status = account_status
+        # The description of the member.
         self.description = description
+        # The time when the member was added.
         self.gmt_create = gmt_create
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8831,15 +10319,17 @@
 
 class DescribeMemberAccountsResponseBody(TeaModel):
     def __init__(
         self,
         account_infos: List[DescribeMemberAccountsResponseBodyAccountInfos] = None,
         request_id: str = None,
     ):
+        # The information about the member.
         self.account_infos = account_infos
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.account_infos:
             for k in self.account_infos:
                 if k:
                     k.validate()
@@ -9148,14 +10638,15 @@
         resource_product: str = None,
         resource_region_id: str = None,
     ):
         # The ID of the WAF instance.
         # 
         # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
         self.instance_id = instance_id
+        # The ID of the Alibaba Cloud account to which the resource belongs.
         self.owner_user_id = owner_user_id
         # The page number. Default value: **1**.
         self.page_number = page_number
         # The number of entries per page. Default value: **10**.
         self.page_size = page_size
         # The region in which the WAF instance is deployed. Valid values:
         # 
@@ -9518,29 +11009,170 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeProductInstancesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribePunishedDomainsRequest(TeaModel):
+    def __init__(
+        self,
+        domains: List[str] = None,
+        instance_id: str = None,
+        region_id: str = None,
+        resource_manager_resource_group_id: str = None,
+    ):
+        # The domain names.
+        self.domains = domains
+        # The ID of the WAF instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id
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
+        if self.domains is not None:
+            result['Domains'] = self.domains
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_manager_resource_group_id is not None:
+            result['ResourceManagerResourceGroupId'] = self.resource_manager_resource_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Domains') is not None:
+            self.domains = m.get('Domains')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceManagerResourceGroupId') is not None:
+            self.resource_manager_resource_group_id = m.get('ResourceManagerResourceGroupId')
+        return self
+
+
+class DescribePunishedDomainsResponseBody(TeaModel):
+    def __init__(
+        self,
+        punished_domains: List[str] = None,
+        request_id: str = None,
+    ):
+        # The domain names that are penalized for failing to obtain an ICP filing.
+        self.punished_domains = punished_domains
+        # The request ID.
+        self.request_id = request_id
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
+        if self.punished_domains is not None:
+            result['PunishedDomains'] = self.punished_domains
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('PunishedDomains') is not None:
+            self.punished_domains = m.get('PunishedDomains')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribePunishedDomainsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribePunishedDomainsResponseBody = None,
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
+            temp_model = DescribePunishedDomainsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeResourceInstanceCertsRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         page_number: int = None,
         page_size: int = None,
         region_id: str = None,
         resource_instance_id: str = None,
         resource_manager_resource_group_id: str = None,
     ):
+        # The ID of the WAF instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
         self.instance_id = instance_id
+        # The page number. Default value: **1**.
         self.page_number = page_number
+        # The number of entries per page. Default value: **10**.
         self.page_size = page_size
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
         self.region_id = region_id
+        # The ID of the instance.
         self.resource_instance_id = resource_instance_id
+        # The ID of the Alibaba Cloud resource group.
         self.resource_manager_resource_group_id = resource_manager_resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9586,20 +11218,27 @@
         before_date: int = None,
         cert_identifier: str = None,
         cert_name: str = None,
         common_name: str = None,
         domain: str = None,
         is_chain_completed: bool = None,
     ):
+        # The time when the certificate expires.
         self.after_date = after_date
+        # The time when the certificate was issued.
         self.before_date = before_date
+        # The globally unique ID of the certificate. The value is in the "Certificate ID-cn-hangzhou" format. For example, if the ID of the certificate is 123, the value of CertIdentifier is 123-cn-hangzhou.
         self.cert_identifier = cert_identifier
+        # The name of the certificate.
         self.cert_name = cert_name
+        # The common name.
         self.common_name = common_name
+        # The domain name for which the certificate is issued.
         self.domain = domain
+        # Indicates whether the certificate chain is complete.
         self.is_chain_completed = is_chain_completed
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9645,16 +11284,19 @@
 class DescribeResourceInstanceCertsResponseBody(TeaModel):
     def __init__(
         self,
         certs: List[DescribeResourceInstanceCertsResponseBodyCerts] = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The certificates.
         self.certs = certs
+        # The request ID.
         self.request_id = request_id
+        # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
         if self.certs:
             for k in self.certs:
                 if k:
                     k.validate()
@@ -10368,22 +12010,25 @@
 
 
 class DescribeResponseCodeTrendGraphResponseBodyResponseCodes(TeaModel):
     def __init__(
         self,
         code_302pv: int = None,
         code_405pv: int = None,
+        code_444pv: int = None,
         code_499pv: int = None,
         code_5xx_pv: int = None,
         index: int = None,
     ):
         # The number of 302 error codes that are returned.
         self.code_302pv = code_302pv
         # The number of 405 error codes that are returned.
         self.code_405pv = code_405pv
+        # The number of 444 error codes that are returned.
+        self.code_444pv = code_444pv
         # The number of 499 error codes that are returned.
         self.code_499pv = code_499pv
         # The number of 5xx error codes that are returned.
         self.code_5xx_pv = code_5xx_pv
         # The serial number of the time interval. The serial numbers are arranged in chronological order.
         self.index = index
 
@@ -10396,28 +12041,32 @@
             return _map
 
         result = dict()
         if self.code_302pv is not None:
             result['302Pv'] = self.code_302pv
         if self.code_405pv is not None:
             result['405Pv'] = self.code_405pv
+        if self.code_444pv is not None:
+            result['444Pv'] = self.code_444pv
         if self.code_499pv is not None:
             result['499Pv'] = self.code_499pv
         if self.code_5xx_pv is not None:
             result['5xxPv'] = self.code_5xx_pv
         if self.index is not None:
             result['Index'] = self.index
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('302Pv') is not None:
             self.code_302pv = m.get('302Pv')
         if m.get('405Pv') is not None:
             self.code_405pv = m.get('405Pv')
+        if m.get('444Pv') is not None:
+            self.code_444pv = m.get('444Pv')
         if m.get('499Pv') is not None:
             self.code_499pv = m.get('499Pv')
         if m.get('5xxPv') is not None:
             self.code_5xx_pv = m.get('5xxPv')
         if m.get('Index') is not None:
             self.index = m.get('Index')
         return self
@@ -12332,14 +13981,194 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeSlsLogStoreStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeTemplateResourceCountRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        region_id: str = None,
+        resource_manager_resource_group_id: str = None,
+        template_ids: str = None,
+    ):
+        # The ID of the Web Application Firewall (WAF) instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id
+        # The IDs of the protection templates that you want to query. Separate multiple template IDs with commas (,).
+        self.template_ids = template_ids
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
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_manager_resource_group_id is not None:
+            result['ResourceManagerResourceGroupId'] = self.resource_manager_resource_group_id
+        if self.template_ids is not None:
+            result['TemplateIds'] = self.template_ids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceManagerResourceGroupId') is not None:
+            self.resource_manager_resource_group_id = m.get('ResourceManagerResourceGroupId')
+        if m.get('TemplateIds') is not None:
+            self.template_ids = m.get('TemplateIds')
+        return self
+
+
+class DescribeTemplateResourceCountResponseBodyResourceCount(TeaModel):
+    def __init__(
+        self,
+        group_count: int = None,
+        single_count: int = None,
+        template_id: int = None,
+    ):
+        # The number of protected object groups.
+        self.group_count = group_count
+        # The number of protected objects.
+        self.single_count = single_count
+        # The ID of the protection template.
+        self.template_id = template_id
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
+        if self.group_count is not None:
+            result['GroupCount'] = self.group_count
+        if self.single_count is not None:
+            result['SingleCount'] = self.single_count
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('GroupCount') is not None:
+            self.group_count = m.get('GroupCount')
+        if m.get('SingleCount') is not None:
+            self.single_count = m.get('SingleCount')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        return self
+
+
+class DescribeTemplateResourceCountResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        resource_count: List[DescribeTemplateResourceCountResponseBodyResourceCount] = None,
+    ):
+        # The request ID.
+        self.request_id = request_id
+        # The number of protected objects or protected object groups for which the protection template takes effect.
+        self.resource_count = resource_count
+
+    def validate(self):
+        if self.resource_count:
+            for k in self.resource_count:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['ResourceCount'] = []
+        if self.resource_count is not None:
+            for k in self.resource_count:
+                result['ResourceCount'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.resource_count = []
+        if m.get('ResourceCount') is not None:
+            for k in m.get('ResourceCount'):
+                temp_model = DescribeTemplateResourceCountResponseBodyResourceCount()
+                self.resource_count.append(temp_model.from_map(k))
+        return self
+
+
+class DescribeTemplateResourceCountResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeTemplateResourceCountResponseBody = None,
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
+            temp_model = DescribeTemplateResourceCountResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeTemplateResourcesRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         region_id: str = None,
         resource_manager_resource_group_id: str = None,
         resource_type: str = None,
@@ -13302,14 +15131,574 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeWafSourceIpSegmentResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListTagKeysRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        next_token: str = None,
+        region_id: str = None,
+        resource_type: str = None,
+    ):
+        # The ID of the WAF instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id
+        # The pagination token that is used in the next request to retrieve a new page of results.
+        self.next_token = next_token
+        # The region in which the Web Application Firewall (WAF) instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id
+        # The type of the resource. Set the value to ALIYUN::WAF::DEFENSERESOURCE.
+        self.resource_type = resource_type
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
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        return self
+
+
+class ListTagKeysResponseBodyKeys(TeaModel):
+    def __init__(
+        self,
+        category: str = None,
+        key: str = None,
+    ):
+        # The type of the tag. Valid values:
+        # 
+        # *   custom
+        # *   system
+        self.category = category
+        # The key of the tag.
+        self.key = key
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
+        if self.category is not None:
+            result['Category'] = self.category
+        if self.key is not None:
+            result['Key'] = self.key
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Category') is not None:
+            self.category = m.get('Category')
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        return self
+
+
+class ListTagKeysResponseBody(TeaModel):
+    def __init__(
+        self,
+        keys: List[ListTagKeysResponseBodyKeys] = None,
+        next_token: str = None,
+        request_id: str = None,
+    ):
+        # The keys and types of the tags.
+        self.keys = keys
+        # A pagination token. It can be used in the next request to retrieve a new page of results. If NextToken is empty, no next page exists.
+        self.next_token = next_token
+        # The request ID.
+        self.request_id = request_id
+
+    def validate(self):
+        if self.keys:
+            for k in self.keys:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Keys'] = []
+        if self.keys is not None:
+            for k in self.keys:
+                result['Keys'].append(k.to_map() if k else None)
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.keys = []
+        if m.get('Keys') is not None:
+            for k in m.get('Keys'):
+                temp_model = ListTagKeysResponseBodyKeys()
+                self.keys.append(temp_model.from_map(k))
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ListTagKeysResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListTagKeysResponseBody = None,
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
+            temp_model = ListTagKeysResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListTagResourcesRequestTag(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        # The key of tag N that is added to the resource. Valid values of N: 1 to 20.
+        self.key = key
+        # The value of tag N that is added to the resource. Valid values of N: 1 to 20.
+        self.value = value
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
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class ListTagResourcesRequest(TeaModel):
+    def __init__(
+        self,
+        next_token: str = None,
+        region_id: str = None,
+        resource_id: List[str] = None,
+        resource_type: str = None,
+        tag: List[ListTagResourcesRequestTag] = None,
+    ):
+        # The pagination token that is used in the next request to retrieve a new page of results.
+        self.next_token = next_token
+        # The region in which the Web Application Firewall (WAF) instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id
+        # The resource IDs. You can specify up to 50 resource IDs.
+        self.resource_id = resource_id
+        # The type of the resource. Set the value to ALIYUN::WAF::DEFENSERESOURCE.
+        self.resource_type = resource_type
+        # The tags that are added to the resource.
+        self.tag = tag
+
+    def validate(self):
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_id is not None:
+            result['ResourceId'] = self.resource_id
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceId') is not None:
+            self.resource_id = m.get('ResourceId')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = ListTagResourcesRequestTag()
+                self.tag.append(temp_model.from_map(k))
+        return self
+
+
+class ListTagResourcesResponseBodyTagResources(TeaModel):
+    def __init__(
+        self,
+        resource_id: str = None,
+        resource_type: str = None,
+        tag_key: str = None,
+        tag_value: str = None,
+    ):
+        # The resource ID.
+        self.resource_id = resource_id
+        # The type of the resource. ALIYUN::WAF::DEFENSERESOURCE is returned.
+        self.resource_type = resource_type
+        # The key of tag N that is added to the resource.
+        self.tag_key = tag_key
+        # The value of tag N that is added to the resource.
+        self.tag_value = tag_value
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
+        if self.resource_id is not None:
+            result['ResourceId'] = self.resource_id
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        if self.tag_key is not None:
+            result['TagKey'] = self.tag_key
+        if self.tag_value is not None:
+            result['TagValue'] = self.tag_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ResourceId') is not None:
+            self.resource_id = m.get('ResourceId')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        if m.get('TagKey') is not None:
+            self.tag_key = m.get('TagKey')
+        if m.get('TagValue') is not None:
+            self.tag_value = m.get('TagValue')
+        return self
+
+
+class ListTagResourcesResponseBody(TeaModel):
+    def __init__(
+        self,
+        next_token: str = None,
+        request_id: str = None,
+        tag_resources: List[ListTagResourcesResponseBodyTagResources] = None,
+    ):
+        # A pagination token. It can be used in the next request to retrieve a new page of results. If NextToken is empty, no next page exists.
+        self.next_token = next_token
+        # The request ID.
+        self.request_id = request_id
+        # The list of resources.
+        self.tag_resources = tag_resources
+
+    def validate(self):
+        if self.tag_resources:
+            for k in self.tag_resources:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['TagResources'] = []
+        if self.tag_resources is not None:
+            for k in self.tag_resources:
+                result['TagResources'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.tag_resources = []
+        if m.get('TagResources') is not None:
+            for k in m.get('TagResources'):
+                temp_model = ListTagResourcesResponseBodyTagResources()
+                self.tag_resources.append(temp_model.from_map(k))
+        return self
+
+
+class ListTagResourcesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListTagResourcesResponseBody = None,
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
+            temp_model = ListTagResourcesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListTagValuesRequest(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        next_token: str = None,
+        region_id: str = None,
+        resource_type: str = None,
+    ):
+        # The tag key.
+        self.key = key
+        # The pagination token that is used in the next request to retrieve a new page of results.
+        self.next_token = next_token
+        # The region in which the Web Application Firewall (WAF) instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id
+        # The type of the resource. Set the value to ALIYUN::WAF::DEFENSERESOURCE.
+        self.resource_type = resource_type
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
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        return self
+
+
+class ListTagValuesResponseBody(TeaModel):
+    def __init__(
+        self,
+        next_token: str = None,
+        request_id: str = None,
+        values: List[str] = None,
+    ):
+        # A pagination token. It can be used in the next request to retrieve a new page of results. If NextToken is empty, no next page exists.
+        self.next_token = next_token
+        # The request ID.
+        self.request_id = request_id
+        # The tag values.
+        self.values = values
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
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.values is not None:
+            result['Values'] = self.values
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Values') is not None:
+            self.values = m.get('Values')
+        return self
+
+
+class ListTagValuesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListTagValuesResponseBody = None,
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
+            temp_model = ListTagValuesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ModifyDefenseResourceGroupRequest(TeaModel):
     def __init__(
         self,
         add_list: str = None,
         delete_list: str = None,
         description: str = None,
         group_name: str = None,
@@ -14954,14 +17343,137 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyDomainResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ModifyDomainPunishStatusRequest(TeaModel):
+    def __init__(
+        self,
+        domain: str = None,
+        instance_id: str = None,
+        region_id: str = None,
+        resource_manager_resource_group_id: str = None,
+    ):
+        # The domain name that is penalized for failing to obtain an ICP filing.
+        self.domain = domain
+        # The ID of the WAF instance.
+        # 
+        # > You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id
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
+        if self.domain is not None:
+            result['Domain'] = self.domain
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_manager_resource_group_id is not None:
+            result['ResourceManagerResourceGroupId'] = self.resource_manager_resource_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Domain') is not None:
+            self.domain = m.get('Domain')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceManagerResourceGroupId') is not None:
+            self.resource_manager_resource_group_id = m.get('ResourceManagerResourceGroupId')
+        return self
+
+
+class ModifyDomainPunishStatusResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        # The ID of the request.
+        self.request_id = request_id
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
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ModifyDomainPunishStatusResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ModifyDomainPunishStatusResponseBody = None,
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
+            temp_model = ModifyDomainPunishStatusResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ModifyHybridCloudClusterBypassStatusRequest(TeaModel):
     def __init__(
         self,
         cluster_resource_id: str = None,
         instance_id: str = None,
         rule_status: str = None,
     ):
@@ -15235,19 +17747,30 @@
         description: str = None,
         instance_id: str = None,
         member_account_id: str = None,
         region_id: str = None,
         resource_manager_resource_group_id: str = None,
         source_ip: str = None,
     ):
+        # The description of the member. The description must be 1 to 256 characters in length, and can contain letters, digits, periods (.), underscores (\_), hyphens (-), and asterisks (\*).
         self.description = description
+        # The ID of the WAF instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
         self.instance_id = instance_id
+        # The Alibaba Cloud account ID of the managed member.
         self.member_account_id = member_account_id
+        # The region in which the Web Application Firewall (WAF) instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
         self.region_id = region_id
+        # The ID of the Alibaba Cloud resource group.
         self.resource_manager_resource_group_id = resource_manager_resource_group_id
+        # The source IP address of the request. The system automatically obtains the value of this parameter.
         self.source_ip = source_ip
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15287,14 +17810,15 @@
 
 
 class ModifyMemberAccountResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15760,7 +18284,302 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SyncProductInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class TagResourcesRequestTag(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        # The key of tag N to add to the resource. Valid values of N: 1 to 20.
+        self.key = key
+        # The value of tag N to add to the resource. Valid values of N: 1 to 20.
+        self.value = value
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
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class TagResourcesRequest(TeaModel):
+    def __init__(
+        self,
+        region_id: str = None,
+        resource_id: List[str] = None,
+        resource_type: str = None,
+        tag: List[TagResourcesRequestTag] = None,
+    ):
+        # The region in which the Web Application Firewall (WAF) instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id
+        # The IDs of the resources. You can specify up to 50 resource IDs.
+        self.resource_id = resource_id
+        # The type of the resource. Set the value to ALIYUN::WAF::DEFENSERESOURCE.
+        self.resource_type = resource_type
+        # The tags to add to the resource.
+        self.tag = tag
+
+    def validate(self):
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_id is not None:
+            result['ResourceId'] = self.resource_id
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceId') is not None:
+            self.resource_id = m.get('ResourceId')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = TagResourcesRequestTag()
+                self.tag.append(temp_model.from_map(k))
+        return self
+
+
+class TagResourcesResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        # The request ID.
+        self.request_id = request_id
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
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class TagResourcesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: TagResourcesResponseBody = None,
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
+            temp_model = TagResourcesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class UntagResourcesRequest(TeaModel):
+    def __init__(
+        self,
+        all: bool = None,
+        region_id: str = None,
+        resource_id: List[str] = None,
+        resource_type: str = None,
+        tag_key: List[str] = None,
+    ):
+        # Specifies whether to remove all tags from the specified resource groups or members. Valid values:
+        # 
+        # *   false (default)
+        # *   true
+        self.all = all
+        # The region in which the Web Application Firewall (WAF) instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id
+        # The resource IDs. You can specify up to 50 resource IDs.
+        self.resource_id = resource_id
+        # The type of the resource. Set the value to ALIYUN::WAF::DEFENSERESOURCE.
+        self.resource_type = resource_type
+        # The tag keys. You can specify up to 20 tag keys.
+        self.tag_key = tag_key
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
+        if self.all is not None:
+            result['All'] = self.all
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_id is not None:
+            result['ResourceId'] = self.resource_id
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        if self.tag_key is not None:
+            result['TagKey'] = self.tag_key
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('All') is not None:
+            self.all = m.get('All')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceId') is not None:
+            self.resource_id = m.get('ResourceId')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        if m.get('TagKey') is not None:
+            self.tag_key = m.get('TagKey')
+        return self
+
+
+class UntagResourcesResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        # The request ID.
+        self.request_id = request_id
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
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UntagResourcesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UntagResourcesResponseBody = None,
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
+            temp_model = UntagResourcesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001.egg-info/PKG-INFO` & `alibabacloud_waf-openapi20211001-3.4.0/alibabacloud_waf_openapi20211001.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-waf-openapi20211001
-Version: 3.3.0
+Version: 3.4.0
 Summary: Alibaba Cloud waf-openapi (20211001) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_waf-openapi20211001-3.3.0/setup.py` & `alibabacloud_waf-openapi20211001-3.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_waf-openapi20211001.
 
-Created on 07/04/2024
+Created on 24/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_waf_openapi20211001"
 NAME = "alibabacloud_waf-openapi20211001" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud waf-openapi (20211001) SDK Library for Python"
```

