# Comparing `tmp/alibabacloud_tablestore20201209_py2-1.0.0.tar.gz` & `tmp/alibabacloud_tablestore20201209_py2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_tablestore20201209_py2-1.0.0.tar", last modified: Thu Jan 25 04:44:51 2024, max compression
+gzip compressed data, was "dist/alibabacloud_tablestore20201209_py2-1.0.1.tar", last modified: Wed Apr 24 09:02:33 2024, max compression
```

## Comparing `alibabacloud_tablestore20201209_py2-1.0.0.tar` & `alibabacloud_tablestore20201209_py2-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-25 04:44:51.000000 alibabacloud_tablestore20201209_py2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      588 2024-01-25 04:44:50.000000 alibabacloud_tablestore20201209_py2-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-01-25 04:44:50.000000 alibabacloud_tablestore20201209_py2-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2514 2024-01-25 04:44:51.000000 alibabacloud_tablestore20201209_py2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1054 2024-01-25 04:44:50.000000 alibabacloud_tablestore20201209_py2-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1137 2024-01-25 04:44:50.000000 alibabacloud_tablestore20201209_py2-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-25 04:44:51.000000 alibabacloud_tablestore20201209_py2-1.0.0/alibabacloud_tablestore20201209/
--rw-r--r--   0 root         (0) root         (0)       21 2024-01-25 04:44:50.000000 alibabacloud_tablestore20201209_py2-1.0.0/alibabacloud_tablestore20201209/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15713 2024-01-25 04:44:50.000000 alibabacloud_tablestore20201209_py2-1.0.0/alibabacloud_tablestore20201209/client.py
--rw-r--r--   0 root         (0) root         (0)    54902 2024-01-25 04:44:50.000000 alibabacloud_tablestore20201209_py2-1.0.0/alibabacloud_tablestore20201209/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-25 04:44:51.000000 alibabacloud_tablestore20201209_py2-1.0.0/alibabacloud_tablestore20201209_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2514 2024-01-25 04:44:51.000000 alibabacloud_tablestore20201209_py2-1.0.0/alibabacloud_tablestore20201209_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      483 2024-01-25 04:44:51.000000 alibabacloud_tablestore20201209_py2-1.0.0/alibabacloud_tablestore20201209_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-25 04:44:51.000000 alibabacloud_tablestore20201209_py2-1.0.0/alibabacloud_tablestore20201209_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-01-25 04:44:51.000000 alibabacloud_tablestore20201209_py2-1.0.0/alibabacloud_tablestore20201209_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-01-25 04:44:51.000000 alibabacloud_tablestore20201209_py2-1.0.0/alibabacloud_tablestore20201209_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-01-25 04:44:51.000000 alibabacloud_tablestore20201209_py2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2938 2024-01-25 04:44:50.000000 alibabacloud_tablestore20201209_py2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:02:33.000000 alibabacloud_tablestore20201209_py2-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       74 2024-04-24 09:02:32.000000 alibabacloud_tablestore20201209_py2-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-24 09:02:32.000000 alibabacloud_tablestore20201209_py2-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-24 09:02:32.000000 alibabacloud_tablestore20201209_py2-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2514 2024-04-24 09:02:33.000000 alibabacloud_tablestore20201209_py2-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-04-24 09:02:32.000000 alibabacloud_tablestore20201209_py2-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1137 2024-04-24 09:02:32.000000 alibabacloud_tablestore20201209_py2-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:02:33.000000 alibabacloud_tablestore20201209_py2-1.0.1/alibabacloud_tablestore20201209/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-24 09:02:32.000000 alibabacloud_tablestore20201209_py2-1.0.1/alibabacloud_tablestore20201209/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15847 2024-04-24 09:02:32.000000 alibabacloud_tablestore20201209_py2-1.0.1/alibabacloud_tablestore20201209/client.py
+-rw-r--r--   0 root         (0) root         (0)    53946 2024-04-24 09:02:32.000000 alibabacloud_tablestore20201209_py2-1.0.1/alibabacloud_tablestore20201209/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:02:33.000000 alibabacloud_tablestore20201209_py2-1.0.1/alibabacloud_tablestore20201209_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2514 2024-04-24 09:02:33.000000 alibabacloud_tablestore20201209_py2-1.0.1/alibabacloud_tablestore20201209_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      496 2024-04-24 09:02:33.000000 alibabacloud_tablestore20201209_py2-1.0.1/alibabacloud_tablestore20201209_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 09:02:33.000000 alibabacloud_tablestore20201209_py2-1.0.1/alibabacloud_tablestore20201209_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-24 09:02:33.000000 alibabacloud_tablestore20201209_py2-1.0.1/alibabacloud_tablestore20201209_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-04-24 09:02:33.000000 alibabacloud_tablestore20201209_py2-1.0.1/alibabacloud_tablestore20201209_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-24 09:02:33.000000 alibabacloud_tablestore20201209_py2-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2938 2024-04-24 09:02:32.000000 alibabacloud_tablestore20201209_py2-1.0.1/setup.py
```

### Comparing `alibabacloud_tablestore20201209_py2-1.0.0/LICENSE` & `alibabacloud_tablestore20201209_py2-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_tablestore20201209_py2-1.0.0/PKG-INFO` & `alibabacloud_tablestore20201209_py2-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_tablestore20201209_py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud Tablestore (20201209) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_tablestore20201209_py2-1.0.0/README-CN.md` & `alibabacloud_tablestore20201209_py2-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_tablestore20201209_py2-1.0.0/README.md` & `alibabacloud_tablestore20201209_py2-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_tablestore20201209_py2-1.0.0/alibabacloud_tablestore20201209/client.py` & `alibabacloud_tablestore20201209_py2-1.0.1/alibabacloud_tablestore20201209/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,16 @@
         return self.change_resource_group_with_options(request, headers, runtime)
 
     def create_instance_with_options(self, request, headers, runtime):
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

### Comparing `alibabacloud_tablestore20201209_py2-1.0.0/alibabacloud_tablestore20201209/models.py` & `alibabacloud_tablestore20201209_py2-1.0.1/alibabacloud_tablestore20201209/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,17 +59,14 @@
 class ChangeResourceGroupResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ChangeResourceGroupResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ChangeResourceGroupResponse, self).to_map()
         if _map is not None:
             return _map
@@ -121,17 +118,19 @@
             self.key = m.get('Key')
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class CreateInstanceRequest(TeaModel):
-    def __init__(self, cluster_type=None, instance_description=None, instance_name=None, network=None,
-                 network_source_acl=None, network_type_acl=None, policy=None, resource_group_id=None, tags=None):
+    def __init__(self, cluster_type=None, disable_replication=None, instance_description=None, instance_name=None,
+                 network=None, network_source_acl=None, network_type_acl=None, policy=None, resource_group_id=None,
+                 tags=None):
         self.cluster_type = cluster_type  # type: str
+        self.disable_replication = disable_replication  # type: bool
         self.instance_description = instance_description  # type: str
         self.instance_name = instance_name  # type: str
         self.network = network  # type: str
         self.network_source_acl = network_source_acl  # type: list[str]
         self.network_type_acl = network_type_acl  # type: list[str]
         self.policy = policy  # type: str
         self.resource_group_id = resource_group_id  # type: str
@@ -147,14 +146,16 @@
         _map = super(CreateInstanceRequest, self).to_map()
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
@@ -171,14 +172,16 @@
                 result['Tags'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m=None):
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
@@ -234,17 +237,14 @@
 class CreateInstanceResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CreateInstanceResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateInstanceResponse, self).to_map()
         if _map is not None:
             return _map
@@ -321,17 +321,14 @@
 class DeleteInstanceResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DeleteInstanceResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteInstanceResponse, self).to_map()
         if _map is not None:
             return _map
@@ -450,17 +447,14 @@
 class DescribeRegionsResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DescribeRegionsResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeRegionsResponse, self).to_map()
         if _map is not None:
             return _map
@@ -507,39 +501,49 @@
         m = m or dict()
         if m.get('InstanceName') is not None:
             self.instance_name = m.get('InstanceName')
         return self
 
 
 class GetInstanceResponseBodyTags(TeaModel):
-    def __init__(self, tag_key=None, tag_value=None):
+    def __init__(self, key=None, tag_key=None, tag_value=None, value=None):
+        self.key = key  # type: str
         self.tag_key = tag_key  # type: str
         self.tag_value = tag_value  # type: str
+        self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetInstanceResponseBodyTags, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, alias_name=None, create_time=None, instance_description=None, instance_name=None,
                  instance_specification=None, instance_status=None, network=None, network_source_acl=None, network_type_acl=None,
                  payment_type=None, policy=None, policy_version=None, region_id=None, request_id=None, resource_group_id=None,
@@ -677,17 +681,14 @@
 class GetInstanceResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetInstanceResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetInstanceResponse, self).to_map()
         if _map is not None:
             return _map
@@ -893,17 +894,14 @@
 class ListInstancesResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListInstancesResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListInstancesResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1144,17 +1142,14 @@
 class ListTagResourcesResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListTagResourcesResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListTagResourcesResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1278,17 +1273,14 @@
 class TagResourcesResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: TagResourcesResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(TagResourcesResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1380,17 +1372,14 @@
 class UntagResourcesResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: UntagResourcesResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(UntagResourcesResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1493,17 +1482,14 @@
 class UpdateInstanceResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: UpdateInstanceResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(UpdateInstanceResponse, self).to_map()
         if _map is not None:
             return _map
```

### Comparing `alibabacloud_tablestore20201209_py2-1.0.0/alibabacloud_tablestore20201209_py2.egg-info/PKG-INFO` & `alibabacloud_tablestore20201209_py2-1.0.1/alibabacloud_tablestore20201209_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-tablestore20201209-py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud Tablestore (20201209) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_tablestore20201209_py2-1.0.0/setup.py` & `alibabacloud_tablestore20201209_py2-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_tablestore20201209_py2.
 
-Created on 25/01/2024
+Created on 24/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_tablestore20201209"
 NAME = "alibabacloud_tablestore20201209_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Tablestore (20201209) SDK Library for Python2"
```

