# Comparing `tmp/alibabacloud_waf-openapi20211001_py2-3.3.0.tar.gz` & `tmp/alibabacloud_waf-openapi20211001_py2-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_waf-openapi20211001_py2-3.3.0.tar", last modified: Sun Apr  7 03:49:23 2024, max compression
+gzip compressed data, was "dist/alibabacloud_waf-openapi20211001_py2-3.4.0.tar", last modified: Wed Apr 24 17:13:42 2024, max compression
```

## Comparing `alibabacloud_waf-openapi20211001_py2-3.3.0.tar` & `alibabacloud_waf-openapi20211001_py2-3.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/
--rw-r--r--   0 root         (0) root         (0)     1629 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2520 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1057 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1140 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001/__init__.py
--rw-r--r--   0 root         (0) root         (0)   122943 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001/client.py
--rw-r--r--   0 root         (0) root         (0)   590442 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2520 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      504 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2945 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 17:13:42.000000 alibabacloud_waf-openapi20211001_py2-3.4.0/
+-rw-r--r--   0 root         (0) root         (0)     2002 2024-04-24 17:13:41.000000 alibabacloud_waf-openapi20211001_py2-3.4.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-24 17:13:41.000000 alibabacloud_waf-openapi20211001_py2-3.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-24 17:13:41.000000 alibabacloud_waf-openapi20211001_py2-3.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-04-24 17:13:42.000000 alibabacloud_waf-openapi20211001_py2-3.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1057 2024-04-24 17:13:41.000000 alibabacloud_waf-openapi20211001_py2-3.4.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1140 2024-04-24 17:13:41.000000 alibabacloud_waf-openapi20211001_py2-3.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 17:13:42.000000 alibabacloud_waf-openapi20211001_py2-3.4.0/alibabacloud_waf_openapi20211001/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-24 17:13:41.000000 alibabacloud_waf-openapi20211001_py2-3.4.0/alibabacloud_waf_openapi20211001/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   146348 2024-04-24 17:13:41.000000 alibabacloud_waf-openapi20211001_py2-3.4.0/alibabacloud_waf_openapi20211001/client.py
+-rw-r--r--   0 root         (0) root         (0)   689082 2024-04-24 17:13:41.000000 alibabacloud_waf-openapi20211001_py2-3.4.0/alibabacloud_waf_openapi20211001/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 17:13:42.000000 alibabacloud_waf-openapi20211001_py2-3.4.0/alibabacloud_waf_openapi20211001_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-04-24 17:13:42.000000 alibabacloud_waf-openapi20211001_py2-3.4.0/alibabacloud_waf_openapi20211001_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      504 2024-04-24 17:13:42.000000 alibabacloud_waf-openapi20211001_py2-3.4.0/alibabacloud_waf_openapi20211001_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 17:13:42.000000 alibabacloud_waf-openapi20211001_py2-3.4.0/alibabacloud_waf_openapi20211001_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-24 17:13:42.000000 alibabacloud_waf-openapi20211001_py2-3.4.0/alibabacloud_waf_openapi20211001_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-24 17:13:42.000000 alibabacloud_waf-openapi20211001_py2-3.4.0/alibabacloud_waf_openapi20211001_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-24 17:13:42.000000 alibabacloud_waf-openapi20211001_py2-3.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2945 2024-04-24 17:13:41.000000 alibabacloud_waf-openapi20211001_py2-3.4.0/setup.py
```

### Comparing `alibabacloud_waf-openapi20211001_py2-3.3.0/ChangeLog.md` & `alibabacloud_waf-openapi20211001_py2-3.4.0/ChangeLog.md`

 * *Files 20% similar despite different names*

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

### Comparing `alibabacloud_waf-openapi20211001_py2-3.3.0/LICENSE` & `alibabacloud_waf-openapi20211001_py2-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_waf-openapi20211001_py2-3.3.0/PKG-INFO` & `alibabacloud_waf-openapi20211001_py2-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_waf-openapi20211001_py2
-Version: 3.3.0
+Version: 3.4.0
 Summary: Alibaba Cloud waf-openapi (20211001) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_waf-openapi20211001_py2-3.3.0/README-CN.md` & `alibabacloud_waf-openapi20211001_py2-3.4.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_waf-openapi20211001_py2-3.3.0/README.md` & `alibabacloud_waf-openapi20211001_py2-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001/client.py` & `alibabacloud_waf-openapi20211001_py2-3.4.0/alibabacloud_waf_openapi20211001/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,14 +88,48 @@
             self.call_api(params, req, runtime)
         )
 
     def clear_major_protection_black_ip(self, request):
         runtime = util_models.RuntimeOptions()
         return self.clear_major_protection_black_ip_with_options(request, runtime)
 
+    def copy_defense_template_with_options(self, request, runtime):
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
+    def copy_defense_template(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.copy_defense_template_with_options(request, runtime)
+
     def create_defense_resource_group_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.add_list):
             query['AddList'] = request.add_list
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
@@ -350,14 +384,44 @@
             self.call_api(params, req, runtime)
         )
 
     def create_member_accounts(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_member_accounts_with_options(request, runtime)
 
+    def create_postpaid_instance_with_options(self, request, runtime):
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
+    def create_postpaid_instance(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.create_postpaid_instance_with_options(request, runtime)
+
     def delete_defense_resource_group_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.group_name):
             query['GroupName'] = request.group_name
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
@@ -596,14 +660,48 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_account_delegated_status(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_account_delegated_status_with_options(request, runtime)
 
+    def describe_cert_detail_with_options(self, request, runtime):
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
+    def describe_cert_detail(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_cert_detail_with_options(request, runtime)
+
     def describe_certs_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.algorithm):
             query['Algorithm'] = request.algorithm
         if not UtilClient.is_unset(request.domain):
             query['Domain'] = request.domain
@@ -688,14 +786,48 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_cloud_resources(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_cloud_resources_with_options(request, runtime)
 
+    def describe_defense_resource_with_options(self, request, runtime):
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
+    def describe_defense_resource(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_defense_resource_with_options(request, runtime)
+
     def describe_defense_resource_group_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.group_name):
             query['GroupName'] = request.group_name
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
@@ -722,14 +854,130 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_defense_resource_group(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_defense_resource_group_with_options(request, runtime)
 
+    def describe_defense_resource_group_names_with_options(self, request, runtime):
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
+    def describe_defense_resource_group_names(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_defense_resource_group_names_with_options(request, runtime)
+
+    def describe_defense_resource_groups_with_options(self, request, runtime):
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
+    def describe_defense_resource_groups(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_defense_resource_groups_with_options(request, runtime)
+
+    def describe_defense_resource_names_with_options(self, request, runtime):
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
+    def describe_defense_resource_names(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_defense_resource_names_with_options(request, runtime)
+
     def describe_defense_resource_templates_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
@@ -912,14 +1160,56 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_defense_template(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_defense_template_with_options(request, runtime)
 
+    def describe_defense_template_valid_groups_with_options(self, request, runtime):
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
+    def describe_defense_template_valid_groups(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_defense_template_valid_groups_with_options(request, runtime)
+
     def describe_defense_templates_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.defense_scene):
             query['DefenseScene'] = request.defense_scene
         if not UtilClient.is_unset(request.defense_sub_scene):
             query['DefenseSubScene'] = request.defense_sub_scene
@@ -1498,14 +1788,48 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_product_instances(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_product_instances_with_options(request, runtime)
 
+    def describe_punished_domains_with_options(self, request, runtime):
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
+    def describe_punished_domains(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_punished_domains_with_options(request, runtime)
+
     def describe_resource_instance_certs_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
@@ -2080,14 +2404,48 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_sls_log_store_status(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_sls_log_store_status_with_options(request, runtime)
 
+    def describe_template_resource_count_with_options(self, request, runtime):
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
+    def describe_template_resource_count(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_template_resource_count_with_options(request, runtime)
+
     def describe_template_resources_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
@@ -2286,14 +2644,118 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_waf_source_ip_segment(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_waf_source_ip_segment_with_options(request, runtime)
 
+    def list_tag_keys_with_options(self, request, runtime):
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
+    def list_tag_keys(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_tag_keys_with_options(request, runtime)
+
+    def list_tag_resources_with_options(self, request, runtime):
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
+    def list_tag_resources(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_tag_resources_with_options(request, runtime)
+
+    def list_tag_values_with_options(self, request, runtime):
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
+    def list_tag_values(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_tag_values_with_options(request, runtime)
+
     def modify_defense_resource_group_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.add_list):
             query['AddList'] = request.add_list
         if not UtilClient.is_unset(request.delete_list):
             query['DeleteList'] = request.delete_list
@@ -2600,14 +3062,48 @@
             self.call_api(params, req, runtime)
         )
 
     def modify_domain(self, request):
         runtime = util_models.RuntimeOptions()
         return self.modify_domain_with_options(request, runtime)
 
+    def modify_domain_punish_status_with_options(self, request, runtime):
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
+    def modify_domain_punish_status(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.modify_domain_punish_status_with_options(request, runtime)
+
     def modify_hybrid_cloud_cluster_bypass_status_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cluster_resource_id):
             query['ClusterResourceId'] = request.cluster_resource_id
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
@@ -2839,7 +3335,77 @@
 
         @param request: SyncProductInstanceRequest
 
         @return: SyncProductInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.sync_product_instance_with_options(request, runtime)
+
+    def tag_resources_with_options(self, request, runtime):
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
+    def tag_resources(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.tag_resources_with_options(request, runtime)
+
+    def untag_resources_with_options(self, request, runtime):
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
+    def untag_resources(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.untag_resources_with_options(request, runtime)
```

### Comparing `alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001/models.py` & `alibabacloud_waf-openapi20211001_py2-3.4.0/alibabacloud_waf_openapi20211001/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -115,14 +115,129 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ClearMajorProtectionBlackIpResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CopyDefenseTemplateRequest(TeaModel):
+    def __init__(self, instance_id=None, region_id=None, resource_manager_resource_group_id=None, template_id=None):
+        # The ID of the Web Application Firewall (WAF) instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id  # type: str
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id  # type: str
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id  # type: str
+        # The ID of the protection template that you want to copy.
+        self.template_id = template_id  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CopyDefenseTemplateRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None, template_id=None):
+        # The request ID.
+        self.request_id = request_id  # type: str
+        # The ID of the new protection template.
+        self.template_id = template_id  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CopyDefenseTemplateResponseBody, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        return self
+
+
+class CopyDefenseTemplateResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: CopyDefenseTemplateResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(CopyDefenseTemplateResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, add_list=None, description=None, group_name=None, instance_id=None, region_id=None,
                  resource_manager_resource_group_id=None):
         # The protected objects that you want to add to the protected object group. You can add multiple protected objects to a protected object group at the same time. You can specify multiple protected objects. Separate them with commas (,).
         self.add_list = add_list  # type: str
         # The description of the protected object group.
         self.description = description  # type: str
@@ -1254,18 +1369,28 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateMemberAccountsRequest(TeaModel):
     def __init__(self, instance_id=None, member_account_ids=None, region_id=None,
                  resource_manager_resource_group_id=None, source_ip=None):
+        # The ID of the WAF instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
         self.instance_id = instance_id  # type: str
+        # The Alibaba Cloud account IDs of the members that you want to add. You can add up to 10 members at the same time.
         self.member_account_ids = member_account_ids  # type: list[str]
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
         self.region_id = region_id  # type: str
+        # The ID of the Alibaba Cloud resource group.
         self.resource_manager_resource_group_id = resource_manager_resource_group_id  # type: str
+        # The source IP address of the request. The system automatically obtains the value of this parameter.
         self.source_ip = source_ip  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateMemberAccountsRequest, self).to_map()
@@ -1298,14 +1423,15 @@
         if m.get('SourceIp') is not None:
             self.source_ip = m.get('SourceIp')
         return self
 
 
 class CreateMemberAccountsResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateMemberAccountsResponseBody, self).to_map()
@@ -1356,14 +1482,115 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateMemberAccountsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreatePostpaidInstanceRequest(TeaModel):
+    def __init__(self, region_id=None, resource_manager_resource_group_id=None):
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id  # type: str
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreatePostpaidInstanceRequest, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceManagerResourceGroupId') is not None:
+            self.resource_manager_resource_group_id = m.get('ResourceManagerResourceGroupId')
+        return self
+
+
+class CreatePostpaidInstanceResponseBody(TeaModel):
+    def __init__(self, instance_id=None, request_id=None):
+        # The ID of the WAF instance.
+        self.instance_id = instance_id  # type: str
+        # The ID of the request.
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreatePostpaidInstanceResponseBody, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CreatePostpaidInstanceResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: CreatePostpaidInstanceResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(CreatePostpaidInstanceResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, group_name=None, instance_id=None, region_id=None, resource_manager_resource_group_id=None):
         # The name of the protected object group that you want to delete.
         self.group_name = group_name  # type: str
         # The ID of the Web Application Firewall (WAF) instance.
         # 
         # >  You can call the [DescribeInstance](~~433756~~) operation to obtain the ID of the WAF instance.
@@ -1933,18 +2160,28 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteMemberAccountRequest(TeaModel):
     def __init__(self, instance_id=None, member_account_id=None, region_id=None,
                  resource_manager_resource_group_id=None, source_ip=None):
+        # The ID of the WAF instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
         self.instance_id = instance_id  # type: str
+        # The Alibaba Cloud account ID of the managed member.
         self.member_account_id = member_account_id  # type: str
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
         self.region_id = region_id  # type: str
+        # The ID of the Alibaba Cloud resource group.
         self.resource_manager_resource_group_id = resource_manager_resource_group_id  # type: str
+        # The source IP address of the request. The system automatically obtains the value of this parameter.
         self.source_ip = source_ip  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteMemberAccountRequest, self).to_map()
@@ -1977,14 +2214,15 @@
         if m.get('SourceIp') is not None:
             self.source_ip = m.get('SourceIp')
         return self
 
 
 class DeleteMemberAccountResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteMemberAccountResponseBody, self).to_map()
@@ -2037,16 +2275,24 @@
             temp_model = DeleteMemberAccountResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAccountDelegatedStatusRequest(TeaModel):
     def __init__(self, instance_id=None, region_id=None, resource_manager_resource_group_id=None):
+        # The ID of the WAF instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
         self.instance_id = instance_id  # type: str
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
         self.region_id = region_id  # type: str
+        # The ID of the Alibaba Cloud resource group.
         self.resource_manager_resource_group_id = resource_manager_resource_group_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeAccountDelegatedStatusRequest, self).to_map()
@@ -2071,17 +2317,24 @@
         if m.get('ResourceManagerResourceGroupId') is not None:
             self.resource_manager_resource_group_id = m.get('ResourceManagerResourceGroupId')
         return self
 
 
 class DescribeAccountDelegatedStatusResponseBody(TeaModel):
     def __init__(self, account_id=None, account_name=None, delegated_status=None, request_id=None):
+        # The ID of the Alibaba Cloud account.
         self.account_id = account_id  # type: str
+        # The name of the Alibaba Cloud account. This parameter is returned only if the account is the delegated administrator account.
         self.account_name = account_name  # type: str
+        # Indicates whether the Alibaba Cloud account is the delegated administrator account of the WAF instance.
+        # 
+        # *   **true**\
+        # *   **false**\
         self.delegated_status = delegated_status  # type: bool
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeAccountDelegatedStatusResponseBody, self).to_map()
@@ -2144,14 +2397,194 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeAccountDelegatedStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeCertDetailRequest(TeaModel):
+    def __init__(self, cert_identifier=None, instance_id=None, region_id=None,
+                 resource_manager_resource_group_id=None):
+        # The ID of the certificate.
+        self.cert_identifier = cert_identifier  # type: str
+        # The ID of the WAF instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id  # type: str
+        # The region in which the Web Application Firewall (WAF) instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id  # type: str
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeCertDetailRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, after_date=None, before_date=None, cert_identifier=None, cert_name=None, common_name=None,
+                 domain=None, sans=None):
+        # The time when the certificate expires. This value is a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
+        self.after_date = after_date  # type: long
+        # The time when the certificate was issued. This value is a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
+        self.before_date = before_date  # type: long
+        # The ID of the certificate.
+        self.cert_identifier = cert_identifier  # type: str
+        # The name of the certificate.
+        self.cert_name = cert_name  # type: str
+        # The primary domain name, which is a common name.
+        self.common_name = common_name  # type: str
+        # The domain name that is associated with the certificate.
+        self.domain = domain  # type: str
+        # The other domain names that are associated with the certificate.
+        self.sans = sans  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeCertDetailResponseBodyCertDetail, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, cert_detail=None, request_id=None):
+        # The details of the certificate.
+        self.cert_detail = cert_detail  # type: DescribeCertDetailResponseBodyCertDetail
+        # The ID of the request.
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.cert_detail:
+            self.cert_detail.validate()
+
+    def to_map(self):
+        _map = super(DescribeCertDetailResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeCertDetailResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeCertDetailResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, algorithm=None, domain=None, instance_id=None, page_number=None, page_size=None,
                  region_id=None, resource_manager_resource_group_id=None):
         # The type of the encryption algorithm. Valid values:
         # 
         # *   **NotSM2**: The encryption algorithm is not the SM2 algorithm. This is the default value.
         # *   **SM2**: The encryption algorithm is the SM2 algorithm.
@@ -2634,14 +3067,266 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeCloudResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeDefenseResourceRequest(TeaModel):
+    def __init__(self, instance_id=None, region_id=None, resource=None, resource_manager_resource_group_id=None):
+        # The ID of the Web Application Firewall (WAF) instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id  # type: str
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id  # type: str
+        # The name of the protected object that you want to query. Only exact queries are supported.
+        self.resource = resource  # type: str
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDefenseResourceRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, acw_cookie_status=None, acw_secure_status=None, acw_v3secure_status=None,
+                 custom_headers=None, description=None, detail=None, gmt_create=None, gmt_modified=None, owner_user_id=None,
+                 pattern=None, product=None, resource=None, resource_group=None, resource_manager_resource_group_id=None,
+                 resource_origin=None, xff_status=None):
+        # The status of the tracking cookie.
+        # 
+        # *   **0**: disabled.
+        # *   **1**: enabled.
+        self.acw_cookie_status = acw_cookie_status  # type: int
+        # The status of the secure attribute of the tracking cookie.
+        # 
+        # *   **0**: disabled.
+        # *   **1**: enabled.
+        self.acw_secure_status = acw_secure_status  # type: int
+        # The status of the secure attribute of the slider CAPTCHA cookie.
+        # 
+        # *   **0**: disabled.
+        # *   **1**: enabled.
+        self.acw_v3secure_status = acw_v3secure_status  # type: int
+        # The custom header fields.
+        # 
+        # >  If the value of XffStatus is 1, the first IP address in the specified header field is used as the originating IP address of the client to prevent X-Forwarded-For (XFF) forgery. If you specify multiple header fields, WAF reads the values of the header fields in sequence until the originating IP address is obtained. If the originating IP address cannot be obtained, the first IP address in the XFF header field is used as the originating IP address of the client.
+        self.custom_headers = custom_headers  # type: list[str]
+        # The description of the protected object.
+        self.description = description  # type: str
+        # The details of the protected object. Different key-value pairs indicate different attributes of the protected object.
+        self.detail = detail  # type: dict[str, any]
+        # The time when the protected object was created. Unit: milliseconds.
+        self.gmt_create = gmt_create  # type: long
+        # The time when the protected object was modified. Unit: milliseconds.
+        self.gmt_modified = gmt_modified  # type: long
+        # The user ID (UID) of the Alibaba Cloud account to which the protected object belongs.
+        self.owner_user_id = owner_user_id  # type: str
+        # The pattern used for the protected object.
+        self.pattern = pattern  # type: str
+        # The name of the cloud service.
+        self.product = product  # type: str
+        # The name of the protected object.
+        self.resource = resource  # type: str
+        # The name of the protected object group to which the protected object belongs.
+        self.resource_group = resource_group  # type: str
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id  # type: str
+        # The origin of the protected object. Valid values:
+        # 
+        # *   **custom**\
+        # *   **access**\
+        self.resource_origin = resource_origin  # type: str
+        # Indicates whether a Layer 7 proxy is deployed in front of WAF, such as Anti-DDoS Proxy and Alibaba Cloud CDN. Valid values:
+        # 
+        # *   **0**: No Layer 7 proxy is deployed.
+        # *   **1**: A Layer 7 proxy is deployed.
+        self.xff_status = xff_status  # type: int
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDefenseResourceResponseBodyResource, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None, resource=None):
+        # The request ID.
+        self.request_id = request_id  # type: str
+        # The information about the protected object.
+        self.resource = resource  # type: DescribeDefenseResourceResponseBodyResource
+
+    def validate(self):
+        if self.resource:
+            self.resource.validate()
+
+    def to_map(self):
+        _map = super(DescribeDefenseResourceResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeDefenseResourceResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeDefenseResourceResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, group_name=None, instance_id=None, region_id=None, resource_manager_resource_group_id=None):
         # The name of the protected object group whose information you want to query.
         self.group_name = group_name  # type: str
         # The ID of the Web Application Firewall (WAF) instance.
         # 
         # >  You can call the [DescribeInstance](~~433756~~) operation to obtain the ID of the WAF instance.
@@ -2800,14 +3485,479 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeDefenseResourceGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeDefenseResourceGroupNamesRequest(TeaModel):
+    def __init__(self, group_name_like=None, instance_id=None, page_number=None, page_size=None, region_id=None,
+                 resource_manager_resource_group_id=None):
+        # The name of the protected object group. Fuzzy queries are supported.
+        self.group_name_like = group_name_like  # type: str
+        # The ID of the Web Application Firewall (WAF) instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id  # type: str
+        # The page number. Default value: **1**.
+        self.page_number = page_number  # type: int
+        # The number of entries per page. Default value: **20**.
+        self.page_size = page_size  # type: int
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id  # type: str
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDefenseResourceGroupNamesRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, group_names=None, request_id=None, total_count=None):
+        # The names of the protected object groups.
+        self.group_names = group_names  # type: list[str]
+        # The request ID.
+        self.request_id = request_id  # type: str
+        # The total number of entries returned.
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDefenseResourceGroupNamesResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeDefenseResourceGroupNamesResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeDefenseResourceGroupNamesResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, group_name_like=None, group_names=None, instance_id=None, page_number=None, page_size=None,
+                 region_id=None, resource_manager_resource_group_id=None):
+        # The name of the protected object group that you want to query. Fuzzy queries are supported.
+        self.group_name_like = group_name_like  # type: str
+        # The names of the protected object groups that you want to query. Separate multiple names with commas (,).
+        self.group_names = group_names  # type: str
+        # The ID of the Web Application Firewall (WAF) instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id  # type: str
+        # The page number. Default value: **1**.
+        self.page_number = page_number  # type: int
+        # The number of entries per page. Default value: **20**.
+        self.page_size = page_size  # type: int
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id  # type: str
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDefenseResourceGroupsRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, description=None, gmt_create=None, gmt_modified=None, group_name=None, resource_list=None):
+        # The description of the protected object group.
+        self.description = description  # type: str
+        # The time when the protected object group was created. Unit: milliseconds.
+        self.gmt_create = gmt_create  # type: long
+        # The most recent time when the protected object group was modified. Unit: milliseconds.
+        self.gmt_modified = gmt_modified  # type: long
+        # The name of the protected object group.
+        self.group_name = group_name  # type: str
+        # The names of the protected objects that are added to the protected object group. Separate multiple protected objects with commas (,).
+        self.resource_list = resource_list  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDefenseResourceGroupsResponseBodyGroups, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, groups=None, request_id=None, total_count=None):
+        # The list of protected object groups.
+        self.groups = groups  # type: list[DescribeDefenseResourceGroupsResponseBodyGroups]
+        # The request ID.
+        self.request_id = request_id  # type: str
+        # The total number of entries returned.
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        if self.groups:
+            for k in self.groups:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeDefenseResourceGroupsResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeDefenseResourceGroupsResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeDefenseResourceGroupsResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, instance_id=None, page_number=None, page_size=None, region_id=None, resource=None,
+                 resource_manager_resource_group_id=None):
+        # The ID of the Web Application Firewall (WAF) instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id  # type: str
+        # The page number. Default value: **1**.
+        self.page_number = page_number  # type: int
+        # The number of entries per page. Default value: **20**.
+        self.page_size = page_size  # type: int
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id  # type: str
+        # The name of the protected object that you want to query.
+        self.resource = resource  # type: str
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDefenseResourceNamesRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None, resources=None, total_count=None):
+        # The ID of the request.
+        self.request_id = request_id  # type: str
+        # The names of the protected objects.
+        self.resources = resources  # type: list[str]
+        # The total number of entries returned.
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDefenseResourceNamesResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeDefenseResourceNamesResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeDefenseResourceNamesResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, instance_id=None, region_id=None, resource=None, resource_manager_resource_group_id=None,
                  resource_type=None, rule_id=None, rule_type=None):
         # The ID of the Web Application Firewall (WAF) instance.
         # 
         # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
         self.instance_id = instance_id  # type: str
@@ -3166,15 +4316,15 @@
         # *   **1:** enabled.
         self.acw_cookie_status = acw_cookie_status  # type: int
         # The status of the secure attribute in the tracking cookie.
         # 
         # *   **0:** disabled.
         # *   **1:** enabled.
         self.acw_secure_status = acw_secure_status  # type: int
-        # The status of the slider CAPTCHA cookie.
+        # The status of the secure attribute in the slider CAPTCHA cookie.
         # 
         # *   **0:** disabled.
         # *   **1:** enabled.
         self.acw_v3secure_status = acw_v3secure_status  # type: int
         # The custom XFF headers that are used to identify the originating IP addresses of clients. If the value of XffStatus is 1 and CustomHeaders is left empty, the first IP addresses in the XFF headers are used as the originating IP addresses of clients.
         self.custom_headers = custom_headers  # type: list[str]
         # The description of the protected object.
@@ -3195,15 +4345,15 @@
         self.resource = resource  # type: str
         # The name of the protected object group to which the protected object belongs.
         self.resource_group = resource_group  # type: str
         # The ID of the Alibaba Cloud resource group.
         self.resource_manager_resource_group_id = resource_manager_resource_group_id  # type: str
         # The origin of the protected object.
         self.resource_origin = resource_origin  # type: str
-        # Indicates whether the X-Forwarded-For (XFF) proxy feature is enabled for the protected object.
+        # Indicates whether the X-Forwarded-For (XFF) proxy is enabled.
         self.xff_status = xff_status  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDefenseResourcesResponseBodyResources, self).to_map()
@@ -3985,14 +5135,171 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeDefenseTemplateResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeDefenseTemplateValidGroupsRequest(TeaModel):
+    def __init__(self, defense_scene=None, group_name=None, instance_id=None, page_number=None, page_size=None,
+                 region_id=None, resource_manager_resource_group_id=None, template_id=None):
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
+        self.defense_scene = defense_scene  # type: str
+        # The name of the protected object group that you want to query.
+        self.group_name = group_name  # type: str
+        # The ID of the Web Application Firewall (WAF) instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id  # type: str
+        # The page number. Default value: **1**.
+        self.page_number = page_number  # type: int
+        # The number of entries per page. Default value: **20**.
+        self.page_size = page_size  # type: int
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id  # type: str
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id  # type: str
+        # The ID of the protection template.
+        self.template_id = template_id  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDefenseTemplateValidGroupsRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, groups=None, request_id=None, total_count=None):
+        # The names of the protected object groups.
+        self.groups = groups  # type: list[str]
+        # The ID of the request.
+        self.request_id = request_id  # type: str
+        # The total number of entries returned.
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDefenseTemplateValidGroupsResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeDefenseTemplateValidGroupsResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeDefenseTemplateValidGroupsResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, defense_scene=None, defense_sub_scene=None, instance_id=None, page_number=None,
                  page_size=None, region_id=None, resource=None, resource_manager_resource_group_id=None, resource_type=None,
                  template_id=None, template_type=None):
         # The scenario in which the protection template is used.
         # 
         # *   **waf_group**: basic protection.
@@ -7809,18 +9116,32 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeMemberAccountsRequest(TeaModel):
     def __init__(self, account_status=None, instance_id=None, region_id=None,
                  resource_manager_resource_group_id=None, source_ip=None):
+        # The status of the member that you want to query.
+        # 
+        # *   **enabled**: managed.
+        # *   **disabled**: not managed.
+        # *   **disabling**: being deleted.
         self.account_status = account_status  # type: str
+        # The ID of the Web Application Firewall (WAF) instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
         self.instance_id = instance_id  # type: str
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
         self.region_id = region_id  # type: str
+        # The ID of the Alibaba Cloud resource group.
         self.resource_manager_resource_group_id = resource_manager_resource_group_id  # type: str
+        # The source IP address of the request. The system specifies this parameter.
         self.source_ip = source_ip  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeMemberAccountsRequest, self).to_map()
@@ -7853,18 +9174,27 @@
         if m.get('SourceIp') is not None:
             self.source_ip = m.get('SourceIp')
         return self
 
 
 class DescribeMemberAccountsResponseBodyAccountInfos(TeaModel):
     def __init__(self, account_id=None, account_name=None, account_status=None, description=None, gmt_create=None):
+        # The ID of the member.
         self.account_id = account_id  # type: str
+        # The name of the member.
         self.account_name = account_name  # type: str
+        # The status of the member.
+        # 
+        # *   **enabled**: managed.
+        # *   **disabled**: not managed.
+        # *   **disabling**: being deleted.
         self.account_status = account_status  # type: str
+        # The description of the member.
         self.description = description  # type: str
+        # The time when the member was added.
         self.gmt_create = gmt_create  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeMemberAccountsResponseBodyAccountInfos, self).to_map()
@@ -7897,15 +9227,17 @@
         if m.get('GmtCreate') is not None:
             self.gmt_create = m.get('GmtCreate')
         return self
 
 
 class DescribeMemberAccountsResponseBody(TeaModel):
     def __init__(self, account_infos=None, request_id=None):
+        # The information about the member.
         self.account_infos = account_infos  # type: list[DescribeMemberAccountsResponseBodyAccountInfos]
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.account_infos:
             for k in self.account_infos:
                 if k:
                     k.validate()
@@ -8173,14 +9505,15 @@
     def __init__(self, instance_id=None, owner_user_id=None, page_number=None, page_size=None, region_id=None,
                  resource_instance_id=None, resource_ip=None, resource_manager_resource_group_id=None, resource_name=None,
                  resource_product=None, resource_region_id=None):
         # The ID of the WAF instance.
         # 
         # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
         self.instance_id = instance_id  # type: str
+        # The ID of the Alibaba Cloud account to which the resource belongs.
         self.owner_user_id = owner_user_id  # type: str
         # The page number. Default value: **1**.
         self.page_number = page_number  # type: long
         # The number of entries per page. Default value: **10**.
         self.page_size = page_size  # type: long
         # The region in which the WAF instance is deployed. Valid values:
         # 
@@ -8516,22 +9849,148 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeProductInstancesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribePunishedDomainsRequest(TeaModel):
+    def __init__(self, domains=None, instance_id=None, region_id=None, resource_manager_resource_group_id=None):
+        # The domain names.
+        self.domains = domains  # type: list[str]
+        # The ID of the WAF instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id  # type: str
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id  # type: str
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribePunishedDomainsRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, punished_domains=None, request_id=None):
+        # The domain names that are penalized for failing to obtain an ICP filing.
+        self.punished_domains = punished_domains  # type: list[str]
+        # The request ID.
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribePunishedDomainsResponseBody, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('PunishedDomains') is not None:
+            self.punished_domains = m.get('PunishedDomains')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribePunishedDomainsResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribePunishedDomainsResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribePunishedDomainsResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, instance_id=None, page_number=None, page_size=None, region_id=None,
                  resource_instance_id=None, resource_manager_resource_group_id=None):
+        # The ID of the WAF instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
         self.instance_id = instance_id  # type: str
+        # The page number. Default value: **1**.
         self.page_number = page_number  # type: long
+        # The number of entries per page. Default value: **10**.
         self.page_size = page_size  # type: long
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
         self.region_id = region_id  # type: str
+        # The ID of the instance.
         self.resource_instance_id = resource_instance_id  # type: str
+        # The ID of the Alibaba Cloud resource group.
         self.resource_manager_resource_group_id = resource_manager_resource_group_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeResourceInstanceCertsRequest, self).to_map()
@@ -8569,20 +10028,27 @@
             self.resource_manager_resource_group_id = m.get('ResourceManagerResourceGroupId')
         return self
 
 
 class DescribeResourceInstanceCertsResponseBodyCerts(TeaModel):
     def __init__(self, after_date=None, before_date=None, cert_identifier=None, cert_name=None, common_name=None,
                  domain=None, is_chain_completed=None):
+        # The time when the certificate expires.
         self.after_date = after_date  # type: long
+        # The time when the certificate was issued.
         self.before_date = before_date  # type: long
+        # The globally unique ID of the certificate. The value is in the "Certificate ID-cn-hangzhou" format. For example, if the ID of the certificate is 123, the value of CertIdentifier is 123-cn-hangzhou.
         self.cert_identifier = cert_identifier  # type: str
+        # The name of the certificate.
         self.cert_name = cert_name  # type: str
+        # The common name.
         self.common_name = common_name  # type: str
+        # The domain name for which the certificate is issued.
         self.domain = domain  # type: str
+        # Indicates whether the certificate chain is complete.
         self.is_chain_completed = is_chain_completed  # type: bool
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeResourceInstanceCertsResponseBodyCerts, self).to_map()
@@ -8623,16 +10089,19 @@
         if m.get('IsChainCompleted') is not None:
             self.is_chain_completed = m.get('IsChainCompleted')
         return self
 
 
 class DescribeResourceInstanceCertsResponseBody(TeaModel):
     def __init__(self, certs=None, request_id=None, total_count=None):
+        # The certificates.
         self.certs = certs  # type: list[DescribeResourceInstanceCertsResponseBodyCerts]
+        # The request ID.
         self.request_id = request_id  # type: str
+        # The total number of entries returned.
         self.total_count = total_count  # type: long
 
     def validate(self):
         if self.certs:
             for k in self.certs:
                 if k:
                     k.validate()
@@ -9267,19 +10736,22 @@
             self.start_timestamp = m.get('StartTimestamp')
         if m.get('Type') is not None:
             self.type = m.get('Type')
         return self
 
 
 class DescribeResponseCodeTrendGraphResponseBodyResponseCodes(TeaModel):
-    def __init__(self, code_302pv=None, code_405pv=None, code_499pv=None, code_5xx_pv=None, index=None):
+    def __init__(self, code_302pv=None, code_405pv=None, code_444pv=None, code_499pv=None, code_5xx_pv=None,
+                 index=None):
         # The number of 302 error codes that are returned.
         self.code_302pv = code_302pv  # type: long
         # The number of 405 error codes that are returned.
         self.code_405pv = code_405pv  # type: long
+        # The number of 444 error codes that are returned.
+        self.code_444pv = code_444pv  # type: long
         # The number of 499 error codes that are returned.
         self.code_499pv = code_499pv  # type: long
         # The number of 5xx error codes that are returned.
         self.code_5xx_pv = code_5xx_pv  # type: long
         # The serial number of the time interval. The serial numbers are arranged in chronological order.
         self.index = index  # type: long
 
@@ -9292,28 +10764,32 @@
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
 
     def from_map(self, m=None):
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
@@ -11023,14 +12499,175 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeSlsLogStoreStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeTemplateResourceCountRequest(TeaModel):
+    def __init__(self, instance_id=None, region_id=None, resource_manager_resource_group_id=None,
+                 template_ids=None):
+        # The ID of the Web Application Firewall (WAF) instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id  # type: str
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id  # type: str
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id  # type: str
+        # The IDs of the protection templates that you want to query. Separate multiple template IDs with commas (,).
+        self.template_ids = template_ids  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeTemplateResourceCountRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, group_count=None, single_count=None, template_id=None):
+        # The number of protected object groups.
+        self.group_count = group_count  # type: int
+        # The number of protected objects.
+        self.single_count = single_count  # type: int
+        # The ID of the protection template.
+        self.template_id = template_id  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeTemplateResourceCountResponseBodyResourceCount, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None, resource_count=None):
+        # The request ID.
+        self.request_id = request_id  # type: str
+        # The number of protected objects or protected object groups for which the protection template takes effect.
+        self.resource_count = resource_count  # type: list[DescribeTemplateResourceCountResponseBodyResourceCount]
+
+    def validate(self):
+        if self.resource_count:
+            for k in self.resource_count:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeTemplateResourceCountResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeTemplateResourceCountResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeTemplateResourceCountResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, instance_id=None, region_id=None, resource_manager_resource_group_id=None,
                  resource_type=None, template_id=None):
         # The ID of the Web Application Firewall (WAF) instance.
         # 
         # >  You can call the [DescribeInstance](~~433756~~) operation to obtain the ID of the WAF instance.
         self.instance_id = instance_id  # type: str
@@ -11888,14 +13525,511 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeWafSourceIpSegmentResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListTagKeysRequest(TeaModel):
+    def __init__(self, instance_id=None, next_token=None, region_id=None, resource_type=None):
+        # The ID of the WAF instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id  # type: str
+        # The pagination token that is used in the next request to retrieve a new page of results.
+        self.next_token = next_token  # type: str
+        # The region in which the Web Application Firewall (WAF) instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id  # type: str
+        # The type of the resource. Set the value to ALIYUN::WAF::DEFENSERESOURCE.
+        self.resource_type = resource_type  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListTagKeysRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, category=None, key=None):
+        # The type of the tag. Valid values:
+        # 
+        # *   custom
+        # *   system
+        self.category = category  # type: str
+        # The key of the tag.
+        self.key = key  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListTagKeysResponseBodyKeys, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Category') is not None:
+            self.category = m.get('Category')
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        return self
+
+
+class ListTagKeysResponseBody(TeaModel):
+    def __init__(self, keys=None, next_token=None, request_id=None):
+        # The keys and types of the tags.
+        self.keys = keys  # type: list[ListTagKeysResponseBodyKeys]
+        # A pagination token. It can be used in the next request to retrieve a new page of results. If NextToken is empty, no next page exists.
+        self.next_token = next_token  # type: str
+        # The request ID.
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.keys:
+            for k in self.keys:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListTagKeysResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListTagKeysResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListTagKeysResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, key=None, value=None):
+        # The key of tag N that is added to the resource. Valid values of N: 1 to 20.
+        self.key = key  # type: str
+        # The value of tag N that is added to the resource. Valid values of N: 1 to 20.
+        self.value = value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListTagResourcesRequestTag, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class ListTagResourcesRequest(TeaModel):
+    def __init__(self, next_token=None, region_id=None, resource_id=None, resource_type=None, tag=None):
+        # The pagination token that is used in the next request to retrieve a new page of results.
+        self.next_token = next_token  # type: str
+        # The region in which the Web Application Firewall (WAF) instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id  # type: str
+        # The resource IDs. You can specify up to 50 resource IDs.
+        self.resource_id = resource_id  # type: list[str]
+        # The type of the resource. Set the value to ALIYUN::WAF::DEFENSERESOURCE.
+        self.resource_type = resource_type  # type: str
+        # The tags that are added to the resource.
+        self.tag = tag  # type: list[ListTagResourcesRequestTag]
+
+    def validate(self):
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListTagResourcesRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, resource_id=None, resource_type=None, tag_key=None, tag_value=None):
+        # The resource ID.
+        self.resource_id = resource_id  # type: str
+        # The type of the resource. ALIYUN::WAF::DEFENSERESOURCE is returned.
+        self.resource_type = resource_type  # type: str
+        # The key of tag N that is added to the resource.
+        self.tag_key = tag_key  # type: str
+        # The value of tag N that is added to the resource.
+        self.tag_value = tag_value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListTagResourcesResponseBodyTagResources, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, next_token=None, request_id=None, tag_resources=None):
+        # A pagination token. It can be used in the next request to retrieve a new page of results. If NextToken is empty, no next page exists.
+        self.next_token = next_token  # type: str
+        # The request ID.
+        self.request_id = request_id  # type: str
+        # The list of resources.
+        self.tag_resources = tag_resources  # type: list[ListTagResourcesResponseBodyTagResources]
+
+    def validate(self):
+        if self.tag_resources:
+            for k in self.tag_resources:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListTagResourcesResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListTagResourcesResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListTagResourcesResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, key=None, next_token=None, region_id=None, resource_type=None):
+        # The tag key.
+        self.key = key  # type: str
+        # The pagination token that is used in the next request to retrieve a new page of results.
+        self.next_token = next_token  # type: str
+        # The region in which the Web Application Firewall (WAF) instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id  # type: str
+        # The type of the resource. Set the value to ALIYUN::WAF::DEFENSERESOURCE.
+        self.resource_type = resource_type  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListTagValuesRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, next_token=None, request_id=None, values=None):
+        # A pagination token. It can be used in the next request to retrieve a new page of results. If NextToken is empty, no next page exists.
+        self.next_token = next_token  # type: str
+        # The request ID.
+        self.request_id = request_id  # type: str
+        # The tag values.
+        self.values = values  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListTagValuesResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListTagValuesResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListTagValuesResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, add_list=None, delete_list=None, description=None, group_name=None, instance_id=None,
                  region_id=None, resource_manager_resource_group_id=None):
         # The protected objects that you want to add to the protected object group. Separate the protected objects with commas (,). If you leave this parameter empty, no protected objects are added to the protected object group.
         self.add_list = add_list  # type: str
         # The protected objects that you want to remove from the protected object group. Separate the protected objects with commas (,). If you leave this parameter empty, no protected objects are removed from the protected object group.
         self.delete_list = delete_list  # type: str
@@ -13370,14 +15504,123 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyDomainResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ModifyDomainPunishStatusRequest(TeaModel):
+    def __init__(self, domain=None, instance_id=None, region_id=None, resource_manager_resource_group_id=None):
+        # The domain name that is penalized for failing to obtain an ICP filing.
+        self.domain = domain  # type: str
+        # The ID of the WAF instance.
+        # 
+        # > You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id  # type: str
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id  # type: str
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyDomainPunishStatusRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        # The ID of the request.
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyDomainPunishStatusResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ModifyDomainPunishStatusResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ModifyDomainPunishStatusResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ModifyDomainPunishStatusResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, cluster_resource_id=None, instance_id=None, rule_status=None):
         # The ID of the hybrid cloud cluster.
         self.cluster_resource_id = cluster_resource_id  # type: str
         # The ID of the Web Application Firewall (WAF) instance.
         # 
         # **\
@@ -13614,19 +15857,30 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyMemberAccountRequest(TeaModel):
     def __init__(self, description=None, instance_id=None, member_account_id=None, region_id=None,
                  resource_manager_resource_group_id=None, source_ip=None):
+        # The description of the member. The description must be 1 to 256 characters in length, and can contain letters, digits, periods (.), underscores (\_), hyphens (-), and asterisks (\*).
         self.description = description  # type: str
+        # The ID of the WAF instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
         self.instance_id = instance_id  # type: str
+        # The Alibaba Cloud account ID of the managed member.
         self.member_account_id = member_account_id  # type: str
+        # The region in which the Web Application Firewall (WAF) instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
         self.region_id = region_id  # type: str
+        # The ID of the Alibaba Cloud resource group.
         self.resource_manager_resource_group_id = resource_manager_resource_group_id  # type: str
+        # The source IP address of the request. The system automatically obtains the value of this parameter.
         self.source_ip = source_ip  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyMemberAccountRequest, self).to_map()
@@ -13663,14 +15917,15 @@
         if m.get('SourceIp') is not None:
             self.source_ip = m.get('SourceIp')
         return self
 
 
 class ModifyMemberAccountResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyMemberAccountResponseBody, self).to_map()
@@ -14086,7 +16341,269 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SyncProductInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class TagResourcesRequestTag(TeaModel):
+    def __init__(self, key=None, value=None):
+        # The key of tag N to add to the resource. Valid values of N: 1 to 20.
+        self.key = key  # type: str
+        # The value of tag N to add to the resource. Valid values of N: 1 to 20.
+        self.value = value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(TagResourcesRequestTag, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class TagResourcesRequest(TeaModel):
+    def __init__(self, region_id=None, resource_id=None, resource_type=None, tag=None):
+        # The region in which the Web Application Firewall (WAF) instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id  # type: str
+        # The IDs of the resources. You can specify up to 50 resource IDs.
+        self.resource_id = resource_id  # type: list[str]
+        # The type of the resource. Set the value to ALIYUN::WAF::DEFENSERESOURCE.
+        self.resource_type = resource_type  # type: str
+        # The tags to add to the resource.
+        self.tag = tag  # type: list[TagResourcesRequestTag]
+
+    def validate(self):
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(TagResourcesRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        # The request ID.
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(TagResourcesResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class TagResourcesResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: TagResourcesResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(TagResourcesResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, all=None, region_id=None, resource_id=None, resource_type=None, tag_key=None):
+        # Specifies whether to remove all tags from the specified resource groups or members. Valid values:
+        # 
+        # *   false (default)
+        # *   true
+        self.all = all  # type: bool
+        # The region in which the Web Application Firewall (WAF) instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id  # type: str
+        # The resource IDs. You can specify up to 50 resource IDs.
+        self.resource_id = resource_id  # type: list[str]
+        # The type of the resource. Set the value to ALIYUN::WAF::DEFENSERESOURCE.
+        self.resource_type = resource_type  # type: str
+        # The tag keys. You can specify up to 20 tag keys.
+        self.tag_key = tag_key  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UntagResourcesRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        # The request ID.
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UntagResourcesResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class UntagResourcesResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: UntagResourcesResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(UntagResourcesResponse, self).to_map()
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
+    def from_map(self, m=None):
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

### Comparing `alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001_py2.egg-info/PKG-INFO` & `alibabacloud_waf-openapi20211001_py2-3.4.0/alibabacloud_waf_openapi20211001_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-waf-openapi20211001-py2
-Version: 3.3.0
+Version: 3.4.0
 Summary: Alibaba Cloud waf-openapi (20211001) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_waf-openapi20211001_py2-3.3.0/setup.py` & `alibabacloud_waf-openapi20211001_py2-3.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_waf-openapi20211001_py2.
 
-Created on 07/04/2024
+Created on 24/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_waf_openapi20211001"
 NAME = "alibabacloud_waf-openapi20211001_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud waf-openapi (20211001) SDK Library for Python2"
```

