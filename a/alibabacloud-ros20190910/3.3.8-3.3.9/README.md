# Comparing `tmp/alibabacloud_ros20190910-3.3.8.tar.gz` & `tmp/alibabacloud_ros20190910-3.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ros20190910-3.3.8.tar", last modified: Wed Feb 21 17:14:18 2024, max compression
+gzip compressed data, was "dist/alibabacloud_ros20190910-3.3.9.tar", last modified: Thu Feb 29 09:18:01 2024, max compression
```

## Comparing `alibabacloud_ros20190910-3.3.8.tar` & `alibabacloud_ros20190910-3.3.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 17:14:18.000000 alibabacloud_ros20190910-3.3.8/
--rw-r--r--   0 root         (0) root         (0)     8072 2024-02-21 17:14:18.000000 alibabacloud_ros20190910-3.3.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-02-21 17:14:18.000000 alibabacloud_ros20190910-3.3.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-21 17:14:18.000000 alibabacloud_ros20190910-3.3.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2428 2024-02-21 17:14:18.000000 alibabacloud_ros20190910-3.3.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1095 2024-02-21 17:14:18.000000 alibabacloud_ros20190910-3.3.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1180 2024-02-21 17:14:18.000000 alibabacloud_ros20190910-3.3.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 17:14:18.000000 alibabacloud_ros20190910-3.3.8/alibabacloud_ros20190910/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-21 17:14:18.000000 alibabacloud_ros20190910-3.3.8/alibabacloud_ros20190910/__init__.py
--rw-r--r--   0 root         (0) root         (0)   447545 2024-02-21 17:14:18.000000 alibabacloud_ros20190910-3.3.8/alibabacloud_ros20190910/client.py
--rw-r--r--   0 root         (0) root         (0)   989323 2024-02-21 17:14:18.000000 alibabacloud_ros20190910-3.3.8/alibabacloud_ros20190910/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 17:14:18.000000 alibabacloud_ros20190910-3.3.8/alibabacloud_ros20190910.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2428 2024-02-21 17:14:18.000000 alibabacloud_ros20190910-3.3.8/alibabacloud_ros20190910.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2024-02-21 17:14:18.000000 alibabacloud_ros20190910-3.3.8/alibabacloud_ros20190910.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-21 17:14:18.000000 alibabacloud_ros20190910-3.3.8/alibabacloud_ros20190910.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-02-21 17:14:18.000000 alibabacloud_ros20190910-3.3.8/alibabacloud_ros20190910.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-02-21 17:14:18.000000 alibabacloud_ros20190910-3.3.8/alibabacloud_ros20190910.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-21 17:14:18.000000 alibabacloud_ros20190910-3.3.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2638 2024-02-21 17:14:18.000000 alibabacloud_ros20190910-3.3.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 09:18:01.000000 alibabacloud_ros20190910-3.3.9/
+-rw-r--r--   0 root         (0) root         (0)     8209 2024-02-29 09:18:01.000000 alibabacloud_ros20190910-3.3.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-02-29 09:18:01.000000 alibabacloud_ros20190910-3.3.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-02-29 09:18:01.000000 alibabacloud_ros20190910-3.3.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2428 2024-02-29 09:18:01.000000 alibabacloud_ros20190910-3.3.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-02-29 09:18:01.000000 alibabacloud_ros20190910-3.3.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-02-29 09:18:01.000000 alibabacloud_ros20190910-3.3.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 09:18:01.000000 alibabacloud_ros20190910-3.3.9/alibabacloud_ros20190910/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-02-29 09:18:01.000000 alibabacloud_ros20190910-3.3.9/alibabacloud_ros20190910/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   447545 2024-02-29 09:18:01.000000 alibabacloud_ros20190910-3.3.9/alibabacloud_ros20190910/client.py
+-rw-r--r--   0 root         (0) root         (0)   989721 2024-02-29 09:18:01.000000 alibabacloud_ros20190910-3.3.9/alibabacloud_ros20190910/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-29 09:18:01.000000 alibabacloud_ros20190910-3.3.9/alibabacloud_ros20190910.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2428 2024-02-29 09:18:01.000000 alibabacloud_ros20190910-3.3.9/alibabacloud_ros20190910.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-02-29 09:18:01.000000 alibabacloud_ros20190910-3.3.9/alibabacloud_ros20190910.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-29 09:18:01.000000 alibabacloud_ros20190910-3.3.9/alibabacloud_ros20190910.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-02-29 09:18:01.000000 alibabacloud_ros20190910-3.3.9/alibabacloud_ros20190910.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-02-29 09:18:01.000000 alibabacloud_ros20190910-3.3.9/alibabacloud_ros20190910.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-02-29 09:18:01.000000 alibabacloud_ros20190910-3.3.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2638 2024-02-29 09:18:01.000000 alibabacloud_ros20190910-3.3.9/setup.py
```

### Comparing `alibabacloud_ros20190910-3.3.8/ChangeLog.md` & `alibabacloud_ros20190910-3.3.9/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2024-02-21 Version: 3.3.8
+- Update API GetStackInstance: add param OutputOption.
+- Update API GetStackInstance: update response param.
+
+
 2024-02-21 Version: 3.3.7
 - Generated python 2019-09-10 for ROS.
 
 2024-01-30 Version: 3.3.6
 - Update API DeleteStackInstancesupdate DeploymentTargets param.
```

### Comparing `alibabacloud_ros20190910-3.3.8/LICENSE` & `alibabacloud_ros20190910-3.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ros20190910-3.3.8/PKG-INFO` & `alibabacloud_ros20190910-3.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ros20190910
-Version: 3.3.8
+Version: 3.3.9
 Summary: Alibaba Cloud Resource Orchestration Service (20190910) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ros20190910-3.3.8/README-CN.md` & `alibabacloud_ros20190910-3.3.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ros20190910-3.3.8/README.md` & `alibabacloud_ros20190910-3.3.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ros20190910-3.3.8/alibabacloud_ros20190910/client.py` & `alibabacloud_ros20190910-3.3.9/alibabacloud_ros20190910/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_ros20190910-3.3.8/alibabacloud_ros20190910/models.py` & `alibabacloud_ros20190910-3.3.9/alibabacloud_ros20190910/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8930,14 +8930,15 @@
         parameters: List[GetStackResponseBodyParameters] = None,
         parent_stack_id: str = None,
         ram_role_name: str = None,
         region_id: str = None,
         request_id: str = None,
         resource_group_id: str = None,
         resource_progress: GetStackResponseBodyResourceProgress = None,
+        rollback_failed_root_reason: str = None,
         root_stack_id: str = None,
         service_managed: bool = None,
         service_name: str = None,
         stack_drift_status: str = None,
         stack_id: str = None,
         stack_name: str = None,
         stack_type: str = None,
@@ -9010,14 +9011,15 @@
         self.region_id = region_id
         # The ID of the request.
         self.request_id = request_id
         # The ID of the resource group to which the instances belong.
         self.resource_group_id = resource_group_id
         # The creation progress of resources.
         self.resource_progress = resource_progress
+        self.rollback_failed_root_reason = rollback_failed_root_reason
         # The ID of the root stack. This parameter is returned if the specified stack is a nested stack.
         self.root_stack_id = root_stack_id
         # Indicates whether the stack is a managed stack. Valid values: 
         # 
         # - true
         # - false
         self.service_managed = service_managed
@@ -9158,14 +9160,16 @@
             result['RegionId'] = self.region_id
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
         if self.resource_progress is not None:
             result['ResourceProgress'] = self.resource_progress.to_map()
+        if self.rollback_failed_root_reason is not None:
+            result['RollbackFailedRootReason'] = self.rollback_failed_root_reason
         if self.root_stack_id is not None:
             result['RootStackId'] = self.root_stack_id
         if self.service_managed is not None:
             result['ServiceManaged'] = self.service_managed
         if self.service_name is not None:
             result['ServiceName'] = self.service_name
         if self.stack_drift_status is not None:
@@ -9244,14 +9248,16 @@
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         if m.get('ResourceProgress') is not None:
             temp_model = GetStackResponseBodyResourceProgress()
             self.resource_progress = temp_model.from_map(m['ResourceProgress'])
+        if m.get('RollbackFailedRootReason') is not None:
+            self.rollback_failed_root_reason = m.get('RollbackFailedRootReason')
         if m.get('RootStackId') is not None:
             self.root_stack_id = m.get('RootStackId')
         if m.get('ServiceManaged') is not None:
             self.service_managed = m.get('ServiceManaged')
         if m.get('ServiceName') is not None:
             self.service_name = m.get('ServiceName')
         if m.get('StackDriftStatus') is not None:
```

### Comparing `alibabacloud_ros20190910-3.3.8/alibabacloud_ros20190910.egg-info/PKG-INFO` & `alibabacloud_ros20190910-3.3.9/alibabacloud_ros20190910.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ros20190910
-Version: 3.3.8
+Version: 3.3.9
 Summary: Alibaba Cloud Resource Orchestration Service (20190910) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ros20190910-3.3.8/setup.py` & `alibabacloud_ros20190910-3.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ros20190910.
 
-Created on 21/02/2024
+Created on 29/02/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ros20190910"
 NAME = "alibabacloud_ros20190910" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Resource Orchestration Service (20190910) SDK Library for Python"
```

