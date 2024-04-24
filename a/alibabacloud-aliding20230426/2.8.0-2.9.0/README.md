# Comparing `tmp/alibabacloud_aliding20230426-2.8.0.tar.gz` & `tmp/alibabacloud_aliding20230426-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aliding20230426-2.8.0.tar", last modified: Mon Feb 26 12:32:14 2024, max compression
+gzip compressed data, was "dist/alibabacloud_aliding20230426-2.9.0.tar", last modified: Tue Feb 27 02:08:33 2024, max compression
```

## Comparing `alibabacloud_aliding20230426-2.8.0.tar` & `alibabacloud_aliding20230426-2.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 12:32:14.000000 alibabacloud_aliding20230426-2.8.0/
--rw-r--r--   0 root         (0) root         (0)     2145 2024-02-26 12:32:14.000000 alibabacloud_aliding20230426-2.8.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-02-26 12:32:14.000000 alibabacloud_aliding20230426-2.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-26 12:32:14.000000 alibabacloud_aliding20230426-2.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2429 2024-02-26 12:32:14.000000 alibabacloud_aliding20230426-2.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1111 2024-02-26 12:32:14.000000 alibabacloud_aliding20230426-2.8.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1196 2024-02-26 12:32:14.000000 alibabacloud_aliding20230426-2.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 12:32:14.000000 alibabacloud_aliding20230426-2.8.0/alibabacloud_aliding20230426/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-26 12:32:14.000000 alibabacloud_aliding20230426-2.8.0/alibabacloud_aliding20230426/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1030031 2024-02-26 12:32:14.000000 alibabacloud_aliding20230426-2.8.0/alibabacloud_aliding20230426/client.py
--rw-r--r--   0 root         (0) root         (0)  2047077 2024-02-26 12:32:14.000000 alibabacloud_aliding20230426-2.8.0/alibabacloud_aliding20230426/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 12:32:14.000000 alibabacloud_aliding20230426-2.8.0/alibabacloud_aliding20230426.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2429 2024-02-26 12:32:14.000000 alibabacloud_aliding20230426-2.8.0/alibabacloud_aliding20230426.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2024-02-26 12:32:14.000000 alibabacloud_aliding20230426-2.8.0/alibabacloud_aliding20230426.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-26 12:32:14.000000 alibabacloud_aliding20230426-2.8.0/alibabacloud_aliding20230426.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-02-26 12:32:14.000000 alibabacloud_aliding20230426-2.8.0/alibabacloud_aliding20230426.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-26 12:32:14.000000 alibabacloud_aliding20230426-2.8.0/alibabacloud_aliding20230426.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-26 12:32:14.000000 alibabacloud_aliding20230426-2.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2631 2024-02-26 12:32:14.000000 alibabacloud_aliding20230426-2.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 02:08:33.000000 alibabacloud_aliding20230426-2.9.0/
+-rw-r--r--   0 root         (0) root         (0)     2664 2024-02-27 02:08:33.000000 alibabacloud_aliding20230426-2.9.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-02-27 02:08:33.000000 alibabacloud_aliding20230426-2.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-02-27 02:08:33.000000 alibabacloud_aliding20230426-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2429 2024-02-27 02:08:33.000000 alibabacloud_aliding20230426-2.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1111 2024-02-27 02:08:33.000000 alibabacloud_aliding20230426-2.9.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-02-27 02:08:33.000000 alibabacloud_aliding20230426-2.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 02:08:33.000000 alibabacloud_aliding20230426-2.9.0/alibabacloud_aliding20230426/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-02-27 02:08:33.000000 alibabacloud_aliding20230426-2.9.0/alibabacloud_aliding20230426/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1030031 2024-02-27 02:08:33.000000 alibabacloud_aliding20230426-2.9.0/alibabacloud_aliding20230426/client.py
+-rw-r--r--   0 root         (0) root         (0)  2047077 2024-02-27 02:08:33.000000 alibabacloud_aliding20230426-2.9.0/alibabacloud_aliding20230426/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 02:08:33.000000 alibabacloud_aliding20230426-2.9.0/alibabacloud_aliding20230426.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2429 2024-02-27 02:08:33.000000 alibabacloud_aliding20230426-2.9.0/alibabacloud_aliding20230426.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2024-02-27 02:08:33.000000 alibabacloud_aliding20230426-2.9.0/alibabacloud_aliding20230426.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 02:08:33.000000 alibabacloud_aliding20230426-2.9.0/alibabacloud_aliding20230426.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-02-27 02:08:33.000000 alibabacloud_aliding20230426-2.9.0/alibabacloud_aliding20230426.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-02-27 02:08:33.000000 alibabacloud_aliding20230426-2.9.0/alibabacloud_aliding20230426.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-02-27 02:08:33.000000 alibabacloud_aliding20230426-2.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2631 2024-02-27 02:08:33.000000 alibabacloud_aliding20230426-2.9.0/setup.py
```

### Comparing `alibabacloud_aliding20230426-2.8.0/ChangeLog.md` & `alibabacloud_aliding20230426-2.9.0/ChangeLog.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+2024-02-26 Version: 2.8.0
+- Support API CheckUserIsGroupMember.
+- Support API ExpandGroupCapacity.
+- Support API GetConversaionSpace.
+- Support API GetFileDownloadInfo.
+- Support API GetInnerGroupMembers.
+- Support API GetNewestInnerGroups.
+- Support API GetRelatedWorkspaces.
+- Support API ListDentries.
+- Support API SearchInnerGroups.
+- Support API UpdateScheduleConfSettings.
+- Update API QueryScheduleConference: add param scheduleConferenceId.
+- Update API QueryScheduleConference: update param AccountContext.
+
+
 2024-02-26 Version: 2.7.0
 - Support API CheckUserIsGroupMember.
 - Support API ExpandGroupCapacity.
 - Support API GetConversaionSpace.
 - Support API GetFileDownloadInfo.
 - Support API GetInnerGroupMembers.
 - Support API GetNewestInnerGroups.
```

### Comparing `alibabacloud_aliding20230426-2.8.0/LICENSE` & `alibabacloud_aliding20230426-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aliding20230426-2.8.0/PKG-INFO` & `alibabacloud_aliding20230426-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_aliding20230426
-Version: 2.8.0
+Version: 2.9.0
 Summary: Alibaba Cloud aliding (20230426) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aliding20230426-2.8.0/README-CN.md` & `alibabacloud_aliding20230426-2.9.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aliding20230426-2.8.0/README.md` & `alibabacloud_aliding20230426-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aliding20230426-2.8.0/alibabacloud_aliding20230426/client.py` & `alibabacloud_aliding20230426-2.9.0/alibabacloud_aliding20230426/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_aliding20230426-2.8.0/alibabacloud_aliding20230426/models.py` & `alibabacloud_aliding20230426-2.9.0/alibabacloud_aliding20230426/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_aliding20230426-2.8.0/alibabacloud_aliding20230426.egg-info/PKG-INFO` & `alibabacloud_aliding20230426-2.9.0/alibabacloud_aliding20230426.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-aliding20230426
-Version: 2.8.0
+Version: 2.9.0
 Summary: Alibaba Cloud aliding (20230426) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aliding20230426-2.8.0/setup.py` & `alibabacloud_aliding20230426-2.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_aliding20230426.
 
-Created on 26/02/2024
+Created on 27/02/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_aliding20230426"
 NAME = "alibabacloud_aliding20230426" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud aliding (20230426) SDK Library for Python"
```

