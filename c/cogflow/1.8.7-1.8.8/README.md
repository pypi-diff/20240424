# Comparing `tmp/cogflow-1.8.7.tar.gz` & `tmp/cogflow-1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogflow-1.8.7.tar", last modified: Thu Apr 18 08:38:40 2024, max compression
+gzip compressed data, was "cogflow-1.8.8.tar", last modified: Tue Apr 23 11:32:20 2024, max compression
```

## Comparing `cogflow-1.8.7.tar` & `cogflow-1.8.8.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 08:38:40.971369 cogflow-1.8.7/
--rw-rw-rw-   0        0        0      401 2024-04-18 08:38:40.960842 cogflow-1.8.7/PKG-INFO
--rw-rw-rw-   0        0        0     4024 2024-04-15 10:04:49.000000 cogflow-1.8.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 08:38:40.901188 cogflow-1.8.7/cogflow/
--rw-rw-rw-   0        0        0      757 2024-04-17 15:25:52.000000 cogflow-1.8.7/cogflow/__init__.py
--rw-rw-rw-   0        0        0     5085 2024-04-18 07:46:17.000000 cogflow-1.8.7/cogflow/dataset_plugin.py
--rw-rw-rw-   0        0        0     8959 2024-04-17 15:27:00.000000 cogflow-1.8.7/cogflow/kubeflowplugin.py
--rw-rw-rw-   0        0        0    11107 2024-04-17 15:27:24.000000 cogflow-1.8.7/cogflow/mlflowplugin.py
--rw-rw-rw-   0        0        0      714 2024-04-17 14:53:54.000000 cogflow-1.8.7/cogflow/plugin_config.py
--rw-rw-rw-   0        0        0      620 2024-04-15 10:04:49.000000 cogflow-1.8.7/cogflow/plugin_status.py
--rw-rw-rw-   0        0        0      174 2024-04-15 10:04:49.000000 cogflow-1.8.7/cogflow/pluginerrors.py
--rw-rw-rw-   0        0        0     5492 2024-04-17 15:29:41.000000 cogflow-1.8.7/cogflow/pluginmanager.py
-drwxrwxrwx   0        0        0        0 2024-04-18 08:38:40.954843 cogflow-1.8.7/cogflow.egg-info/
--rw-rw-rw-   0        0        0      401 2024-04-18 08:38:40.000000 cogflow-1.8.7/cogflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2024-04-18 08:38:40.000000 cogflow-1.8.7/cogflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 08:38:40.000000 cogflow-1.8.7/cogflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2024-04-18 08:38:40.000000 cogflow-1.8.7/cogflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 08:38:40.000000 cogflow-1.8.7/cogflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 08:38:40.972876 cogflow-1.8.7/setup.cfg
--rw-rw-rw-   0        0        0     1594 2024-04-18 08:37:47.000000 cogflow-1.8.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:32:20.474009 cogflow-1.8.8/
+-rw-rw-rw-   0        0        0      401 2024-04-23 11:32:20.468382 cogflow-1.8.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4024 2024-04-15 10:04:49.000000 cogflow-1.8.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 11:32:20.373327 cogflow-1.8.8/cogflow/
+-rw-rw-rw-   0        0        0      729 2024-04-19 11:20:35.000000 cogflow-1.8.8/cogflow/__init__.py
+-rw-rw-rw-   0        0        0     5430 2024-04-23 07:55:42.000000 cogflow-1.8.8/cogflow/dataset_plugin.py
+-rw-rw-rw-   0        0        0     8953 2024-04-19 10:48:05.000000 cogflow-1.8.8/cogflow/kubeflowplugin.py
+-rw-rw-rw-   0        0        0    11091 2024-04-23 11:21:10.000000 cogflow-1.8.8/cogflow/mlflowplugin.py
+-rw-rw-rw-   0        0        0      874 2024-04-19 11:28:02.000000 cogflow-1.8.8/cogflow/plugin_config.py
+-rw-rw-rw-   0        0        0      620 2024-04-15 10:04:49.000000 cogflow-1.8.8/cogflow/plugin_status.py
+-rw-rw-rw-   0        0        0      174 2024-04-15 10:04:49.000000 cogflow-1.8.8/cogflow/pluginerrors.py
+-rw-rw-rw-   0        0        0    10836 2024-04-23 07:55:42.000000 cogflow-1.8.8/cogflow/pluginmanager.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:32:20.426741 cogflow-1.8.8/cogflow.egg-info/
+-rw-rw-rw-   0        0        0      401 2024-04-23 11:32:19.000000 cogflow-1.8.8/cogflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-04-23 11:32:19.000000 cogflow-1.8.8/cogflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 11:32:19.000000 cogflow-1.8.8/cogflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      214 2024-04-23 11:32:19.000000 cogflow-1.8.8/cogflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-23 11:32:19.000000 cogflow-1.8.8/cogflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 11:32:20.474009 cogflow-1.8.8/setup.cfg
+-rw-rw-rw-   0        0        0     1646 2024-04-23 11:31:44.000000 cogflow-1.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:32:20.461031 cogflow-1.8.8/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-19 10:16:11.000000 cogflow-1.8.8/tests/__init__.py
+-rw-rw-rw-   0        0        0    10080 2024-04-23 07:55:42.000000 cogflow-1.8.8/tests/test_dataset_plugin.py
+-rw-rw-rw-   0        0        0     5369 2024-04-22 07:43:51.000000 cogflow-1.8.8/tests/test_kubeflowplugin.py
+-rw-rw-rw-   0        0        0    14194 2024-04-23 09:54:27.000000 cogflow-1.8.8/tests/test_mlflowplugin.py
+-rw-rw-rw-   0        0        0     7868 2024-04-23 07:55:42.000000 cogflow-1.8.8/tests/test_plugin_manager.py
```

### Comparing `cogflow-1.8.7/README.md` & `cogflow-1.8.8/README.md`

 * *Files identical despite different names*

### Comparing `cogflow-1.8.7/cogflow/__init__.py` & `cogflow-1.8.8/cogflow/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,18 +6,18 @@
     TIMER_IN_SEC (int): Timer interval in seconds.
     ML_TOOL (str): Machine learning tool being used.
     ACCESS_KEY_ID (str): Access key ID for authentication.
     SECRET_ACCESS_KEY (str): Secret access key for authentication.
     S3_ENDPOINT_URL (str): Endpoint URL for Amazon S3.
 """
 
-from cogflow.plugin_config import (
+from .plugin_config import (
     TRACKING_URI,
     TIMER_IN_SEC,
     ML_TOOL,
     ACCESS_KEY_ID,
     SECRET_ACCESS_KEY,
     S3_ENDPOINT_URL,
 )
-from cogflow.plugin_status import plugin_statuses
-from cogflow.pluginerrors import PluginErrors
-from cogflow.pluginmanager import PluginManager
+from .plugin_status import plugin_statuses
+from .pluginerrors import PluginErrors
+from .pluginmanager import PluginManager
```

### Comparing `cogflow-1.8.7/cogflow/dataset_plugin.py` & `cogflow-1.8.8/cogflow/dataset_plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,33 @@
         Initializes DatasetPlugin with environment variables.
         """
         # Retrieve MinIO connection details from environment variables
         self.minio_endpoint = os.getenv("MINIO_ENDPOINT_URL")
         self.minio_access_key = os.getenv("MINIO_ACCESS_KEY")
         self.minio_secret_key = os.getenv("MINIO_SECRET_ACCESS_KEY")
 
+    @staticmethod
+    def version():
+        """
+        Retrieve the version of the DatasetPlugin.
+
+        Returns:
+            str: Version of the DatasetPlugin.
+        """
+        return None
+
+    def is_alive(self):
+        """
+        Check if DatasetPlugin is accessible.
+
+        Returns:
+            None
+        """
+        return None
+
     def create_minio_client(self):
         """
         Creates a MinIO client object.
 
         Returns:
             Minio: The MinIO client object.
         """
@@ -50,18 +69,16 @@
 
         Returns:
             tuple: A tuple containing a boolean indicating success and the file URL if successful.
         """
         try:
             response = requests.get(url)
             if response.status_code == 200:
-                file_url = self.save_to_minio(
-                    response.content, output_file, bucket_name
-                )
-                return True, file_url
+                self.save_to_minio(response.content, output_file, bucket_name)
+                return True
             print(f"Request failed with status code {response.status_code}")
             raise Exception("Request could not be successful due to error")
 
         except requests.exceptions.RequestException as exp:
             print(f"An error occurred: {exp}")
             raise Exception("Exception occurred during the requested operation")
 
@@ -84,16 +101,17 @@
 
         # Check if the bucket exists, if not, create it
         bucket_exists = minio_client.bucket_exists(bucket_name)
         if not bucket_exists:
             try:
                 minio_client.make_bucket(bucket_name)
                 print(f"Bucket '{bucket_name}' created successfully.")
-            except Exception:
-                print(f"Bucket '{bucket_name}' already exists.")
+            except Exception as exp:
+                print(f"Bucket '{bucket_name}' couldnot be created.")
+                raise exp
         # Put file to MinIO
         try:
             # Upload content to MinIO bucket
             minio_client.put_object(
                 bucket_name,
                 object_name,
                 io.BytesIO(file_content),
```

### Comparing `cogflow-1.8.7/cogflow/kubeflowplugin.py` & `cogflow-1.8.8/cogflow/kubeflowplugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     V1beta1SKLearnSpec,
     constants,
     utils,
 )
 from kubernetes import client
 from kubernetes.client import V1ObjectMeta
 from kubernetes.client.models import V1EnvVar
-from cogflow import plugin_config
+from . import plugin_config
 
 
 class CogContainer(kfp.dsl._container_op.Container):
     """
     Subclass of Container to add model access environment variables.
     """
```

### Comparing `cogflow-1.8.7/cogflow/mlflowplugin.py` & `cogflow-1.8.8/cogflow/mlflowplugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import numpy as np
 import pandas as pd
 import requests
 from mlflow.models.signature import ModelSignature
 from mlflow.tracking import MlflowClient
 from scipy.sparse import csr_matrix, csc_matrix
 
-from cogflow import plugin_config
+from . import plugin_config
 
 
 class CogModel(ml.pyfunc.PythonModel):
     """
     A custom Mlflow PythonModel implementation for demonstration purposes.
     """
 
@@ -69,38 +69,40 @@
         """
         Initializes the MlFlowPlugin class.
         """
         self.mlflow = ml
         self.sklearn = ml.sklearn
         self.cogclient = MlflowClient()
         self.pyfunc = ml.pyfunc
+        self.tensorflow = ml.tensorflow
+        self.pytorch = ml.pytorch
         self.models = ml.models
 
     def is_alive(self):
         """
         Check if Mlflow UI is accessible.
 
         Returns:
             tuple: A tuple containing a boolean indicating if Mlflow UI is accessible
              and the status code of the response.
         """
-        response = requests.get(os.getenv(plugin_config.TRACKING_URI))
         try:
+            response = requests.get(os.getenv(plugin_config.TRACKING_URI))
+
             if response.status_code == 200:
-                return response.status_code, response.text
-            print(
-                f"Mlflow UI is not accessible. Status code: {response.status_code}, "
-                f"Message: {response.text}"
-            )
+                pass
+            else:
+                print(
+                    f"Mlflow UI is not accessible. Status code: {response.status_code}, "
+                    f"Message: {response.text}"
+                )
+            return response.status_code, response.text
         except Exception as e:
-            print(
-                f"An error occurred while accessing Mlflow UI: {str(e)}, "
-                f"Status code: {response.status_code}, Message: {response.text}"
-            )
-        return response.status_code, response.text
+            print(f"An error occurred while accessing Mlflow UI: {str(e)}, ")
+            raise e
 
     @staticmethod
     def version():
         """
         Retrieve the version of the Mlflow.
 
         Returns:
```

### Comparing `cogflow-1.8.7/cogflow/plugin_config.py` & `cogflow-1.8.8/cogflow/plugin_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,7 +12,14 @@
 
 TRACKING_URI = "MLFLOW_TRACKING_URI"
 S3_ENDPOINT_URL = "MLFLOW_S3_ENDPOINT_URL"
 ACCESS_KEY_ID = "AWS_ACCESS_KEY_ID"
 SECRET_ACCESS_KEY = "AWS_SECRET_ACCESS_KEY"
 TIMER_IN_SEC = 10
 ML_TOOL = "mlflow"
+
+# Mlflow DB Details
+ML_USERNAME = "root"
+ML_PASSWORD = "2VTvuL7oxiPNyj3e9j47kAj7"
+ML_HOST = "10.100.98.73"
+ML_PORT = "3306"
+ML_DATABASE_NAME = "mlflow"
```

### Comparing `cogflow-1.8.7/cogflow/plugin_status.py` & `cogflow-1.8.8/cogflow/plugin_status.py`

 * *Files identical despite different names*

