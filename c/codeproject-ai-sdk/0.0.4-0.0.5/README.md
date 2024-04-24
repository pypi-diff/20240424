# Comparing `tmp/codeproject_ai_sdk-0.0.4.tar.gz` & `tmp/codeproject_ai_sdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeproject_ai_sdk-0.0.4.tar", last modified: Wed Apr 24 14:21:46 2024, max compression
+gzip compressed data, was "codeproject_ai_sdk-0.0.5.tar", last modified: Wed Apr 24 15:07:31 2024, max compression
```

## Comparing `codeproject_ai_sdk-0.0.4.tar` & `codeproject_ai_sdk-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 14:21:46.069189 codeproject_ai_sdk-0.0.4/
--rw-rw-rw-   0        0        0      985 2024-04-24 14:21:46.069189 codeproject_ai_sdk-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-04-24 13:58:44.000000 codeproject_ai_sdk-0.0.4/README.md
--rw-rw-rw-   0        0        0      860 2024-04-24 14:20:57.000000 codeproject_ai_sdk-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-24 14:21:46.069189 codeproject_ai_sdk-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-24 14:21:45.931091 codeproject_ai_sdk-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:21:46.006237 codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/
--rw-rw-rw-   0        0        0      530 2024-04-24 14:20:30.000000 codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/__init__.py
--rw-rw-rw-   0        0        0     4745 2024-04-24 13:58:44.000000 codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/common.py
--rw-rw-rw-   0        0        0    14243 2024-04-24 14:02:18.000000 codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/module_logging.py
--rw-rw-rw-   0        0        0     5209 2024-04-24 13:58:44.000000 codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/module_options.py
--rw-rw-rw-   0        0        0    61588 2024-04-24 14:02:18.000000 codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/module_runner.py
--rw-rw-rw-   0        0        0     9686 2024-04-24 13:58:44.000000 codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/request_data.py
--rw-rw-rw-   0        0        0    15501 2024-04-24 14:02:18.000000 codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/system_info.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:21:46.037736 codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/training/
--rw-rw-rw-   0        0        0     8344 2024-04-24 13:58:44.000000 codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/training/augmentation.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:21:46.069189 codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/utils/
--rw-rw-rw-   0        0        0      328 2024-04-24 13:58:44.000000 codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0    26205 2024-04-24 13:58:44.000000 codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/utils/cpuinfo.py
--rw-rw-rw-   0        0        0     2746 2024-04-24 13:58:44.000000 codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/utils/environment_check.py
--rw-rw-rw-   0        0        0     1419 2024-04-24 13:58:44.000000 codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/utils/image_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:21:46.069189 codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk.egg-info/
--rw-rw-rw-   0        0        0      985 2024-04-24 14:21:45.000000 codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      743 2024-04-24 14:21:45.000000 codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 14:21:45.000000 codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-24 14:21:45.000000 codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-24 14:21:45.000000 codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 15:07:31.168357 codeproject_ai_sdk-0.0.5/
+-rw-rw-rw-   0        0        0      985 2024-04-24 15:07:31.166436 codeproject_ai_sdk-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-04-24 13:58:44.000000 codeproject_ai_sdk-0.0.5/README.md
+-rw-rw-rw-   0        0        0      860 2024-04-24 14:54:35.000000 codeproject_ai_sdk-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-24 15:07:31.168357 codeproject_ai_sdk-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 15:07:31.114276 codeproject_ai_sdk-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 15:07:31.132202 codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/
+-rw-rw-rw-   0        0        0      339 2024-04-24 14:54:24.000000 codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/__init__.py
+-rw-rw-rw-   0        0        0     4745 2024-04-24 13:58:44.000000 codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/common.py
+-rw-rw-rw-   0        0        0    14243 2024-04-24 14:02:18.000000 codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/module_logging.py
+-rw-rw-rw-   0        0        0     5209 2024-04-24 13:58:44.000000 codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/module_options.py
+-rw-rw-rw-   0        0        0    61588 2024-04-24 14:02:18.000000 codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/module_runner.py
+-rw-rw-rw-   0        0        0     9686 2024-04-24 13:58:44.000000 codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/request_data.py
+-rw-rw-rw-   0        0        0    15501 2024-04-24 14:02:18.000000 codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/system_info.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:07:31.145573 codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/training/
+-rw-rw-rw-   0        0        0     8344 2024-04-24 13:58:44.000000 codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/training/augmentation.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:07:31.161424 codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/utils/
+-rw-rw-rw-   0        0        0      328 2024-04-24 13:58:44.000000 codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0    26205 2024-04-24 13:58:44.000000 codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/utils/cpuinfo.py
+-rw-rw-rw-   0        0        0     2746 2024-04-24 13:58:44.000000 codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/utils/environment_check.py
+-rw-rw-rw-   0        0        0     1419 2024-04-24 13:58:44.000000 codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/utils/image_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:07:31.165359 codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk.egg-info/
+-rw-rw-rw-   0        0        0      985 2024-04-24 15:07:31.000000 codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      743 2024-04-24 15:07:31.000000 codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 15:07:31.000000 codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-24 15:07:31.000000 codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-24 15:07:31.000000 codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk.egg-info/top_level.txt
```

### Comparing `codeproject_ai_sdk-0.0.4/PKG-INFO` & `codeproject_ai_sdk-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeproject-ai-sdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python SDK for writing Modules for CodeProject AI Server
 Author: Chris Maunder, Matthew Dennis
 License: SSPL
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `codeproject_ai_sdk-0.0.4/pyproject.toml` & `codeproject_ai_sdk-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "codeproject-ai-sdk"
-version = "0.0.4"
+version = "0.0.5"
 description = "Python SDK for writing Modules for CodeProject AI Server"
 authors = [
     {name = "Chris Maunder"},
     {name = "Matthew Dennis"}
 ]
 license = {text = "SSPL"}
 readme = "README.md"
```

### Comparing `codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/common.py` & `codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/common.py`

 * *Files identical despite different names*

### Comparing `codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/module_logging.py` & `codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/module_logging.py`

 * *Files identical despite different names*

### Comparing `codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/module_options.py` & `codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/module_options.py`

 * *Files identical despite different names*

### Comparing `codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/module_runner.py` & `codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/module_runner.py`

 * *Files identical despite different names*

### Comparing `codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/request_data.py` & `codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/request_data.py`

 * *Files identical despite different names*

### Comparing `codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/system_info.py` & `codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/system_info.py`

 * *Files identical despite different names*

### Comparing `codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/training/augmentation.py` & `codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/training/augmentation.py`

 * *Files identical despite different names*

### Comparing `codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/utils/cpuinfo.py` & `codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/utils/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/utils/environment_check.py` & `codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/utils/environment_check.py`

 * *Files identical despite different names*

### Comparing `codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk/utils/image_utils.py` & `codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk.egg-info/PKG-INFO` & `codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeproject-ai-sdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python SDK for writing Modules for CodeProject AI Server
 Author: Chris Maunder, Matthew Dennis
 License: SSPL
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `codeproject_ai_sdk-0.0.4/src/codeproject_ai_sdk.egg-info/SOURCES.txt` & `codeproject_ai_sdk-0.0.5/src/codeproject_ai_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

