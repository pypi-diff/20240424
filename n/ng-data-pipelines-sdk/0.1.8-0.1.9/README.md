# Comparing `tmp/ng_data_pipelines_sdk-0.1.8.tar.gz` & `tmp/ng_data_pipelines_sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng_data_pipelines_sdk-0.1.8.tar", max compression
+gzip compressed data, was "ng_data_pipelines_sdk-0.1.9.tar", max compression
```

## Comparing `ng_data_pipelines_sdk-0.1.8.tar` & `ng_data_pipelines_sdk-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      106 2024-04-18 21:47:43.514634 ng_data_pipelines_sdk-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-04-18 21:47:43.539633 ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/__init__.py
--rw-r--r--   0        0        0     4766 2024-04-18 21:47:43.514634 ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/aws_interface.py
--rw-r--r--   0        0        0      231 2024-04-18 21:47:43.514634 ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/custom_logger.py
--rw-r--r--   0        0        0    24231 2024-04-18 21:47:43.514634 ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/dataframe_manager.py
--rw-r--r--   0        0        0     8365 2024-04-18 21:47:43.514634 ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/interfaces.py
--rw-r--r--   0        0        0     2878 2024-04-18 21:47:43.514634 ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/spark_manager.py
--rw-r--r--   0        0        0     3498 2024-04-18 21:47:43.514634 ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/utils.py
--rw-r--r--   0        0        0      671 2024-04-18 21:47:43.516634 ng_data_pipelines_sdk-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-04-22 12:26:18.737067 ng_data_pipelines_sdk-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 12:26:18.764067 ng_data_pipelines_sdk-0.1.9/ng_data_pipelines_sdk/__init__.py
+-rw-r--r--   0        0        0     4932 2024-04-22 12:26:18.737067 ng_data_pipelines_sdk-0.1.9/ng_data_pipelines_sdk/aws_interface.py
+-rw-r--r--   0        0        0      231 2024-04-22 12:26:18.737067 ng_data_pipelines_sdk-0.1.9/ng_data_pipelines_sdk/custom_logger.py
+-rw-r--r--   0        0        0    24231 2024-04-22 12:26:18.738067 ng_data_pipelines_sdk-0.1.9/ng_data_pipelines_sdk/dataframe_manager.py
+-rw-r--r--   0        0        0     8365 2024-04-22 12:26:18.738067 ng_data_pipelines_sdk-0.1.9/ng_data_pipelines_sdk/interfaces.py
+-rw-r--r--   0        0        0     2878 2024-04-22 12:26:18.739067 ng_data_pipelines_sdk-0.1.9/ng_data_pipelines_sdk/spark_manager.py
+-rw-r--r--   0        0        0     3498 2024-04-22 12:26:18.739067 ng_data_pipelines_sdk-0.1.9/ng_data_pipelines_sdk/utils.py
+-rw-r--r--   0        0        0      671 2024-04-22 12:26:18.740067 ng_data_pipelines_sdk-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.1.9/PKG-INFO
```

### Comparing `ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/aws_interface.py` & `ng_data_pipelines_sdk-0.1.9/ng_data_pipelines_sdk/aws_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import json
 
 from ng_data_pipelines_sdk.interfaces import AWSCredentials, Env
 
 
 class AWSServiceClient:
     def __init__(
-        self, region_name: str, aws_credentials: Optional[AWSCredentials] = None
+        self, region_name: Optional[str] = None, aws_credentials: Optional[AWSCredentials] = None
     ):
+        region_name = region_name if region_name else None
         aws_access_key_id = (
             aws_credentials.aws_access_key_id if aws_credentials else None
         )
         aws_secret_access_key = (
             aws_credentials.aws_secret_access_key if aws_credentials else None
         )
 
@@ -36,23 +37,26 @@
         )
 
 
 class AWSInterface:
     def __init__(
         self,
         region_name: str,
-        aws_credentials_dict: Optional[Dict[Env, Optional[AWSCredentials]]] = None,
+        aws_credentials_dict: Optional[Dict[Env, AWSCredentials]] = None,
     ):
         if not aws_credentials_dict:
-            aws_credentials_dict = {Env.DEV: None, Env.PRD: None}
-
-        self.client_managers = {
-            env: AWSServiceClient(region_name, credentials)
-            for env, credentials in aws_credentials_dict.items()
-        }
+            self.client_managers = {
+                env: AWSServiceClient()
+                for env in [Env.DEV, Env.PRD]
+            }
+        else:
+            self.client_managers = {
+                env: AWSServiceClient(region_name, credentials)
+                for env, credentials in aws_credentials_dict.items()
+            }
 
     def get_service_client(self, env: Env) -> AWSServiceClient:
         if env not in self.client_managers:
             raise ValueError(f"No AWS credentials found for environment {env.value}")
         return self.client_managers[env]
 
     def get_object_aws(self, env: Env, bucket_name: str, object_name: str) -> bytes:
```

### Comparing `ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/dataframe_manager.py` & `ng_data_pipelines_sdk-0.1.9/ng_data_pipelines_sdk/dataframe_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/interfaces.py` & `ng_data_pipelines_sdk-0.1.9/ng_data_pipelines_sdk/interfaces.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/spark_manager.py` & `ng_data_pipelines_sdk-0.1.9/ng_data_pipelines_sdk/spark_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.8/ng_data_pipelines_sdk/utils.py` & `ng_data_pipelines_sdk-0.1.9/ng_data_pipelines_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.8/pyproject.toml` & `ng_data_pipelines_sdk-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ng-data-pipelines-sdk"
-version = "0.1.8"
+version = "0.1.9"
 description = "A library for facilitating the development of data engineering pipelines using pyspark. Compatible with MWAA running airlow 2.8.1."
 authors = ["ng.cash"]
 readme = "README.md"
 exclude = [".git/", ".gitignore", "tests/", "docs/", "*.yml", "__pycache__/", "*.pyc", "*.ipynb", "playground/", "poetry.lock", "dist/", "build/"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
```

