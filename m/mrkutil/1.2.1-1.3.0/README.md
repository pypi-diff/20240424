# Comparing `tmp/mrkutil-1.2.1.tar.gz` & `tmp/mrkutil-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrkutil-1.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mrkutil-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mrkutil-1.2.1.tar` & `mrkutil-1.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       91 2024-04-10 18:38:36.896155 mrkutil-1.2.1/.flake8
--rw-r--r--   0        0        0     1800 2024-04-10 13:44:48.196615 mrkutil-1.2.1/.gitignore
--rw-r--r--   0        0        0      366 2024-04-10 18:38:32.560123 mrkutil-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11358 2024-04-10 13:44:48.196615 mrkutil-1.2.1/LICENSE
--rw-r--r--   0        0        0     3057 2024-04-11 06:14:47.021960 mrkutil-1.2.1/README.md
--rw-r--r--   0        0        0      113 2024-04-12 08:51:59.483455 mrkutil-1.2.1/mrkutil/__init__.py
--rw-r--r--   0        0        0       72 2024-04-10 13:44:48.196615 mrkutil-1.2.1/mrkutil/base/__init__.py
--rw-r--r--   0        0        0     1748 2024-04-10 19:00:33.746768 mrkutil-1.2.1/mrkutil/base/base_handler.py
--rw-r--r--   0        0        0       60 2024-04-10 18:50:04.170994 mrkutil-1.2.1/mrkutil/cache/__init__.py
--rw-r--r--   0        0        0     2406 2024-04-10 19:02:46.268056 mrkutil-1.2.1/mrkutil/cache/base_redis.py
--rw-r--r--   0        0        0      183 2024-04-10 13:44:48.196615 mrkutil-1.2.1/mrkutil/communication/__init__.py
--rw-r--r--   0        0        0      982 2024-04-10 19:03:10.640291 mrkutil-1.2.1/mrkutil/communication/call_service.py
--rw-r--r--   0        0        0     2362 2024-04-10 19:03:50.272675 mrkutil-1.2.1/mrkutil/communication/listen.py
--rw-r--r--   0        0        0     1346 2024-04-10 19:05:17.377524 mrkutil-1.2.1/mrkutil/communication/trigger_service.py
--rw-r--r--   0        0        0      154 2024-04-10 13:44:48.196615 mrkutil-1.2.1/mrkutil/logging/__init__.py
--rw-r--r--   0        0        0     2681 2024-04-10 19:05:36.249709 mrkutil-1.2.1/mrkutil/logging/logging_config.py
--rw-r--r--   0        0        0     1831 2024-04-10 19:05:53.713880 mrkutil-1.2.1/mrkutil/logging/logging_formatter.py
--rw-r--r--   0        0        0      143 2024-04-10 13:44:48.196615 mrkutil-1.2.1/mrkutil/pagination/__init__.py
--rw-r--r--   0        0        0      805 2024-04-10 19:06:55.098484 mrkutil-1.2.1/mrkutil/pagination/dependency.py
--rw-r--r--   0        0        0     1692 2024-04-10 19:12:12.205642 mrkutil-1.2.1/mrkutil/pagination/mongoengine.py
--rw-r--r--   0        0        0     2552 2024-04-10 19:12:07.341593 mrkutil-1.2.1/mrkutil/pagination/sqlalchemy.py
--rw-r--r--   0        0        0       77 2024-04-10 18:53:14.101683 mrkutil-1.2.1/mrkutil/responses/__init__.py
--rw-r--r--   0        0        0     3225 2024-04-12 08:51:40.055110 mrkutil-1.2.1/mrkutil/responses/response_helper.py
--rw-r--r--   0        0        0      256 2024-04-10 18:53:21.969785 mrkutil-1.2.1/mrkutil/utilities.py
--rw-r--r--   0        0        0      822 2024-04-10 19:16:04.147979 mrkutil-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3853 1970-01-01 00:00:00.000000 mrkutil-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0       91 2024-04-10 18:38:36.896155 mrkutil-1.3.0/.flake8
+-rw-r--r--   0        0        0     1800 2024-04-10 13:44:48.196615 mrkutil-1.3.0/.gitignore
+-rw-r--r--   0        0        0      366 2024-04-10 18:38:32.560123 mrkutil-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11358 2024-04-10 13:44:48.196615 mrkutil-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3057 2024-04-11 06:14:47.021960 mrkutil-1.3.0/README.md
+-rw-r--r--   0        0        0      113 2024-04-24 10:12:08.416533 mrkutil-1.3.0/mrkutil/__init__.py
+-rw-r--r--   0        0        0       72 2024-04-10 13:44:48.196615 mrkutil-1.3.0/mrkutil/base/__init__.py
+-rw-r--r--   0        0        0     1748 2024-04-10 19:00:33.746768 mrkutil-1.3.0/mrkutil/base/base_handler.py
+-rw-r--r--   0        0        0       60 2024-04-10 18:50:04.170994 mrkutil-1.3.0/mrkutil/cache/__init__.py
+-rw-r--r--   0        0        0     2406 2024-04-10 19:02:46.268056 mrkutil-1.3.0/mrkutil/cache/base_redis.py
+-rw-r--r--   0        0        0      262 2024-04-24 12:44:29.700772 mrkutil-1.3.0/mrkutil/communication/__init__.py
+-rw-r--r--   0        0        0     1462 2024-04-24 11:50:42.829911 mrkutil-1.3.0/mrkutil/communication/call_service.py
+-rw-r--r--   0        0        0     2362 2024-04-24 07:44:16.079573 mrkutil-1.3.0/mrkutil/communication/listen.py
+-rw-r--r--   0        0        0     1375 2024-04-24 12:37:29.267696 mrkutil-1.3.0/mrkutil/communication/trigger_service.py
+-rw-r--r--   0        0        0      154 2024-04-10 13:44:48.196615 mrkutil-1.3.0/mrkutil/logging/__init__.py
+-rw-r--r--   0        0        0     2681 2024-04-10 19:05:36.249709 mrkutil-1.3.0/mrkutil/logging/logging_config.py
+-rw-r--r--   0        0        0     1831 2024-04-10 19:05:53.713880 mrkutil-1.3.0/mrkutil/logging/logging_formatter.py
+-rw-r--r--   0        0        0      143 2024-04-10 13:44:48.196615 mrkutil-1.3.0/mrkutil/pagination/__init__.py
+-rw-r--r--   0        0        0      805 2024-04-10 19:06:55.098484 mrkutil-1.3.0/mrkutil/pagination/dependency.py
+-rw-r--r--   0        0        0     1692 2024-04-10 19:12:12.205642 mrkutil-1.3.0/mrkutil/pagination/mongoengine.py
+-rw-r--r--   0        0        0     2552 2024-04-10 19:12:07.341593 mrkutil-1.3.0/mrkutil/pagination/sqlalchemy.py
+-rw-r--r--   0        0        0       77 2024-04-10 18:53:14.101683 mrkutil-1.3.0/mrkutil/responses/__init__.py
+-rw-r--r--   0        0        0     3225 2024-04-12 08:51:40.055110 mrkutil-1.3.0/mrkutil/responses/response_helper.py
+-rw-r--r--   0        0        0      256 2024-04-10 18:53:21.969785 mrkutil-1.3.0/mrkutil/utilities.py
+-rw-r--r--   0        0        0      822 2024-04-24 12:36:34.647032 mrkutil-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3853 1970-01-01 00:00:00.000000 mrkutil-1.3.0/PKG-INFO
```

### Comparing `mrkutil-1.2.1/.gitignore` & `mrkutil-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mrkutil-1.2.1/LICENSE` & `mrkutil-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mrkutil-1.2.1/README.md` & `mrkutil-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mrkutil-1.2.1/mrkutil/base/base_handler.py` & `mrkutil-1.3.0/mrkutil/base/base_handler.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.2.1/mrkutil/cache/base_redis.py` & `mrkutil-1.3.0/mrkutil/cache/base_redis.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.2.1/mrkutil/communication/listen.py` & `mrkutil-1.3.0/mrkutil/communication/listen.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.2.1/mrkutil/communication/trigger_service.py` & `mrkutil-1.3.0/mrkutil/communication/trigger_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,44 @@
-from rabbitmqpubsub.rabbit_pubsub import Publisher
-from mrkutil.responses import ServiceResponse
+from rabbitmqpubsub.rabbit_pubsub import Publisher, AsyncRpcClient
+from mrkutil.utilities import random_string
 import logging
 import uuid
 import os
 
 logger = logging.getLogger(__name__)
 
 
 def trigger_service(request_data, destination, source, corr_id="none"):
     """
-    Sends a message to a RabbitMQ queue using the provided request data, destination, source, and correlation ID.
+    Sends a message to a RabbitMQ queue using the provided
+    request data, destination, source, and correlation ID.
 
     Args:
         request_data (any): The data to be sent in the message.
         destination (str): The destination queue name.
         source (str): The source of the message.
         corr_id (str, optional): The correlation ID for the message. Defaults to "none".
 
     Returns:
         bool: True if the message was successfully sent, False otherwise.
     """
-    try:
-        if not corr_id:
-            corr_id = str(uuid.uuid4())
-        Publisher(os.getenv("RABBIT_URL")).publish_message(
-            data=request_data, destination=destination, source=source, corr_id=corr_id
-        )
-        return True
-    except Exception as e:
-        logger.error(
-            "Issue sending message to rabbit. Error message: {}".format(str(e))
-        )
-
-    response = ServiceResponse(code=500, message="Service issue")
+    if not corr_id:
+        corr_id = str(uuid.uuid4())
     Publisher(os.getenv("RABBIT_URL")).publish_message(
-        data=response, destination=destination, source=source, corr_id=corr_id
+        data=request_data, destination=destination, source=source, corr_id=corr_id
+    )
+
+
+async def atrigger_service(request_data, destination, source, corr_id="none"):
+    if not corr_id:
+        corr_id = str(uuid.uuid4())
+    rpc = AsyncRpcClient(
+        amqp_url=os.getenv("RABBIT_URL"),
+        exchange=source,
+        queue="temp_{}".format(random_string(6)),
+    )
+    await rpc.call(
+        data=request_data,
+        recipient=destination,
+        corr_id=corr_id,
+        wait_response=False,
     )
-    return False
```

### Comparing `mrkutil-1.2.1/mrkutil/logging/logging_config.py` & `mrkutil-1.3.0/mrkutil/logging/logging_config.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.2.1/mrkutil/logging/logging_formatter.py` & `mrkutil-1.3.0/mrkutil/logging/logging_formatter.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.2.1/mrkutil/pagination/dependency.py` & `mrkutil-1.3.0/mrkutil/pagination/dependency.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.2.1/mrkutil/pagination/mongoengine.py` & `mrkutil-1.3.0/mrkutil/pagination/mongoengine.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.2.1/mrkutil/pagination/sqlalchemy.py` & `mrkutil-1.3.0/mrkutil/pagination/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.2.1/mrkutil/responses/response_helper.py` & `mrkutil-1.3.0/mrkutil/responses/response_helper.py`

 * *Files identical despite different names*

### Comparing `mrkutil-1.2.1/pyproject.toml` & `mrkutil-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "mrkutil"
-dependencies = ["RabbitMQPubSub>=1.0.0"]
+dependencies = ["RabbitMQPubSub>=1.1.1"]
 authors = [{ name = "Nebojsa Mrkic", email = "mrkic.nebojsa@gmail.com" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = ['License :: OSI Approved :: Apache Software License']
 dynamic = ["version", "description"]
 
 [project.urls]
```

### Comparing `mrkutil-1.2.1/PKG-INFO` & `mrkutil-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: mrkutil
-Version: 1.2.1
+Version: 1.3.0
 Summary: Python package containing common functions for python service based architecture.
 Author-email: Nebojsa Mrkic <mrkic.nebojsa@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: RabbitMQPubSub>=1.0.0
+Requires-Dist: RabbitMQPubSub>=1.1.1
 Requires-Dist: redis>=4.3 ; extra == "extras"
 Requires-Dist: sqlalchemy>=1.4 ; extra == "extras"
 Requires-Dist: pytest ; extra == "tests"
 Requires-Dist: mock ; extra == "tests"
 Requires-Dist: requests ; extra == "tests"
 Requires-Dist: pytest-runner ; extra == "tests"
 Requires-Dist: pre-commit ; extra == "tests"
```

