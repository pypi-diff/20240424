# Comparing `tmp/latch_cloud_clients-0.1.1.tar.gz` & `tmp/latch_cloud_clients-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_cloud_clients-0.1.1.tar", max compression
+gzip compressed data, was "latch_cloud_clients-0.1.2.tar", max compression
```

## Comparing `latch_cloud_clients-0.1.1.tar` & `latch_cloud_clients-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     7052 2024-04-19 18:57:40.206110 latch_cloud_clients-0.1.1/LICENSE
--rw-r--r--   0        0        0      121 2024-04-23 21:26:46.040298 latch_cloud_clients-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-19 18:57:40.207571 latch_cloud_clients-0.1.1/latch_cloud_clients/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 19:11:11.691773 latch_cloud_clients-0.1.1/latch_cloud_clients/aws/__init__.py
--rw-r--r--   0        0        0     9677 2024-04-23 19:11:28.023463 latch_cloud_clients-0.1.1/latch_cloud_clients/aws/aws.py
--rw-r--r--   0        0        0     4098 2024-04-23 19:11:50.057387 latch_cloud_clients-0.1.1/latch_cloud_clients/aws/client_pool.py
--rw-r--r--   0        0        0        0 2024-04-23 19:28:36.193575 latch_cloud_clients-0.1.1/latch_cloud_clients/gcp/__init__.py
--rw-r--r--   0        0        0     3100 2024-04-23 19:28:30.737616 latch_cloud_clients-0.1.1/latch_cloud_clients/gcp/client_pool.py
--rw-r--r--   0        0        0     2679 2024-04-23 19:28:30.743461 latch_cloud_clients-0.1.1/latch_cloud_clients/gcp/pubsub.py
--rw-r--r--   0        0        0        0 2024-04-23 19:28:30.747372 latch_cloud_clients-0.1.1/latch_cloud_clients/gcp/py.typed
--rw-r--r--   0        0        0    13697 2024-04-23 21:29:39.780408 latch_cloud_clients-0.1.1/latch_cloud_clients/gcp/storage.py
--rw-r--r--   0        0        0        0 2024-04-19 18:57:40.208421 latch_cloud_clients-0.1.1/latch_cloud_clients/py.typed
--rw-r--r--   0        0        0    24433 2024-04-23 21:05:58.652500 latch_cloud_clients-0.1.1/latch_cloud_clients/storage_clients.py
--rw-r--r--   0        0        0     1455 2024-04-23 21:29:46.861861 latch_cloud_clients-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 latch_cloud_clients-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     7052 2024-04-19 18:57:40.206110 latch_cloud_clients-0.1.2/LICENSE
+-rw-r--r--   0        0        0      121 2024-04-23 21:26:46.040298 latch_cloud_clients-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 18:57:40.207571 latch_cloud_clients-0.1.2/latch_cloud_clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 19:11:11.691773 latch_cloud_clients-0.1.2/latch_cloud_clients/aws/__init__.py
+-rw-r--r--   0        0        0     9677 2024-04-23 19:11:28.023463 latch_cloud_clients-0.1.2/latch_cloud_clients/aws/aws.py
+-rw-r--r--   0        0        0     4098 2024-04-23 19:11:50.057387 latch_cloud_clients-0.1.2/latch_cloud_clients/aws/client_pool.py
+-rw-r--r--   0        0        0        0 2024-04-23 19:28:36.193575 latch_cloud_clients-0.1.2/latch_cloud_clients/gcp/__init__.py
+-rw-r--r--   0        0        0     3100 2024-04-23 19:28:30.737616 latch_cloud_clients-0.1.2/latch_cloud_clients/gcp/client_pool.py
+-rw-r--r--   0        0        0     3369 2024-04-23 22:28:19.034702 latch_cloud_clients-0.1.2/latch_cloud_clients/gcp/pubsub.py
+-rw-r--r--   0        0        0        0 2024-04-23 19:28:30.747372 latch_cloud_clients-0.1.2/latch_cloud_clients/gcp/py.typed
+-rw-r--r--   0        0        0    13697 2024-04-23 22:29:19.411186 latch_cloud_clients-0.1.2/latch_cloud_clients/gcp/storage.py
+-rw-r--r--   0        0        0        0 2024-04-19 18:57:40.208421 latch_cloud_clients-0.1.2/latch_cloud_clients/py.typed
+-rw-r--r--   0        0        0    24433 2024-04-23 22:23:31.663069 latch_cloud_clients-0.1.2/latch_cloud_clients/storage_clients.py
+-rw-r--r--   0        0        0     1455 2024-04-23 22:29:39.245203 latch_cloud_clients-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 latch_cloud_clients-0.1.2/PKG-INFO
```

### Comparing `latch_cloud_clients-0.1.1/LICENSE` & `latch_cloud_clients-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.1/latch_cloud_clients/aws/aws.py` & `latch_cloud_clients-0.1.2/latch_cloud_clients/aws/aws.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.1/latch_cloud_clients/aws/client_pool.py` & `latch_cloud_clients-0.1.2/latch_cloud_clients/aws/client_pool.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.1/latch_cloud_clients/gcp/client_pool.py` & `latch_cloud_clients-0.1.2/latch_cloud_clients/gcp/client_pool.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.1/latch_cloud_clients/gcp/pubsub.py` & `latch_cloud_clients-0.1.2/latch_cloud_clients/gcp/pubsub.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,32 +2,30 @@
 from dataclasses import dataclass
 from typing import Any
 
 import aiohttp
 from google.api_core.exceptions import ServerError
 from google.auth import default
 from google.auth.transport import requests
-from latch_data_validation.data_validation import validate
 
 
 @dataclass(frozen=True)
 class PubsubMessage:
-    data: str
-    attributes: dict[str, str]
+    data: str | None
+    attributes: dict[str, str] | None
     messageId: str
     publishTime: str
     orderingKey: str | None = None
 
 
 @dataclass(frozen=True)
 class SubscriptionMessage:
-    ackId: str
-    message: PubsubMessage
-    # todo(taras): need to fix validation library so that optional fields are allowed
-    # deliveryAttempt: Optional[int]
+    ackId: str | None
+    message: PubsubMessage | None
+    deliveryAttempt: int | None
 
 
 @dataclass(frozen=True)
 class SubscriptionMessageResp:
     receivedMessages: list[SubscriptionMessage]
 
 
@@ -72,15 +70,34 @@
                     "returnImmediately": False,
                     "maxMessages": max_messages,
                 },
             )
 
             if "receivedMessages" not in body:
                 return []
-            return validate(body, SubscriptionMessageResp).receivedMessages
+
+            messages = []
+            for message in body["receivedMessages"]:
+                body = message.get("message")
+                if body is not None:
+                    body = PubsubMessage(
+                        data=message["message"].get("data"),
+                        attributes=dict(message["message"].get("attributes", {})),
+                        messageId=message["message"]["messageId"],
+                        publishTime=message["message"]["publishTime"],
+                        orderingKey=message["message"].get("orderingKey"),
+                    )
+                messages.append(
+                    SubscriptionMessage(
+                        ackId=message.get("ackId"),
+                        message=body,
+                        deliveryAttempt=message.get("deliveryAttempt"),
+                    )
+                )
+            return messages
 
     async def acknowledge(self, ack_ids: list[str]):
         await self._make_api_request(
             "POST",
             f"{self.api_url}:acknowledge",
             {
                 "ackIds": ack_ids,
```

### Comparing `latch_cloud_clients-0.1.1/latch_cloud_clients/gcp/storage.py` & `latch_cloud_clients-0.1.2/latch_cloud_clients/gcp/storage.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.1/latch_cloud_clients/storage_clients.py` & `latch_cloud_clients-0.1.2/latch_cloud_clients/storage_clients.py`

 * *Files identical despite different names*

### Comparing `latch_cloud_clients-0.1.1/pyproject.toml` & `latch_cloud_clients-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latch-cloud-clients"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Taras Priadka <taras@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_cloud_clients"}]
 
 [tool.poetry.dependencies]
@@ -13,25 +13,25 @@
 latch-data-validation = "^0.1.3"
 latch-o11y = "^0.1.4"
 aiobotocore = { extras = ["s3"], version = "^2.4.2" }
 types-aiobotocore = { extras = ["s3"], version = "^2.4.2" }
 google-auth = "^2.29.0"
 requests = "^2.31.0"
 google-cloud = "^0.34.0"
+google-cloud-storage = "^2.16.0"
 google-api-core = "^2.18.0"
 xmltodict = "^0.13.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.12.0"
 isort = "^5.11.4"
 rich = "^13.2.0"
 ruff = "^0.0.269"
 pytest = "^8.1.1"
 pytest-asyncio = "^0.23.6"
-google-cloud-storage = "^2.16.0"
 
 [tool.black]
 preview = true
 target-version = ["py311"]
 
 [tool.isort]
 profile = "black"
```

### Comparing `latch_cloud_clients-0.1.1/PKG-INFO` & `latch_cloud_clients-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: latch-cloud-clients
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 License: CC0 1.0
 Author: Taras Priadka
 Author-email: taras@latch.bio
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiobotocore[s3] (>=2.4.2,<3.0.0)
 Requires-Dist: google-api-core (>=2.18.0,<3.0.0)
 Requires-Dist: google-auth (>=2.29.0,<3.0.0)
 Requires-Dist: google-cloud (>=0.34.0,<0.35.0)
+Requires-Dist: google-cloud-storage (>=2.16.0,<3.0.0)
 Requires-Dist: latch-data-validation (>=0.1.3,<0.2.0)
 Requires-Dist: latch-o11y (>=0.1.4,<0.2.0)
 Requires-Dist: opentelemetry-sdk (>=1.15.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: types-aiobotocore[s3] (>=2.4.2,<3.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
```

