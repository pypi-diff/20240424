# Comparing `tmp/npgsm-1.0.4.tar.gz` & `tmp/npgsm-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npgsm-1.0.4.tar", last modified: Mon Apr  1 12:20:42 2024, max compression
+gzip compressed data, was "npgsm-1.0.5.tar", last modified: Wed Apr 24 04:02:32 2024, max compression
```

## Comparing `npgsm-1.0.4.tar` & `npgsm-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 nnopp     (1000) nnopp     (1000)        0 2024-04-01 12:20:42.146693 npgsm-1.0.4/
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)     1062 2023-12-12 02:21:56.000000 npgsm-1.0.4/LICENSE
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)     1449 2024-04-01 12:20:42.146693 npgsm-1.0.4/PKG-INFO
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)      341 2024-04-01 12:20:30.000000 npgsm-1.0.4/README.md
-drwxr-xr-x   0 nnopp     (1000) nnopp     (1000)        0 2024-04-01 12:20:42.146693 npgsm-1.0.4/npgsm/
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)      621 2023-12-12 02:21:56.000000 npgsm-1.0.4/npgsm/__init__.py
-drwxr-xr-x   0 nnopp     (1000) nnopp     (1000)        0 2024-04-01 12:20:42.146693 npgsm-1.0.4/npgsm/core/
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)        0 2023-12-12 02:21:56.000000 npgsm-1.0.4/npgsm/core/__init__.py
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)     5400 2024-04-01 12:08:49.000000 npgsm-1.0.4/npgsm/core/tools.py
-drwxr-xr-x   0 nnopp     (1000) nnopp     (1000)        0 2024-04-01 12:20:42.146693 npgsm-1.0.4/npgsm.egg-info/
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)     1449 2024-04-01 12:20:42.000000 npgsm-1.0.4/npgsm.egg-info/PKG-INFO
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)      373 2024-04-01 12:20:42.000000 npgsm-1.0.4/npgsm.egg-info/SOURCES.txt
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)        1 2024-04-01 12:20:42.000000 npgsm-1.0.4/npgsm.egg-info/dependency_links.txt
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)      103 2024-04-01 12:20:42.000000 npgsm-1.0.4/npgsm.egg-info/requires.txt
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)        6 2024-04-01 12:20:42.000000 npgsm-1.0.4/npgsm.egg-info/top_level.txt
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)       38 2024-04-01 12:20:42.146693 npgsm-1.0.4/setup.cfg
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)     1474 2024-04-01 12:19:56.000000 npgsm-1.0.4/setup.py
-drwxr-xr-x   0 nnopp     (1000) nnopp     (1000)        0 2024-04-01 12:20:42.146693 npgsm-1.0.4/tests/
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)      576 2023-12-12 02:21:56.000000 npgsm-1.0.4/tests/test_create_delete.py
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)      470 2024-04-01 12:13:15.000000 npgsm-1.0.4/tests/test_disable_secret.py
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)      447 2023-12-12 02:21:56.000000 npgsm-1.0.4/tests/test_list_secret.py
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)      357 2024-04-01 12:15:24.000000 npgsm-1.0.4/tests/test_list_versions.py
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)     3099 2023-12-12 02:21:56.000000 npgsm-1.0.4/tests/test_remove_oldsecret.py
+drwxr-xr-x   0 cto        (501) staff       (20)        0 2024-04-24 04:02:32.964802 npgsm-1.0.5/
+-rw-r--r--   0 cto        (501) staff       (20)     1062 2023-12-12 02:19:01.000000 npgsm-1.0.5/LICENSE
+-rw-r--r--   0 cto        (501) staff       (20)     1449 2024-04-24 04:02:32.964279 npgsm-1.0.5/PKG-INFO
+-rw-r--r--   0 cto        (501) staff       (20)      341 2024-04-24 03:37:42.000000 npgsm-1.0.5/README.md
+drwxr-xr-x   0 cto        (501) staff       (20)        0 2024-04-24 04:02:32.953326 npgsm-1.0.5/npgsm/
+-rw-r--r--   0 cto        (501) staff       (20)      621 2023-12-12 02:19:01.000000 npgsm-1.0.5/npgsm/__init__.py
+drwxr-xr-x   0 cto        (501) staff       (20)        0 2024-04-24 04:02:32.957677 npgsm-1.0.5/npgsm/core/
+-rw-r--r--   0 cto        (501) staff       (20)        0 2023-12-12 02:19:01.000000 npgsm-1.0.5/npgsm/core/__init__.py
+-rw-r--r--   0 cto        (501) staff       (20)     5475 2024-04-24 03:58:01.000000 npgsm-1.0.5/npgsm/core/tools.py
+drwxr-xr-x   0 cto        (501) staff       (20)        0 2024-04-24 04:02:32.963261 npgsm-1.0.5/npgsm.egg-info/
+-rw-r--r--   0 cto        (501) staff       (20)     1449 2024-04-24 04:02:32.000000 npgsm-1.0.5/npgsm.egg-info/PKG-INFO
+-rw-r--r--   0 cto        (501) staff       (20)      401 2024-04-24 04:02:32.000000 npgsm-1.0.5/npgsm.egg-info/SOURCES.txt
+-rw-r--r--   0 cto        (501) staff       (20)        1 2024-04-24 04:02:32.000000 npgsm-1.0.5/npgsm.egg-info/dependency_links.txt
+-rw-r--r--   0 cto        (501) staff       (20)      103 2024-04-24 04:02:32.000000 npgsm-1.0.5/npgsm.egg-info/requires.txt
+-rw-r--r--   0 cto        (501) staff       (20)        6 2024-04-24 04:02:32.000000 npgsm-1.0.5/npgsm.egg-info/top_level.txt
+-rw-r--r--   0 cto        (501) staff       (20)       38 2024-04-24 04:02:32.964853 npgsm-1.0.5/setup.cfg
+-rw-r--r--   0 cto        (501) staff       (20)     1515 2024-04-24 04:00:30.000000 npgsm-1.0.5/setup.py
+drwxr-xr-x   0 cto        (501) staff       (20)        0 2024-04-24 04:02:32.961940 npgsm-1.0.5/tests/
+-rw-r--r--   0 cto        (501) staff       (20)      576 2023-12-12 02:19:01.000000 npgsm-1.0.5/tests/test_create_delete.py
+-rw-r--r--   0 cto        (501) staff       (20)      344 2024-04-24 03:53:19.000000 npgsm-1.0.5/tests/test_create_simple.py
+-rw-r--r--   0 cto        (501) staff       (20)      470 2024-04-24 03:37:42.000000 npgsm-1.0.5/tests/test_disable_secret.py
+-rw-r--r--   0 cto        (501) staff       (20)      447 2023-12-12 02:19:01.000000 npgsm-1.0.5/tests/test_list_secret.py
+-rw-r--r--   0 cto        (501) staff       (20)      357 2024-04-24 03:37:42.000000 npgsm-1.0.5/tests/test_list_versions.py
+-rw-r--r--   0 cto        (501) staff       (20)     3099 2023-12-12 02:19:01.000000 npgsm-1.0.5/tests/test_remove_oldsecret.py
```

### Comparing `npgsm-1.0.4/LICENSE` & `npgsm-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `npgsm-1.0.4/PKG-INFO` & `npgsm-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npgsm
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package that could help you manage your secrets in Google Secret Manager
 Home-page: https://github.com/noppGithub/npgsm
 Author: Nopporn Phantawee
 Author-email: n.phantawee@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `npgsm-1.0.4/npgsm/__init__.py` & `npgsm-1.0.5/npgsm/__init__.py`

 * *Files identical despite different names*

### Comparing `npgsm-1.0.4/npgsm/core/tools.py` & `npgsm-1.0.5/npgsm/core/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _MY_RETRIABLE_TYPES = (
     exceptions.TooManyRequests,  # 429
     exceptions.InternalServerError,  # 500
     exceptions.BadGateway,  # 502
     exceptions.ServiceUnavailable,  # 503
 )
 
-# ref: https://github.com/googleapis/python-secret-manager/blob/main/samples/snippets/delete_secret.py
+
 class NPGSM(object):
     def __init__(self, project_id, gcp_service_account_path: Optional[str] = None):
         self.project_id = project_id
         self.path_json_key = gcp_service_account_path
         self.__add_environment()
         self.client = self.__get_client()
 
@@ -29,25 +29,30 @@
 
     def __get_client(self):
         client = google.cloud.logging.Client(project=self.project_id)
         client.setup_logging(log_level=logging.INFO)
         return secretmanager.SecretManagerServiceClient()
 
     # ================================= Utility functions =================================
-    def create_secret(self, secret_id):
+    def create_secret(self, secret_id, region=""):
         """Create the secret_id in Google Cloud Secret Manager
         Args:
             secret_id (str): The secret name to store secret value
         """
         # Example input: create_secret("my_secret_value")
         # Create the Secret Manager client.
         # Build the resource name of the parent project.
         parent = f"projects/{self.project_id}"
         # Build a dict of settings for the secret
-        secret = {"replication": {"automatic": {}}}
+        if region:
+            secret = {
+                "replication": {"user_managed": {"replicas": [{"location": region}]}}
+            }
+        else:
+            secret = {"replication": {"automatic": {}}}
         # Create the secret
         try:
             response = self.client.create_secret(
                 secret_id=secret_id, parent=parent, secret=secret  # type: ignore
             )
         except Exception as e:
             print(f"Can not create the secret:{secret_id} with error {e}")
@@ -78,38 +83,38 @@
         name = f"projects/{self.project_id}/secrets/{secret_id}/versions/{version_id}"
         # Access the secret version.
         response = self.client.access_secret_version(name=name)
         # Return the decoded payload.
         payload = response.payload.data.decode("UTF-8")  # type: ignore
         return payload
 
-    def get_versions(self,secret_id):
+    def get_versions(self, secret_id):
         name = f"projects/{self.project_id}/secrets/{secret_id}"
         request = secretmanager.ListSecretVersionsRequest(parent=name)
         page_result = self.client.list_secret_versions(request=request)
         # client.list_secret_versions(request={"parent": parent})
         # Handle the response
-        versions = [v.name for v in page_result if v.state.name != 'DESTROYED']
+        versions = [v.name for v in page_result if v.state.name != "DESTROYED"]
         return versions
 
     def delete_secret(self, secret_id):
         name = self.client.secret_path(self.project_id, secret_id)
         print(f"Deleting Secret: {name}")
         self.client.delete_secret(request={"name": name})
         print(f"Deleted secret {secret_id}")
 
-    def delete_secret_version(self,secret_name,version_id):
+    def delete_secret_version(self, secret_name, version_id):
         name = f"projects/{self.project_id}/secrets/{secret_name}/versions/{version_id}"
         request = secretmanager.DestroySecretVersionRequest(
             name=name,
         )
         response = self.client.destroy_secret_version(request=request)
         print(response)
 
-    def disable_secret_version(self,secret_name,version_id):
+    def disable_secret_version(self, secret_name, version_id):
         name = f"projects/{self.project_id}/secrets/{secret_name}/versions/{version_id}"
         request = secretmanager.DisableSecretVersionRequest(
             name=name,
         )
         response = self.client.disable_secret_version(request=request)
         print(response)
 
@@ -122,8 +127,8 @@
         secrets = []
         for secret in data:
             secrets.append(secret.name.split("/")[-1])
         return secrets
 
     def secret_hash(self, secret_value):
         # return the sha224 hash of the secret value
-        return hashlib.sha224(bytes(secret_value, "utf-8")).hexdigest()
+        return hashlib.sha224(bytes(secret_value, "utf-8")).hexdigest()
```

### Comparing `npgsm-1.0.4/npgsm.egg-info/PKG-INFO` & `npgsm-1.0.5/npgsm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npgsm
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package that could help you manage your secrets in Google Secret Manager
 Home-page: https://github.com/noppGithub/npgsm
 Author: Nopporn Phantawee
 Author-email: n.phantawee@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `npgsm-1.0.4/setup.py` & `npgsm-1.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import pathlib
 
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Read long description from the readme.md file
-with open("README.md") as f:
+with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
-with open("LICENSE") as f:
-    license = f.read()
+with open("LICENSE", encoding="utf-8") as f:
+    license_data = f.read()
 
 setup(
     name="npgsm",
-    version="1.0.4",
+    version="1.0.5",
     description="A package that could help you manage your secrets in Google Secret Manager",
     long_description_content_type="text/markdown",
     long_description=readme,
     author="Nopporn Phantawee",
     author_email="n.phantawee@gmail.com",
     url="https://github.com/noppGithub/npgsm",
     license="MIT",
```

### Comparing `npgsm-1.0.4/tests/test_create_delete.py` & `npgsm-1.0.5/tests/test_create_delete.py`

 * *Files identical despite different names*

### Comparing `npgsm-1.0.4/tests/test_remove_oldsecret.py` & `npgsm-1.0.5/tests/test_remove_oldsecret.py`

 * *Files identical despite different names*

