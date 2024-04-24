# Comparing `tmp/alibabacloud_polardb20170801_py2-4.0.8.tar.gz` & `tmp/alibabacloud_polardb20170801_py2-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_polardb20170801_py2-4.0.8.tar", last modified: Thu Apr 18 17:12:33 2024, max compression
+gzip compressed data, was "dist/alibabacloud_polardb20170801_py2-4.1.0.tar", last modified: Wed Apr 24 01:47:36 2024, max compression
```

## Comparing `alibabacloud_polardb20170801_py2-4.0.8.tar` & `alibabacloud_polardb20170801_py2-4.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/
--rw-r--r--   0 root         (0) root         (0)     4281 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2509 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1045 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1128 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801/__init__.py
--rw-r--r--   0 root         (0) root         (0)   318134 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801/client.py
--rw-r--r--   0 root         (0) root         (0)  1223147 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2509 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2936 2024-04-18 17:12:33.000000 alibabacloud_polardb20170801_py2-4.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 01:47:36.000000 alibabacloud_polardb20170801_py2-4.1.0/
+-rw-r--r--   0 root         (0) root         (0)     4429 2024-04-24 01:47:36.000000 alibabacloud_polardb20170801_py2-4.1.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-24 01:47:36.000000 alibabacloud_polardb20170801_py2-4.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-24 01:47:36.000000 alibabacloud_polardb20170801_py2-4.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2509 2024-04-24 01:47:36.000000 alibabacloud_polardb20170801_py2-4.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1045 2024-04-24 01:47:36.000000 alibabacloud_polardb20170801_py2-4.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-04-24 01:47:36.000000 alibabacloud_polardb20170801_py2-4.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 01:47:36.000000 alibabacloud_polardb20170801_py2-4.1.0/alibabacloud_polardb20170801/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-24 01:47:36.000000 alibabacloud_polardb20170801_py2-4.1.0/alibabacloud_polardb20170801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   319716 2024-04-24 01:47:36.000000 alibabacloud_polardb20170801_py2-4.1.0/alibabacloud_polardb20170801/client.py
+-rw-r--r--   0 root         (0) root         (0)  1227553 2024-04-24 01:47:36.000000 alibabacloud_polardb20170801_py2-4.1.0/alibabacloud_polardb20170801/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 01:47:36.000000 alibabacloud_polardb20170801_py2-4.1.0/alibabacloud_polardb20170801_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2509 2024-04-24 01:47:36.000000 alibabacloud_polardb20170801_py2-4.1.0/alibabacloud_polardb20170801_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2024-04-24 01:47:36.000000 alibabacloud_polardb20170801_py2-4.1.0/alibabacloud_polardb20170801_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 01:47:36.000000 alibabacloud_polardb20170801_py2-4.1.0/alibabacloud_polardb20170801_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-24 01:47:36.000000 alibabacloud_polardb20170801_py2-4.1.0/alibabacloud_polardb20170801_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-24 01:47:36.000000 alibabacloud_polardb20170801_py2-4.1.0/alibabacloud_polardb20170801_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-24 01:47:36.000000 alibabacloud_polardb20170801_py2-4.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2936 2024-04-24 01:47:36.000000 alibabacloud_polardb20170801_py2-4.1.0/setup.py
```

### Comparing `alibabacloud_polardb20170801_py2-4.0.8/ChangeLog.md` & `alibabacloud_polardb20170801_py2-4.1.0/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2024-04-18 Version: 4.0.8
+- Update API DescribeDBClusterAttribute: update response param.
+- Update API DescribeDBClusters: update response param.
+
+
 2024-04-09 Version: 4.0.7
 - Update API DescribeDBClusters: update response param.
 
 
 2024-04-09 Version: 4.0.7
 - Update API DescribeDBClusters: update response param.
```

### Comparing `alibabacloud_polardb20170801_py2-4.0.8/LICENSE` & `alibabacloud_polardb20170801_py2-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_polardb20170801_py2-4.0.8/PKG-INFO` & `alibabacloud_polardb20170801_py2-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_polardb20170801_py2
-Version: 4.0.8
+Version: 4.1.0
 Summary: Alibaba Cloud ApsaraDB for POLARDB (20170801) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_polardb20170801_py2-4.0.8/README-CN.md` & `alibabacloud_polardb20170801_py2-4.1.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_polardb20170801_py2-4.0.8/README.md` & `alibabacloud_polardb20170801_py2-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801/client.py` & `alibabacloud_polardb20170801_py2-4.1.0/alibabacloud_polardb20170801/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -6530,14 +6530,52 @@
             self.call_api(params, req, runtime)
         )
 
     def reset_global_database_network(self, request):
         runtime = util_models.RuntimeOptions()
         return self.reset_global_database_network_with_options(request, runtime)
 
+    def restart_dblink_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dbcluster_id):
+            query['DBClusterId'] = request.dbcluster_id
+        if not UtilClient.is_unset(request.owner_account):
+            query['OwnerAccount'] = request.owner_account
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='RestartDBLink',
+            version='2017-08-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            polardb_20170801_models.RestartDBLinkResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def restart_dblink(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.restart_dblink_with_options(request, runtime)
+
     def restart_dbnode_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbnode_id):
             query['DBNodeId'] = request.dbnode_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
```

### Comparing `alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801/models.py` & `alibabacloud_polardb20170801_py2-4.1.0/alibabacloud_polardb20170801/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -27119,14 +27119,134 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ResetGlobalDatabaseNetworkResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class RestartDBLinkRequest(TeaModel):
+    def __init__(self, dbcluster_id=None, owner_account=None, owner_id=None, resource_owner_account=None,
+                 resource_owner_id=None, security_token=None):
+        self.dbcluster_id = dbcluster_id  # type: str
+        self.owner_account = owner_account  # type: str
+        self.owner_id = owner_id  # type: long
+        self.resource_owner_account = resource_owner_account  # type: str
+        self.resource_owner_id = resource_owner_id  # type: long
+        self.security_token = security_token  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(RestartDBLinkRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dbcluster_id is not None:
+            result['DBClusterId'] = self.dbcluster_id
+        if self.owner_account is not None:
+            result['OwnerAccount'] = self.owner_account
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.resource_owner_account is not None:
+            result['ResourceOwnerAccount'] = self.resource_owner_account
+        if self.resource_owner_id is not None:
+            result['ResourceOwnerId'] = self.resource_owner_id
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DBClusterId') is not None:
+            self.dbcluster_id = m.get('DBClusterId')
+        if m.get('OwnerAccount') is not None:
+            self.owner_account = m.get('OwnerAccount')
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('ResourceOwnerAccount') is not None:
+            self.resource_owner_account = m.get('ResourceOwnerAccount')
+        if m.get('ResourceOwnerId') is not None:
+            self.resource_owner_id = m.get('ResourceOwnerId')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        return self
+
+
+class RestartDBLinkResponseBody(TeaModel):
+    def __init__(self, dbcluster_id=None, request_id=None, task_id=None):
+        self.dbcluster_id = dbcluster_id  # type: str
+        self.request_id = request_id  # type: str
+        self.task_id = task_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(RestartDBLinkResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dbcluster_id is not None:
+            result['DBClusterId'] = self.dbcluster_id
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.task_id is not None:
+            result['TaskId'] = self.task_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DBClusterId') is not None:
+            self.dbcluster_id = m.get('DBClusterId')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TaskId') is not None:
+            self.task_id = m.get('TaskId')
+        return self
+
+
+class RestartDBLinkResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: RestartDBLinkResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(RestartDBLinkResponse, self).to_map()
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
+            temp_model = RestartDBLinkResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class RestartDBNodeRequest(TeaModel):
     def __init__(self, dbnode_id=None, owner_account=None, owner_id=None, resource_owner_account=None,
                  resource_owner_id=None):
         # The ID of the node.
         # 
         # >  You can call the [DescribeDBClusters](~~185342~~) operation to query the details of all clusters that belong to your Alibaba Cloud account, such as cluster IDs.
         self.dbnode_id = dbnode_id  # type: str
```

### Comparing `alibabacloud_polardb20170801_py2-4.0.8/alibabacloud_polardb20170801_py2.egg-info/PKG-INFO` & `alibabacloud_polardb20170801_py2-4.1.0/alibabacloud_polardb20170801_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-polardb20170801-py2
-Version: 4.0.8
+Version: 4.1.0
 Summary: Alibaba Cloud ApsaraDB for POLARDB (20170801) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_polardb20170801_py2-4.0.8/setup.py` & `alibabacloud_polardb20170801_py2-4.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_polardb20170801_py2.
 
-Created on 18/04/2024
+Created on 24/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_polardb20170801"
 NAME = "alibabacloud_polardb20170801_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ApsaraDB for POLARDB (20170801) SDK Library for Python2"
```

