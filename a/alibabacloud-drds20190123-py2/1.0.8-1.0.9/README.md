# Comparing `tmp/alibabacloud_drds20190123_py2-1.0.8.tar.gz` & `tmp/alibabacloud_drds20190123_py2-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_drds20190123_py2-1.0.8.tar", last modified: Tue Dec  7 02:36:16 2021, max compression
+gzip compressed data, was "dist/alibabacloud_drds20190123_py2-1.0.9.tar", last modified: Fri Jan  7 06:13:02 2022, max compression
```

## Comparing `alibabacloud_drds20190123_py2-1.0.8.tar` & `alibabacloud_drds20190123_py2-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-07 02:36:16.000000 alibabacloud_drds20190123_py2-1.0.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-07 02:36:16.000000 alibabacloud_drds20190123_py2-1.0.8/alibabacloud_drds20190123_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)       26 2021-12-07 02:36:16.000000 alibabacloud_drds20190123_py2-1.0.8/alibabacloud_drds20190123_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2473 2021-12-07 02:36:16.000000 alibabacloud_drds20190123_py2-1.0.8/alibabacloud_drds20190123_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      448 2021-12-07 02:36:16.000000 alibabacloud_drds20190123_py2-1.0.8/alibabacloud_drds20190123_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-07 02:36:16.000000 alibabacloud_drds20190123_py2-1.0.8/alibabacloud_drds20190123_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      175 2021-12-07 02:36:16.000000 alibabacloud_drds20190123_py2-1.0.8/alibabacloud_drds20190123_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      588 2021-12-07 02:36:16.000000 alibabacloud_drds20190123_py2-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1119 2021-12-07 02:36:16.000000 alibabacloud_drds20190123_py2-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)     2473 2021-12-07 02:36:16.000000 alibabacloud_drds20190123_py2-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       28 2021-12-07 02:36:16.000000 alibabacloud_drds20190123_py2-1.0.8/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-07 02:36:16.000000 alibabacloud_drds20190123_py2-1.0.8/alibabacloud_drds20190123/
--rw-r--r--   0 root         (0) root         (0)   155833 2021-12-07 02:36:16.000000 alibabacloud_drds20190123_py2-1.0.8/alibabacloud_drds20190123/client.py
--rw-r--r--   0 root         (0) root         (0)   780004 2021-12-07 02:36:16.000000 alibabacloud_drds20190123_py2-1.0.8/alibabacloud_drds20190123/models.py
--rw-r--r--   0 root         (0) root         (0)       21 2021-12-07 02:36:16.000000 alibabacloud_drds20190123_py2-1.0.8/alibabacloud_drds20190123/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1036 2021-12-07 02:36:16.000000 alibabacloud_drds20190123_py2-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     2943 2021-12-07 02:36:16.000000 alibabacloud_drds20190123_py2-1.0.8/setup.py
--rw-r--r--   0 root         (0) root         (0)       94 2021-12-07 02:36:16.000000 alibabacloud_drds20190123_py2-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      713 2021-12-07 02:36:16.000000 alibabacloud_drds20190123_py2-1.0.8/ChangeLog.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-07 06:13:02.000000 alibabacloud_drds20190123_py2-1.0.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-07 06:13:02.000000 alibabacloud_drds20190123_py2-1.0.9/alibabacloud_drds20190123_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       26 2022-01-07 06:13:02.000000 alibabacloud_drds20190123_py2-1.0.9/alibabacloud_drds20190123_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2473 2022-01-07 06:13:02.000000 alibabacloud_drds20190123_py2-1.0.9/alibabacloud_drds20190123_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      448 2022-01-07 06:13:02.000000 alibabacloud_drds20190123_py2-1.0.9/alibabacloud_drds20190123_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-07 06:13:02.000000 alibabacloud_drds20190123_py2-1.0.9/alibabacloud_drds20190123_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      175 2022-01-07 06:13:02.000000 alibabacloud_drds20190123_py2-1.0.9/alibabacloud_drds20190123_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      588 2022-01-07 06:13:02.000000 alibabacloud_drds20190123_py2-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1119 2022-01-07 06:13:02.000000 alibabacloud_drds20190123_py2-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)     2473 2022-01-07 06:13:02.000000 alibabacloud_drds20190123_py2-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       28 2022-01-07 06:13:02.000000 alibabacloud_drds20190123_py2-1.0.9/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-07 06:13:02.000000 alibabacloud_drds20190123_py2-1.0.9/alibabacloud_drds20190123/
+-rw-r--r--   0 root         (0) root         (0)   147081 2022-01-07 06:13:02.000000 alibabacloud_drds20190123_py2-1.0.9/alibabacloud_drds20190123/client.py
+-rw-r--r--   0 root         (0) root         (0)   620365 2022-01-07 06:13:02.000000 alibabacloud_drds20190123_py2-1.0.9/alibabacloud_drds20190123/models.py
+-rw-r--r--   0 root         (0) root         (0)       21 2022-01-07 06:13:02.000000 alibabacloud_drds20190123_py2-1.0.9/alibabacloud_drds20190123/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2022-01-07 06:13:02.000000 alibabacloud_drds20190123_py2-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     2943 2022-01-07 06:13:02.000000 alibabacloud_drds20190123_py2-1.0.9/setup.py
+-rw-r--r--   0 root         (0) root         (0)       94 2022-01-07 06:13:02.000000 alibabacloud_drds20190123_py2-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      759 2022-01-07 06:13:02.000000 alibabacloud_drds20190123_py2-1.0.9/ChangeLog.md
```

### Comparing `alibabacloud_drds20190123_py2-1.0.8/alibabacloud_drds20190123_py2.egg-info/PKG-INFO` & `alibabacloud_drds20190123_py2-1.0.9/alibabacloud_drds20190123_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: alibabacloud-drds20190123-py2
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud Distributed Relational Database Service (20190123) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_drds20190123_py2-1.0.8/LICENSE` & `alibabacloud_drds20190123_py2-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_drds20190123_py2-1.0.8/README.md` & `alibabacloud_drds20190123_py2-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_drds20190123_py2-1.0.8/PKG-INFO` & `alibabacloud_drds20190123_py2-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: alibabacloud_drds20190123_py2
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud Distributed Relational Database Service (20190123) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_drds20190123_py2-1.0.8/alibabacloud_drds20190123/client.py` & `alibabacloud_drds20190123_py2-1.0.9/alibabacloud_drds20190123/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -72,4126 +72,3625 @@
         if not UtilClient.is_unset(endpoint_map) and not UtilClient.empty(endpoint_map.get(region_id)):
             return endpoint_map.get(region_id)
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def change_account_password_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['AccountName'] = request.account_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['Password'] = request.password
+        if not UtilClient.is_unset(request.account_name):
+            query['AccountName'] = request.account_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.password):
+            query['Password'] = request.password
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ChangeAccountPassword',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.ChangeAccountPasswordResponse(),
             self.call_api(params, req, runtime)
         )
 
     def change_account_password(self, request):
         runtime = util_models.RuntimeOptions()
         return self.change_account_password_with_options(request, runtime)
 
     def change_instance_azone_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['DrdsRegionId'] = request.drds_region_id
-        query['OriginAzoneId'] = request.origin_azone_id
-        query['TargetAzoneId'] = request.target_azone_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.drds_region_id):
+            query['DrdsRegionId'] = request.drds_region_id
+        if not UtilClient.is_unset(request.origin_azone_id):
+            query['OriginAzoneId'] = request.origin_azone_id
+        if not UtilClient.is_unset(request.target_azone_id):
+            query['TargetAzoneId'] = request.target_azone_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ChangeInstanceAzone',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.ChangeInstanceAzoneResponse(),
             self.call_api(params, req, runtime)
         )
 
     def change_instance_azone(self, request):
         runtime = util_models.RuntimeOptions()
         return self.change_instance_azone_with_options(request, runtime)
 
-    def change_instance_network_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['ClassicExpiredDays'] = request.classic_expired_days
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RetainClassic'] = request.retain_classic
-        query['SrcInstanceNetworkType'] = request.src_instance_network_type
-        query['VpcId'] = request.vpc_id
-        query['VswitchId'] = request.vswitch_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='ChangeInstanceNetwork',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.ChangeInstanceNetworkResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def change_instance_network(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.change_instance_network_with_options(request, runtime)
-
     def check_drds_db_name_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CheckDrdsDbName',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.CheckDrdsDbNameResponse(),
             self.call_api(params, req, runtime)
         )
 
     def check_drds_db_name(self, request):
         runtime = util_models.RuntimeOptions()
         return self.check_drds_db_name_with_options(request, runtime)
 
     def check_expand_status_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CheckExpandStatus',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.CheckExpandStatusResponse(),
             self.call_api(params, req, runtime)
         )
 
     def check_expand_status(self, request):
         runtime = util_models.RuntimeOptions()
         return self.check_expand_status_with_options(request, runtime)
 
-    def check_rds_super_account_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['AccountName'] = request.account_name
-        query['DbInstanceId'] = request.db_instance_id
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['Password'] = request.password
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='CheckRdsSuperAccount',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.CheckRdsSuperAccountResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def check_rds_super_account(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.check_rds_super_account_with_options(request, runtime)
-
     def check_sql_audit_enable_status_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CheckSqlAuditEnableStatus',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.CheckSqlAuditEnableStatusResponse(),
             self.call_api(params, req, runtime)
         )
 
     def check_sql_audit_enable_status(self, request):
         runtime = util_models.RuntimeOptions()
         return self.check_sql_audit_enable_status_with_options(request, runtime)
 
-    def configure_drds_db_instances_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['DbInstance'] = request.db_instance
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='ConfigureDrdsDbInstances',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.ConfigureDrdsDbInstancesResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def configure_drds_db_instances(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.configure_drds_db_instances_with_options(request, runtime)
-
     def create_drds_dbwith_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['AccountName'] = request.account_name
-        query['DbInstType'] = request.db_inst_type
-        query['DbInstanceIsCreating'] = request.db_instance_is_creating
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['Encode'] = request.encode
-        query['InstDbName'] = request.inst_db_name
-        query['Password'] = request.password
-        query['RdsInstance'] = request.rds_instance
-        query['RdsSuperAccount'] = request.rds_super_account
-        query['Type'] = request.type
+        if not UtilClient.is_unset(request.account_name):
+            query['AccountName'] = request.account_name
+        if not UtilClient.is_unset(request.db_inst_type):
+            query['DbInstType'] = request.db_inst_type
+        if not UtilClient.is_unset(request.db_instance_is_creating):
+            query['DbInstanceIsCreating'] = request.db_instance_is_creating
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.encode):
+            query['Encode'] = request.encode
+        if not UtilClient.is_unset(request.inst_db_name):
+            query['InstDbName'] = request.inst_db_name
+        if not UtilClient.is_unset(request.password):
+            query['Password'] = request.password
+        if not UtilClient.is_unset(request.rds_instance):
+            query['RdsInstance'] = request.rds_instance
+        if not UtilClient.is_unset(request.rds_super_account):
+            query['RdsSuperAccount'] = request.rds_super_account
+        if not UtilClient.is_unset(request.type):
+            query['Type'] = request.type
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateDrdsDB',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.CreateDrdsDBResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_drds_db(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_drds_dbwith_options(request, runtime)
 
-    def create_drds_dbpre_check_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['AccountName'] = request.account_name
-        query['DbInstType'] = request.db_inst_type
-        query['DbInstanceIsCreating'] = request.db_instance_is_creating
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['Encode'] = request.encode
-        query['InstDbName'] = request.inst_db_name
-        query['Password'] = request.password
-        query['RdsInstance'] = request.rds_instance
-        query['RdsSuperAccount'] = request.rds_super_account
-        query['Type'] = request.type
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='CreateDrdsDBPreCheck',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.CreateDrdsDBPreCheckResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def create_drds_dbpre_check(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.create_drds_dbpre_check_with_options(request, runtime)
-
-    def create_drds_dbpreview_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['AccountName'] = request.account_name
-        query['DbInstType'] = request.db_inst_type
-        query['DbInstanceIsCreating'] = request.db_instance_is_creating
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['InstDbName'] = request.inst_db_name
-        query['OrderId'] = request.order_id
-        query['RdsInstance'] = request.rds_instance
-        query['Type'] = request.type
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='CreateDrdsDBPreview',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.CreateDrdsDBPreviewResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def create_drds_dbpreview(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.create_drds_dbpreview_with_options(request, runtime)
-
     def create_drds_instance_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['ClientToken'] = request.client_token
-        query['Description'] = request.description
-        query['Duration'] = request.duration
-        query['InstanceSeries'] = request.instance_series
-        query['IsAutoRenew'] = request.is_auto_renew
-        query['MasterInstId'] = request.master_inst_id
-        query['MySQLVersion'] = request.my_sqlversion
-        query['PayType'] = request.pay_type
-        query['PricingCycle'] = request.pricing_cycle
-        query['Quantity'] = request.quantity
-        query['RegionId'] = request.region_id
-        query['ResourceGroupId'] = request.resource_group_id
-        query['Specification'] = request.specification
-        query['Type'] = request.type
-        query['VpcId'] = request.vpc_id
-        query['VswitchId'] = request.vswitch_id
-        query['ZoneId'] = request.zone_id
-        query['isHa'] = request.is_ha
+        if not UtilClient.is_unset(request.client_token):
+            query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.description):
+            query['Description'] = request.description
+        if not UtilClient.is_unset(request.duration):
+            query['Duration'] = request.duration
+        if not UtilClient.is_unset(request.instance_series):
+            query['InstanceSeries'] = request.instance_series
+        if not UtilClient.is_unset(request.is_auto_renew):
+            query['IsAutoRenew'] = request.is_auto_renew
+        if not UtilClient.is_unset(request.master_inst_id):
+            query['MasterInstId'] = request.master_inst_id
+        if not UtilClient.is_unset(request.my_sqlversion):
+            query['MySQLVersion'] = request.my_sqlversion
+        if not UtilClient.is_unset(request.pay_type):
+            query['PayType'] = request.pay_type
+        if not UtilClient.is_unset(request.pricing_cycle):
+            query['PricingCycle'] = request.pricing_cycle
+        if not UtilClient.is_unset(request.quantity):
+            query['Quantity'] = request.quantity
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.specification):
+            query['Specification'] = request.specification
+        if not UtilClient.is_unset(request.type):
+            query['Type'] = request.type
+        if not UtilClient.is_unset(request.vpc_id):
+            query['VpcId'] = request.vpc_id
+        if not UtilClient.is_unset(request.vswitch_id):
+            query['VswitchId'] = request.vswitch_id
+        if not UtilClient.is_unset(request.zone_id):
+            query['ZoneId'] = request.zone_id
+        if not UtilClient.is_unset(request.is_ha):
+            query['isHa'] = request.is_ha
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateDrdsInstance',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.CreateDrdsInstanceResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_drds_instance(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_drds_instance_with_options(request, runtime)
 
-    def create_evaluate_pre_check_task_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['AvgQpsGrowthScale'] = request.avg_qps_growth_scale
-        query['DataGrowthScale'] = request.data_growth_scale
-        query['DbInfo'] = request.db_info
-        query['EvaluateHours'] = request.evaluate_hours
-        query['TaskName'] = request.task_name
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='CreateEvaluatePreCheckTask',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.CreateEvaluatePreCheckTaskResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def create_evaluate_pre_check_task(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.create_evaluate_pre_check_task_with_options(request, runtime)
-
     def create_instance_account_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['AccountName'] = request.account_name
-        query['DbPrivilege'] = request.db_privilege
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['Password'] = request.password
+        if not UtilClient.is_unset(request.account_name):
+            query['AccountName'] = request.account_name
+        if not UtilClient.is_unset(request.db_privilege):
+            query['DbPrivilege'] = request.db_privilege
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.password):
+            query['Password'] = request.password
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateInstanceAccount',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.CreateInstanceAccountResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_instance_account(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_instance_account_with_options(request, runtime)
 
     def create_instance_internet_address_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateInstanceInternetAddress',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.CreateInstanceInternetAddressResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_instance_internet_address(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_instance_internet_address_with_options(request, runtime)
 
     def create_order_for_rds_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['Params'] = request.params
-        query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.params):
+            query['Params'] = request.params
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateOrderForRds',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.CreateOrderForRdsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_order_for_rds(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_order_for_rds_with_options(request, runtime)
 
     def create_shard_task_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RegionId'] = request.region_id
-        query['SourceTableName'] = request.source_table_name
-        query['TargetTableName'] = request.target_table_name
-        query['TaskType'] = request.task_type
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.source_table_name):
+            query['SourceTableName'] = request.source_table_name
+        if not UtilClient.is_unset(request.target_table_name):
+            query['TargetTableName'] = request.target_table_name
+        if not UtilClient.is_unset(request.task_type):
+            query['TaskType'] = request.task_type
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateShardTask',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.CreateShardTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_shard_task(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_shard_task_with_options(request, runtime)
 
     def describe_back_menu_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeBackMenu',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeBackMenuResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_back_menu(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_back_menu_with_options(request, runtime)
 
     def describe_backup_dbs_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['BackupId'] = request.backup_id
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['PreferredRestoreTime'] = request.preferred_restore_time
+        if not UtilClient.is_unset(request.backup_id):
+            query['BackupId'] = request.backup_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.preferred_restore_time):
+            query['PreferredRestoreTime'] = request.preferred_restore_time
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeBackupDbs',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeBackupDbsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_backup_dbs(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_backup_dbs_with_options(request, runtime)
 
     def describe_backup_local_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeBackupLocal',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeBackupLocalResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_backup_local(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_backup_local_with_options(request, runtime)
 
     def describe_backup_policy_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeBackupPolicy',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeBackupPolicyResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_backup_policy(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_backup_policy_with_options(request, runtime)
 
     def describe_backup_sets_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['EndTime'] = request.end_time
-        query['StartTime'] = request.start_time
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeBackupSets',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeBackupSetsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_backup_sets(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_backup_sets_with_options(request, runtime)
 
     def describe_backup_times_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeBackupTimes',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeBackupTimesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_backup_times(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_backup_times_with_options(request, runtime)
 
     def describe_broadcast_tables_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['CurrentPage'] = request.current_page
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['PageSize'] = request.page_size
-        query['Query'] = request.query
-        query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.current_page):
+            query['CurrentPage'] = request.current_page
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.query):
+            query['Query'] = request.query
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeBroadcastTables',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeBroadcastTablesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_broadcast_tables(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_broadcast_tables_with_options(request, runtime)
 
-    def describe_data_import_task_report_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['TaskId'] = request.task_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='DescribeDataImportTaskReport',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.DescribeDataImportTaskReportResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def describe_data_import_task_report(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.describe_data_import_task_report_with_options(request, runtime)
-
     def describe_db_instance_dbs_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['AccountName'] = request.account_name
-        query['DbInstType'] = request.db_inst_type
-        query['DbInstanceId'] = request.db_instance_id
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['Password'] = request.password
+        if not UtilClient.is_unset(request.account_name):
+            query['AccountName'] = request.account_name
+        if not UtilClient.is_unset(request.db_inst_type):
+            query['DbInstType'] = request.db_inst_type
+        if not UtilClient.is_unset(request.db_instance_id):
+            query['DbInstanceId'] = request.db_instance_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.password):
+            query['Password'] = request.password
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDbInstanceDbs',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeDbInstanceDbsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_db_instance_dbs(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_db_instance_dbs_with_options(request, runtime)
 
     def describe_db_instances_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbInstType'] = request.db_inst_type
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['PageNumber'] = request.page_number
-        query['PageSize'] = request.page_size
-        query['Search'] = request.search
+        if not UtilClient.is_unset(request.db_inst_type):
+            query['DbInstType'] = request.db_inst_type
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.search):
+            query['Search'] = request.search
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDbInstances',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeDbInstancesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_db_instances(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_db_instances_with_options(request, runtime)
 
     def describe_drds_dbwith_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDrdsDB',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeDrdsDBResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_drds_db(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_drds_dbwith_options(request, runtime)
 
     def describe_drds_dbcluster_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbInstanceId'] = request.db_instance_id
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.db_instance_id):
+            query['DbInstanceId'] = request.db_instance_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDrdsDBCluster',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeDrdsDBClusterResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_drds_dbcluster(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_drds_dbcluster_with_options(request, runtime)
 
     def describe_drds_dbip_white_list_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['GroupName'] = request.group_name
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.group_name):
+            query['GroupName'] = request.group_name
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDrdsDBIpWhiteList',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeDrdsDBIpWhiteListResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_drds_dbip_white_list(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_drds_dbip_white_list_with_options(request, runtime)
 
     def describe_drds_dbs_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['PageNumber'] = request.page_number
-        query['PageSize'] = request.page_size
-        query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDrdsDBs',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeDrdsDBsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_drds_dbs(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_drds_dbs_with_options(request, runtime)
 
     def describe_drds_db_instance_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbInstanceId'] = request.db_instance_id
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.db_instance_id):
+            query['DbInstanceId'] = request.db_instance_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDrdsDbInstance',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeDrdsDbInstanceResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_drds_db_instance(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_drds_db_instance_with_options(request, runtime)
 
     def describe_drds_db_instances_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['PageNumber'] = request.page_number
-        query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDrdsDbInstances',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeDrdsDbInstancesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_drds_db_instances(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_drds_db_instances_with_options(request, runtime)
 
     def describe_drds_db_rds_name_list_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDrdsDbRdsNameList',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeDrdsDbRdsNameListResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_drds_db_rds_name_list(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_drds_db_rds_name_list_with_options(request, runtime)
 
-    def describe_drds_db_spec_and_price_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['DBName'] = request.dbname
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='DescribeDrdsDbSpecAndPrice',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.DescribeDrdsDbSpecAndPriceResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def describe_drds_db_spec_and_price(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.describe_drds_db_spec_and_price_with_options(request, runtime)
-
     def describe_drds_db_tasks_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['TaskType'] = request.task_type
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.task_type):
+            query['TaskType'] = request.task_type
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDrdsDbTasks',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeDrdsDbTasksResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_drds_db_tasks(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_drds_db_tasks_with_options(request, runtime)
 
     def describe_drds_instance_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDrdsInstance',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeDrdsInstanceResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_drds_instance(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_drds_instance_with_options(request, runtime)
 
     def describe_drds_instance_db_monitor_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['EndTime'] = request.end_time
-        query['Key'] = request.key
-        query['RegionId'] = request.region_id
-        query['StartTime'] = request.start_time
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.key):
+            query['Key'] = request.key
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDrdsInstanceDbMonitor',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeDrdsInstanceDbMonitorResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_drds_instance_db_monitor(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_drds_instance_db_monitor_with_options(request, runtime)
 
     def describe_drds_instance_level_tasks_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDrdsInstanceLevelTasks',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeDrdsInstanceLevelTasksResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_drds_instance_level_tasks(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_drds_instance_level_tasks_with_options(request, runtime)
 
     def describe_drds_instance_monitor_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['EndTime'] = request.end_time
-        query['Key'] = request.key
-        query['PeriodMultiple'] = request.period_multiple
-        query['RegionId'] = request.region_id
-        query['StartTime'] = request.start_time
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.key):
+            query['Key'] = request.key
+        if not UtilClient.is_unset(request.period_multiple):
+            query['PeriodMultiple'] = request.period_multiple
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDrdsInstanceMonitor',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeDrdsInstanceMonitorResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_drds_instance_monitor(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_drds_instance_monitor_with_options(request, runtime)
 
     def describe_drds_instance_version_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDrdsInstanceVersion',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeDrdsInstanceVersionResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_drds_instance_version(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_drds_instance_version_with_options(request, runtime)
 
     def describe_drds_instances_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['Description'] = request.description
-        query['Expired'] = request.expired
-        query['Mix'] = request.mix
-        query['PageNumber'] = request.page_number
-        query['PageSize'] = request.page_size
-        query['ProductVersion'] = request.product_version
-        query['RegionId'] = request.region_id
-        query['ResourceGroupId'] = request.resource_group_id
-        query['Tag'] = request.tag
-        query['Type'] = request.type
+        if not UtilClient.is_unset(request.description):
+            query['Description'] = request.description
+        if not UtilClient.is_unset(request.expired):
+            query['Expired'] = request.expired
+        if not UtilClient.is_unset(request.mix):
+            query['Mix'] = request.mix
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.product_version):
+            query['ProductVersion'] = request.product_version
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
+        if not UtilClient.is_unset(request.type):
+            query['Type'] = request.type
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDrdsInstances',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeDrdsInstancesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_drds_instances(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_drds_instances_with_options(request, runtime)
 
     def describe_drds_params_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['ParamLevel'] = request.param_level
-        query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.param_level):
+            query['ParamLevel'] = request.param_level
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDrdsParams',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeDrdsParamsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_drds_params(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_drds_params_with_options(request, runtime)
 
     def describe_drds_rds_instances_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDrdsRdsInstances',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeDrdsRdsInstancesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_drds_rds_instances(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_drds_rds_instances_with_options(request, runtime)
 
     def describe_drds_sharding_dbs_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DbNamePattern'] = request.db_name_pattern
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['PageNumber'] = request.page_number
-        query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.db_name_pattern):
+            query['DbNamePattern'] = request.db_name_pattern
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDrdsShardingDbs',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeDrdsShardingDbsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_drds_sharding_dbs(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_drds_sharding_dbs_with_options(request, runtime)
 
     def describe_drds_slow_sqls_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['EndTime'] = request.end_time
-        query['ExeTime'] = request.exe_time
-        query['PageNumber'] = request.page_number
-        query['PageSize'] = request.page_size
-        query['StartTime'] = request.start_time
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.exe_time):
+            query['ExeTime'] = request.exe_time
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDrdsSlowSqls',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeDrdsSlowSqlsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_drds_slow_sqls(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_drds_slow_sqls_with_options(request, runtime)
 
     def describe_drds_sql_audit_status_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDrdsSqlAuditStatus',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeDrdsSqlAuditStatusResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_drds_sql_audit_status(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_drds_sql_audit_status_with_options(request, runtime)
 
     def describe_drds_tasks_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['TaskType'] = request.task_type
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.task_type):
+            query['TaskType'] = request.task_type
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDrdsTasks',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeDrdsTasksResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_drds_tasks(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_drds_tasks_with_options(request, runtime)
 
     def describe_expand_logic_table_info_list_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeExpandLogicTableInfoList',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeExpandLogicTableInfoListResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_expand_logic_table_info_list(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_expand_logic_table_info_list_with_options(request, runtime)
 
-    def describe_hi_store_instance_info_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['HistoreInstanceId'] = request.histore_instance_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='DescribeHiStoreInstanceInfo',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.DescribeHiStoreInstanceInfoResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def describe_hi_store_instance_info(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.describe_hi_store_instance_info_with_options(request, runtime)
-
     def describe_hot_db_list_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeHotDbList',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeHotDbListResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_hot_db_list(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_hot_db_list_with_options(request, runtime)
 
     def describe_inst_db_log_info_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeInstDbLogInfo',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeInstDbLogInfoResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_inst_db_log_info(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_inst_db_log_info_with_options(request, runtime)
 
     def describe_inst_db_sls_info_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeInstDbSlsInfo',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeInstDbSlsInfoResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_inst_db_sls_info(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_inst_db_sls_info_with_options(request, runtime)
 
     def describe_instance_accounts_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeInstanceAccounts',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeInstanceAccountsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_instance_accounts(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_instance_accounts_with_options(request, runtime)
 
-    def describe_instance_menu_switch_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='DescribeInstanceMenuSwitch',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.DescribeInstanceMenuSwitchResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def describe_instance_menu_switch(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.describe_instance_menu_switch_with_options(request, runtime)
-
     def describe_instance_switch_azone_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeInstanceSwitchAzone',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeInstanceSwitchAzoneResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_instance_switch_azone(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_instance_switch_azone_with_options(request, runtime)
 
     def describe_instance_switch_network_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeInstanceSwitchNetwork',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeInstanceSwitchNetworkResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_instance_switch_network(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_instance_switch_network_with_options(request, runtime)
 
     def describe_pre_check_result_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RegionId'] = request.region_id
-        query['TaskId'] = request.task_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.task_id):
+            query['TaskId'] = request.task_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribePreCheckResult',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribePreCheckResultResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_pre_check_result(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_pre_check_result_with_options(request, runtime)
 
     def describe_rdsperformance_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbInstType'] = request.db_inst_type
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['EndTime'] = request.end_time
-        query['Keys'] = request.keys
-        query['RdsInstanceId'] = request.rds_instance_id
-        query['StartTime'] = request.start_time
+        if not UtilClient.is_unset(request.db_inst_type):
+            query['DbInstType'] = request.db_inst_type
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.keys):
+            query['Keys'] = request.keys
+        if not UtilClient.is_unset(request.rds_instance_id):
+            query['RdsInstanceId'] = request.rds_instance_id
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeRDSPerformance',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeRDSPerformanceResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_rdsperformance(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_rdsperformance_with_options(request, runtime)
 
     def describe_rds_commodity_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['CommodityCode'] = request.commodity_code
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['OrderType'] = request.order_type
+        if not UtilClient.is_unset(request.commodity_code):
+            query['CommodityCode'] = request.commodity_code
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.order_type):
+            query['OrderType'] = request.order_type
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeRdsCommodity',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeRdsCommodityResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_rds_commodity(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_rds_commodity_with_options(request, runtime)
 
-    def describe_rds_drds_dbwith_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RdsInstanceId'] = request.rds_instance_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='DescribeRdsDrdsDB',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.DescribeRdsDrdsDBResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def describe_rds_drds_db(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.describe_rds_drds_dbwith_options(request, runtime)
-
     def describe_rds_performance_summary_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RdsInstanceId'] = request.rds_instance_id
-        query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.rds_instance_id):
+            query['RdsInstanceId'] = request.rds_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeRdsPerformanceSummary',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeRdsPerformanceSummaryResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_rds_performance_summary(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_rds_performance_summary_with_options(request, runtime)
 
-    def describe_rds_price_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['Params'] = request.params
-        query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='DescribeRdsPrice',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.DescribeRdsPriceResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def describe_rds_price(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.describe_rds_price_with_options(request, runtime)
-
-    def describe_rds_read_only_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['DbInstType'] = request.db_inst_type
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RdsInstanceId'] = request.rds_instance_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='DescribeRdsReadOnly',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.DescribeRdsReadOnlyResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def describe_rds_read_only(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.describe_rds_read_only_with_options(request, runtime)
-
     def describe_rds_super_account_instances_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbInstType'] = request.db_inst_type
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RdsInstance'] = request.rds_instance
+        if not UtilClient.is_unset(request.db_inst_type):
+            query['DbInstType'] = request.db_inst_type
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.rds_instance):
+            query['RdsInstance'] = request.rds_instance
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeRdsSuperAccountInstances',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeRdsSuperAccountInstancesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_rds_super_account_instances(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_rds_super_account_instances_with_options(request, runtime)
 
-    def describe_rds_vpc_for_zone_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['RegionId'] = request.region_id
-        query['ZoneId'] = request.zone_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='DescribeRdsVpcForZone',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.DescribeRdsVpcForZoneResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def describe_rds_vpc_for_zone(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.describe_rds_vpc_for_zone_with_options(request, runtime)
-
     def describe_recycle_bin_status_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeRecycleBinStatus',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeRecycleBinStatusResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_recycle_bin_status(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_recycle_bin_status_with_options(request, runtime)
 
     def describe_recycle_bin_tables_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeRecycleBinTables',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeRecycleBinTablesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_recycle_bin_tables(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_recycle_bin_tables_with_options(request, runtime)
 
     def describe_restore_order_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['BackupDbNames'] = request.backup_db_names
-        query['BackupId'] = request.backup_id
-        query['BackupLevel'] = request.backup_level
-        query['BackupMode'] = request.backup_mode
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['PreferredBackupTime'] = request.preferred_backup_time
+        if not UtilClient.is_unset(request.backup_db_names):
+            query['BackupDbNames'] = request.backup_db_names
+        if not UtilClient.is_unset(request.backup_id):
+            query['BackupId'] = request.backup_id
+        if not UtilClient.is_unset(request.backup_level):
+            query['BackupLevel'] = request.backup_level
+        if not UtilClient.is_unset(request.backup_mode):
+            query['BackupMode'] = request.backup_mode
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.preferred_backup_time):
+            query['PreferredBackupTime'] = request.preferred_backup_time
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeRestoreOrder',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeRestoreOrderResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_restore_order(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_restore_order_with_options(request, runtime)
 
     def describe_shard_task_info_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RegionId'] = request.region_id
-        query['SourceTableName'] = request.source_table_name
-        query['TargetTableName'] = request.target_table_name
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.source_table_name):
+            query['SourceTableName'] = request.source_table_name
+        if not UtilClient.is_unset(request.target_table_name):
+            query['TargetTableName'] = request.target_table_name
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeShardTaskInfo',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeShardTaskInfoResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_shard_task_info(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_shard_task_info_with_options(request, runtime)
 
     def describe_shard_task_list_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['CurrentPage'] = request.current_page
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['PageSize'] = request.page_size
-        query['Query'] = request.query
-        query['RegionId'] = request.region_id
-        query['TaskType'] = request.task_type
+        if not UtilClient.is_unset(request.current_page):
+            query['CurrentPage'] = request.current_page
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.query):
+            query['Query'] = request.query
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.task_type):
+            query['TaskType'] = request.task_type
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeShardTaskList',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeShardTaskListResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_shard_task_list(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_shard_task_list_with_options(request, runtime)
 
     def describe_sql_flashbak_task_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeSqlFlashbakTask',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeSqlFlashbakTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_sql_flashbak_task(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_sql_flashbak_task_with_options(request, runtime)
 
-    def describe_src_rds_list_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['PartitionMapping'] = request.partition_mapping
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='DescribeSrcRdsList',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.DescribeSrcRdsListResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def describe_src_rds_list(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.describe_src_rds_list_with_options(request, runtime)
-
     def describe_table_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RegionId'] = request.region_id
-        query['TableName'] = request.table_name
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.table_name):
+            query['TableName'] = request.table_name
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeTable',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeTableResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_table(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_table_with_options(request, runtime)
 
     def describe_table_list_by_type_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['CurrentPage'] = request.current_page
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['PageSize'] = request.page_size
-        query['Query'] = request.query
-        query['RegionId'] = request.region_id
-        query['TableType'] = request.table_type
+        if not UtilClient.is_unset(request.current_page):
+            query['CurrentPage'] = request.current_page
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.query):
+            query['Query'] = request.query
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.table_type):
+            query['TableType'] = request.table_type
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeTableListByType',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeTableListByTypeResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_table_list_by_type(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_table_list_by_type_with_options(request, runtime)
 
     def describe_tables_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['CurrentPage'] = request.current_page
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['PageSize'] = request.page_size
-        query['Query'] = request.query
-        query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.current_page):
+            query['CurrentPage'] = request.current_page
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.query):
+            query['Query'] = request.query
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeTables',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DescribeTablesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_tables(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_tables_with_options(request, runtime)
 
     def disable_sql_audit_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DisableSqlAudit',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.DisableSqlAuditResponse(),
             self.call_api(params, req, runtime)
         )
 
     def disable_sql_audit(self, request):
         runtime = util_models.RuntimeOptions()
         return self.disable_sql_audit_with_options(request, runtime)
 
     def enable_instance_ipv_6address_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='EnableInstanceIpv6Address',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.EnableInstanceIpv6AddressResponse(),
             self.call_api(params, req, runtime)
         )
 
     def enable_instance_ipv_6address(self, request):
         runtime = util_models.RuntimeOptions()
         return self.enable_instance_ipv_6address_with_options(request, runtime)
 
     def enable_sql_audit_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['IsRecall'] = request.is_recall
-        query['RecallEndTimestamp'] = request.recall_end_timestamp
-        query['RecallStartTimestamp'] = request.recall_start_timestamp
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.is_recall):
+            query['IsRecall'] = request.is_recall
+        if not UtilClient.is_unset(request.recall_end_timestamp):
+            query['RecallEndTimestamp'] = request.recall_end_timestamp
+        if not UtilClient.is_unset(request.recall_start_timestamp):
+            query['RecallStartTimestamp'] = request.recall_start_timestamp
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='EnableSqlAudit',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.EnableSqlAuditResponse(),
             self.call_api(params, req, runtime)
         )
 
     def enable_sql_audit(self, request):
         runtime = util_models.RuntimeOptions()
         return self.enable_sql_audit_with_options(request, runtime)
 
     def enable_sql_flashback_match_switch_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='EnableSqlFlashbackMatchSwitch',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.EnableSqlFlashbackMatchSwitchResponse(),
             self.call_api(params, req, runtime)
         )
 
     def enable_sql_flashback_match_switch(self, request):
         runtime = util_models.RuntimeOptions()
         return self.enable_sql_flashback_match_switch_with_options(request, runtime)
 
     def flashback_recycle_bin_table_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RegionId'] = request.region_id
-        query['TableName'] = request.table_name
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.table_name):
+            query['TableName'] = request.table_name
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='FlashbackRecycleBinTable',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.FlashbackRecycleBinTableResponse(),
             self.call_api(params, req, runtime)
         )
 
     def flashback_recycle_bin_table(self, request):
         runtime = util_models.RuntimeOptions()
         return self.flashback_recycle_bin_table_with_options(request, runtime)
 
     def get_drds_db_rds_relation_info_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetDrdsDbRdsRelationInfo',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.GetDrdsDbRdsRelationInfoResponse(),
             self.call_api(params, req, runtime)
         )
 
     def get_drds_db_rds_relation_info(self, request):
         runtime = util_models.RuntimeOptions()
         return self.get_drds_db_rds_relation_info_with_options(request, runtime)
 
     def list_tag_resources_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['NextToken'] = request.next_token
-        query['RegionId'] = request.region_id
-        query['ResourceId'] = request.resource_id
-        query['ResourceType'] = request.resource_type
-        query['Tag'] = request.tag
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
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListTagResources',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.ListTagResourcesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def list_tag_resources(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_tag_resources_with_options(request, runtime)
 
-    def list_user_reports_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['ReportId'] = request.report_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='ListUserReports',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.ListUserReportsResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def list_user_reports(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.list_user_reports_with_options(request, runtime)
-
-    def list_versions_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['DrdsVer'] = request.drds_ver
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='ListVersions',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.ListVersionsResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def list_versions(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.list_versions_with_options(request, runtime)
-
     def manage_private_rds_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DBInstanceId'] = request.dbinstance_id
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['Params'] = request.params
-        query['RdsAction'] = request.rds_action
-        query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.dbinstance_id):
+            query['DBInstanceId'] = request.dbinstance_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.params):
+            query['Params'] = request.params
+        if not UtilClient.is_unset(request.rds_action):
+            query['RdsAction'] = request.rds_action
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ManagePrivateRds',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.ManagePrivateRdsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def manage_private_rds(self, request):
         runtime = util_models.RuntimeOptions()
         return self.manage_private_rds_with_options(request, runtime)
 
     def modify_account_description_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['AccountName'] = request.account_name
-        query['Description'] = request.description
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.account_name):
+            query['AccountName'] = request.account_name
+        if not UtilClient.is_unset(request.description):
+            query['Description'] = request.description
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyAccountDescription',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.ModifyAccountDescriptionResponse(),
             self.call_api(params, req, runtime)
         )
 
     def modify_account_description(self, request):
         runtime = util_models.RuntimeOptions()
         return self.modify_account_description_with_options(request, runtime)
 
     def modify_account_privilege_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['AccountName'] = request.account_name
-        query['DbPrivilege'] = request.db_privilege
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.account_name):
+            query['AccountName'] = request.account_name
+        if not UtilClient.is_unset(request.db_privilege):
+            query['DbPrivilege'] = request.db_privilege
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyAccountPrivilege',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.ModifyAccountPrivilegeResponse(),
             self.call_api(params, req, runtime)
         )
 
     def modify_account_privilege(self, request):
         runtime = util_models.RuntimeOptions()
         return self.modify_account_privilege_with_options(request, runtime)
 
     def modify_drds_instance_description_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['Description'] = request.description
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.description):
+            query['Description'] = request.description
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyDrdsInstanceDescription',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.ModifyDrdsInstanceDescriptionResponse(),
             self.call_api(params, req, runtime)
         )
 
     def modify_drds_instance_description(self, request):
         runtime = util_models.RuntimeOptions()
         return self.modify_drds_instance_description_with_options(request, runtime)
 
     def modify_drds_ip_white_list_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['GroupAttribute'] = request.group_attribute
-        query['GroupName'] = request.group_name
-        query['IpWhiteList'] = request.ip_white_list
-        query['Mode'] = request.mode
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.group_attribute):
+            query['GroupAttribute'] = request.group_attribute
+        if not UtilClient.is_unset(request.group_name):
+            query['GroupName'] = request.group_name
+        if not UtilClient.is_unset(request.ip_white_list):
+            query['IpWhiteList'] = request.ip_white_list
+        if not UtilClient.is_unset(request.mode):
+            query['Mode'] = request.mode
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyDrdsIpWhiteList',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.ModifyDrdsIpWhiteListResponse(),
             self.call_api(params, req, runtime)
         )
 
     def modify_drds_ip_white_list(self, request):
         runtime = util_models.RuntimeOptions()
         return self.modify_drds_ip_white_list_with_options(request, runtime)
 
-    def modify_event_task_status_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['EventId'] = request.event_id
-        query['Region'] = request.region
-        query['SwitchTime'] = request.switch_time
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='ModifyEventTaskStatus',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.ModifyEventTaskStatusResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def modify_event_task_status(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.modify_event_task_status_with_options(request, runtime)
-
     def modify_polar_db_read_weight_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbInstanceId'] = request.db_instance_id
-        query['DbName'] = request.db_name
-        query['DbNodeIds'] = request.db_node_ids
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['Weights'] = request.weights
+        if not UtilClient.is_unset(request.db_instance_id):
+            query['DbInstanceId'] = request.db_instance_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.db_node_ids):
+            query['DbNodeIds'] = request.db_node_ids
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.weights):
+            query['Weights'] = request.weights
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyPolarDbReadWeight',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.ModifyPolarDbReadWeightResponse(),
             self.call_api(params, req, runtime)
         )
 
     def modify_polar_db_read_weight(self, request):
         runtime = util_models.RuntimeOptions()
         return self.modify_polar_db_read_weight_with_options(request, runtime)
 
     def modify_rds_read_weight_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['InstanceNames'] = request.instance_names
-        query['Weights'] = request.weights
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.instance_names):
+            query['InstanceNames'] = request.instance_names
+        if not UtilClient.is_unset(request.weights):
+            query['Weights'] = request.weights
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyRdsReadWeight',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.ModifyRdsReadWeightResponse(),
             self.call_api(params, req, runtime)
         )
 
     def modify_rds_read_weight(self, request):
         runtime = util_models.RuntimeOptions()
         return self.modify_rds_read_weight_with_options(request, runtime)
 
-    def pre_check_sql_flashback_task_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['EndTime'] = request.end_time
-        query['StartTime'] = request.start_time
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='PreCheckSqlFlashbackTask',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.PreCheckSqlFlashbackTaskResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def pre_check_sql_flashback_task(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.pre_check_sql_flashback_task_with_options(request, runtime)
-
-    def put_restore_pre_check_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['BackupDbNames'] = request.backup_db_names
-        query['BackupId'] = request.backup_id
-        query['BackupLevel'] = request.backup_level
-        query['BackupMode'] = request.backup_mode
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['PreferredBackupTime'] = request.preferred_backup_time
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='PutRestorePreCheck',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.PutRestorePreCheckResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def put_restore_pre_check(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.put_restore_pre_check_with_options(request, runtime)
-
     def put_start_backup_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['BackupDbNames'] = request.backup_db_names
-        query['BackupLevel'] = request.backup_level
-        query['BackupMode'] = request.backup_mode
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.backup_db_names):
+            query['BackupDbNames'] = request.backup_db_names
+        if not UtilClient.is_unset(request.backup_level):
+            query['BackupLevel'] = request.backup_level
+        if not UtilClient.is_unset(request.backup_mode):
+            query['BackupMode'] = request.backup_mode
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='PutStartBackup',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.PutStartBackupResponse(),
             self.call_api(params, req, runtime)
         )
 
     def put_start_backup(self, request):
         runtime = util_models.RuntimeOptions()
         return self.put_start_backup_with_options(request, runtime)
 
-    def rearrange_db_to_instance_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['ChooseRds'] = request.choose_rds
-        query['ChooseSubDb'] = request.choose_sub_db
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['InstanceList'] = request.instance_list
-        query['OrderId'] = request.order_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='RearrangeDbToInstance',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.RearrangeDbToInstanceResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def rearrange_db_to_instance(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.rearrange_db_to_instance_with_options(request, runtime)
-
     def refresh_drds_atom_url_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='RefreshDrdsAtomUrl',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.RefreshDrdsAtomUrlResponse(),
             self.call_api(params, req, runtime)
         )
 
     def refresh_drds_atom_url(self, request):
         runtime = util_models.RuntimeOptions()
         return self.refresh_drds_atom_url_with_options(request, runtime)
 
     def release_instance_internet_address_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ReleaseInstanceInternetAddress',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.ReleaseInstanceInternetAddressResponse(),
             self.call_api(params, req, runtime)
         )
 
     def release_instance_internet_address(self, request):
         runtime = util_models.RuntimeOptions()
         return self.release_instance_internet_address_with_options(request, runtime)
 
     def remove_backups_set_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['BackupId'] = request.backup_id
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.backup_id):
+            query['BackupId'] = request.backup_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='RemoveBackupsSet',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.RemoveBackupsSetResponse(),
             self.call_api(params, req, runtime)
         )
 
     def remove_backups_set(self, request):
         runtime = util_models.RuntimeOptions()
         return self.remove_backups_set_with_options(request, runtime)
 
     def remove_drds_db_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='RemoveDrdsDb',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.RemoveDrdsDbResponse(),
             self.call_api(params, req, runtime)
         )
 
     def remove_drds_db(self, request):
         runtime = util_models.RuntimeOptions()
         return self.remove_drds_db_with_options(request, runtime)
 
     def remove_drds_db_failed_record_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='RemoveDrdsDbFailedRecord',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.RemoveDrdsDbFailedRecordResponse(),
             self.call_api(params, req, runtime)
         )
 
     def remove_drds_db_failed_record(self, request):
         runtime = util_models.RuntimeOptions()
         return self.remove_drds_db_failed_record_with_options(request, runtime)
 
     def remove_drds_instance_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='RemoveDrdsInstance',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.RemoveDrdsInstanceResponse(),
             self.call_api(params, req, runtime)
         )
 
     def remove_drds_instance(self, request):
         runtime = util_models.RuntimeOptions()
         return self.remove_drds_instance_with_options(request, runtime)
 
-    def remove_drds_mysql_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['DbInstanceId'] = request.db_instance_id
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['Force'] = request.force
-        query['RoDbInstanceId'] = request.ro_db_instance_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='RemoveDrdsMysql',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.RemoveDrdsMysqlResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def remove_drds_mysql(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.remove_drds_mysql_with_options(request, runtime)
-
     def remove_instance_account_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['AccountName'] = request.account_name
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.account_name):
+            query['AccountName'] = request.account_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='RemoveInstanceAccount',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.RemoveInstanceAccountResponse(),
             self.call_api(params, req, runtime)
         )
 
     def remove_instance_account(self, request):
         runtime = util_models.RuntimeOptions()
         return self.remove_instance_account_with_options(request, runtime)
 
     def remove_recycle_bin_table_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RegionId'] = request.region_id
-        query['TableName'] = request.table_name
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.table_name):
+            query['TableName'] = request.table_name
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='RemoveRecycleBinTable',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.RemoveRecycleBinTableResponse(),
             self.call_api(params, req, runtime)
         )
 
     def remove_recycle_bin_table(self, request):
         runtime = util_models.RuntimeOptions()
         return self.remove_recycle_bin_table_with_options(request, runtime)
 
     def restart_drds_instance_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='RestartDrdsInstance',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.RestartDrdsInstanceResponse(),
             self.call_api(params, req, runtime)
         )
 
     def restart_drds_instance(self, request):
         runtime = util_models.RuntimeOptions()
         return self.restart_drds_instance_with_options(request, runtime)
 
     def rollback_instance_version_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='RollbackInstanceVersion',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.RollbackInstanceVersionResponse(),
             self.call_api(params, req, runtime)
         )
 
     def rollback_instance_version(self, request):
         runtime = util_models.RuntimeOptions()
         return self.rollback_instance_version_with_options(request, runtime)
 
     def set_backup_local_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['HighSpaceUsageProtection'] = request.high_space_usage_protection
-        query['LocalLogRetentionHours'] = request.local_log_retention_hours
-        query['LocalLogRetentionSpace'] = request.local_log_retention_space
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.high_space_usage_protection):
+            query['HighSpaceUsageProtection'] = request.high_space_usage_protection
+        if not UtilClient.is_unset(request.local_log_retention_hours):
+            query['LocalLogRetentionHours'] = request.local_log_retention_hours
+        if not UtilClient.is_unset(request.local_log_retention_space):
+            query['LocalLogRetentionSpace'] = request.local_log_retention_space
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SetBackupLocal',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.SetBackupLocalResponse(),
             self.call_api(params, req, runtime)
         )
 
     def set_backup_local(self, request):
         runtime = util_models.RuntimeOptions()
         return self.set_backup_local_with_options(request, runtime)
 
     def set_backup_policy_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['BackupDbNames'] = request.backup_db_names
-        query['BackupLevel'] = request.backup_level
-        query['BackupLog'] = request.backup_log
-        query['BackupMode'] = request.backup_mode
-        query['DataBackupRetentionPeriod'] = request.data_backup_retention_period
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['LogBackupRetentionPeriod'] = request.log_backup_retention_period
-        query['PreferredBackupEndTime'] = request.preferred_backup_end_time
-        query['PreferredBackupPeriod'] = request.preferred_backup_period
-        query['PreferredBackupStartTime'] = request.preferred_backup_start_time
+        if not UtilClient.is_unset(request.backup_db_names):
+            query['BackupDbNames'] = request.backup_db_names
+        if not UtilClient.is_unset(request.backup_level):
+            query['BackupLevel'] = request.backup_level
+        if not UtilClient.is_unset(request.backup_log):
+            query['BackupLog'] = request.backup_log
+        if not UtilClient.is_unset(request.backup_mode):
+            query['BackupMode'] = request.backup_mode
+        if not UtilClient.is_unset(request.data_backup_retention_period):
+            query['DataBackupRetentionPeriod'] = request.data_backup_retention_period
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.log_backup_retention_period):
+            query['LogBackupRetentionPeriod'] = request.log_backup_retention_period
+        if not UtilClient.is_unset(request.preferred_backup_end_time):
+            query['PreferredBackupEndTime'] = request.preferred_backup_end_time
+        if not UtilClient.is_unset(request.preferred_backup_period):
+            query['PreferredBackupPeriod'] = request.preferred_backup_period
+        if not UtilClient.is_unset(request.preferred_backup_start_time):
+            query['PreferredBackupStartTime'] = request.preferred_backup_start_time
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SetBackupPolicy',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.SetBackupPolicyResponse(),
             self.call_api(params, req, runtime)
         )
 
     def set_backup_policy(self, request):
         runtime = util_models.RuntimeOptions()
         return self.set_backup_policy_with_options(request, runtime)
 
     def setup_broadcast_tables_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['Active'] = request.active
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RegionId'] = request.region_id
-        query['TableName'] = request.table_name
+        if not UtilClient.is_unset(request.active):
+            query['Active'] = request.active
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.table_name):
+            query['TableName'] = request.table_name
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SetupBroadcastTables',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.SetupBroadcastTablesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def setup_broadcast_tables(self, request):
         runtime = util_models.RuntimeOptions()
         return self.setup_broadcast_tables_with_options(request, runtime)
 
     def setup_drds_params_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['Data'] = request.data
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['ParamLevel'] = request.param_level
-        query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.data):
+            query['Data'] = request.data
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.param_level):
+            query['ParamLevel'] = request.param_level
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SetupDrdsParams',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.SetupDrdsParamsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def setup_drds_params(self, request):
         runtime = util_models.RuntimeOptions()
         return self.setup_drds_params_with_options(request, runtime)
 
     def setup_recycle_bin_status_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RegionId'] = request.region_id
-        query['StatusAction'] = request.status_action
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.status_action):
+            query['StatusAction'] = request.status_action
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SetupRecycleBinStatus',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.SetupRecycleBinStatusResponse(),
             self.call_api(params, req, runtime)
         )
 
     def setup_recycle_bin_status(self, request):
         runtime = util_models.RuntimeOptions()
         return self.setup_recycle_bin_status_with_options(request, runtime)
 
     def setup_table_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['AllowFullTableScan'] = request.allow_full_table_scan
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RegionId'] = request.region_id
-        query['TableName'] = request.table_name
+        if not UtilClient.is_unset(request.allow_full_table_scan):
+            query['AllowFullTableScan'] = request.allow_full_table_scan
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.table_name):
+            query['TableName'] = request.table_name
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SetupTable',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.SetupTableResponse(),
             self.call_api(params, req, runtime)
         )
 
     def setup_table(self, request):
         runtime = util_models.RuntimeOptions()
         return self.setup_table_with_options(request, runtime)
 
-    def setup_table_async_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['AllowFullTableScan'] = request.allow_full_table_scan
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RegionId'] = request.region_id
-        query['TableName'] = request.table_name
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='SetupTableAsync',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.SetupTableAsyncResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def setup_table_async(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.setup_table_async_with_options(request, runtime)
-
-    def sql_compatibility_cancel_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['TaskId'] = request.task_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='SqlCompatibilityCancel',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.SqlCompatibilityCancelResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def sql_compatibility_cancel(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.sql_compatibility_cancel_with_options(request, runtime)
-
-    def sql_compatibility_start_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['PerformanceTest'] = request.performance_test
-        query['TargetVersion'] = request.target_version
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='SqlCompatibilityStart',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.SqlCompatibilityStartResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def sql_compatibility_start(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.sql_compatibility_start_with_options(request, runtime)
-
     def start_restore_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['BackupDbNames'] = request.backup_db_names
-        query['BackupId'] = request.backup_id
-        query['BackupLevel'] = request.backup_level
-        query['BackupMode'] = request.backup_mode
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['PreferredBackupTime'] = request.preferred_backup_time
+        if not UtilClient.is_unset(request.backup_db_names):
+            query['BackupDbNames'] = request.backup_db_names
+        if not UtilClient.is_unset(request.backup_id):
+            query['BackupId'] = request.backup_id
+        if not UtilClient.is_unset(request.backup_level):
+            query['BackupLevel'] = request.backup_level
+        if not UtilClient.is_unset(request.backup_mode):
+            query['BackupMode'] = request.backup_mode
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.preferred_backup_time):
+            query['PreferredBackupTime'] = request.preferred_backup_time
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='StartRestore',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.StartRestoreResponse(),
             self.call_api(params, req, runtime)
         )
 
     def start_restore(self, request):
         runtime = util_models.RuntimeOptions()
         return self.start_restore_with_options(request, runtime)
 
     def submit_clean_task_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['ExpandType'] = request.expand_type
-        query['JobId'] = request.job_id
-        query['ParentJobId'] = request.parent_job_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.expand_type):
+            query['ExpandType'] = request.expand_type
+        if not UtilClient.is_unset(request.job_id):
+            query['JobId'] = request.job_id
+        if not UtilClient.is_unset(request.parent_job_id):
+            query['ParentJobId'] = request.parent_job_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SubmitCleanTask',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.SubmitCleanTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
     def submit_clean_task(self, request):
         runtime = util_models.RuntimeOptions()
         return self.submit_clean_task_with_options(request, runtime)
 
     def submit_hot_expand_pre_check_task_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbInstType'] = request.db_inst_type
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['TableList'] = request.table_list
+        if not UtilClient.is_unset(request.db_inst_type):
+            query['DbInstType'] = request.db_inst_type
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.table_list):
+            query['TableList'] = request.table_list
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SubmitHotExpandPreCheckTask',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.SubmitHotExpandPreCheckTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
     def submit_hot_expand_pre_check_task(self, request):
         runtime = util_models.RuntimeOptions()
         return self.submit_hot_expand_pre_check_task_with_options(request, runtime)
 
     def submit_hot_expand_task_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['ExtendedMapping'] = request.extended_mapping
-        query['InstanceDbMapping'] = request.instance_db_mapping
-        query['Mapping'] = request.mapping
-        query['SupperAccountMapping'] = request.supper_account_mapping
-        query['TaskDesc'] = request.task_desc
-        query['TaskName'] = request.task_name
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.extended_mapping):
+            query['ExtendedMapping'] = request.extended_mapping
+        if not UtilClient.is_unset(request.instance_db_mapping):
+            query['InstanceDbMapping'] = request.instance_db_mapping
+        if not UtilClient.is_unset(request.mapping):
+            query['Mapping'] = request.mapping
+        if not UtilClient.is_unset(request.supper_account_mapping):
+            query['SupperAccountMapping'] = request.supper_account_mapping
+        if not UtilClient.is_unset(request.task_desc):
+            query['TaskDesc'] = request.task_desc
+        if not UtilClient.is_unset(request.task_name):
+            query['TaskName'] = request.task_name
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SubmitHotExpandTask',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.SubmitHotExpandTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
     def submit_hot_expand_task(self, request):
         runtime = util_models.RuntimeOptions()
         return self.submit_hot_expand_task_with_options(request, runtime)
 
     def submit_smooth_expand_pre_check_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbInstType'] = request.db_inst_type
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.db_inst_type):
+            query['DbInstType'] = request.db_inst_type
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SubmitSmoothExpandPreCheck',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.SubmitSmoothExpandPreCheckResponse(),
             self.call_api(params, req, runtime)
         )
 
     def submit_smooth_expand_pre_check(self, request):
         runtime = util_models.RuntimeOptions()
         return self.submit_smooth_expand_pre_check_with_options(request, runtime)
 
     def submit_smooth_expand_pre_check_task_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SubmitSmoothExpandPreCheckTask',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.SubmitSmoothExpandPreCheckTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
     def submit_smooth_expand_pre_check_task(self, request):
         runtime = util_models.RuntimeOptions()
         return self.submit_smooth_expand_pre_check_task_with_options(request, runtime)
 
     def submit_sql_flashback_task_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['EndTime'] = request.end_time
-        query['RecallRestoreType'] = request.recall_restore_type
-        query['RecallType'] = request.recall_type
-        query['SqlPk'] = request.sql_pk
-        query['SqlType'] = request.sql_type
-        query['StartTime'] = request.start_time
-        query['TableName'] = request.table_name
-        query['TraceId'] = request.trace_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.recall_restore_type):
+            query['RecallRestoreType'] = request.recall_restore_type
+        if not UtilClient.is_unset(request.recall_type):
+            query['RecallType'] = request.recall_type
+        if not UtilClient.is_unset(request.sql_pk):
+            query['SqlPk'] = request.sql_pk
+        if not UtilClient.is_unset(request.sql_type):
+            query['SqlType'] = request.sql_type
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        if not UtilClient.is_unset(request.table_name):
+            query['TableName'] = request.table_name
+        if not UtilClient.is_unset(request.trace_id):
+            query['TraceId'] = request.trace_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SubmitSqlFlashbackTask',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.SubmitSqlFlashbackTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
     def submit_sql_flashback_task(self, request):
         runtime = util_models.RuntimeOptions()
         return self.submit_sql_flashback_task_with_options(request, runtime)
 
     def switch_global_broadcast_type_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SwitchGlobalBroadcastType',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.SwitchGlobalBroadcastTypeResponse(),
             self.call_api(params, req, runtime)
         )
 
     def switch_global_broadcast_type(self, request):
         runtime = util_models.RuntimeOptions()
         return self.switch_global_broadcast_type_with_options(request, runtime)
 
     def tag_resources_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['RegionId'] = request.region_id
-        query['ResourceId'] = request.resource_id
-        query['ResourceType'] = request.resource_type
-        query['Tag'] = request.tag
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_id):
+            query['ResourceId'] = request.resource_id
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='TagResources',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.TagResourcesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def tag_resources(self, request):
         runtime = util_models.RuntimeOptions()
         return self.tag_resources_with_options(request, runtime)
 
     def untag_resources_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['All'] = request.all
-        query['RegionId'] = request.region_id
-        query['ResourceId'] = request.resource_id
-        query['ResourceType'] = request.resource_type
-        query['TagKey'] = request.tag_key
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
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='UntagResources',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.UntagResourcesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def untag_resources(self, request):
         runtime = util_models.RuntimeOptions()
         return self.untag_resources_with_options(request, runtime)
 
     def update_instance_network_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['ClassicExpiredDays'] = request.classic_expired_days
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RetainClassic'] = request.retain_classic
-        query['SrcInstanceNetworkType'] = request.src_instance_network_type
+        if not UtilClient.is_unset(request.classic_expired_days):
+            query['ClassicExpiredDays'] = request.classic_expired_days
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.retain_classic):
+            query['RetainClassic'] = request.retain_classic
+        if not UtilClient.is_unset(request.src_instance_network_type):
+            query['SrcInstanceNetworkType'] = request.src_instance_network_type
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='UpdateInstanceNetwork',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.UpdateInstanceNetworkResponse(),
             self.call_api(params, req, runtime)
         )
 
     def update_instance_network(self, request):
         runtime = util_models.RuntimeOptions()
         return self.update_instance_network_with_options(request, runtime)
 
     def update_private_rds_class_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['AutoUseCoupon'] = request.auto_use_coupon
-        query['DBInstanceId'] = request.dbinstance_id
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['PrePayDuration'] = request.pre_pay_duration
-        query['RdsClass'] = request.rds_class
-        query['Storage'] = request.storage
+        if not UtilClient.is_unset(request.auto_use_coupon):
+            query['AutoUseCoupon'] = request.auto_use_coupon
+        if not UtilClient.is_unset(request.dbinstance_id):
+            query['DBInstanceId'] = request.dbinstance_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.pre_pay_duration):
+            query['PrePayDuration'] = request.pre_pay_duration
+        if not UtilClient.is_unset(request.rds_class):
+            query['RdsClass'] = request.rds_class
+        if not UtilClient.is_unset(request.storage):
+            query['Storage'] = request.storage
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='UpdatePrivateRdsClass',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.UpdatePrivateRdsClassResponse(),
             self.call_api(params, req, runtime)
         )
 
     def update_private_rds_class(self, request):
         runtime = util_models.RuntimeOptions()
         return self.update_private_rds_class_with_options(request, runtime)
 
     def update_resource_group_attribute_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['NewResourceGroupId'] = request.new_resource_group_id
-        query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.new_resource_group_id):
+            query['NewResourceGroupId'] = request.new_resource_group_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='UpdateResourceGroupAttribute',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.UpdateResourceGroupAttributeResponse(),
             self.call_api(params, req, runtime)
         )
 
     def update_resource_group_attribute(self, request):
         runtime = util_models.RuntimeOptions()
         return self.update_resource_group_attribute_with_options(request, runtime)
 
     def upgrade_hi_store_instance_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['HistoreInstanceId'] = request.histore_instance_id
-        query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.histore_instance_id):
+            query['HistoreInstanceId'] = request.histore_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='UpgradeHiStoreInstance',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.UpgradeHiStoreInstanceResponse(),
             self.call_api(params, req, runtime)
         )
 
     def upgrade_hi_store_instance(self, request):
         runtime = util_models.RuntimeOptions()
         return self.upgrade_hi_store_instance_with_options(request, runtime)
 
     def upgrade_instance_version_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RegionId'] = request.region_id
-        query['Rpm'] = request.rpm
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.rpm):
+            query['Rpm'] = request.rpm
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='UpgradeInstanceVersion',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.UpgradeInstanceVersionResponse(),
             self.call_api(params, req, runtime)
         )
 
     def upgrade_instance_version(self, request):
         runtime = util_models.RuntimeOptions()
         return self.upgrade_instance_version_with_options(request, runtime)
 
     def validate_shard_task_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
-        query['DbName'] = request.db_name
-        query['DrdsInstanceId'] = request.drds_instance_id
-        query['RegionId'] = request.region_id
-        query['SourceTableName'] = request.source_table_name
-        query['TargetTableName'] = request.target_table_name
-        query['TaskType'] = request.task_type
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.drds_instance_id):
+            query['DrdsInstanceId'] = request.drds_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.source_table_name):
+            query['SourceTableName'] = request.source_table_name
+        if not UtilClient.is_unset(request.target_table_name):
+            query['TargetTableName'] = request.target_table_name
+        if not UtilClient.is_unset(request.task_type):
+            query['TaskType'] = request.task_type
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ValidateShardTask',
             version='2019-01-23',
             protocol='HTTPS',
             pathname='/',
             method='POST',
             auth_type='AK',
             style='RPC',
-            req_body_type='json',
+            req_body_type='formData',
             body_type='json'
         )
         return TeaCore.from_map(
             drds_20190123_models.ValidateShardTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
     def validate_shard_task(self, request):
         runtime = util_models.RuntimeOptions()
         return self.validate_shard_task_with_options(request, runtime)
-
-    def describe_rds_inst_infos_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        query['PageNumber'] = request.page_number
-        query['PageSize'] = request.page_size
-        query['Search'] = request.search
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query),
-            body=UtilClient.to_map(request)
-        )
-        params = open_api_models.Params(
-            action='describeRdsInstInfos',
-            version='2019-01-23',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='json',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            drds_20190123_models.DescribeRdsInstInfosResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def describe_rds_inst_infos(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.describe_rds_inst_infos_with_options(request, runtime)
```

### Comparing `alibabacloud_drds20190123_py2-1.0.8/alibabacloud_drds20190123/models.py` & `alibabacloud_drds20190123_py2-1.0.9/alibabacloud_drds20190123/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -196,126 +196,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = ChangeInstanceAzoneResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ChangeInstanceNetworkRequest(TeaModel):
-    def __init__(self, classic_expired_days=None, drds_instance_id=None, retain_classic=None,
-                 src_instance_network_type=None, vpc_id=None, vswitch_id=None):
-        self.classic_expired_days = classic_expired_days  # type: int
-        self.drds_instance_id = drds_instance_id  # type: str
-        self.retain_classic = retain_classic  # type: bool
-        self.src_instance_network_type = src_instance_network_type  # type: str
-        self.vpc_id = vpc_id  # type: str
-        self.vswitch_id = vswitch_id  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ChangeInstanceNetworkRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.classic_expired_days is not None:
-            result['ClassicExpiredDays'] = self.classic_expired_days
-        if self.drds_instance_id is not None:
-            result['DrdsInstanceId'] = self.drds_instance_id
-        if self.retain_classic is not None:
-            result['RetainClassic'] = self.retain_classic
-        if self.src_instance_network_type is not None:
-            result['SrcInstanceNetworkType'] = self.src_instance_network_type
-        if self.vpc_id is not None:
-            result['VpcId'] = self.vpc_id
-        if self.vswitch_id is not None:
-            result['VswitchId'] = self.vswitch_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('ClassicExpiredDays') is not None:
-            self.classic_expired_days = m.get('ClassicExpiredDays')
-        if m.get('DrdsInstanceId') is not None:
-            self.drds_instance_id = m.get('DrdsInstanceId')
-        if m.get('RetainClassic') is not None:
-            self.retain_classic = m.get('RetainClassic')
-        if m.get('SrcInstanceNetworkType') is not None:
-            self.src_instance_network_type = m.get('SrcInstanceNetworkType')
-        if m.get('VpcId') is not None:
-            self.vpc_id = m.get('VpcId')
-        if m.get('VswitchId') is not None:
-            self.vswitch_id = m.get('VswitchId')
-        return self
-
-
-class ChangeInstanceNetworkResponseBody(TeaModel):
-    def __init__(self, request_id=None, success=None):
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ChangeInstanceNetworkResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class ChangeInstanceNetworkResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: ChangeInstanceNetworkResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(ChangeInstanceNetworkResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = ChangeInstanceNetworkResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class CheckDrdsDbNameRequest(TeaModel):
     def __init__(self, db_name=None, drds_instance_id=None):
         self.db_name = db_name  # type: str
         self.drds_instance_id = drds_instance_id  # type: str
 
     def validate(self):
         pass
@@ -531,115 +419,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = CheckExpandStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class CheckRdsSuperAccountRequest(TeaModel):
-    def __init__(self, account_name=None, db_instance_id=None, drds_instance_id=None, password=None):
-        self.account_name = account_name  # type: str
-        self.db_instance_id = db_instance_id  # type: str
-        self.drds_instance_id = drds_instance_id  # type: str
-        self.password = password  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(CheckRdsSuperAccountRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.account_name is not None:
-            result['AccountName'] = self.account_name
-        if self.db_instance_id is not None:
-            result['DbInstanceId'] = self.db_instance_id
-        if self.drds_instance_id is not None:
-            result['DrdsInstanceId'] = self.drds_instance_id
-        if self.password is not None:
-            result['Password'] = self.password
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('AccountName') is not None:
-            self.account_name = m.get('AccountName')
-        if m.get('DbInstanceId') is not None:
-            self.db_instance_id = m.get('DbInstanceId')
-        if m.get('DrdsInstanceId') is not None:
-            self.drds_instance_id = m.get('DrdsInstanceId')
-        if m.get('Password') is not None:
-            self.password = m.get('Password')
-        return self
-
-
-class CheckRdsSuperAccountResponseBody(TeaModel):
-    def __init__(self, request_id=None, success=None):
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(CheckRdsSuperAccountResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class CheckRdsSuperAccountResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: CheckRdsSuperAccountResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(CheckRdsSuperAccountResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = CheckRdsSuperAccountResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class CheckSqlAuditEnableStatusRequest(TeaModel):
     def __init__(self, db_name=None, drds_instance_id=None):
         self.db_name = db_name  # type: str
         self.drds_instance_id = drds_instance_id  # type: str
 
     def validate(self):
         pass
@@ -728,152 +515,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = CheckSqlAuditEnableStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ConfigureDrdsDbInstancesRequestDbInstance(TeaModel):
-    def __init__(self, master_db_instance_id=None, slave_db_instance_id=None, slave_db_instance_type=None):
-        self.master_db_instance_id = master_db_instance_id  # type: str
-        self.slave_db_instance_id = slave_db_instance_id  # type: str
-        self.slave_db_instance_type = slave_db_instance_type  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ConfigureDrdsDbInstancesRequestDbInstance, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.master_db_instance_id is not None:
-            result['MasterDbInstanceId'] = self.master_db_instance_id
-        if self.slave_db_instance_id is not None:
-            result['SlaveDbInstanceId'] = self.slave_db_instance_id
-        if self.slave_db_instance_type is not None:
-            result['SlaveDbInstanceType'] = self.slave_db_instance_type
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('MasterDbInstanceId') is not None:
-            self.master_db_instance_id = m.get('MasterDbInstanceId')
-        if m.get('SlaveDbInstanceId') is not None:
-            self.slave_db_instance_id = m.get('SlaveDbInstanceId')
-        if m.get('SlaveDbInstanceType') is not None:
-            self.slave_db_instance_type = m.get('SlaveDbInstanceType')
-        return self
-
-
-class ConfigureDrdsDbInstancesRequest(TeaModel):
-    def __init__(self, db_instance=None, db_name=None, drds_instance_id=None):
-        self.db_instance = db_instance  # type: list[ConfigureDrdsDbInstancesRequestDbInstance]
-        self.db_name = db_name  # type: str
-        self.drds_instance_id = drds_instance_id  # type: str
-
-    def validate(self):
-        if self.db_instance:
-            for k in self.db_instance:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super(ConfigureDrdsDbInstancesRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        result['DbInstance'] = []
-        if self.db_instance is not None:
-            for k in self.db_instance:
-                result['DbInstance'].append(k.to_map() if k else None)
-        if self.db_name is not None:
-            result['DbName'] = self.db_name
-        if self.drds_instance_id is not None:
-            result['DrdsInstanceId'] = self.drds_instance_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        self.db_instance = []
-        if m.get('DbInstance') is not None:
-            for k in m.get('DbInstance'):
-                temp_model = ConfigureDrdsDbInstancesRequestDbInstance()
-                self.db_instance.append(temp_model.from_map(k))
-        if m.get('DbName') is not None:
-            self.db_name = m.get('DbName')
-        if m.get('DrdsInstanceId') is not None:
-            self.drds_instance_id = m.get('DrdsInstanceId')
-        return self
-
-
-class ConfigureDrdsDbInstancesResponseBody(TeaModel):
-    def __init__(self, request_id=None, success=None):
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ConfigureDrdsDbInstancesResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class ConfigureDrdsDbInstancesResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: ConfigureDrdsDbInstancesResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(ConfigureDrdsDbInstancesResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = ConfigureDrdsDbInstancesResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class CreateDrdsDBRequestInstDbName(TeaModel):
     def __init__(self, db_instance_id=None, shard_db_name=None):
         self.db_instance_id = db_instance_id  # type: str
         self.shard_db_name = shard_db_name  # type: list[str]
 
     def validate(self):
         pass
@@ -1084,495 +733,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = CreateDrdsDBResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class CreateDrdsDBPreCheckRequestInstDbName(TeaModel):
-    def __init__(self, db_instance_id=None, shard_db_name=None):
-        self.db_instance_id = db_instance_id  # type: str
-        self.shard_db_name = shard_db_name  # type: list[str]
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(CreateDrdsDBPreCheckRequestInstDbName, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.db_instance_id is not None:
-            result['DbInstanceId'] = self.db_instance_id
-        if self.shard_db_name is not None:
-            result['ShardDbName'] = self.shard_db_name
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DbInstanceId') is not None:
-            self.db_instance_id = m.get('DbInstanceId')
-        if m.get('ShardDbName') is not None:
-            self.shard_db_name = m.get('ShardDbName')
-        return self
-
-
-class CreateDrdsDBPreCheckRequestRdsSuperAccount(TeaModel):
-    def __init__(self, account_name=None, db_instance_id=None, password=None):
-        self.account_name = account_name  # type: str
-        self.db_instance_id = db_instance_id  # type: str
-        self.password = password  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(CreateDrdsDBPreCheckRequestRdsSuperAccount, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.account_name is not None:
-            result['AccountName'] = self.account_name
-        if self.db_instance_id is not None:
-            result['DbInstanceId'] = self.db_instance_id
-        if self.password is not None:
-            result['Password'] = self.password
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('AccountName') is not None:
-            self.account_name = m.get('AccountName')
-        if m.get('DbInstanceId') is not None:
-            self.db_instance_id = m.get('DbInstanceId')
-        if m.get('Password') is not None:
-            self.password = m.get('Password')
-        return self
-
-
-class CreateDrdsDBPreCheckRequest(TeaModel):
-    def __init__(self, account_name=None, db_inst_type=None, db_instance_is_creating=None, db_name=None,
-                 drds_instance_id=None, encode=None, inst_db_name=None, password=None, rds_instance=None, rds_super_account=None,
-                 type=None):
-        self.account_name = account_name  # type: str
-        self.db_inst_type = db_inst_type  # type: str
-        self.db_instance_is_creating = db_instance_is_creating  # type: bool
-        self.db_name = db_name  # type: str
-        self.drds_instance_id = drds_instance_id  # type: str
-        self.encode = encode  # type: str
-        self.inst_db_name = inst_db_name  # type: list[CreateDrdsDBPreCheckRequestInstDbName]
-        self.password = password  # type: str
-        self.rds_instance = rds_instance  # type: list[str]
-        self.rds_super_account = rds_super_account  # type: list[CreateDrdsDBPreCheckRequestRdsSuperAccount]
-        self.type = type  # type: str
-
-    def validate(self):
-        if self.inst_db_name:
-            for k in self.inst_db_name:
-                if k:
-                    k.validate()
-        if self.rds_super_account:
-            for k in self.rds_super_account:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super(CreateDrdsDBPreCheckRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.account_name is not None:
-            result['AccountName'] = self.account_name
-        if self.db_inst_type is not None:
-            result['DbInstType'] = self.db_inst_type
-        if self.db_instance_is_creating is not None:
-            result['DbInstanceIsCreating'] = self.db_instance_is_creating
-        if self.db_name is not None:
-            result['DbName'] = self.db_name
-        if self.drds_instance_id is not None:
-            result['DrdsInstanceId'] = self.drds_instance_id
-        if self.encode is not None:
-            result['Encode'] = self.encode
-        result['InstDbName'] = []
-        if self.inst_db_name is not None:
-            for k in self.inst_db_name:
-                result['InstDbName'].append(k.to_map() if k else None)
-        if self.password is not None:
-            result['Password'] = self.password
-        if self.rds_instance is not None:
-            result['RdsInstance'] = self.rds_instance
-        result['RdsSuperAccount'] = []
-        if self.rds_super_account is not None:
-            for k in self.rds_super_account:
-                result['RdsSuperAccount'].append(k.to_map() if k else None)
-        if self.type is not None:
-            result['Type'] = self.type
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('AccountName') is not None:
-            self.account_name = m.get('AccountName')
-        if m.get('DbInstType') is not None:
-            self.db_inst_type = m.get('DbInstType')
-        if m.get('DbInstanceIsCreating') is not None:
-            self.db_instance_is_creating = m.get('DbInstanceIsCreating')
-        if m.get('DbName') is not None:
-            self.db_name = m.get('DbName')
-        if m.get('DrdsInstanceId') is not None:
-            self.drds_instance_id = m.get('DrdsInstanceId')
-        if m.get('Encode') is not None:
-            self.encode = m.get('Encode')
-        self.inst_db_name = []
-        if m.get('InstDbName') is not None:
-            for k in m.get('InstDbName'):
-                temp_model = CreateDrdsDBPreCheckRequestInstDbName()
-                self.inst_db_name.append(temp_model.from_map(k))
-        if m.get('Password') is not None:
-            self.password = m.get('Password')
-        if m.get('RdsInstance') is not None:
-            self.rds_instance = m.get('RdsInstance')
-        self.rds_super_account = []
-        if m.get('RdsSuperAccount') is not None:
-            for k in m.get('RdsSuperAccount'):
-                temp_model = CreateDrdsDBPreCheckRequestRdsSuperAccount()
-                self.rds_super_account.append(temp_model.from_map(k))
-        if m.get('Type') is not None:
-            self.type = m.get('Type')
-        return self
-
-
-class CreateDrdsDBPreCheckResponseBody(TeaModel):
-    def __init__(self, request_id=None, success=None, task_id=None):
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-        self.task_id = task_id  # type: long
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(CreateDrdsDBPreCheckResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        if self.task_id is not None:
-            result['TaskId'] = self.task_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        if m.get('TaskId') is not None:
-            self.task_id = m.get('TaskId')
-        return self
-
-
-class CreateDrdsDBPreCheckResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: CreateDrdsDBPreCheckResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(CreateDrdsDBPreCheckResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = CreateDrdsDBPreCheckResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
-class CreateDrdsDBPreviewRequestInstDbName(TeaModel):
-    def __init__(self, db_instance_id=None, shard_db_name=None):
-        self.db_instance_id = db_instance_id  # type: str
-        self.shard_db_name = shard_db_name  # type: list[str]
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(CreateDrdsDBPreviewRequestInstDbName, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.db_instance_id is not None:
-            result['DbInstanceId'] = self.db_instance_id
-        if self.shard_db_name is not None:
-            result['ShardDbName'] = self.shard_db_name
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DbInstanceId') is not None:
-            self.db_instance_id = m.get('DbInstanceId')
-        if m.get('ShardDbName') is not None:
-            self.shard_db_name = m.get('ShardDbName')
-        return self
-
-
-class CreateDrdsDBPreviewRequest(TeaModel):
-    def __init__(self, account_name=None, db_inst_type=None, db_instance_is_creating=None, db_name=None,
-                 drds_instance_id=None, inst_db_name=None, order_id=None, rds_instance=None, type=None):
-        self.account_name = account_name  # type: str
-        self.db_inst_type = db_inst_type  # type: str
-        self.db_instance_is_creating = db_instance_is_creating  # type: bool
-        self.db_name = db_name  # type: str
-        self.drds_instance_id = drds_instance_id  # type: str
-        self.inst_db_name = inst_db_name  # type: list[CreateDrdsDBPreviewRequestInstDbName]
-        self.order_id = order_id  # type: str
-        self.rds_instance = rds_instance  # type: list[str]
-        self.type = type  # type: str
-
-    def validate(self):
-        if self.inst_db_name:
-            for k in self.inst_db_name:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super(CreateDrdsDBPreviewRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.account_name is not None:
-            result['AccountName'] = self.account_name
-        if self.db_inst_type is not None:
-            result['DbInstType'] = self.db_inst_type
-        if self.db_instance_is_creating is not None:
-            result['DbInstanceIsCreating'] = self.db_instance_is_creating
-        if self.db_name is not None:
-            result['DbName'] = self.db_name
-        if self.drds_instance_id is not None:
-            result['DrdsInstanceId'] = self.drds_instance_id
-        result['InstDbName'] = []
-        if self.inst_db_name is not None:
-            for k in self.inst_db_name:
-                result['InstDbName'].append(k.to_map() if k else None)
-        if self.order_id is not None:
-            result['OrderId'] = self.order_id
-        if self.rds_instance is not None:
-            result['RdsInstance'] = self.rds_instance
-        if self.type is not None:
-            result['Type'] = self.type
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('AccountName') is not None:
-            self.account_name = m.get('AccountName')
-        if m.get('DbInstType') is not None:
-            self.db_inst_type = m.get('DbInstType')
-        if m.get('DbInstanceIsCreating') is not None:
-            self.db_instance_is_creating = m.get('DbInstanceIsCreating')
-        if m.get('DbName') is not None:
-            self.db_name = m.get('DbName')
-        if m.get('DrdsInstanceId') is not None:
-            self.drds_instance_id = m.get('DrdsInstanceId')
-        self.inst_db_name = []
-        if m.get('InstDbName') is not None:
-            for k in m.get('InstDbName'):
-                temp_model = CreateDrdsDBPreviewRequestInstDbName()
-                self.inst_db_name.append(temp_model.from_map(k))
-        if m.get('OrderId') is not None:
-            self.order_id = m.get('OrderId')
-        if m.get('RdsInstance') is not None:
-            self.rds_instance = m.get('RdsInstance')
-        if m.get('Type') is not None:
-            self.type = m.get('Type')
-        return self
-
-
-class CreateDrdsDBPreviewResponseBodyItemsItemDbNames(TeaModel):
-    def __init__(self, db_name=None):
-        self.db_name = db_name  # type: list[str]
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(CreateDrdsDBPreviewResponseBodyItemsItemDbNames, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.db_name is not None:
-            result['DbName'] = self.db_name
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DbName') is not None:
-            self.db_name = m.get('DbName')
-        return self
-
-
-class CreateDrdsDBPreviewResponseBodyItemsItem(TeaModel):
-    def __init__(self, db_instance_id=None, db_names=None):
-        self.db_instance_id = db_instance_id  # type: str
-        self.db_names = db_names  # type: CreateDrdsDBPreviewResponseBodyItemsItemDbNames
-
-    def validate(self):
-        if self.db_names:
-            self.db_names.validate()
-
-    def to_map(self):
-        _map = super(CreateDrdsDBPreviewResponseBodyItemsItem, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.db_instance_id is not None:
-            result['DbInstanceId'] = self.db_instance_id
-        if self.db_names is not None:
-            result['DbNames'] = self.db_names.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DbInstanceId') is not None:
-            self.db_instance_id = m.get('DbInstanceId')
-        if m.get('DbNames') is not None:
-            temp_model = CreateDrdsDBPreviewResponseBodyItemsItemDbNames()
-            self.db_names = temp_model.from_map(m['DbNames'])
-        return self
-
-
-class CreateDrdsDBPreviewResponseBodyItems(TeaModel):
-    def __init__(self, item=None):
-        self.item = item  # type: list[CreateDrdsDBPreviewResponseBodyItemsItem]
-
-    def validate(self):
-        if self.item:
-            for k in self.item:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super(CreateDrdsDBPreviewResponseBodyItems, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        result['Item'] = []
-        if self.item is not None:
-            for k in self.item:
-                result['Item'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        self.item = []
-        if m.get('Item') is not None:
-            for k in m.get('Item'):
-                temp_model = CreateDrdsDBPreviewResponseBodyItemsItem()
-                self.item.append(temp_model.from_map(k))
-        return self
-
-
-class CreateDrdsDBPreviewResponseBody(TeaModel):
-    def __init__(self, items=None, request_id=None, success=None):
-        self.items = items  # type: CreateDrdsDBPreviewResponseBodyItems
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-
-    def validate(self):
-        if self.items:
-            self.items.validate()
-
-    def to_map(self):
-        _map = super(CreateDrdsDBPreviewResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.items is not None:
-            result['Items'] = self.items.to_map()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Items') is not None:
-            temp_model = CreateDrdsDBPreviewResponseBodyItems()
-            self.items = temp_model.from_map(m['Items'])
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class CreateDrdsDBPreviewResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: CreateDrdsDBPreviewResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(CreateDrdsDBPreviewResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = CreateDrdsDBPreviewResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class CreateDrdsInstanceRequest(TeaModel):
     def __init__(self, client_token=None, description=None, duration=None, instance_series=None, is_auto_renew=None,
                  master_inst_id=None, my_sqlversion=None, pay_type=None, pricing_cycle=None, quantity=None, region_id=None,
                  resource_group_id=None, specification=None, type=None, vpc_id=None, vswitch_id=None, zone_id=None, is_ha=None):
         self.client_token = client_token  # type: str
         self.description = description  # type: str
         self.duration = duration  # type: int
@@ -1800,178 +968,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = CreateDrdsInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class CreateEvaluatePreCheckTaskRequestDbInfo(TeaModel):
-    def __init__(self, db_name=None, db_password=None, db_port=None, db_user=None, inst_id=None):
-        self.db_name = db_name  # type: str
-        self.db_password = db_password  # type: str
-        self.db_port = db_port  # type: str
-        self.db_user = db_user  # type: str
-        self.inst_id = inst_id  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(CreateEvaluatePreCheckTaskRequestDbInfo, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.db_name is not None:
-            result['DbName'] = self.db_name
-        if self.db_password is not None:
-            result['DbPassword'] = self.db_password
-        if self.db_port is not None:
-            result['DbPort'] = self.db_port
-        if self.db_user is not None:
-            result['DbUser'] = self.db_user
-        if self.inst_id is not None:
-            result['InstId'] = self.inst_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DbName') is not None:
-            self.db_name = m.get('DbName')
-        if m.get('DbPassword') is not None:
-            self.db_password = m.get('DbPassword')
-        if m.get('DbPort') is not None:
-            self.db_port = m.get('DbPort')
-        if m.get('DbUser') is not None:
-            self.db_user = m.get('DbUser')
-        if m.get('InstId') is not None:
-            self.inst_id = m.get('InstId')
-        return self
-
-
-class CreateEvaluatePreCheckTaskRequest(TeaModel):
-    def __init__(self, avg_qps_growth_scale=None, data_growth_scale=None, db_info=None, evaluate_hours=None,
-                 task_name=None):
-        self.avg_qps_growth_scale = avg_qps_growth_scale  # type: int
-        self.data_growth_scale = data_growth_scale  # type: int
-        self.db_info = db_info  # type: list[CreateEvaluatePreCheckTaskRequestDbInfo]
-        self.evaluate_hours = evaluate_hours  # type: int
-        self.task_name = task_name  # type: str
-
-    def validate(self):
-        if self.db_info:
-            for k in self.db_info:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super(CreateEvaluatePreCheckTaskRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.avg_qps_growth_scale is not None:
-            result['AvgQpsGrowthScale'] = self.avg_qps_growth_scale
-        if self.data_growth_scale is not None:
-            result['DataGrowthScale'] = self.data_growth_scale
-        result['DbInfo'] = []
-        if self.db_info is not None:
-            for k in self.db_info:
-                result['DbInfo'].append(k.to_map() if k else None)
-        if self.evaluate_hours is not None:
-            result['EvaluateHours'] = self.evaluate_hours
-        if self.task_name is not None:
-            result['TaskName'] = self.task_name
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('AvgQpsGrowthScale') is not None:
-            self.avg_qps_growth_scale = m.get('AvgQpsGrowthScale')
-        if m.get('DataGrowthScale') is not None:
-            self.data_growth_scale = m.get('DataGrowthScale')
-        self.db_info = []
-        if m.get('DbInfo') is not None:
-            for k in m.get('DbInfo'):
-                temp_model = CreateEvaluatePreCheckTaskRequestDbInfo()
-                self.db_info.append(temp_model.from_map(k))
-        if m.get('EvaluateHours') is not None:
-            self.evaluate_hours = m.get('EvaluateHours')
-        if m.get('TaskName') is not None:
-            self.task_name = m.get('TaskName')
-        return self
-
-
-class CreateEvaluatePreCheckTaskResponseBody(TeaModel):
-    def __init__(self, request_id=None, success=None, task_id=None):
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-        self.task_id = task_id  # type: long
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(CreateEvaluatePreCheckTaskResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        if self.task_id is not None:
-            result['TaskId'] = self.task_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        if m.get('TaskId') is not None:
-            self.task_id = m.get('TaskId')
-        return self
-
-
-class CreateEvaluatePreCheckTaskResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: CreateEvaluatePreCheckTaskResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(CreateEvaluatePreCheckTaskResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = CreateEvaluatePreCheckTaskResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class CreateInstanceAccountRequestDbPrivilege(TeaModel):
     def __init__(self, db_name=None, privilege=None):
         self.db_name = db_name  # type: str
         self.privilege = privilege  # type: str
 
     def validate(self):
         pass
@@ -3664,105 +2668,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = DescribeBroadcastTablesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class DescribeDataImportTaskReportRequest(TeaModel):
-    def __init__(self, task_id=None):
-        self.task_id = task_id  # type: long
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeDataImportTaskReportRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.task_id is not None:
-            result['TaskId'] = self.task_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('TaskId') is not None:
-            self.task_id = m.get('TaskId')
-        return self
-
-
-class DescribeDataImportTaskReportResponseBody(TeaModel):
-    def __init__(self, data=None, request_id=None, success=None):
-        self.data = data  # type: str
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeDataImportTaskReportResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.data is not None:
-            result['Data'] = self.data
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Data') is not None:
-            self.data = m.get('Data')
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class DescribeDataImportTaskReportResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: DescribeDataImportTaskReportResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(DescribeDataImportTaskReportResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = DescribeDataImportTaskReportResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class DescribeDbInstanceDbsRequest(TeaModel):
     def __init__(self, account_name=None, db_inst_type=None, db_instance_id=None, drds_instance_id=None,
                  password=None):
         self.account_name = account_name  # type: str
         self.db_inst_type = db_inst_type  # type: str
         self.db_instance_id = db_instance_id  # type: str
         self.drds_instance_id = drds_instance_id  # type: str
@@ -5825,512 +4738,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = DescribeDrdsDbRdsNameListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class DescribeDrdsDbSpecAndPriceRequest(TeaModel):
-    def __init__(self, dbname=None, drds_instance_id=None, region_id=None):
-        self.dbname = dbname  # type: str
-        self.drds_instance_id = drds_instance_id  # type: str
-        self.region_id = region_id  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeDrdsDbSpecAndPriceRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.dbname is not None:
-            result['DBName'] = self.dbname
-        if self.drds_instance_id is not None:
-            result['DrdsInstanceId'] = self.drds_instance_id
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DBName') is not None:
-            self.dbname = m.get('DBName')
-        if m.get('DrdsInstanceId') is not None:
-            self.drds_instance_id = m.get('DrdsInstanceId')
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
-        return self
-
-
-class DescribeDrdsDbSpecAndPriceResponseBodyDataDrdsDbPrice(TeaModel):
-    def __init__(self, currency=None, discount_price=None, original_price=None, trade_price=None):
-        self.currency = currency  # type: str
-        self.discount_price = discount_price  # type: float
-        self.original_price = original_price  # type: float
-        self.trade_price = trade_price  # type: float
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeDrdsDbSpecAndPriceResponseBodyDataDrdsDbPrice, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.currency is not None:
-            result['Currency'] = self.currency
-        if self.discount_price is not None:
-            result['DiscountPrice'] = self.discount_price
-        if self.original_price is not None:
-            result['OriginalPrice'] = self.original_price
-        if self.trade_price is not None:
-            result['TradePrice'] = self.trade_price
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Currency') is not None:
-            self.currency = m.get('Currency')
-        if m.get('DiscountPrice') is not None:
-            self.discount_price = m.get('DiscountPrice')
-        if m.get('OriginalPrice') is not None:
-            self.original_price = m.get('OriginalPrice')
-        if m.get('TradePrice') is not None:
-            self.trade_price = m.get('TradePrice')
-        return self
-
-
-class DescribeDrdsDbSpecAndPriceResponseBodyDataDrdsInstance(TeaModel):
-    def __init__(self, drds_instance_id=None, inst_role=None, instance_series=None, instance_spec=None,
-                 machine_type=None, network_type=None, product_version=None, protocol_type=None, region_id=None, status=None,
-                 type=None, version_action=None, vpc_cloud_instance_id=None, vpc_id=None, zone_id=None):
-        self.drds_instance_id = drds_instance_id  # type: str
-        self.inst_role = inst_role  # type: str
-        self.instance_series = instance_series  # type: str
-        self.instance_spec = instance_spec  # type: str
-        self.machine_type = machine_type  # type: str
-        self.network_type = network_type  # type: str
-        self.product_version = product_version  # type: str
-        self.protocol_type = protocol_type  # type: int
-        self.region_id = region_id  # type: str
-        self.status = status  # type: str
-        self.type = type  # type: str
-        self.version_action = version_action  # type: str
-        self.vpc_cloud_instance_id = vpc_cloud_instance_id  # type: str
-        self.vpc_id = vpc_id  # type: str
-        self.zone_id = zone_id  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeDrdsDbSpecAndPriceResponseBodyDataDrdsInstance, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.drds_instance_id is not None:
-            result['DrdsInstanceId'] = self.drds_instance_id
-        if self.inst_role is not None:
-            result['InstRole'] = self.inst_role
-        if self.instance_series is not None:
-            result['InstanceSeries'] = self.instance_series
-        if self.instance_spec is not None:
-            result['InstanceSpec'] = self.instance_spec
-        if self.machine_type is not None:
-            result['MachineType'] = self.machine_type
-        if self.network_type is not None:
-            result['NetworkType'] = self.network_type
-        if self.product_version is not None:
-            result['ProductVersion'] = self.product_version
-        if self.protocol_type is not None:
-            result['ProtocolType'] = self.protocol_type
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
-        if self.status is not None:
-            result['Status'] = self.status
-        if self.type is not None:
-            result['Type'] = self.type
-        if self.version_action is not None:
-            result['VersionAction'] = self.version_action
-        if self.vpc_cloud_instance_id is not None:
-            result['VpcCloudInstanceId'] = self.vpc_cloud_instance_id
-        if self.vpc_id is not None:
-            result['VpcId'] = self.vpc_id
-        if self.zone_id is not None:
-            result['ZoneId'] = self.zone_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DrdsInstanceId') is not None:
-            self.drds_instance_id = m.get('DrdsInstanceId')
-        if m.get('InstRole') is not None:
-            self.inst_role = m.get('InstRole')
-        if m.get('InstanceSeries') is not None:
-            self.instance_series = m.get('InstanceSeries')
-        if m.get('InstanceSpec') is not None:
-            self.instance_spec = m.get('InstanceSpec')
-        if m.get('MachineType') is not None:
-            self.machine_type = m.get('MachineType')
-        if m.get('NetworkType') is not None:
-            self.network_type = m.get('NetworkType')
-        if m.get('ProductVersion') is not None:
-            self.product_version = m.get('ProductVersion')
-        if m.get('ProtocolType') is not None:
-            self.protocol_type = m.get('ProtocolType')
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
-        if m.get('Status') is not None:
-            self.status = m.get('Status')
-        if m.get('Type') is not None:
-            self.type = m.get('Type')
-        if m.get('VersionAction') is not None:
-            self.version_action = m.get('VersionAction')
-        if m.get('VpcCloudInstanceId') is not None:
-            self.vpc_cloud_instance_id = m.get('VpcCloudInstanceId')
-        if m.get('VpcId') is not None:
-            self.vpc_id = m.get('VpcId')
-        if m.get('ZoneId') is not None:
-            self.zone_id = m.get('ZoneId')
-        return self
-
-
-class DescribeDrdsDbSpecAndPriceResponseBodyDataRdsInstanceSpecsAndPricesRdsPrice(TeaModel):
-    def __init__(self, coupons=None, currency=None, discount_price=None, original_price=None, rule_ids=None,
-                 trade_price=None):
-        self.coupons = coupons  # type: str
-        self.currency = currency  # type: str
-        self.discount_price = discount_price  # type: float
-        self.original_price = original_price  # type: float
-        self.rule_ids = rule_ids  # type: list[str]
-        self.trade_price = trade_price  # type: float
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeDrdsDbSpecAndPriceResponseBodyDataRdsInstanceSpecsAndPricesRdsPrice, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.coupons is not None:
-            result['Coupons'] = self.coupons
-        if self.currency is not None:
-            result['Currency'] = self.currency
-        if self.discount_price is not None:
-            result['DiscountPrice'] = self.discount_price
-        if self.original_price is not None:
-            result['OriginalPrice'] = self.original_price
-        if self.rule_ids is not None:
-            result['RuleIds'] = self.rule_ids
-        if self.trade_price is not None:
-            result['TradePrice'] = self.trade_price
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Coupons') is not None:
-            self.coupons = m.get('Coupons')
-        if m.get('Currency') is not None:
-            self.currency = m.get('Currency')
-        if m.get('DiscountPrice') is not None:
-            self.discount_price = m.get('DiscountPrice')
-        if m.get('OriginalPrice') is not None:
-            self.original_price = m.get('OriginalPrice')
-        if m.get('RuleIds') is not None:
-            self.rule_ids = m.get('RuleIds')
-        if m.get('TradePrice') is not None:
-            self.trade_price = m.get('TradePrice')
-        return self
-
-
-class DescribeDrdsDbSpecAndPriceResponseBodyDataRdsInstanceSpecsAndPricesStorageInstance(TeaModel):
-    def __init__(self, connect_url=None, dbinst_type=None, dbinstance_cpu=None, dbinstance_class=None,
-                 dbinstance_class_type=None, dbinstance_description=None, dbinstance_id=None, dbinstance_memory=None,
-                 dbinstance_status=None, dbinstance_storage=None, dbinstance_storage_type=None, engine=None, engine_version=None,
-                 expire_time=None, network_type=None, pay_type=None, port=None, rdsinst_type=None, read_weight=None,
-                 region_id=None, remain_days=None, zone_id=None):
-        self.connect_url = connect_url  # type: str
-        self.dbinst_type = dbinst_type  # type: str
-        self.dbinstance_cpu = dbinstance_cpu  # type: str
-        self.dbinstance_class = dbinstance_class  # type: str
-        self.dbinstance_class_type = dbinstance_class_type  # type: str
-        self.dbinstance_description = dbinstance_description  # type: str
-        self.dbinstance_id = dbinstance_id  # type: str
-        self.dbinstance_memory = dbinstance_memory  # type: int
-        self.dbinstance_status = dbinstance_status  # type: int
-        self.dbinstance_storage = dbinstance_storage  # type: int
-        self.dbinstance_storage_type = dbinstance_storage_type  # type: str
-        self.engine = engine  # type: str
-        self.engine_version = engine_version  # type: str
-        self.expire_time = expire_time  # type: str
-        self.network_type = network_type  # type: str
-        self.pay_type = pay_type  # type: str
-        self.port = port  # type: int
-        self.rdsinst_type = rdsinst_type  # type: str
-        self.read_weight = read_weight  # type: int
-        self.region_id = region_id  # type: str
-        self.remain_days = remain_days  # type: int
-        self.zone_id = zone_id  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeDrdsDbSpecAndPriceResponseBodyDataRdsInstanceSpecsAndPricesStorageInstance, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.connect_url is not None:
-            result['ConnectUrl'] = self.connect_url
-        if self.dbinst_type is not None:
-            result['DBInstType'] = self.dbinst_type
-        if self.dbinstance_cpu is not None:
-            result['DBInstanceCPU'] = self.dbinstance_cpu
-        if self.dbinstance_class is not None:
-            result['DBInstanceClass'] = self.dbinstance_class
-        if self.dbinstance_class_type is not None:
-            result['DBInstanceClassType'] = self.dbinstance_class_type
-        if self.dbinstance_description is not None:
-            result['DBInstanceDescription'] = self.dbinstance_description
-        if self.dbinstance_id is not None:
-            result['DBInstanceId'] = self.dbinstance_id
-        if self.dbinstance_memory is not None:
-            result['DBInstanceMemory'] = self.dbinstance_memory
-        if self.dbinstance_status is not None:
-            result['DBInstanceStatus'] = self.dbinstance_status
-        if self.dbinstance_storage is not None:
-            result['DBInstanceStorage'] = self.dbinstance_storage
-        if self.dbinstance_storage_type is not None:
-            result['DBInstanceStorageType'] = self.dbinstance_storage_type
-        if self.engine is not None:
-            result['Engine'] = self.engine
-        if self.engine_version is not None:
-            result['EngineVersion'] = self.engine_version
-        if self.expire_time is not None:
-            result['ExpireTime'] = self.expire_time
-        if self.network_type is not None:
-            result['NetworkType'] = self.network_type
-        if self.pay_type is not None:
-            result['PayType'] = self.pay_type
-        if self.port is not None:
-            result['Port'] = self.port
-        if self.rdsinst_type is not None:
-            result['RDSInstType'] = self.rdsinst_type
-        if self.read_weight is not None:
-            result['ReadWeight'] = self.read_weight
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
-        if self.remain_days is not None:
-            result['RemainDays'] = self.remain_days
-        if self.zone_id is not None:
-            result['ZoneId'] = self.zone_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('ConnectUrl') is not None:
-            self.connect_url = m.get('ConnectUrl')
-        if m.get('DBInstType') is not None:
-            self.dbinst_type = m.get('DBInstType')
-        if m.get('DBInstanceCPU') is not None:
-            self.dbinstance_cpu = m.get('DBInstanceCPU')
-        if m.get('DBInstanceClass') is not None:
-            self.dbinstance_class = m.get('DBInstanceClass')
-        if m.get('DBInstanceClassType') is not None:
-            self.dbinstance_class_type = m.get('DBInstanceClassType')
-        if m.get('DBInstanceDescription') is not None:
-            self.dbinstance_description = m.get('DBInstanceDescription')
-        if m.get('DBInstanceId') is not None:
-            self.dbinstance_id = m.get('DBInstanceId')
-        if m.get('DBInstanceMemory') is not None:
-            self.dbinstance_memory = m.get('DBInstanceMemory')
-        if m.get('DBInstanceStatus') is not None:
-            self.dbinstance_status = m.get('DBInstanceStatus')
-        if m.get('DBInstanceStorage') is not None:
-            self.dbinstance_storage = m.get('DBInstanceStorage')
-        if m.get('DBInstanceStorageType') is not None:
-            self.dbinstance_storage_type = m.get('DBInstanceStorageType')
-        if m.get('Engine') is not None:
-            self.engine = m.get('Engine')
-        if m.get('EngineVersion') is not None:
-            self.engine_version = m.get('EngineVersion')
-        if m.get('ExpireTime') is not None:
-            self.expire_time = m.get('ExpireTime')
-        if m.get('NetworkType') is not None:
-            self.network_type = m.get('NetworkType')
-        if m.get('PayType') is not None:
-            self.pay_type = m.get('PayType')
-        if m.get('Port') is not None:
-            self.port = m.get('Port')
-        if m.get('RDSInstType') is not None:
-            self.rdsinst_type = m.get('RDSInstType')
-        if m.get('ReadWeight') is not None:
-            self.read_weight = m.get('ReadWeight')
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
-        if m.get('RemainDays') is not None:
-            self.remain_days = m.get('RemainDays')
-        if m.get('ZoneId') is not None:
-            self.zone_id = m.get('ZoneId')
-        return self
-
-
-class DescribeDrdsDbSpecAndPriceResponseBodyDataRdsInstanceSpecsAndPrices(TeaModel):
-    def __init__(self, rds_price=None, storage_instance=None):
-        self.rds_price = rds_price  # type: DescribeDrdsDbSpecAndPriceResponseBodyDataRdsInstanceSpecsAndPricesRdsPrice
-        self.storage_instance = storage_instance  # type: DescribeDrdsDbSpecAndPriceResponseBodyDataRdsInstanceSpecsAndPricesStorageInstance
-
-    def validate(self):
-        if self.rds_price:
-            self.rds_price.validate()
-        if self.storage_instance:
-            self.storage_instance.validate()
-
-    def to_map(self):
-        _map = super(DescribeDrdsDbSpecAndPriceResponseBodyDataRdsInstanceSpecsAndPrices, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.rds_price is not None:
-            result['RdsPrice'] = self.rds_price.to_map()
-        if self.storage_instance is not None:
-            result['StorageInstance'] = self.storage_instance.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('RdsPrice') is not None:
-            temp_model = DescribeDrdsDbSpecAndPriceResponseBodyDataRdsInstanceSpecsAndPricesRdsPrice()
-            self.rds_price = temp_model.from_map(m['RdsPrice'])
-        if m.get('StorageInstance') is not None:
-            temp_model = DescribeDrdsDbSpecAndPriceResponseBodyDataRdsInstanceSpecsAndPricesStorageInstance()
-            self.storage_instance = temp_model.from_map(m['StorageInstance'])
-        return self
-
-
-class DescribeDrdsDbSpecAndPriceResponseBodyData(TeaModel):
-    def __init__(self, drds_db_price=None, drds_instance=None, rds_instance_specs_and_prices=None):
-        self.drds_db_price = drds_db_price  # type: DescribeDrdsDbSpecAndPriceResponseBodyDataDrdsDbPrice
-        self.drds_instance = drds_instance  # type: DescribeDrdsDbSpecAndPriceResponseBodyDataDrdsInstance
-        self.rds_instance_specs_and_prices = rds_instance_specs_and_prices  # type: list[DescribeDrdsDbSpecAndPriceResponseBodyDataRdsInstanceSpecsAndPrices]
-
-    def validate(self):
-        if self.drds_db_price:
-            self.drds_db_price.validate()
-        if self.drds_instance:
-            self.drds_instance.validate()
-        if self.rds_instance_specs_and_prices:
-            for k in self.rds_instance_specs_and_prices:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super(DescribeDrdsDbSpecAndPriceResponseBodyData, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.drds_db_price is not None:
-            result['DrdsDbPrice'] = self.drds_db_price.to_map()
-        if self.drds_instance is not None:
-            result['DrdsInstance'] = self.drds_instance.to_map()
-        result['RdsInstanceSpecsAndPrices'] = []
-        if self.rds_instance_specs_and_prices is not None:
-            for k in self.rds_instance_specs_and_prices:
-                result['RdsInstanceSpecsAndPrices'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DrdsDbPrice') is not None:
-            temp_model = DescribeDrdsDbSpecAndPriceResponseBodyDataDrdsDbPrice()
-            self.drds_db_price = temp_model.from_map(m['DrdsDbPrice'])
-        if m.get('DrdsInstance') is not None:
-            temp_model = DescribeDrdsDbSpecAndPriceResponseBodyDataDrdsInstance()
-            self.drds_instance = temp_model.from_map(m['DrdsInstance'])
-        self.rds_instance_specs_and_prices = []
-        if m.get('RdsInstanceSpecsAndPrices') is not None:
-            for k in m.get('RdsInstanceSpecsAndPrices'):
-                temp_model = DescribeDrdsDbSpecAndPriceResponseBodyDataRdsInstanceSpecsAndPrices()
-                self.rds_instance_specs_and_prices.append(temp_model.from_map(k))
-        return self
-
-
-class DescribeDrdsDbSpecAndPriceResponseBody(TeaModel):
-    def __init__(self, data=None, request_id=None):
-        self.data = data  # type: DescribeDrdsDbSpecAndPriceResponseBodyData
-        self.request_id = request_id  # type: str
-
-    def validate(self):
-        if self.data:
-            self.data.validate()
-
-    def to_map(self):
-        _map = super(DescribeDrdsDbSpecAndPriceResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.data is not None:
-            result['Data'] = self.data.to_map()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Data') is not None:
-            temp_model = DescribeDrdsDbSpecAndPriceResponseBodyData()
-            self.data = temp_model.from_map(m['Data'])
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        return self
-
-
-class DescribeDrdsDbSpecAndPriceResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: DescribeDrdsDbSpecAndPriceResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(DescribeDrdsDbSpecAndPriceResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = DescribeDrdsDbSpecAndPriceResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class DescribeDrdsDbTasksRequest(TeaModel):
     def __init__(self, db_name=None, drds_instance_id=None, task_type=None):
         self.db_name = db_name  # type: str
         self.drds_instance_id = drds_instance_id  # type: str
         self.task_type = task_type  # type: str
 
     def validate(self):
@@ -9501,157 +7916,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = DescribeExpandLogicTableInfoListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class DescribeHiStoreInstanceInfoRequest(TeaModel):
-    def __init__(self, drds_instance_id=None, histore_instance_id=None):
-        self.drds_instance_id = drds_instance_id  # type: str
-        self.histore_instance_id = histore_instance_id  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeHiStoreInstanceInfoRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.drds_instance_id is not None:
-            result['DrdsInstanceId'] = self.drds_instance_id
-        if self.histore_instance_id is not None:
-            result['HistoreInstanceId'] = self.histore_instance_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DrdsInstanceId') is not None:
-            self.drds_instance_id = m.get('DrdsInstanceId')
-        if m.get('HistoreInstanceId') is not None:
-            self.histore_instance_id = m.get('HistoreInstanceId')
-        return self
-
-
-class DescribeHiStoreInstanceInfoResponseBodyHiStoreInstanceInfo(TeaModel):
-    def __init__(self, disk_size=None, gmt_create=None, histore_instance_id=None, machine_spec=None,
-                 rpm_version=None):
-        self.disk_size = disk_size  # type: int
-        self.gmt_create = gmt_create  # type: long
-        self.histore_instance_id = histore_instance_id  # type: str
-        self.machine_spec = machine_spec  # type: str
-        self.rpm_version = rpm_version  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeHiStoreInstanceInfoResponseBodyHiStoreInstanceInfo, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.disk_size is not None:
-            result['DiskSize'] = self.disk_size
-        if self.gmt_create is not None:
-            result['GmtCreate'] = self.gmt_create
-        if self.histore_instance_id is not None:
-            result['HistoreInstanceId'] = self.histore_instance_id
-        if self.machine_spec is not None:
-            result['MachineSpec'] = self.machine_spec
-        if self.rpm_version is not None:
-            result['RpmVersion'] = self.rpm_version
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DiskSize') is not None:
-            self.disk_size = m.get('DiskSize')
-        if m.get('GmtCreate') is not None:
-            self.gmt_create = m.get('GmtCreate')
-        if m.get('HistoreInstanceId') is not None:
-            self.histore_instance_id = m.get('HistoreInstanceId')
-        if m.get('MachineSpec') is not None:
-            self.machine_spec = m.get('MachineSpec')
-        if m.get('RpmVersion') is not None:
-            self.rpm_version = m.get('RpmVersion')
-        return self
-
-
-class DescribeHiStoreInstanceInfoResponseBody(TeaModel):
-    def __init__(self, hi_store_instance_info=None, request_id=None, success=None):
-        self.hi_store_instance_info = hi_store_instance_info  # type: DescribeHiStoreInstanceInfoResponseBodyHiStoreInstanceInfo
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-
-    def validate(self):
-        if self.hi_store_instance_info:
-            self.hi_store_instance_info.validate()
-
-    def to_map(self):
-        _map = super(DescribeHiStoreInstanceInfoResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.hi_store_instance_info is not None:
-            result['HiStoreInstanceInfo'] = self.hi_store_instance_info.to_map()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('HiStoreInstanceInfo') is not None:
-            temp_model = DescribeHiStoreInstanceInfoResponseBodyHiStoreInstanceInfo()
-            self.hi_store_instance_info = temp_model.from_map(m['HiStoreInstanceInfo'])
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class DescribeHiStoreInstanceInfoResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: DescribeHiStoreInstanceInfoResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(DescribeHiStoreInstanceInfoResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = DescribeHiStoreInstanceInfoResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class DescribeHotDbListRequest(TeaModel):
     def __init__(self, db_name=None, drds_instance_id=None):
         self.db_name = db_name  # type: str
         self.drds_instance_id = drds_instance_id  # type: str
 
     def validate(self):
         pass
@@ -10351,105 +8623,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = DescribeInstanceAccountsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class DescribeInstanceMenuSwitchRequest(TeaModel):
-    def __init__(self, drds_instance_id=None):
-        self.drds_instance_id = drds_instance_id  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeInstanceMenuSwitchRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.drds_instance_id is not None:
-            result['DrdsInstanceId'] = self.drds_instance_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DrdsInstanceId') is not None:
-            self.drds_instance_id = m.get('DrdsInstanceId')
-        return self
-
-
-class DescribeInstanceMenuSwitchResponseBody(TeaModel):
-    def __init__(self, config=None, request_id=None, success=None):
-        self.config = config  # type: dict[str, any]
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeInstanceMenuSwitchResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.config is not None:
-            result['Config'] = self.config
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Config') is not None:
-            self.config = m.get('Config')
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class DescribeInstanceMenuSwitchResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: DescribeInstanceMenuSwitchResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(DescribeInstanceMenuSwitchResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = DescribeInstanceMenuSwitchResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class DescribeInstanceSwitchAzoneRequest(TeaModel):
     def __init__(self, drds_instance_id=None):
         self.drds_instance_id = drds_instance_id  # type: str
 
     def validate(self):
         pass
 
@@ -11333,199 +9514,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = DescribeRdsCommodityResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class DescribeRdsDrdsDBRequest(TeaModel):
-    def __init__(self, drds_instance_id=None, rds_instance_id=None):
-        self.drds_instance_id = drds_instance_id  # type: str
-        self.rds_instance_id = rds_instance_id  # type: list[str]
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeRdsDrdsDBRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.drds_instance_id is not None:
-            result['DrdsInstanceId'] = self.drds_instance_id
-        if self.rds_instance_id is not None:
-            result['RdsInstanceId'] = self.rds_instance_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DrdsInstanceId') is not None:
-            self.drds_instance_id = m.get('DrdsInstanceId')
-        if m.get('RdsInstanceId') is not None:
-            self.rds_instance_id = m.get('RdsInstanceId')
-        return self
-
-
-class DescribeRdsDrdsDBResponseBodyRdsDrdsDbsRdsDrdsDbDBList(TeaModel):
-    def __init__(self, db=None):
-        self.db = db  # type: list[str]
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeRdsDrdsDBResponseBodyRdsDrdsDbsRdsDrdsDbDBList, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.db is not None:
-            result['DB'] = self.db
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DB') is not None:
-            self.db = m.get('DB')
-        return self
-
-
-class DescribeRdsDrdsDBResponseBodyRdsDrdsDbsRdsDrdsDb(TeaModel):
-    def __init__(self, dblist=None, rds_id=None):
-        self.dblist = dblist  # type: DescribeRdsDrdsDBResponseBodyRdsDrdsDbsRdsDrdsDbDBList
-        self.rds_id = rds_id  # type: str
-
-    def validate(self):
-        if self.dblist:
-            self.dblist.validate()
-
-    def to_map(self):
-        _map = super(DescribeRdsDrdsDBResponseBodyRdsDrdsDbsRdsDrdsDb, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.dblist is not None:
-            result['DBList'] = self.dblist.to_map()
-        if self.rds_id is not None:
-            result['RdsId'] = self.rds_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DBList') is not None:
-            temp_model = DescribeRdsDrdsDBResponseBodyRdsDrdsDbsRdsDrdsDbDBList()
-            self.dblist = temp_model.from_map(m['DBList'])
-        if m.get('RdsId') is not None:
-            self.rds_id = m.get('RdsId')
-        return self
-
-
-class DescribeRdsDrdsDBResponseBodyRdsDrdsDbs(TeaModel):
-    def __init__(self, rds_drds_db=None):
-        self.rds_drds_db = rds_drds_db  # type: list[DescribeRdsDrdsDBResponseBodyRdsDrdsDbsRdsDrdsDb]
-
-    def validate(self):
-        if self.rds_drds_db:
-            for k in self.rds_drds_db:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super(DescribeRdsDrdsDBResponseBodyRdsDrdsDbs, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        result['RdsDrdsDb'] = []
-        if self.rds_drds_db is not None:
-            for k in self.rds_drds_db:
-                result['RdsDrdsDb'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        self.rds_drds_db = []
-        if m.get('RdsDrdsDb') is not None:
-            for k in m.get('RdsDrdsDb'):
-                temp_model = DescribeRdsDrdsDBResponseBodyRdsDrdsDbsRdsDrdsDb()
-                self.rds_drds_db.append(temp_model.from_map(k))
-        return self
-
-
-class DescribeRdsDrdsDBResponseBody(TeaModel):
-    def __init__(self, rds_drds_dbs=None, request_id=None, success=None):
-        self.rds_drds_dbs = rds_drds_dbs  # type: DescribeRdsDrdsDBResponseBodyRdsDrdsDbs
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-
-    def validate(self):
-        if self.rds_drds_dbs:
-            self.rds_drds_dbs.validate()
-
-    def to_map(self):
-        _map = super(DescribeRdsDrdsDBResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.rds_drds_dbs is not None:
-            result['RdsDrdsDbs'] = self.rds_drds_dbs.to_map()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('RdsDrdsDbs') is not None:
-            temp_model = DescribeRdsDrdsDBResponseBodyRdsDrdsDbs()
-            self.rds_drds_dbs = temp_model.from_map(m['RdsDrdsDbs'])
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class DescribeRdsDrdsDBResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: DescribeRdsDrdsDBResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(DescribeRdsDrdsDBResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = DescribeRdsDrdsDBResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class DescribeRdsPerformanceSummaryRequest(TeaModel):
     def __init__(self, drds_instance_id=None, rds_instance_id=None, region_id=None):
         self.drds_instance_id = drds_instance_id  # type: str
         self.rds_instance_id = rds_instance_id  # type: list[str]
         self.region_id = region_id  # type: str
 
     def validate(self):
@@ -11676,357 +9672,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = DescribeRdsPerformanceSummaryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class DescribeRdsPriceRequest(TeaModel):
-    def __init__(self, params=None, region_id=None):
-        self.params = params  # type: str
-        self.region_id = region_id  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeRdsPriceRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.params is not None:
-            result['Params'] = self.params
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Params') is not None:
-            self.params = m.get('Params')
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
-        return self
-
-
-class DescribeRdsPriceResponseBody(TeaModel):
-    def __init__(self, data=None, request_id=None, success=None):
-        self.data = data  # type: str
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeRdsPriceResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.data is not None:
-            result['Data'] = self.data
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Data') is not None:
-            self.data = m.get('Data')
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class DescribeRdsPriceResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: DescribeRdsPriceResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(DescribeRdsPriceResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = DescribeRdsPriceResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
-class DescribeRdsReadOnlyRequest(TeaModel):
-    def __init__(self, db_inst_type=None, drds_instance_id=None, rds_instance_id=None):
-        self.db_inst_type = db_inst_type  # type: str
-        self.drds_instance_id = drds_instance_id  # type: str
-        self.rds_instance_id = rds_instance_id  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeRdsReadOnlyRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.db_inst_type is not None:
-            result['DbInstType'] = self.db_inst_type
-        if self.drds_instance_id is not None:
-            result['DrdsInstanceId'] = self.drds_instance_id
-        if self.rds_instance_id is not None:
-            result['RdsInstanceId'] = self.rds_instance_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DbInstType') is not None:
-            self.db_inst_type = m.get('DbInstType')
-        if m.get('DrdsInstanceId') is not None:
-            self.drds_instance_id = m.get('DrdsInstanceId')
-        if m.get('RdsInstanceId') is not None:
-            self.rds_instance_id = m.get('RdsInstanceId')
-        return self
-
-
-class DescribeRdsReadOnlyResponseBodyDbInstancesDbInstance(TeaModel):
-    def __init__(self, connect_url=None, dbinstance_cpu=None, dbinstance_class_type=None, dbinstance_id=None,
-                 dbinstance_memory=None, dbinstance_status=None, dbinstance_storage=None, db_inst_type=None, dm_instance_id=None,
-                 engine=None, engine_version=None, expire_time=None, network_type=None, pay_type=None, port=None,
-                 rds_inst_type=None, read_weight=None, remain_days=None):
-        self.connect_url = connect_url  # type: str
-        self.dbinstance_cpu = dbinstance_cpu  # type: str
-        self.dbinstance_class_type = dbinstance_class_type  # type: str
-        self.dbinstance_id = dbinstance_id  # type: str
-        self.dbinstance_memory = dbinstance_memory  # type: long
-        self.dbinstance_status = dbinstance_status  # type: str
-        self.dbinstance_storage = dbinstance_storage  # type: long
-        self.db_inst_type = db_inst_type  # type: str
-        self.dm_instance_id = dm_instance_id  # type: str
-        self.engine = engine  # type: str
-        self.engine_version = engine_version  # type: str
-        self.expire_time = expire_time  # type: str
-        self.network_type = network_type  # type: str
-        self.pay_type = pay_type  # type: str
-        self.port = port  # type: int
-        self.rds_inst_type = rds_inst_type  # type: str
-        self.read_weight = read_weight  # type: int
-        self.remain_days = remain_days  # type: int
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeRdsReadOnlyResponseBodyDbInstancesDbInstance, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.connect_url is not None:
-            result['ConnectUrl'] = self.connect_url
-        if self.dbinstance_cpu is not None:
-            result['DBInstanceCPU'] = self.dbinstance_cpu
-        if self.dbinstance_class_type is not None:
-            result['DBInstanceClassType'] = self.dbinstance_class_type
-        if self.dbinstance_id is not None:
-            result['DBInstanceId'] = self.dbinstance_id
-        if self.dbinstance_memory is not None:
-            result['DBInstanceMemory'] = self.dbinstance_memory
-        if self.dbinstance_status is not None:
-            result['DBInstanceStatus'] = self.dbinstance_status
-        if self.dbinstance_storage is not None:
-            result['DBInstanceStorage'] = self.dbinstance_storage
-        if self.db_inst_type is not None:
-            result['DbInstType'] = self.db_inst_type
-        if self.dm_instance_id is not None:
-            result['DmInstanceId'] = self.dm_instance_id
-        if self.engine is not None:
-            result['Engine'] = self.engine
-        if self.engine_version is not None:
-            result['EngineVersion'] = self.engine_version
-        if self.expire_time is not None:
-            result['ExpireTime'] = self.expire_time
-        if self.network_type is not None:
-            result['NetworkType'] = self.network_type
-        if self.pay_type is not None:
-            result['PayType'] = self.pay_type
-        if self.port is not None:
-            result['Port'] = self.port
-        if self.rds_inst_type is not None:
-            result['RdsInstType'] = self.rds_inst_type
-        if self.read_weight is not None:
-            result['ReadWeight'] = self.read_weight
-        if self.remain_days is not None:
-            result['RemainDays'] = self.remain_days
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('ConnectUrl') is not None:
-            self.connect_url = m.get('ConnectUrl')
-        if m.get('DBInstanceCPU') is not None:
-            self.dbinstance_cpu = m.get('DBInstanceCPU')
-        if m.get('DBInstanceClassType') is not None:
-            self.dbinstance_class_type = m.get('DBInstanceClassType')
-        if m.get('DBInstanceId') is not None:
-            self.dbinstance_id = m.get('DBInstanceId')
-        if m.get('DBInstanceMemory') is not None:
-            self.dbinstance_memory = m.get('DBInstanceMemory')
-        if m.get('DBInstanceStatus') is not None:
-            self.dbinstance_status = m.get('DBInstanceStatus')
-        if m.get('DBInstanceStorage') is not None:
-            self.dbinstance_storage = m.get('DBInstanceStorage')
-        if m.get('DbInstType') is not None:
-            self.db_inst_type = m.get('DbInstType')
-        if m.get('DmInstanceId') is not None:
-            self.dm_instance_id = m.get('DmInstanceId')
-        if m.get('Engine') is not None:
-            self.engine = m.get('Engine')
-        if m.get('EngineVersion') is not None:
-            self.engine_version = m.get('EngineVersion')
-        if m.get('ExpireTime') is not None:
-            self.expire_time = m.get('ExpireTime')
-        if m.get('NetworkType') is not None:
-            self.network_type = m.get('NetworkType')
-        if m.get('PayType') is not None:
-            self.pay_type = m.get('PayType')
-        if m.get('Port') is not None:
-            self.port = m.get('Port')
-        if m.get('RdsInstType') is not None:
-            self.rds_inst_type = m.get('RdsInstType')
-        if m.get('ReadWeight') is not None:
-            self.read_weight = m.get('ReadWeight')
-        if m.get('RemainDays') is not None:
-            self.remain_days = m.get('RemainDays')
-        return self
-
-
-class DescribeRdsReadOnlyResponseBodyDbInstances(TeaModel):
-    def __init__(self, db_instance=None):
-        self.db_instance = db_instance  # type: list[DescribeRdsReadOnlyResponseBodyDbInstancesDbInstance]
-
-    def validate(self):
-        if self.db_instance:
-            for k in self.db_instance:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super(DescribeRdsReadOnlyResponseBodyDbInstances, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        result['DbInstance'] = []
-        if self.db_instance is not None:
-            for k in self.db_instance:
-                result['DbInstance'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        self.db_instance = []
-        if m.get('DbInstance') is not None:
-            for k in m.get('DbInstance'):
-                temp_model = DescribeRdsReadOnlyResponseBodyDbInstancesDbInstance()
-                self.db_instance.append(temp_model.from_map(k))
-        return self
-
-
-class DescribeRdsReadOnlyResponseBody(TeaModel):
-    def __init__(self, db_instances=None, request_id=None, success=None):
-        self.db_instances = db_instances  # type: DescribeRdsReadOnlyResponseBodyDbInstances
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-
-    def validate(self):
-        if self.db_instances:
-            self.db_instances.validate()
-
-    def to_map(self):
-        _map = super(DescribeRdsReadOnlyResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.db_instances is not None:
-            result['DbInstances'] = self.db_instances.to_map()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DbInstances') is not None:
-            temp_model = DescribeRdsReadOnlyResponseBodyDbInstances()
-            self.db_instances = temp_model.from_map(m['DbInstances'])
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class DescribeRdsReadOnlyResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: DescribeRdsReadOnlyResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(DescribeRdsReadOnlyResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = DescribeRdsReadOnlyResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class DescribeRdsSuperAccountInstancesRequest(TeaModel):
     def __init__(self, db_inst_type=None, drds_instance_id=None, rds_instance=None):
         self.db_inst_type = db_inst_type  # type: str
         self.drds_instance_id = drds_instance_id  # type: str
         self.rds_instance = rds_instance  # type: list[str]
 
     def validate(self):
@@ -12141,110 +9794,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = DescribeRdsSuperAccountInstancesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class DescribeRdsVpcForZoneRequest(TeaModel):
-    def __init__(self, region_id=None, zone_id=None):
-        self.region_id = region_id  # type: str
-        self.zone_id = zone_id  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeRdsVpcForZoneRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
-        if self.zone_id is not None:
-            result['ZoneId'] = self.zone_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
-        if m.get('ZoneId') is not None:
-            self.zone_id = m.get('ZoneId')
-        return self
-
-
-class DescribeRdsVpcForZoneResponseBody(TeaModel):
-    def __init__(self, data=None, request_id=None, success=None):
-        self.data = data  # type: str
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeRdsVpcForZoneResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.data is not None:
-            result['Data'] = self.data
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Data') is not None:
-            self.data = m.get('Data')
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class DescribeRdsVpcForZoneResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: DescribeRdsVpcForZoneResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(DescribeRdsVpcForZoneResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = DescribeRdsVpcForZoneResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class DescribeRecycleBinStatusRequest(TeaModel):
     def __init__(self, db_name=None, drds_instance_id=None, region_id=None):
         self.db_name = db_name  # type: str
         self.drds_instance_id = drds_instance_id  # type: str
         self.region_id = region_id  # type: str
 
     def validate(self):
@@ -13757,231 +11314,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = DescribeSqlFlashbakTaskResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class DescribeSrcRdsListRequestPartitionMapping(TeaModel):
-    def __init__(self, db_shard_value=None, hot_db_name=None, hot_table_name=None, logic_table=None,
-                 tb_shard_value=None):
-        self.db_shard_value = db_shard_value  # type: str
-        self.hot_db_name = hot_db_name  # type: str
-        self.hot_table_name = hot_table_name  # type: str
-        self.logic_table = logic_table  # type: str
-        self.tb_shard_value = tb_shard_value  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeSrcRdsListRequestPartitionMapping, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.db_shard_value is not None:
-            result['DbShardValue'] = self.db_shard_value
-        if self.hot_db_name is not None:
-            result['HotDbName'] = self.hot_db_name
-        if self.hot_table_name is not None:
-            result['HotTableName'] = self.hot_table_name
-        if self.logic_table is not None:
-            result['LogicTable'] = self.logic_table
-        if self.tb_shard_value is not None:
-            result['TbShardValue'] = self.tb_shard_value
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DbShardValue') is not None:
-            self.db_shard_value = m.get('DbShardValue')
-        if m.get('HotDbName') is not None:
-            self.hot_db_name = m.get('HotDbName')
-        if m.get('HotTableName') is not None:
-            self.hot_table_name = m.get('HotTableName')
-        if m.get('LogicTable') is not None:
-            self.logic_table = m.get('LogicTable')
-        if m.get('TbShardValue') is not None:
-            self.tb_shard_value = m.get('TbShardValue')
-        return self
-
-
-class DescribeSrcRdsListRequest(TeaModel):
-    def __init__(self, db_name=None, drds_instance_id=None, partition_mapping=None):
-        self.db_name = db_name  # type: str
-        self.drds_instance_id = drds_instance_id  # type: str
-        self.partition_mapping = partition_mapping  # type: list[DescribeSrcRdsListRequestPartitionMapping]
-
-    def validate(self):
-        if self.partition_mapping:
-            for k in self.partition_mapping:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super(DescribeSrcRdsListRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.db_name is not None:
-            result['DbName'] = self.db_name
-        if self.drds_instance_id is not None:
-            result['DrdsInstanceId'] = self.drds_instance_id
-        result['PartitionMapping'] = []
-        if self.partition_mapping is not None:
-            for k in self.partition_mapping:
-                result['PartitionMapping'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DbName') is not None:
-            self.db_name = m.get('DbName')
-        if m.get('DrdsInstanceId') is not None:
-            self.drds_instance_id = m.get('DrdsInstanceId')
-        self.partition_mapping = []
-        if m.get('PartitionMapping') is not None:
-            for k in m.get('PartitionMapping'):
-                temp_model = DescribeSrcRdsListRequestPartitionMapping()
-                self.partition_mapping.append(temp_model.from_map(k))
-        return self
-
-
-class DescribeSrcRdsListResponseBodyDataData(TeaModel):
-    def __init__(self, db_name=None, rds=None):
-        self.db_name = db_name  # type: str
-        self.rds = rds  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeSrcRdsListResponseBodyDataData, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.db_name is not None:
-            result['DbName'] = self.db_name
-        if self.rds is not None:
-            result['Rds'] = self.rds
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DbName') is not None:
-            self.db_name = m.get('DbName')
-        if m.get('Rds') is not None:
-            self.rds = m.get('Rds')
-        return self
-
-
-class DescribeSrcRdsListResponseBodyData(TeaModel):
-    def __init__(self, data=None):
-        self.data = data  # type: list[DescribeSrcRdsListResponseBodyDataData]
-
-    def validate(self):
-        if self.data:
-            for k in self.data:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super(DescribeSrcRdsListResponseBodyData, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        result['data'] = []
-        if self.data is not None:
-            for k in self.data:
-                result['data'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        self.data = []
-        if m.get('data') is not None:
-            for k in m.get('data'):
-                temp_model = DescribeSrcRdsListResponseBodyDataData()
-                self.data.append(temp_model.from_map(k))
-        return self
-
-
-class DescribeSrcRdsListResponseBody(TeaModel):
-    def __init__(self, data=None, request_id=None, success=None):
-        self.data = data  # type: DescribeSrcRdsListResponseBodyData
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-
-    def validate(self):
-        if self.data:
-            self.data.validate()
-
-    def to_map(self):
-        _map = super(DescribeSrcRdsListResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.data is not None:
-            result['Data'] = self.data.to_map()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Data') is not None:
-            temp_model = DescribeSrcRdsListResponseBodyData()
-            self.data = temp_model.from_map(m['Data'])
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class DescribeSrcRdsListResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: DescribeSrcRdsListResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(DescribeSrcRdsListResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = DescribeSrcRdsListResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class DescribeTableRequest(TeaModel):
     def __init__(self, db_name=None, drds_instance_id=None, region_id=None, table_name=None):
         self.db_name = db_name  # type: str
         self.drds_instance_id = drds_instance_id  # type: str
         self.region_id = region_id  # type: str
         self.table_name = table_name  # type: str
 
@@ -15408,389 +12748,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = ListTagResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ListUserReportsRequest(TeaModel):
-    def __init__(self, drds_instance_id=None, report_id=None):
-        self.drds_instance_id = drds_instance_id  # type: str
-        self.report_id = report_id  # type: long
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ListUserReportsRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.drds_instance_id is not None:
-            result['DrdsInstanceId'] = self.drds_instance_id
-        if self.report_id is not None:
-            result['ReportId'] = self.report_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DrdsInstanceId') is not None:
-            self.drds_instance_id = m.get('DrdsInstanceId')
-        if m.get('ReportId') is not None:
-            self.report_id = m.get('ReportId')
-        return self
-
-
-class ListUserReportsResponseBodySqlComparisonReportExecuteDetailListExecuteDetail(TeaModel):
-    def __init__(self, db_name=None, exec_detail_msg=None, execute=None, sql_content=None):
-        self.db_name = db_name  # type: str
-        self.exec_detail_msg = exec_detail_msg  # type: str
-        self.execute = execute  # type: str
-        self.sql_content = sql_content  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ListUserReportsResponseBodySqlComparisonReportExecuteDetailListExecuteDetail, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.db_name is not None:
-            result['DbName'] = self.db_name
-        if self.exec_detail_msg is not None:
-            result['ExecDetailMsg'] = self.exec_detail_msg
-        if self.execute is not None:
-            result['Execute'] = self.execute
-        if self.sql_content is not None:
-            result['SqlContent'] = self.sql_content
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DbName') is not None:
-            self.db_name = m.get('DbName')
-        if m.get('ExecDetailMsg') is not None:
-            self.exec_detail_msg = m.get('ExecDetailMsg')
-        if m.get('Execute') is not None:
-            self.execute = m.get('Execute')
-        if m.get('SqlContent') is not None:
-            self.sql_content = m.get('SqlContent')
-        return self
-
-
-class ListUserReportsResponseBodySqlComparisonReportExecuteDetailList(TeaModel):
-    def __init__(self, execute_detail=None):
-        self.execute_detail = execute_detail  # type: list[ListUserReportsResponseBodySqlComparisonReportExecuteDetailListExecuteDetail]
-
-    def validate(self):
-        if self.execute_detail:
-            for k in self.execute_detail:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super(ListUserReportsResponseBodySqlComparisonReportExecuteDetailList, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        result['executeDetail'] = []
-        if self.execute_detail is not None:
-            for k in self.execute_detail:
-                result['executeDetail'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        self.execute_detail = []
-        if m.get('executeDetail') is not None:
-            for k in m.get('executeDetail'):
-                temp_model = ListUserReportsResponseBodySqlComparisonReportExecuteDetailListExecuteDetail()
-                self.execute_detail.append(temp_model.from_map(k))
-        return self
-
-
-class ListUserReportsResponseBodySqlComparisonReport(TeaModel):
-    def __init__(self, sql_pass_fail_num=None, sql_pass_rate=None, sql_pass_succ_num=None, version=None,
-                 execute_detail_list=None):
-        self.sql_pass_fail_num = sql_pass_fail_num  # type: long
-        self.sql_pass_rate = sql_pass_rate  # type: str
-        self.sql_pass_succ_num = sql_pass_succ_num  # type: long
-        self.version = version  # type: str
-        self.execute_detail_list = execute_detail_list  # type: ListUserReportsResponseBodySqlComparisonReportExecuteDetailList
-
-    def validate(self):
-        if self.execute_detail_list:
-            self.execute_detail_list.validate()
-
-    def to_map(self):
-        _map = super(ListUserReportsResponseBodySqlComparisonReport, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.sql_pass_fail_num is not None:
-            result['SqlPassFailNum'] = self.sql_pass_fail_num
-        if self.sql_pass_rate is not None:
-            result['SqlPassRate'] = self.sql_pass_rate
-        if self.sql_pass_succ_num is not None:
-            result['SqlPassSuccNum'] = self.sql_pass_succ_num
-        if self.version is not None:
-            result['Version'] = self.version
-        if self.execute_detail_list is not None:
-            result['executeDetailList'] = self.execute_detail_list.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('SqlPassFailNum') is not None:
-            self.sql_pass_fail_num = m.get('SqlPassFailNum')
-        if m.get('SqlPassRate') is not None:
-            self.sql_pass_rate = m.get('SqlPassRate')
-        if m.get('SqlPassSuccNum') is not None:
-            self.sql_pass_succ_num = m.get('SqlPassSuccNum')
-        if m.get('Version') is not None:
-            self.version = m.get('Version')
-        if m.get('executeDetailList') is not None:
-            temp_model = ListUserReportsResponseBodySqlComparisonReportExecuteDetailList()
-            self.execute_detail_list = temp_model.from_map(m['executeDetailList'])
-        return self
-
-
-class ListUserReportsResponseBody(TeaModel):
-    def __init__(self, request_id=None, success=None, sql_comparison_report=None):
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-        self.sql_comparison_report = sql_comparison_report  # type: ListUserReportsResponseBodySqlComparisonReport
-
-    def validate(self):
-        if self.sql_comparison_report:
-            self.sql_comparison_report.validate()
-
-    def to_map(self):
-        _map = super(ListUserReportsResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        if self.sql_comparison_report is not None:
-            result['sqlComparisonReport'] = self.sql_comparison_report.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        if m.get('sqlComparisonReport') is not None:
-            temp_model = ListUserReportsResponseBodySqlComparisonReport()
-            self.sql_comparison_report = temp_model.from_map(m['sqlComparisonReport'])
-        return self
-
-
-class ListUserReportsResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: ListUserReportsResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(ListUserReportsResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = ListUserReportsResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
-class ListVersionsRequest(TeaModel):
-    def __init__(self, drds_instance_id=None, drds_ver=None):
-        self.drds_instance_id = drds_instance_id  # type: str
-        self.drds_ver = drds_ver  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ListVersionsRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.drds_instance_id is not None:
-            result['DrdsInstanceId'] = self.drds_instance_id
-        if self.drds_ver is not None:
-            result['DrdsVer'] = self.drds_ver
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DrdsInstanceId') is not None:
-            self.drds_instance_id = m.get('DrdsInstanceId')
-        if m.get('DrdsVer') is not None:
-            self.drds_ver = m.get('DrdsVer')
-        return self
-
-
-class ListVersionsResponseBodyVersionsVersions(TeaModel):
-    def __init__(self, drds_version=None, latest=None):
-        self.drds_version = drds_version  # type: str
-        self.latest = latest  # type: bool
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ListVersionsResponseBodyVersionsVersions, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.drds_version is not None:
-            result['DrdsVersion'] = self.drds_version
-        if self.latest is not None:
-            result['Latest'] = self.latest
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DrdsVersion') is not None:
-            self.drds_version = m.get('DrdsVersion')
-        if m.get('Latest') is not None:
-            self.latest = m.get('Latest')
-        return self
-
-
-class ListVersionsResponseBodyVersions(TeaModel):
-    def __init__(self, versions=None):
-        self.versions = versions  # type: list[ListVersionsResponseBodyVersionsVersions]
-
-    def validate(self):
-        if self.versions:
-            for k in self.versions:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super(ListVersionsResponseBodyVersions, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        result['versions'] = []
-        if self.versions is not None:
-            for k in self.versions:
-                result['versions'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        self.versions = []
-        if m.get('versions') is not None:
-            for k in m.get('versions'):
-                temp_model = ListVersionsResponseBodyVersionsVersions()
-                self.versions.append(temp_model.from_map(k))
-        return self
-
-
-class ListVersionsResponseBody(TeaModel):
-    def __init__(self, request_id=None, success=None, versions=None):
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-        self.versions = versions  # type: ListVersionsResponseBodyVersions
-
-    def validate(self):
-        if self.versions:
-            self.versions.validate()
-
-    def to_map(self):
-        _map = super(ListVersionsResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        if self.versions is not None:
-            result['versions'] = self.versions.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        if m.get('versions') is not None:
-            temp_model = ListVersionsResponseBodyVersions()
-            self.versions = temp_model.from_map(m['versions'])
-        return self
-
-
-class ListVersionsResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: ListVersionsResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(ListVersionsResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = ListVersionsResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class ManagePrivateRdsRequest(TeaModel):
     def __init__(self, dbinstance_id=None, drds_instance_id=None, params=None, rds_action=None, region_id=None):
         self.dbinstance_id = dbinstance_id  # type: str
         self.drds_instance_id = drds_instance_id  # type: str
         self.params = params  # type: str
         self.rds_action = rds_action  # type: str
         self.region_id = region_id  # type: str
@@ -16331,115 +13296,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = ModifyDrdsIpWhiteListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ModifyEventTaskStatusRequest(TeaModel):
-    def __init__(self, event_id=None, ids=None, region=None, switch_time=None):
-        self.event_id = event_id  # type: str
-        self.ids = ids  # type: str
-        self.region = region  # type: str
-        self.switch_time = switch_time  # type: long
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ModifyEventTaskStatusRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.event_id is not None:
-            result['EventId'] = self.event_id
-        if self.ids is not None:
-            result['Ids'] = self.ids
-        if self.region is not None:
-            result['Region'] = self.region
-        if self.switch_time is not None:
-            result['SwitchTime'] = self.switch_time
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('EventId') is not None:
-            self.event_id = m.get('EventId')
-        if m.get('Ids') is not None:
-            self.ids = m.get('Ids')
-        if m.get('Region') is not None:
-            self.region = m.get('Region')
-        if m.get('SwitchTime') is not None:
-            self.switch_time = m.get('SwitchTime')
-        return self
-
-
-class ModifyEventTaskStatusResponseBody(TeaModel):
-    def __init__(self, request_id=None, success=None):
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ModifyEventTaskStatusResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class ModifyEventTaskStatusResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: ModifyEventTaskStatusResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(ModifyEventTaskStatusResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = ModifyEventTaskStatusResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class ModifyPolarDbReadWeightRequest(TeaModel):
     def __init__(self, db_instance_id=None, db_name=None, db_node_ids=None, drds_instance_id=None, weights=None):
         self.db_instance_id = db_instance_id  # type: str
         self.db_name = db_name  # type: str
         self.db_node_ids = db_node_ids  # type: str
         self.drds_instance_id = drds_instance_id  # type: str
         self.weights = weights  # type: str
@@ -16639,399 +13503,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = ModifyRdsReadWeightResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class PreCheckSqlFlashbackTaskRequest(TeaModel):
-    def __init__(self, db_name=None, drds_instance_id=None, end_time=None, start_time=None):
-        self.db_name = db_name  # type: str
-        self.drds_instance_id = drds_instance_id  # type: str
-        self.end_time = end_time  # type: str
-        self.start_time = start_time  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(PreCheckSqlFlashbackTaskRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.db_name is not None:
-            result['DbName'] = self.db_name
-        if self.drds_instance_id is not None:
-            result['DrdsInstanceId'] = self.drds_instance_id
-        if self.end_time is not None:
-            result['EndTime'] = self.end_time
-        if self.start_time is not None:
-            result['StartTime'] = self.start_time
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DbName') is not None:
-            self.db_name = m.get('DbName')
-        if m.get('DrdsInstanceId') is not None:
-            self.drds_instance_id = m.get('DrdsInstanceId')
-        if m.get('EndTime') is not None:
-            self.end_time = m.get('EndTime')
-        if m.get('StartTime') is not None:
-            self.start_time = m.get('StartTime')
-        return self
-
-
-class PreCheckSqlFlashbackTaskResponseBodyCheckResult(TeaModel):
-    def __init__(self, binlog_exists=None, binlog_row_query_event_enabled=None,
-                 can_upgrade_support_binlog_row_query_events=None, has_table=None, support_binlog_row_query_events=None):
-        self.binlog_exists = binlog_exists  # type: bool
-        self.binlog_row_query_event_enabled = binlog_row_query_event_enabled  # type: bool
-        self.can_upgrade_support_binlog_row_query_events = can_upgrade_support_binlog_row_query_events  # type: bool
-        self.has_table = has_table  # type: bool
-        self.support_binlog_row_query_events = support_binlog_row_query_events  # type: bool
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(PreCheckSqlFlashbackTaskResponseBodyCheckResult, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.binlog_exists is not None:
-            result['BinlogExists'] = self.binlog_exists
-        if self.binlog_row_query_event_enabled is not None:
-            result['BinlogRowQueryEventEnabled'] = self.binlog_row_query_event_enabled
-        if self.can_upgrade_support_binlog_row_query_events is not None:
-            result['CanUpgradeSupportBinlogRowQueryEvents'] = self.can_upgrade_support_binlog_row_query_events
-        if self.has_table is not None:
-            result['HasTable'] = self.has_table
-        if self.support_binlog_row_query_events is not None:
-            result['SupportBinlogRowQueryEvents'] = self.support_binlog_row_query_events
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('BinlogExists') is not None:
-            self.binlog_exists = m.get('BinlogExists')
-        if m.get('BinlogRowQueryEventEnabled') is not None:
-            self.binlog_row_query_event_enabled = m.get('BinlogRowQueryEventEnabled')
-        if m.get('CanUpgradeSupportBinlogRowQueryEvents') is not None:
-            self.can_upgrade_support_binlog_row_query_events = m.get('CanUpgradeSupportBinlogRowQueryEvents')
-        if m.get('HasTable') is not None:
-            self.has_table = m.get('HasTable')
-        if m.get('SupportBinlogRowQueryEvents') is not None:
-            self.support_binlog_row_query_events = m.get('SupportBinlogRowQueryEvents')
-        return self
-
-
-class PreCheckSqlFlashbackTaskResponseBody(TeaModel):
-    def __init__(self, check_result=None, request_id=None, success=None):
-        self.check_result = check_result  # type: PreCheckSqlFlashbackTaskResponseBodyCheckResult
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-
-    def validate(self):
-        if self.check_result:
-            self.check_result.validate()
-
-    def to_map(self):
-        _map = super(PreCheckSqlFlashbackTaskResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.check_result is not None:
-            result['CheckResult'] = self.check_result.to_map()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('CheckResult') is not None:
-            temp_model = PreCheckSqlFlashbackTaskResponseBodyCheckResult()
-            self.check_result = temp_model.from_map(m['CheckResult'])
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class PreCheckSqlFlashbackTaskResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: PreCheckSqlFlashbackTaskResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(PreCheckSqlFlashbackTaskResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = PreCheckSqlFlashbackTaskResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
-class PutRestorePreCheckRequest(TeaModel):
-    def __init__(self, backup_db_names=None, backup_id=None, backup_level=None, backup_mode=None,
-                 drds_instance_id=None, preferred_backup_time=None):
-        self.backup_db_names = backup_db_names  # type: str
-        self.backup_id = backup_id  # type: str
-        self.backup_level = backup_level  # type: str
-        self.backup_mode = backup_mode  # type: str
-        self.drds_instance_id = drds_instance_id  # type: str
-        self.preferred_backup_time = preferred_backup_time  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(PutRestorePreCheckRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.backup_db_names is not None:
-            result['BackupDbNames'] = self.backup_db_names
-        if self.backup_id is not None:
-            result['BackupId'] = self.backup_id
-        if self.backup_level is not None:
-            result['BackupLevel'] = self.backup_level
-        if self.backup_mode is not None:
-            result['BackupMode'] = self.backup_mode
-        if self.drds_instance_id is not None:
-            result['DrdsInstanceId'] = self.drds_instance_id
-        if self.preferred_backup_time is not None:
-            result['PreferredBackupTime'] = self.preferred_backup_time
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('BackupDbNames') is not None:
-            self.backup_db_names = m.get('BackupDbNames')
-        if m.get('BackupId') is not None:
-            self.backup_id = m.get('BackupId')
-        if m.get('BackupLevel') is not None:
-            self.backup_level = m.get('BackupLevel')
-        if m.get('BackupMode') is not None:
-            self.backup_mode = m.get('BackupMode')
-        if m.get('DrdsInstanceId') is not None:
-            self.drds_instance_id = m.get('DrdsInstanceId')
-        if m.get('PreferredBackupTime') is not None:
-            self.preferred_backup_time = m.get('PreferredBackupTime')
-        return self
-
-
-class PutRestorePreCheckResponseBodyPrecheckBackupResultListList(TeaModel):
-    def __init__(self, check_fail_reason=None, check_item_content=None, check_item_name=None, check_result=None,
-                 item_id=None, result=None):
-        self.check_fail_reason = check_fail_reason  # type: str
-        self.check_item_content = check_item_content  # type: str
-        self.check_item_name = check_item_name  # type: str
-        self.check_result = check_result  # type: str
-        self.item_id = item_id  # type: long
-        self.result = result  # type: bool
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(PutRestorePreCheckResponseBodyPrecheckBackupResultListList, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.check_fail_reason is not None:
-            result['CheckFailReason'] = self.check_fail_reason
-        if self.check_item_content is not None:
-            result['CheckItemContent'] = self.check_item_content
-        if self.check_item_name is not None:
-            result['CheckItemName'] = self.check_item_name
-        if self.check_result is not None:
-            result['CheckResult'] = self.check_result
-        if self.item_id is not None:
-            result['ItemId'] = self.item_id
-        if self.result is not None:
-            result['Result'] = self.result
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('CheckFailReason') is not None:
-            self.check_fail_reason = m.get('CheckFailReason')
-        if m.get('CheckItemContent') is not None:
-            self.check_item_content = m.get('CheckItemContent')
-        if m.get('CheckItemName') is not None:
-            self.check_item_name = m.get('CheckItemName')
-        if m.get('CheckResult') is not None:
-            self.check_result = m.get('CheckResult')
-        if m.get('ItemId') is not None:
-            self.item_id = m.get('ItemId')
-        if m.get('Result') is not None:
-            self.result = m.get('Result')
-        return self
-
-
-class PutRestorePreCheckResponseBodyPrecheckBackupResultList(TeaModel):
-    def __init__(self, list=None):
-        self.list = list  # type: list[PutRestorePreCheckResponseBodyPrecheckBackupResultListList]
-
-    def validate(self):
-        if self.list:
-            for k in self.list:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super(PutRestorePreCheckResponseBodyPrecheckBackupResultList, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        result['List'] = []
-        if self.list is not None:
-            for k in self.list:
-                result['List'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        self.list = []
-        if m.get('List') is not None:
-            for k in m.get('List'):
-                temp_model = PutRestorePreCheckResponseBodyPrecheckBackupResultListList()
-                self.list.append(temp_model.from_map(k))
-        return self
-
-
-class PutRestorePreCheckResponseBodyPrecheckBackupResult(TeaModel):
-    def __init__(self, list=None, result=None):
-        self.list = list  # type: PutRestorePreCheckResponseBodyPrecheckBackupResultList
-        self.result = result  # type: bool
-
-    def validate(self):
-        if self.list:
-            self.list.validate()
-
-    def to_map(self):
-        _map = super(PutRestorePreCheckResponseBodyPrecheckBackupResult, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.list is not None:
-            result['List'] = self.list.to_map()
-        if self.result is not None:
-            result['Result'] = self.result
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('List') is not None:
-            temp_model = PutRestorePreCheckResponseBodyPrecheckBackupResultList()
-            self.list = temp_model.from_map(m['List'])
-        if m.get('Result') is not None:
-            self.result = m.get('Result')
-        return self
-
-
-class PutRestorePreCheckResponseBody(TeaModel):
-    def __init__(self, precheck_backup_result=None, request_id=None, success=None):
-        self.precheck_backup_result = precheck_backup_result  # type: PutRestorePreCheckResponseBodyPrecheckBackupResult
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-
-    def validate(self):
-        if self.precheck_backup_result:
-            self.precheck_backup_result.validate()
-
-    def to_map(self):
-        _map = super(PutRestorePreCheckResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.precheck_backup_result is not None:
-            result['PrecheckBackupResult'] = self.precheck_backup_result.to_map()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('PrecheckBackupResult') is not None:
-            temp_model = PutRestorePreCheckResponseBodyPrecheckBackupResult()
-            self.precheck_backup_result = temp_model.from_map(m['PrecheckBackupResult'])
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class PutRestorePreCheckResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: PutRestorePreCheckResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(PutRestorePreCheckResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = PutRestorePreCheckResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class PutStartBackupRequest(TeaModel):
     def __init__(self, backup_db_names=None, backup_level=None, backup_mode=None, drds_instance_id=None):
         self.backup_db_names = backup_db_names  # type: str
         self.backup_level = backup_level  # type: str
         self.backup_mode = backup_mode  # type: str
         self.drds_instance_id = drds_instance_id  # type: str
 
@@ -17130,199 +13609,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = PutStartBackupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class RearrangeDbToInstanceRequest(TeaModel):
-    def __init__(self, choose_rds=None, choose_sub_db=None, db_name=None, drds_instance_id=None, instance_list=None,
-                 order_id=None):
-        self.choose_rds = choose_rds  # type: str
-        self.choose_sub_db = choose_sub_db  # type: str
-        self.db_name = db_name  # type: str
-        self.drds_instance_id = drds_instance_id  # type: str
-        self.instance_list = instance_list  # type: list[str]
-        self.order_id = order_id  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(RearrangeDbToInstanceRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.choose_rds is not None:
-            result['ChooseRds'] = self.choose_rds
-        if self.choose_sub_db is not None:
-            result['ChooseSubDb'] = self.choose_sub_db
-        if self.db_name is not None:
-            result['DbName'] = self.db_name
-        if self.drds_instance_id is not None:
-            result['DrdsInstanceId'] = self.drds_instance_id
-        if self.instance_list is not None:
-            result['InstanceList'] = self.instance_list
-        if self.order_id is not None:
-            result['OrderId'] = self.order_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('ChooseRds') is not None:
-            self.choose_rds = m.get('ChooseRds')
-        if m.get('ChooseSubDb') is not None:
-            self.choose_sub_db = m.get('ChooseSubDb')
-        if m.get('DbName') is not None:
-            self.db_name = m.get('DbName')
-        if m.get('DrdsInstanceId') is not None:
-            self.drds_instance_id = m.get('DrdsInstanceId')
-        if m.get('InstanceList') is not None:
-            self.instance_list = m.get('InstanceList')
-        if m.get('OrderId') is not None:
-            self.order_id = m.get('OrderId')
-        return self
-
-
-class RearrangeDbToInstanceResponseBodyDataData(TeaModel):
-    def __init__(self, dst_instance=None, src_db_name=None, src_instance=None):
-        self.dst_instance = dst_instance  # type: str
-        self.src_db_name = src_db_name  # type: str
-        self.src_instance = src_instance  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(RearrangeDbToInstanceResponseBodyDataData, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.dst_instance is not None:
-            result['DstInstance'] = self.dst_instance
-        if self.src_db_name is not None:
-            result['SrcDbName'] = self.src_db_name
-        if self.src_instance is not None:
-            result['SrcInstance'] = self.src_instance
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DstInstance') is not None:
-            self.dst_instance = m.get('DstInstance')
-        if m.get('SrcDbName') is not None:
-            self.src_db_name = m.get('SrcDbName')
-        if m.get('SrcInstance') is not None:
-            self.src_instance = m.get('SrcInstance')
-        return self
-
-
-class RearrangeDbToInstanceResponseBodyData(TeaModel):
-    def __init__(self, data=None):
-        self.data = data  # type: list[RearrangeDbToInstanceResponseBodyDataData]
-
-    def validate(self):
-        if self.data:
-            for k in self.data:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super(RearrangeDbToInstanceResponseBodyData, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        result['data'] = []
-        if self.data is not None:
-            for k in self.data:
-                result['data'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        self.data = []
-        if m.get('data') is not None:
-            for k in m.get('data'):
-                temp_model = RearrangeDbToInstanceResponseBodyDataData()
-                self.data.append(temp_model.from_map(k))
-        return self
-
-
-class RearrangeDbToInstanceResponseBody(TeaModel):
-    def __init__(self, data=None, request_id=None, success=None):
-        self.data = data  # type: RearrangeDbToInstanceResponseBodyData
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-
-    def validate(self):
-        if self.data:
-            self.data.validate()
-
-    def to_map(self):
-        _map = super(RearrangeDbToInstanceResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.data is not None:
-            result['Data'] = self.data.to_map()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Data') is not None:
-            temp_model = RearrangeDbToInstanceResponseBodyData()
-            self.data = temp_model.from_map(m['Data'])
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class RearrangeDbToInstanceResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: RearrangeDbToInstanceResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(RearrangeDbToInstanceResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = RearrangeDbToInstanceResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class RefreshDrdsAtomUrlRequest(TeaModel):
     def __init__(self, db_name=None, drds_instance_id=None):
         self.db_name = db_name  # type: str
         self.drds_instance_id = drds_instance_id  # type: str
 
     def validate(self):
         pass
@@ -17871,156 +14165,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = RemoveDrdsInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class RemoveDrdsMysqlRequest(TeaModel):
-    def __init__(self, db_instance_id=None, db_name=None, drds_instance_id=None, force=None, ro_db_instance_id=None):
-        self.db_instance_id = db_instance_id  # type: str
-        self.db_name = db_name  # type: str
-        self.drds_instance_id = drds_instance_id  # type: str
-        self.force = force  # type: bool
-        self.ro_db_instance_id = ro_db_instance_id  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(RemoveDrdsMysqlRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.db_instance_id is not None:
-            result['DbInstanceId'] = self.db_instance_id
-        if self.db_name is not None:
-            result['DbName'] = self.db_name
-        if self.drds_instance_id is not None:
-            result['DrdsInstanceId'] = self.drds_instance_id
-        if self.force is not None:
-            result['Force'] = self.force
-        if self.ro_db_instance_id is not None:
-            result['RoDbInstanceId'] = self.ro_db_instance_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DbInstanceId') is not None:
-            self.db_instance_id = m.get('DbInstanceId')
-        if m.get('DbName') is not None:
-            self.db_name = m.get('DbName')
-        if m.get('DrdsInstanceId') is not None:
-            self.drds_instance_id = m.get('DrdsInstanceId')
-        if m.get('Force') is not None:
-            self.force = m.get('Force')
-        if m.get('RoDbInstanceId') is not None:
-            self.ro_db_instance_id = m.get('RoDbInstanceId')
-        return self
-
-
-class RemoveDrdsMysqlResponseBodyData(TeaModel):
-    def __init__(self, message=None, result=None):
-        self.message = message  # type: str
-        self.result = result  # type: bool
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(RemoveDrdsMysqlResponseBodyData, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.message is not None:
-            result['Message'] = self.message
-        if self.result is not None:
-            result['Result'] = self.result
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Message') is not None:
-            self.message = m.get('Message')
-        if m.get('Result') is not None:
-            self.result = m.get('Result')
-        return self
-
-
-class RemoveDrdsMysqlResponseBody(TeaModel):
-    def __init__(self, data=None, request_id=None, success=None):
-        self.data = data  # type: RemoveDrdsMysqlResponseBodyData
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-
-    def validate(self):
-        if self.data:
-            self.data.validate()
-
-    def to_map(self):
-        _map = super(RemoveDrdsMysqlResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.data is not None:
-            result['Data'] = self.data.to_map()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Data') is not None:
-            temp_model = RemoveDrdsMysqlResponseBodyData()
-            self.data = temp_model.from_map(m['Data'])
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class RemoveDrdsMysqlResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: RemoveDrdsMysqlResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(RemoveDrdsMysqlResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = RemoveDrdsMysqlResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class RemoveInstanceAccountRequest(TeaModel):
     def __init__(self, account_name=None, drds_instance_id=None):
         self.account_name = account_name  # type: str
         self.drds_instance_id = drds_instance_id  # type: str
 
     def validate(self):
         pass
@@ -19124,323 +15276,14 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = SetupTableResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class SetupTableAsyncRequest(TeaModel):
-    def __init__(self, allow_full_table_scan=None, db_name=None, drds_instance_id=None, region_id=None,
-                 table_name=None):
-        self.allow_full_table_scan = allow_full_table_scan  # type: bool
-        self.db_name = db_name  # type: str
-        self.drds_instance_id = drds_instance_id  # type: str
-        self.region_id = region_id  # type: str
-        self.table_name = table_name  # type: list[str]
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(SetupTableAsyncRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.allow_full_table_scan is not None:
-            result['AllowFullTableScan'] = self.allow_full_table_scan
-        if self.db_name is not None:
-            result['DbName'] = self.db_name
-        if self.drds_instance_id is not None:
-            result['DrdsInstanceId'] = self.drds_instance_id
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
-        if self.table_name is not None:
-            result['TableName'] = self.table_name
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('AllowFullTableScan') is not None:
-            self.allow_full_table_scan = m.get('AllowFullTableScan')
-        if m.get('DbName') is not None:
-            self.db_name = m.get('DbName')
-        if m.get('DrdsInstanceId') is not None:
-            self.drds_instance_id = m.get('DrdsInstanceId')
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
-        if m.get('TableName') is not None:
-            self.table_name = m.get('TableName')
-        return self
-
-
-class SetupTableAsyncResponseBody(TeaModel):
-    def __init__(self, data=None, request_id=None, success=None):
-        self.data = data  # type: str
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(SetupTableAsyncResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.data is not None:
-            result['Data'] = self.data
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Data') is not None:
-            self.data = m.get('Data')
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class SetupTableAsyncResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: SetupTableAsyncResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(SetupTableAsyncResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = SetupTableAsyncResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
-class SqlCompatibilityCancelRequest(TeaModel):
-    def __init__(self, drds_instance_id=None, task_id=None):
-        self.drds_instance_id = drds_instance_id  # type: str
-        self.task_id = task_id  # type: long
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(SqlCompatibilityCancelRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.drds_instance_id is not None:
-            result['DrdsInstanceId'] = self.drds_instance_id
-        if self.task_id is not None:
-            result['TaskId'] = self.task_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DrdsInstanceId') is not None:
-            self.drds_instance_id = m.get('DrdsInstanceId')
-        if m.get('TaskId') is not None:
-            self.task_id = m.get('TaskId')
-        return self
-
-
-class SqlCompatibilityCancelResponseBody(TeaModel):
-    def __init__(self, data=None, request_id=None, success=None):
-        self.data = data  # type: bool
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(SqlCompatibilityCancelResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.data is not None:
-            result['Data'] = self.data
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Data') is not None:
-            self.data = m.get('Data')
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class SqlCompatibilityCancelResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: SqlCompatibilityCancelResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(SqlCompatibilityCancelResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = SqlCompatibilityCancelResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
-class SqlCompatibilityStartRequest(TeaModel):
-    def __init__(self, drds_instance_id=None, performance_test=None, target_version=None):
-        self.drds_instance_id = drds_instance_id  # type: str
-        self.performance_test = performance_test  # type: bool
-        self.target_version = target_version  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(SqlCompatibilityStartRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.drds_instance_id is not None:
-            result['DrdsInstanceId'] = self.drds_instance_id
-        if self.performance_test is not None:
-            result['PerformanceTest'] = self.performance_test
-        if self.target_version is not None:
-            result['TargetVersion'] = self.target_version
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DrdsInstanceId') is not None:
-            self.drds_instance_id = m.get('DrdsInstanceId')
-        if m.get('PerformanceTest') is not None:
-            self.performance_test = m.get('PerformanceTest')
-        if m.get('TargetVersion') is not None:
-            self.target_version = m.get('TargetVersion')
-        return self
-
-
-class SqlCompatibilityStartResponseBody(TeaModel):
-    def __init__(self, data=None, request_id=None, success=None):
-        self.data = data  # type: bool
-        self.request_id = request_id  # type: str
-        self.success = success  # type: bool
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(SqlCompatibilityStartResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.data is not None:
-            result['Data'] = self.data
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Data') is not None:
-            self.data = m.get('Data')
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class SqlCompatibilityStartResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: SqlCompatibilityStartResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(SqlCompatibilityStartResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = SqlCompatibilityStartResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class StartRestoreRequest(TeaModel):
     def __init__(self, backup_db_names=None, backup_id=None, backup_level=None, backup_mode=None,
                  drds_instance_id=None, preferred_backup_time=None):
         self.backup_db_names = backup_db_names  # type: str
         self.backup_id = backup_id  # type: str
         self.backup_level = backup_level  # type: str
         self.backup_mode = backup_mode  # type: str
@@ -21416,234 +17259,7 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = ValidateShardTaskResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class DescribeRdsInstInfosRequest(TeaModel):
-    def __init__(self, page_number=None, page_size=None, search=None):
-        self.page_number = page_number  # type: int
-        self.page_size = page_size  # type: int
-        self.search = search  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeRdsInstInfosRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.page_number is not None:
-            result['PageNumber'] = self.page_number
-        if self.page_size is not None:
-            result['PageSize'] = self.page_size
-        if self.search is not None:
-            result['Search'] = self.search
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('PageNumber') is not None:
-            self.page_number = m.get('PageNumber')
-        if m.get('PageSize') is not None:
-            self.page_size = m.get('PageSize')
-        if m.get('Search') is not None:
-            self.search = m.get('Search')
-        return self
-
-
-class DescribeRdsInstInfosResponseBodyItemsDBInstanceReadOnlyDBInstanceId(TeaModel):
-    def __init__(self, read_only_dbinstance_id=None):
-        self.read_only_dbinstance_id = read_only_dbinstance_id  # type: list[str]
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeRdsInstInfosResponseBodyItemsDBInstanceReadOnlyDBInstanceId, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.read_only_dbinstance_id is not None:
-            result['ReadOnlyDBInstanceId'] = self.read_only_dbinstance_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('ReadOnlyDBInstanceId') is not None:
-            self.read_only_dbinstance_id = m.get('ReadOnlyDBInstanceId')
-        return self
-
-
-class DescribeRdsInstInfosResponseBodyItemsDBInstance(TeaModel):
-    def __init__(self, dbinstance_description=None, dbinstance_id=None, dbinstance_status=None,
-                 dbinstance_type=None, engine=None, engine_version=None, instance_network_type=None, read_only_dbinstance_id=None,
-                 region_id=None, zone_id=None):
-        self.dbinstance_description = dbinstance_description  # type: str
-        self.dbinstance_id = dbinstance_id  # type: str
-        self.dbinstance_status = dbinstance_status  # type: int
-        self.dbinstance_type = dbinstance_type  # type: str
-        self.engine = engine  # type: str
-        self.engine_version = engine_version  # type: str
-        self.instance_network_type = instance_network_type  # type: str
-        self.read_only_dbinstance_id = read_only_dbinstance_id  # type: DescribeRdsInstInfosResponseBodyItemsDBInstanceReadOnlyDBInstanceId
-        self.region_id = region_id  # type: str
-        self.zone_id = zone_id  # type: str
-
-    def validate(self):
-        if self.read_only_dbinstance_id:
-            self.read_only_dbinstance_id.validate()
-
-    def to_map(self):
-        _map = super(DescribeRdsInstInfosResponseBodyItemsDBInstance, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.dbinstance_description is not None:
-            result['DBInstanceDescription'] = self.dbinstance_description
-        if self.dbinstance_id is not None:
-            result['DBInstanceId'] = self.dbinstance_id
-        if self.dbinstance_status is not None:
-            result['DBInstanceStatus'] = self.dbinstance_status
-        if self.dbinstance_type is not None:
-            result['DBInstanceType'] = self.dbinstance_type
-        if self.engine is not None:
-            result['Engine'] = self.engine
-        if self.engine_version is not None:
-            result['EngineVersion'] = self.engine_version
-        if self.instance_network_type is not None:
-            result['InstanceNetworkType'] = self.instance_network_type
-        if self.read_only_dbinstance_id is not None:
-            result['ReadOnlyDBInstanceId'] = self.read_only_dbinstance_id.to_map()
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
-        if self.zone_id is not None:
-            result['ZoneId'] = self.zone_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('DBInstanceDescription') is not None:
-            self.dbinstance_description = m.get('DBInstanceDescription')
-        if m.get('DBInstanceId') is not None:
-            self.dbinstance_id = m.get('DBInstanceId')
-        if m.get('DBInstanceStatus') is not None:
-            self.dbinstance_status = m.get('DBInstanceStatus')
-        if m.get('DBInstanceType') is not None:
-            self.dbinstance_type = m.get('DBInstanceType')
-        if m.get('Engine') is not None:
-            self.engine = m.get('Engine')
-        if m.get('EngineVersion') is not None:
-            self.engine_version = m.get('EngineVersion')
-        if m.get('InstanceNetworkType') is not None:
-            self.instance_network_type = m.get('InstanceNetworkType')
-        if m.get('ReadOnlyDBInstanceId') is not None:
-            temp_model = DescribeRdsInstInfosResponseBodyItemsDBInstanceReadOnlyDBInstanceId()
-            self.read_only_dbinstance_id = temp_model.from_map(m['ReadOnlyDBInstanceId'])
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
-        if m.get('ZoneId') is not None:
-            self.zone_id = m.get('ZoneId')
-        return self
-
-
-class DescribeRdsInstInfosResponseBodyItems(TeaModel):
-    def __init__(self, dbinstance=None):
-        self.dbinstance = dbinstance  # type: list[DescribeRdsInstInfosResponseBodyItemsDBInstance]
-
-    def validate(self):
-        if self.dbinstance:
-            for k in self.dbinstance:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super(DescribeRdsInstInfosResponseBodyItems, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        result['DBInstance'] = []
-        if self.dbinstance is not None:
-            for k in self.dbinstance:
-                result['DBInstance'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        self.dbinstance = []
-        if m.get('DBInstance') is not None:
-            for k in m.get('DBInstance'):
-                temp_model = DescribeRdsInstInfosResponseBodyItemsDBInstance()
-                self.dbinstance.append(temp_model.from_map(k))
-        return self
-
-
-class DescribeRdsInstInfosResponseBody(TeaModel):
-    def __init__(self, items=None, request_id=None):
-        self.items = items  # type: DescribeRdsInstInfosResponseBodyItems
-        self.request_id = request_id  # type: str
-
-    def validate(self):
-        if self.items:
-            self.items.validate()
-
-    def to_map(self):
-        _map = super(DescribeRdsInstInfosResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.items is not None:
-            result['Items'] = self.items.to_map()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Items') is not None:
-            temp_model = DescribeRdsInstInfosResponseBodyItems()
-            self.items = temp_model.from_map(m['Items'])
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        return self
-
-
-class DescribeRdsInstInfosResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: DescribeRdsInstInfosResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(DescribeRdsInstInfosResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('body') is not None:
-            temp_model = DescribeRdsInstInfosResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
```

### Comparing `alibabacloud_drds20190123_py2-1.0.8/README-CN.md` & `alibabacloud_drds20190123_py2-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_drds20190123_py2-1.0.8/setup.py` & `alibabacloud_drds20190123_py2-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_drds20190123_py2.
 
-Created on 07/12/2021
+Created on 07/01/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_drds20190123"
 NAME = "alibabacloud_drds20190123_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Distributed Relational Database Service (20190123) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util_py2>=0.0.5, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.1.0, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.0.7, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.1, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.0.8, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

### Comparing `alibabacloud_drds20190123_py2-1.0.8/ChangeLog.md` & `alibabacloud_drds20190123_py2-1.0.9/ChangeLog.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2021-12-07 Version: 1.0.8
+- Fixed some bugs.
+
 2021-12-06 Version: 1.0.7
 - Fixed some bugs.
 
 2021-11-22 Version: 1.0.6
 - Fixed some bugs.
 
 2021-11-18 Version: 1.0.5
```

