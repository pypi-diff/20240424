# Comparing `tmp/dnv-onecompute-9.2.0.0.tar.gz` & `tmp/dnv-onecompute-9.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnv-onecompute-9.2.0.0.tar", last modified: Fri Mar 15 09:50:34 2024, max compression
+gzip compressed data, was "dnv-onecompute-9.3.0.tar", last modified: Fri Apr 12 10:03:44 2024, max compression
```

## Comparing `dnv-onecompute-9.2.0.0.tar` & `dnv-onecompute-9.3.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-03-15 09:50:34.629139 dnv-onecompute-9.2.0.0/
--rw-rw-rw-   0        0        0     1076 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/LICENSE
--rw-rw-rw-   0        0        0       80 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6639 2024-03-15 09:50:34.629139 dnv-onecompute-9.2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4179 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/README.md
--rw-rw-rw-   0        0        0     2003 2024-03-15 09:50:24.000000 dnv-onecompute-9.2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-15 09:50:34.629139 dnv-onecompute-9.2.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-15 09:50:34.613158 dnv-onecompute-9.2.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-15 09:50:34.613158 dnv-onecompute-9.2.0.0/src/dnv/
--rw-rw-rw-   0        0        0        0 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:50:34.629139 dnv-onecompute-9.2.0.0/src/dnv/onecompute/
--rw-rw-rw-   0        0        0      517 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/__init__.py
--rw-rw-rw-   0        0        0     8909 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/authenticator.py
--rw-rw-rw-   0        0        0    20206 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/azure_blob_storage_file_service.py
--rw-rw-rw-   0        0        0     4605 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/bearer_auth.py
--rw-rw-rw-   0        0        0     2699 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/enums.py
--rw-rw-rw-   0        0        0      584 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/environment.py
--rw-rw-rw-   0        0        0      838 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/event.py
--rw-rw-rw-   0        0        0     6728 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/file_service.py
--rw-rw-rw-   0        0        0      921 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/file_specification.py
--rw-rw-rw-   0        0        0    20372 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/flowmodel.py
--rw-rw-rw-   0        0        0    15577 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/host_file_service.py
--rw-rw-rw-   0        0        0    11255 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/http_retry_transport.py
--rw-rw-rw-   0        0        0     3733 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/httpx_client.py
--rw-rw-rw-   0        0        0      463 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/job_info.py
--rw-rw-rw-   0        0        0     6735 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/job_monitor.py
--rw-rw-rw-   0        0        0     2164 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/json_utils.py
--rw-rw-rw-   0        0        0    19084 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/local_workflow_runtime_service_manager.py
--rw-rw-rw-   0        0        0    24977 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/one_compute_client.py
--rw-rw-rw-   0        0        0     2259 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/one_compute_webapi.py
--rw-rw-rw-   0        0        0      486 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/result.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:50:34.629139 dnv-onecompute-9.2.0.0/src/dnv/onecompute/utils/
--rw-rw-rw-   0        0        0        0 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/utils/__init__.py
--rw-rw-rw-   0        0        0     4301 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/utils/_file_service.py
--rw-rw-rw-   0        0        0     2490 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/utils/_file_size.py
--rw-rw-rw-   0        0        0     3175 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/utils/_progress_reporter.py
--rw-rw-rw-   0        0        0     2994 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/utils/md5_calculator.py
--rw-rw-rw-   0        0        0     2103 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/web_apis_template.py
--rw-rw-rw-   0        0        0      642 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/work_item_info.py
--rw-rw-rw-   0        0        0      813 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/work_item_properties.py
--rw-rw-rw-   0        0        0      332 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/work_item_storage_info.py
--rw-rw-rw-   0        0        0     1120 2024-03-15 09:48:46.000000 dnv-onecompute-9.2.0.0/src/dnv/onecompute/work_status.py
-drwxrwxrwx   0        0        0        0 2024-03-15 09:50:34.629139 dnv-onecompute-9.2.0.0/src/dnv_onecompute.egg-info/
--rw-rw-rw-   0        0        0     6639 2024-03-15 09:50:34.000000 dnv-onecompute-9.2.0.0/src/dnv_onecompute.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1421 2024-03-15 09:50:34.000000 dnv-onecompute-9.2.0.0/src/dnv_onecompute.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-15 09:50:34.000000 dnv-onecompute-9.2.0.0/src/dnv_onecompute.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      212 2024-03-15 09:50:34.000000 dnv-onecompute-9.2.0.0/src/dnv_onecompute.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-03-15 09:50:34.000000 dnv-onecompute-9.2.0.0/src/dnv_onecompute.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 10:03:44.240692 dnv-onecompute-9.3.0/
+-rw-rw-rw-   0        0        0     1076 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/LICENSE
+-rw-rw-rw-   0        0        0       80 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6637 2024-04-12 10:03:44.240692 dnv-onecompute-9.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4179 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/README.md
+-rw-rw-rw-   0        0        0     2001 2024-04-12 10:03:37.000000 dnv-onecompute-9.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 10:03:44.240692 dnv-onecompute-9.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 10:03:44.209444 dnv-onecompute-9.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 10:03:44.209444 dnv-onecompute-9.3.0/src/dnv/
+-rw-rw-rw-   0        0        0        0 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 10:03:44.225068 dnv-onecompute-9.3.0/src/dnv/onecompute/
+-rw-rw-rw-   0        0        0      517 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/__init__.py
+-rw-rw-rw-   0        0        0     8909 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/authenticator.py
+-rw-rw-rw-   0        0        0    20206 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/azure_blob_storage_file_service.py
+-rw-rw-rw-   0        0        0     4605 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/bearer_auth.py
+-rw-rw-rw-   0        0        0     2699 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/enums.py
+-rw-rw-rw-   0        0        0      584 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/environment.py
+-rw-rw-rw-   0        0        0      838 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/event.py
+-rw-rw-rw-   0        0        0     6728 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/file_service.py
+-rw-rw-rw-   0        0        0      921 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/file_specification.py
+-rw-rw-rw-   0        0        0    20372 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/flowmodel.py
+-rw-rw-rw-   0        0        0    15577 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/host_file_service.py
+-rw-rw-rw-   0        0        0    11255 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/http_retry_transport.py
+-rw-rw-rw-   0        0        0     3733 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/httpx_client.py
+-rw-rw-rw-   0        0        0      463 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/job_info.py
+-rw-rw-rw-   0        0        0     6735 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/job_monitor.py
+-rw-rw-rw-   0        0        0     2164 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/json_utils.py
+-rw-rw-rw-   0        0        0    19084 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/local_workflow_runtime_service_manager.py
+-rw-rw-rw-   0        0        0    24977 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/one_compute_client.py
+-rw-rw-rw-   0        0        0     2259 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/one_compute_webapi.py
+-rw-rw-rw-   0        0        0      486 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/result.py
+drwxrwxrwx   0        0        0        0 2024-04-12 10:03:44.225068 dnv-onecompute-9.3.0/src/dnv/onecompute/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/utils/__init__.py
+-rw-rw-rw-   0        0        0     4301 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/utils/_file_service.py
+-rw-rw-rw-   0        0        0     2490 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/utils/_file_size.py
+-rw-rw-rw-   0        0        0     3175 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/utils/_progress_reporter.py
+-rw-rw-rw-   0        0        0     2994 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/utils/md5_calculator.py
+-rw-rw-rw-   0        0        0     2103 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/web_apis_template.py
+-rw-rw-rw-   0        0        0      642 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/work_item_info.py
+-rw-rw-rw-   0        0        0      813 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/work_item_properties.py
+-rw-rw-rw-   0        0        0      332 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/work_item_storage_info.py
+-rw-rw-rw-   0        0        0     1120 2024-04-12 10:01:30.000000 dnv-onecompute-9.3.0/src/dnv/onecompute/work_status.py
+drwxrwxrwx   0        0        0        0 2024-04-12 10:03:44.240692 dnv-onecompute-9.3.0/src/dnv_onecompute.egg-info/
+-rw-rw-rw-   0        0        0     6637 2024-04-12 10:03:44.000000 dnv-onecompute-9.3.0/src/dnv_onecompute.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1421 2024-04-12 10:03:44.000000 dnv-onecompute-9.3.0/src/dnv_onecompute.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 10:03:44.000000 dnv-onecompute-9.3.0/src/dnv_onecompute.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      212 2024-04-12 10:03:44.000000 dnv-onecompute-9.3.0/src/dnv_onecompute.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-12 10:03:44.000000 dnv-onecompute-9.3.0/src/dnv_onecompute.egg-info/top_level.txt
```

### Comparing `dnv-onecompute-9.2.0.0/LICENSE` & `dnv-onecompute-9.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/PKG-INFO` & `dnv-onecompute-9.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnv-onecompute
-Version: 9.2.0.0
+Version: 9.3.0
 Summary: Python package for seamless integration with OneCompute Platform. Streamline job management, workflows, and file operations using intuitive REST APIs. Monitor job progress and efficiently handle file uploads and downloads.
 Author-email: DNV AS <software.support@dnv.com>
 License: MIT License
         Copyright (c) 2024 DNV AS
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `dnv-onecompute-9.2.0.0/README.md` & `dnv-onecompute-9.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/pyproject.toml` & `dnv-onecompute-9.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dnv-onecompute"
-version = "9.2.0.0"
+version = "9.3.0"
 authors = [
     {name = "DNV AS", email = "software.support@dnv.com"},
 ]
 description = "Python package for seamless integration with OneCompute Platform. Streamline job management, workflows, and file operations using intuitive REST APIs. Monitor job progress and efficiently handle file uploads and downloads."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["onecompute", "workflow"]
```

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/__init__.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/__init__.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/authenticator.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/authenticator.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/azure_blob_storage_file_service.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/azure_blob_storage_file_service.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/bearer_auth.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/bearer_auth.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/enums.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/enums.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/environment.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/environment.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/event.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/event.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/file_service.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/file_service.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/file_specification.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/file_specification.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/flowmodel.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/flowmodel.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/host_file_service.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/host_file_service.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/http_retry_transport.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/http_retry_transport.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/httpx_client.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/httpx_client.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/job_monitor.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/job_monitor.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/json_utils.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/json_utils.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/local_workflow_runtime_service_manager.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/local_workflow_runtime_service_manager.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/one_compute_client.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/one_compute_client.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/one_compute_webapi.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/one_compute_webapi.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/utils/_file_service.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/utils/_file_service.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/utils/_file_size.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/utils/_file_size.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/utils/_progress_reporter.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/utils/_progress_reporter.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/utils/md5_calculator.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/utils/md5_calculator.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/web_apis_template.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/web_apis_template.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/work_item_info.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/work_item_info.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/work_item_properties.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/work_item_properties.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv/onecompute/work_status.py` & `dnv-onecompute-9.3.0/src/dnv/onecompute/work_status.py`

 * *Files identical despite different names*

### Comparing `dnv-onecompute-9.2.0.0/src/dnv_onecompute.egg-info/PKG-INFO` & `dnv-onecompute-9.3.0/src/dnv_onecompute.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnv-onecompute
-Version: 9.2.0.0
+Version: 9.3.0
 Summary: Python package for seamless integration with OneCompute Platform. Streamline job management, workflows, and file operations using intuitive REST APIs. Monitor job progress and efficiently handle file uploads and downloads.
 Author-email: DNV AS <software.support@dnv.com>
 License: MIT License
         Copyright (c) 2024 DNV AS
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `dnv-onecompute-9.2.0.0/src/dnv_onecompute.egg-info/SOURCES.txt` & `dnv-onecompute-9.3.0/src/dnv_onecompute.egg-info/SOURCES.txt`

 * *Files identical despite different names*

