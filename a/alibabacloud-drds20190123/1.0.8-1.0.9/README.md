# Comparing `tmp/alibabacloud_drds20190123-1.0.8.tar.gz` & `tmp/alibabacloud_drds20190123-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_drds20190123-1.0.8.tar", last modified: Mon Nov 22 07:18:00 2021, max compression
+gzip compressed data, was "dist/alibabacloud_drds20190123-1.0.9.tar", last modified: Mon Dec  6 03:22:58 2021, max compression
```

## Comparing `alibabacloud_drds20190123-1.0.8.tar` & `alibabacloud_drds20190123-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-22 07:18:00.000000 alibabacloud_drds20190123-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      884 2021-11-22 07:18:00.000000 alibabacloud_drds20190123-1.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2021-11-22 07:18:00.000000 alibabacloud_drds20190123-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2021-11-22 07:18:00.000000 alibabacloud_drds20190123-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2369 2021-11-22 07:18:00.000000 alibabacloud_drds20190123-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2021-11-22 07:18:00.000000 alibabacloud_drds20190123-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1110 2021-11-22 07:18:00.000000 alibabacloud_drds20190123-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-22 07:18:00.000000 alibabacloud_drds20190123-1.0.8/alibabacloud_drds20190123/
--rw-r--r--   0 root         (0) root         (0)       21 2021-11-22 07:18:00.000000 alibabacloud_drds20190123-1.0.8/alibabacloud_drds20190123/__init__.py
--rw-r--r--   0 root         (0) root         (0)   251823 2021-11-22 07:18:00.000000 alibabacloud_drds20190123-1.0.8/alibabacloud_drds20190123/client.py
--rw-r--r--   0 root         (0) root         (0)   771762 2021-11-22 07:18:00.000000 alibabacloud_drds20190123-1.0.8/alibabacloud_drds20190123/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-22 07:18:00.000000 alibabacloud_drds20190123-1.0.8/alibabacloud_drds20190123.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2369 2021-11-22 07:18:00.000000 alibabacloud_drds20190123-1.0.8/alibabacloud_drds20190123.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2021-11-22 07:18:00.000000 alibabacloud_drds20190123-1.0.8/alibabacloud_drds20190123.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-22 07:18:00.000000 alibabacloud_drds20190123-1.0.8/alibabacloud_drds20190123.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2021-11-22 07:18:00.000000 alibabacloud_drds20190123-1.0.8/alibabacloud_drds20190123.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2021-11-22 07:18:00.000000 alibabacloud_drds20190123-1.0.8/alibabacloud_drds20190123.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2021-11-22 07:18:00.000000 alibabacloud_drds20190123-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2602 2021-11-22 07:18:00.000000 alibabacloud_drds20190123-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-06 03:22:58.000000 alibabacloud_drds20190123-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      930 2021-12-06 03:22:58.000000 alibabacloud_drds20190123-1.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2021-12-06 03:22:58.000000 alibabacloud_drds20190123-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2021-12-06 03:22:58.000000 alibabacloud_drds20190123-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2369 2021-12-06 03:22:58.000000 alibabacloud_drds20190123-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2021-12-06 03:22:58.000000 alibabacloud_drds20190123-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1110 2021-12-06 03:22:58.000000 alibabacloud_drds20190123-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-06 03:22:58.000000 alibabacloud_drds20190123-1.0.9/alibabacloud_drds20190123/
+-rw-r--r--   0 root         (0) root         (0)       21 2021-12-06 03:22:58.000000 alibabacloud_drds20190123-1.0.9/alibabacloud_drds20190123/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   251823 2021-12-06 03:22:58.000000 alibabacloud_drds20190123-1.0.9/alibabacloud_drds20190123/client.py
+-rw-r--r--   0 root         (0) root         (0)   771762 2021-12-06 03:22:58.000000 alibabacloud_drds20190123-1.0.9/alibabacloud_drds20190123/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-06 03:22:58.000000 alibabacloud_drds20190123-1.0.9/alibabacloud_drds20190123.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2369 2021-12-06 03:22:58.000000 alibabacloud_drds20190123-1.0.9/alibabacloud_drds20190123.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2021-12-06 03:22:58.000000 alibabacloud_drds20190123-1.0.9/alibabacloud_drds20190123.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-12-06 03:22:58.000000 alibabacloud_drds20190123-1.0.9/alibabacloud_drds20190123.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      117 2021-12-06 03:22:58.000000 alibabacloud_drds20190123-1.0.9/alibabacloud_drds20190123.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2021-12-06 03:22:58.000000 alibabacloud_drds20190123-1.0.9/alibabacloud_drds20190123.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2021-12-06 03:22:58.000000 alibabacloud_drds20190123-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2603 2021-12-06 03:22:58.000000 alibabacloud_drds20190123-1.0.9/setup.py
```

### Comparing `alibabacloud_drds20190123-1.0.8/ChangeLog.md` & `alibabacloud_drds20190123-1.0.9/ChangeLog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2021-11-22 Version: 1.0.8
+- Fixed some bugs.
+
 2021-11-18 Version: 1.0.7
 - Fixed some bugs.
 
 2021-11-18 Version: 1.0.6
 - Fixed some bugs.
 
 2021-11-17 Version: 1.0.5
```

### Comparing `alibabacloud_drds20190123-1.0.8/LICENSE` & `alibabacloud_drds20190123-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_drds20190123-1.0.8/PKG-INFO` & `alibabacloud_drds20190123-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_drds20190123
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud Distributed Relational Database Service (20190123) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_drds20190123-1.0.8/README-CN.md` & `alibabacloud_drds20190123-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_drds20190123-1.0.8/README.md` & `alibabacloud_drds20190123-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_drds20190123-1.0.8/alibabacloud_drds20190123/client.py` & `alibabacloud_drds20190123-1.0.9/alibabacloud_drds20190123/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_drds20190123-1.0.8/alibabacloud_drds20190123/models.py` & `alibabacloud_drds20190123-1.0.9/alibabacloud_drds20190123/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_drds20190123-1.0.8/alibabacloud_drds20190123.egg-info/PKG-INFO` & `alibabacloud_drds20190123-1.0.9/alibabacloud_drds20190123.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-drds20190123
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud Distributed Relational Database Service (20190123) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_drds20190123-1.0.8/setup.py` & `alibabacloud_drds20190123-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_drds20190123.
 
-Created on 22/11/2021
+Created on 06/12/2021
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_drds20190123"
 NAME = "alibabacloud_drds20190123" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Distributed Relational Database Service (20190123) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.5, <1.0.0",
-    "alibabacloud_tea_openapi>=0.2.7, <1.0.0",
+    "alibabacloud_tea_openapi>=0.2.10, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

