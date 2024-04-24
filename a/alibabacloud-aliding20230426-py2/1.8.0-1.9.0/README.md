# Comparing `tmp/alibabacloud_aliding20230426_py2-1.8.0.tar.gz` & `tmp/alibabacloud_aliding20230426_py2-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aliding20230426_py2-1.8.0.tar", last modified: Mon Feb 26 12:06:14 2024, max compression
+gzip compressed data, was "dist/alibabacloud_aliding20230426_py2-1.9.0.tar", last modified: Mon Feb 26 12:31:45 2024, max compression
```

## Comparing `alibabacloud_aliding20230426_py2-1.8.0.tar` & `alibabacloud_aliding20230426_py2-1.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 12:06:14.000000 alibabacloud_aliding20230426_py2-1.8.0/
--rw-r--r--   0 root         (0) root         (0)      937 2024-02-26 12:06:13.000000 alibabacloud_aliding20230426_py2-1.8.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-02-26 12:06:13.000000 alibabacloud_aliding20230426_py2-1.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-02-26 12:06:13.000000 alibabacloud_aliding20230426_py2-1.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2496 2024-02-26 12:06:14.000000 alibabacloud_aliding20230426_py2-1.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1045 2024-02-26 12:06:13.000000 alibabacloud_aliding20230426_py2-1.8.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1128 2024-02-26 12:06:13.000000 alibabacloud_aliding20230426_py2-1.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 12:06:14.000000 alibabacloud_aliding20230426_py2-1.8.0/alibabacloud_aliding20230426/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-26 12:06:13.000000 alibabacloud_aliding20230426_py2-1.8.0/alibabacloud_aliding20230426/__init__.py
--rw-r--r--   0 root         (0) root         (0)   451032 2024-02-26 12:06:13.000000 alibabacloud_aliding20230426_py2-1.8.0/alibabacloud_aliding20230426/client.py
--rw-r--r--   0 root         (0) root         (0)  2064315 2024-02-26 12:06:13.000000 alibabacloud_aliding20230426_py2-1.8.0/alibabacloud_aliding20230426/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 12:06:14.000000 alibabacloud_aliding20230426_py2-1.8.0/alibabacloud_aliding20230426_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2496 2024-02-26 12:06:13.000000 alibabacloud_aliding20230426_py2-1.8.0/alibabacloud_aliding20230426_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2024-02-26 12:06:14.000000 alibabacloud_aliding20230426_py2-1.8.0/alibabacloud_aliding20230426_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-26 12:06:13.000000 alibabacloud_aliding20230426_py2-1.8.0/alibabacloud_aliding20230426_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-02-26 12:06:13.000000 alibabacloud_aliding20230426_py2-1.8.0/alibabacloud_aliding20230426_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-26 12:06:13.000000 alibabacloud_aliding20230426_py2-1.8.0/alibabacloud_aliding20230426_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-26 12:06:14.000000 alibabacloud_aliding20230426_py2-1.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2923 2024-02-26 12:06:13.000000 alibabacloud_aliding20230426_py2-1.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 12:31:45.000000 alibabacloud_aliding20230426_py2-1.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1456 2024-02-26 12:31:45.000000 alibabacloud_aliding20230426_py2-1.9.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-02-26 12:31:45.000000 alibabacloud_aliding20230426_py2-1.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-02-26 12:31:45.000000 alibabacloud_aliding20230426_py2-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2496 2024-02-26 12:31:45.000000 alibabacloud_aliding20230426_py2-1.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1045 2024-02-26 12:31:45.000000 alibabacloud_aliding20230426_py2-1.9.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-02-26 12:31:45.000000 alibabacloud_aliding20230426_py2-1.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 12:31:45.000000 alibabacloud_aliding20230426_py2-1.9.0/alibabacloud_aliding20230426/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-02-26 12:31:45.000000 alibabacloud_aliding20230426_py2-1.9.0/alibabacloud_aliding20230426/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   451032 2024-02-26 12:31:45.000000 alibabacloud_aliding20230426_py2-1.9.0/alibabacloud_aliding20230426/client.py
+-rw-r--r--   0 root         (0) root         (0)  2064315 2024-02-26 12:31:45.000000 alibabacloud_aliding20230426_py2-1.9.0/alibabacloud_aliding20230426/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 12:31:45.000000 alibabacloud_aliding20230426_py2-1.9.0/alibabacloud_aliding20230426_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2496 2024-02-26 12:31:45.000000 alibabacloud_aliding20230426_py2-1.9.0/alibabacloud_aliding20230426_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2024-02-26 12:31:45.000000 alibabacloud_aliding20230426_py2-1.9.0/alibabacloud_aliding20230426_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-26 12:31:45.000000 alibabacloud_aliding20230426_py2-1.9.0/alibabacloud_aliding20230426_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-02-26 12:31:45.000000 alibabacloud_aliding20230426_py2-1.9.0/alibabacloud_aliding20230426_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-02-26 12:31:45.000000 alibabacloud_aliding20230426_py2-1.9.0/alibabacloud_aliding20230426_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-02-26 12:31:45.000000 alibabacloud_aliding20230426_py2-1.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2923 2024-02-26 12:31:45.000000 alibabacloud_aliding20230426_py2-1.9.0/setup.py
```

### Comparing `alibabacloud_aliding20230426_py2-1.8.0/LICENSE` & `alibabacloud_aliding20230426_py2-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aliding20230426_py2-1.8.0/PKG-INFO` & `alibabacloud_aliding20230426_py2-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_aliding20230426_py2
-Version: 1.8.0
+Version: 1.9.0
 Summary: Alibaba Cloud aliding (20230426) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aliding20230426_py2-1.8.0/README-CN.md` & `alibabacloud_aliding20230426_py2-1.9.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aliding20230426_py2-1.8.0/README.md` & `alibabacloud_aliding20230426_py2-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aliding20230426_py2-1.8.0/alibabacloud_aliding20230426/client.py` & `alibabacloud_aliding20230426_py2-1.9.0/alibabacloud_aliding20230426/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_aliding20230426_py2-1.8.0/alibabacloud_aliding20230426/models.py` & `alibabacloud_aliding20230426_py2-1.9.0/alibabacloud_aliding20230426/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_aliding20230426_py2-1.8.0/alibabacloud_aliding20230426_py2.egg-info/PKG-INFO` & `alibabacloud_aliding20230426_py2-1.9.0/alibabacloud_aliding20230426_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-aliding20230426-py2
-Version: 1.8.0
+Version: 1.9.0
 Summary: Alibaba Cloud aliding (20230426) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aliding20230426_py2-1.8.0/setup.py` & `alibabacloud_aliding20230426_py2-1.9.0/setup.py`

 * *Files identical despite different names*

