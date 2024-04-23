# Comparing `tmp/latch_cloud_clients-0.1.0.tar.gz` & `tmp/latch_cloud_clients-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_cloud_clients-0.1.0.tar", max compression
+gzip compressed data, was "latch_cloud_clients-0.1.1.tar", max compression
```

## Comparing `latch_cloud_clients-0.1.0.tar` & `latch_cloud_clients-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     7052 2024-04-19 18:57:40.206110 latch_cloud_clients-0.1.0/LICENSE
--rw-r--r--   0        0        0       13 2024-04-19 20:33:32.480165 latch_cloud_clients-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-19 18:57:40.207571 latch_cloud_clients-0.1.0/latch_cloud_clients/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 19:11:11.691773 latch_cloud_clients-0.1.0/latch_cloud_clients/aws/__init__.py
--rw-r--r--   0        0        0     9677 2024-04-23 19:11:28.023463 latch_cloud_clients-0.1.0/latch_cloud_clients/aws/aws.py
--rw-r--r--   0        0        0     4098 2024-04-23 19:11:50.057387 latch_cloud_clients-0.1.0/latch_cloud_clients/aws/client_pool.py
--rw-r--r--   0        0        0        0 2024-04-23 19:28:36.193575 latch_cloud_clients-0.1.0/latch_cloud_clients/gcp/__init__.py
--rw-r--r--   0        0        0     3100 2024-04-23 19:28:30.737616 latch_cloud_clients-0.1.0/latch_cloud_clients/gcp/client_pool.py
--rw-r--r--   0        0        0     2679 2024-04-23 19:28:30.743461 latch_cloud_clients-0.1.0/latch_cloud_clients/gcp/pubsub.py
--rw-r--r--   0        0        0        0 2024-04-23 19:28:30.747372 latch_cloud_clients-0.1.0/latch_cloud_clients/gcp/py.typed
--rw-r--r--   0        0        0    13693 2024-04-23 21:06:10.781437 latch_cloud_clients-0.1.0/latch_cloud_clients/gcp/storage.py
--rw-r--r--   0        0        0        0 2024-04-19 18:57:40.208421 latch_cloud_clients-0.1.0/latch_cloud_clients/py.typed
--rw-r--r--   0        0        0    24433 2024-04-23 21:05:58.652500 latch_cloud_clients-0.1.0/latch_cloud_clients/storage_clients.py
--rw-r--r--   0        0        0     1455 2024-04-23 21:10:49.552264 latch_cloud_clients-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      902 1970-01-01 00:00:00.000000 latch_cloud_clients-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7052 2024-04-19 18:57:40.206110 latch_cloud_clients-0.1.1/LICENSE
+-rw-r--r--   0        0        0      121 2024-04-23 21:26:46.040298 latch_cloud_clients-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 18:57:40.207571 latch_cloud_clients-0.1.1/latch_cloud_clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 19:11:11.691773 latch_cloud_clients-0.1.1/latch_cloud_clients/aws/__init__.py
+-rw-r--r--   0        0        0     9677 2024-04-23 19:11:28.023463 latch_cloud_clients-0.1.1/latch_cloud_clients/aws/aws.py
+-rw-r--r--   0        0        0     4098 2024-04-23 19:11:50.057387 latch_cloud_clients-0.1.1/latch_cloud_clients/aws/client_pool.py
+-rw-r--r--   0        0        0        0 2024-04-23 19:28:36.193575 latch_cloud_clients-0.1.1/latch_cloud_clients/gcp/__init__.py
+-rw-r--r--   0        0        0     3100 2024-04-23 19:28:30.737616 latch_cloud_clients-0.1.1/latch_cloud_clients/gcp/client_pool.py
+-rw-r--r--   0        0        0     2679 2024-04-23 19:28:30.743461 latch_cloud_clients-0.1.1/latch_cloud_clients/gcp/pubsub.py
+-rw-r--r--   0        0        0        0 2024-04-23 19:28:30.747372 latch_cloud_clients-0.1.1/latch_cloud_clients/gcp/py.typed
+-rw-r--r--   0        0        0    13697 2024-04-23 21:29:39.780408 latch_cloud_clients-0.1.1/latch_cloud_clients/gcp/storage.py
+-rw-r--r--   0        0        0        0 2024-04-19 18:57:40.208421 latch_cloud_clients-0.1.1/latch_cloud_clients/py.typed
+-rw-r--r--   0        0        0    24433 2024-04-23 21:05:58.652500 latch_cloud_clients-0.1.1/latch_cloud_clients/storage_clients.py
+-rw-r--r--   0        0        0     1455 2024-04-23 21:29:46.861861 latch_cloud_clients-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 latch_cloud_clients-0.1.1/PKG-INFO
```

### Comparing `latch_cloud_clients-0.1.0/LICENSE` & `latch_cloud_clients-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.0/latch_cloud_clients/aws/aws.py` & `latch_cloud_clients-0.1.1/latch_cloud_clients/aws/aws.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.0/latch_cloud_clients/aws/client_pool.py` & `latch_cloud_clients-0.1.1/latch_cloud_clients/aws/client_pool.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.0/latch_cloud_clients/gcp/client_pool.py` & `latch_cloud_clients-0.1.1/latch_cloud_clients/gcp/client_pool.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.0/latch_cloud_clients/gcp/pubsub.py` & `latch_cloud_clients-0.1.1/latch_cloud_clients/gcp/pubsub.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.0/latch_cloud_clients/gcp/storage.py` & `latch_cloud_clients-0.1.1/latch_cloud_clients/gcp/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 class AsyncHTTPIterator:
     def __init__(self, url: str, headers: dict, params: dict, storage_client):
         self.url = url
         self.headers = headers
         self.params = params
         self.next_page_token = None
-        self.prefixes = set()
+        self.prefixes = list()
         self.items = []
         self.storage_client = storage_client
 
     def __aiter__(self):
         return self
 
     async def __anext__(self):
@@ -96,15 +96,15 @@
             "GET", self.url, headers=self.headers, params=self.params, return_json=True
         )
 
         if "items" not in res:
             raise StopAsyncIteration
 
         self.items = res.get("items", [])
-        self.prefixes.add(res.get("prefixes", []))
+        self.prefixes.extend(res.get("prefixes", []))
         self.next_page_token = res.get("nextPageToken", "")
 
         return await self.__anext__()
 
 
 class AsyncStorageClient:
     credentials, _ = default(scopes=["https://www.googleapis.com/auth/cloud-platform"])
```

### Comparing `latch_cloud_clients-0.1.0/latch_cloud_clients/storage_clients.py` & `latch_cloud_clients-0.1.1/latch_cloud_clients/storage_clients.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.0/pyproject.toml` & `latch_cloud_clients-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latch-cloud-clients"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Taras Priadka <taras@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_cloud_clients"}]
 
 [tool.poetry.dependencies]
```

### Comparing `latch_cloud_clients-0.1.0/PKG-INFO` & `latch_cloud_clients-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latch-cloud-clients
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: CC0 1.0
 Author: Taras Priadka
 Author-email: taras@latch.bio
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -18,9 +18,14 @@
 Requires-Dist: latch-o11y (>=0.1.4,<0.2.0)
 Requires-Dist: opentelemetry-sdk (>=1.15.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: types-aiobotocore[s3] (>=2.4.2,<3.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
 
-# python-gcp
+# python-cloud-clients
+
+Run storage tests with:
+```
+pytest latch-cloud-clients/test/storage.py --import-mode=prepend
+```
```

