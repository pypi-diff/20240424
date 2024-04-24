# Comparing `tmp/alibabacloud_tablestore20201209-1.0.0.tar.gz` & `tmp/alibabacloud_tablestore20201209-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_tablestore20201209-1.0.0.tar", last modified: Thu Jan 25 04:45:53 2024, max compression
+gzip compressed data, was "dist/alibabacloud_tablestore20201209-1.0.1.tar", last modified: Wed Apr 24 09:03:04 2024, max compression
```

## Comparing `alibabacloud_tablestore20201209-1.0.0.tar` & `alibabacloud_tablestore20201209-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-25 04:45:53.000000 alibabacloud_tablestore20201209-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2024-01-25 04:45:52.000000 alibabacloud_tablestore20201209-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-01-25 04:45:52.000000 alibabacloud_tablestore20201209-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2370 2024-01-25 04:45:53.000000 alibabacloud_tablestore20201209-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1043 2024-01-25 04:45:52.000000 alibabacloud_tablestore20201209-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1128 2024-01-25 04:45:52.000000 alibabacloud_tablestore20201209-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-25 04:45:53.000000 alibabacloud_tablestore20201209-1.0.0/alibabacloud_tablestore20201209/
--rw-r--r--   0 root         (0) root         (0)       21 2024-01-25 04:45:52.000000 alibabacloud_tablestore20201209-1.0.0/alibabacloud_tablestore20201209/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36902 2024-01-25 04:45:52.000000 alibabacloud_tablestore20201209-1.0.0/alibabacloud_tablestore20201209/client.py
--rw-r--r--   0 root         (0) root         (0)    54781 2024-01-25 04:45:52.000000 alibabacloud_tablestore20201209-1.0.0/alibabacloud_tablestore20201209/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-25 04:45:53.000000 alibabacloud_tablestore20201209-1.0.0/alibabacloud_tablestore20201209.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2370 2024-01-25 04:45:53.000000 alibabacloud_tablestore20201209-1.0.0/alibabacloud_tablestore20201209.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      463 2024-01-25 04:45:53.000000 alibabacloud_tablestore20201209-1.0.0/alibabacloud_tablestore20201209.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-25 04:45:53.000000 alibabacloud_tablestore20201209-1.0.0/alibabacloud_tablestore20201209.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-01-25 04:45:53.000000 alibabacloud_tablestore20201209-1.0.0/alibabacloud_tablestore20201209.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-01-25 04:45:53.000000 alibabacloud_tablestore20201209-1.0.0/alibabacloud_tablestore20201209.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-01-25 04:45:53.000000 alibabacloud_tablestore20201209-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2646 2024-01-25 04:45:52.000000 alibabacloud_tablestore20201209-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:03:04.000000 alibabacloud_tablestore20201209-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-24 09:03:04.000000 alibabacloud_tablestore20201209-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-24 09:03:04.000000 alibabacloud_tablestore20201209-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-24 09:03:04.000000 alibabacloud_tablestore20201209-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-04-24 09:03:04.000000 alibabacloud_tablestore20201209-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-04-24 09:03:04.000000 alibabacloud_tablestore20201209-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1208 2024-04-24 09:03:04.000000 alibabacloud_tablestore20201209-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:03:04.000000 alibabacloud_tablestore20201209-1.0.1/alibabacloud_tablestore20201209/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-24 09:03:04.000000 alibabacloud_tablestore20201209-1.0.1/alibabacloud_tablestore20201209/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37170 2024-04-24 09:03:04.000000 alibabacloud_tablestore20201209-1.0.1/alibabacloud_tablestore20201209/client.py
+-rw-r--r--   0 root         (0) root         (0)    53814 2024-04-24 09:03:04.000000 alibabacloud_tablestore20201209-1.0.1/alibabacloud_tablestore20201209/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:03:04.000000 alibabacloud_tablestore20201209-1.0.1/alibabacloud_tablestore20201209.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-04-24 09:03:04.000000 alibabacloud_tablestore20201209-1.0.1/alibabacloud_tablestore20201209.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      476 2024-04-24 09:03:04.000000 alibabacloud_tablestore20201209-1.0.1/alibabacloud_tablestore20201209.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 09:03:04.000000 alibabacloud_tablestore20201209-1.0.1/alibabacloud_tablestore20201209.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-24 09:03:04.000000 alibabacloud_tablestore20201209-1.0.1/alibabacloud_tablestore20201209.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-04-24 09:03:04.000000 alibabacloud_tablestore20201209-1.0.1/alibabacloud_tablestore20201209.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-24 09:03:04.000000 alibabacloud_tablestore20201209-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2646 2024-04-24 09:03:04.000000 alibabacloud_tablestore20201209-1.0.1/setup.py
```

### Comparing `alibabacloud_tablestore20201209-1.0.0/LICENSE` & `alibabacloud_tablestore20201209-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_tablestore20201209-1.0.0/PKG-INFO` & `alibabacloud_tablestore20201209-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_tablestore20201209
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud Tablestore (20201209) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/tablestore-20201209/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_tablestore20201209-1.0.0/README-CN.md` & `alibabacloud_tablestore20201209-1.0.1/README-CN.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## 使用说明
 
 [快速使用](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-CN.md#%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8)
 
 ## 发行说明
 
-每个版本的详细更改记录在[发行说明](./ChangeLog.md)中。
+每个版本的详细更改记录在[发行说明](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/tablestore-20201209/ChangeLog.md)中。
 
 ## 相关
 
 - [最新源码](https://github.com/aliyun/alibabacloud-python-sdk/)
 
 ## 许可证
```

### Comparing `alibabacloud_tablestore20201209-1.0.0/README.md` & `alibabacloud_tablestore20201209-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Usage
 
 [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
 
 ## Changelog
 
-Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/tablestore-20201209/ChangeLog.md).
 
 ## References
 
 - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
 
 ## License
```

### Comparing `alibabacloud_tablestore20201209-1.0.0/alibabacloud_tablestore20201209/client.py` & `alibabacloud_tablestore20201209-1.0.1/alibabacloud_tablestore20201209/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,16 @@
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> tablestore_20201209_models.CreateInstanceResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.cluster_type):
             body['ClusterType'] = request.cluster_type
+        if not UtilClient.is_unset(request.disable_replication):
+            body['DisableReplication'] = request.disable_replication
         if not UtilClient.is_unset(request.instance_description):
             body['InstanceDescription'] = request.instance_description
         if not UtilClient.is_unset(request.instance_name):
             body['InstanceName'] = request.instance_name
         if not UtilClient.is_unset(request.network):
             body['Network'] = request.network
         if not UtilClient.is_unset(request.network_source_acl):
@@ -173,14 +175,16 @@
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> tablestore_20201209_models.CreateInstanceResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.cluster_type):
             body['ClusterType'] = request.cluster_type
+        if not UtilClient.is_unset(request.disable_replication):
+            body['DisableReplication'] = request.disable_replication
         if not UtilClient.is_unset(request.instance_description):
             body['InstanceDescription'] = request.instance_description
         if not UtilClient.is_unset(request.instance_name):
             body['InstanceName'] = request.instance_name
         if not UtilClient.is_unset(request.network):
             body['Network'] = request.network
         if not UtilClient.is_unset(request.network_source_acl):
```

### Comparing `alibabacloud_tablestore20201209-1.0.0/alibabacloud_tablestore20201209/models.py` & `alibabacloud_tablestore20201209-1.0.1/alibabacloud_tablestore20201209/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,17 +72,14 @@
         body: ChangeResourceGroupResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -141,24 +138,26 @@
         return self
 
 
 class CreateInstanceRequest(TeaModel):
     def __init__(
         self,
         cluster_type: str = None,
+        disable_replication: bool = None,
         instance_description: str = None,
         instance_name: str = None,
         network: str = None,
         network_source_acl: List[str] = None,
         network_type_acl: List[str] = None,
         policy: str = None,
         resource_group_id: str = None,
         tags: List[CreateInstanceRequestTags] = None,
     ):
         self.cluster_type = cluster_type
+        self.disable_replication = disable_replication
         self.instance_description = instance_description
         self.instance_name = instance_name
         self.network = network
         self.network_source_acl = network_source_acl
         self.network_type_acl = network_type_acl
         self.policy = policy
         self.resource_group_id = resource_group_id
@@ -174,14 +173,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.cluster_type is not None:
             result['ClusterType'] = self.cluster_type
+        if self.disable_replication is not None:
+            result['DisableReplication'] = self.disable_replication
         if self.instance_description is not None:
             result['InstanceDescription'] = self.instance_description
         if self.instance_name is not None:
             result['InstanceName'] = self.instance_name
         if self.network is not None:
             result['Network'] = self.network
         if self.network_source_acl is not None:
@@ -198,14 +199,16 @@
                 result['Tags'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ClusterType') is not None:
             self.cluster_type = m.get('ClusterType')
+        if m.get('DisableReplication') is not None:
+            self.disable_replication = m.get('DisableReplication')
         if m.get('InstanceDescription') is not None:
             self.instance_description = m.get('InstanceDescription')
         if m.get('InstanceName') is not None:
             self.instance_name = m.get('InstanceName')
         if m.get('Network') is not None:
             self.network = m.get('Network')
         if m.get('NetworkSourceACL') is not None:
@@ -271,17 +274,14 @@
         body: CreateInstanceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -369,17 +369,14 @@
         body: DeleteInstanceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -514,17 +511,14 @@
         body: DescribeRegionsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -576,41 +570,53 @@
             self.instance_name = m.get('InstanceName')
         return self
 
 
 class GetInstanceResponseBodyTags(TeaModel):
     def __init__(
         self,
+        key: str = None,
         tag_key: str = None,
         tag_value: str = None,
+        value: str = None,
     ):
+        self.key = key
         self.tag_key = tag_key
         self.tag_value = tag_value
+        self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
         if self.tag_key is not None:
             result['TagKey'] = self.tag_key
         if self.tag_value is not None:
             result['TagValue'] = self.tag_value
+        if self.value is not None:
+            result['Value'] = self.value
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
         if m.get('TagKey') is not None:
             self.tag_key = m.get('TagKey')
         if m.get('TagValue') is not None:
             self.tag_value = m.get('TagValue')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
         return self
 
 
 class GetInstanceResponseBody(TeaModel):
     def __init__(
         self,
         alias_name: str = None,
@@ -773,17 +779,14 @@
         body: GetInstanceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1020,17 +1023,14 @@
         body: ListInstancesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1305,17 +1305,14 @@
         body: ListTagResourcesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1456,17 +1453,14 @@
         body: TagResourcesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1572,17 +1566,14 @@
         body: UntagResourcesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1700,17 +1691,14 @@
         body: UpdateInstanceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
```

### Comparing `alibabacloud_tablestore20201209-1.0.0/alibabacloud_tablestore20201209.egg-info/PKG-INFO` & `alibabacloud_tablestore20201209-1.0.1/alibabacloud_tablestore20201209.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-tablestore20201209
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud Tablestore (20201209) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/tablestore-20201209/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_tablestore20201209-1.0.0/setup.py` & `alibabacloud_tablestore20201209-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_tablestore20201209.
 
-Created on 25/01/2024
+Created on 24/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_tablestore20201209"
 NAME = "alibabacloud_tablestore20201209" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Tablestore (20201209) SDK Library for Python"
```

