# Comparing `tmp/nuclio_sdk-0.5.8.tar.gz` & `tmp/nuclio_sdk-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/nuclio-sdk-py/nuclio-sdk-py/dist/.tmp-64drca8d/nuclio_sdk-0.5.8.tar", last modified: Thu Dec  7 12:05:02 2023, max compression
+gzip compressed data, was "/home/runner/work/nuclio-sdk-py/nuclio-sdk-py/dist/.tmp-1f1kt_mn/nuclio_sdk-0.5.9.tar", last modified: Mon Jan 15 17:19:47 2024, max compression
```

## Comparing `nuclio_sdk-0.5.8.tar` & `nuclio_sdk-0.5.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 12:05:02.000000 nuclio_sdk-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2023-12-07 12:04:27.000000 nuclio_sdk-0.5.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-12-07 12:04:27.000000 nuclio_sdk-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2023-12-07 12:05:02.000000 nuclio_sdk-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      560 2023-12-07 12:04:27.000000 nuclio_sdk-0.5.8/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)    35663 2023-12-07 12:04:49.000000 nuclio_sdk-0.5.8/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-07 12:04:27.000000 nuclio_sdk-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 12:05:02.000000 nuclio_sdk-0.5.8/nuclio_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      926 2023-12-07 12:04:27.000000 nuclio_sdk-0.5.8/nuclio_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2023-12-07 12:04:27.000000 nuclio_sdk-0.5.8/nuclio_sdk/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     8001 2023-12-07 12:04:27.000000 nuclio_sdk-0.5.8/nuclio_sdk/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2023-12-07 12:04:27.000000 nuclio_sdk-0.5.8/nuclio_sdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-12-07 12:04:27.000000 nuclio_sdk-0.5.8/nuclio_sdk/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2023-12-07 12:04:27.000000 nuclio_sdk-0.5.8/nuclio_sdk/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2023-12-07 12:04:27.000000 nuclio_sdk-0.5.8/nuclio_sdk/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2023-12-07 12:04:27.000000 nuclio_sdk-0.5.8/nuclio_sdk/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2023-12-07 12:04:27.000000 nuclio_sdk-0.5.8/nuclio_sdk/qualified_offset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2023-12-07 12:04:27.000000 nuclio_sdk-0.5.8/nuclio_sdk/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 12:05:02.000000 nuclio_sdk-0.5.8/nuclio_sdk/test/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-12-07 12:04:27.000000 nuclio_sdk-0.5.8/nuclio_sdk/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2023-12-07 12:04:27.000000 nuclio_sdk-0.5.8/nuclio_sdk/test/mock_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2023-12-07 12:04:27.000000 nuclio_sdk-0.5.8/nuclio_sdk/test/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2023-12-07 12:04:27.000000 nuclio_sdk-0.5.8/nuclio_sdk/test/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2023-12-07 12:04:27.000000 nuclio_sdk-0.5.8/nuclio_sdk/test/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2023-12-07 12:04:27.000000 nuclio_sdk-0.5.8/nuclio_sdk/test/test_qualified_offset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2023-12-07 12:04:27.000000 nuclio_sdk-0.5.8/nuclio_sdk/test/test_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 12:05:02.000000 nuclio_sdk-0.5.8/nuclio_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2023-12-07 12:05:02.000000 nuclio_sdk-0.5.8/nuclio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      686 2023-12-07 12:05:02.000000 nuclio_sdk-0.5.8/nuclio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 12:05:02.000000 nuclio_sdk-0.5.8/nuclio_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-07 12:05:02.000000 nuclio_sdk-0.5.8/nuclio_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-12-07 12:04:27.000000 nuclio_sdk-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-12-07 12:05:02.000000 nuclio_sdk-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2023-12-07 12:04:27.000000 nuclio_sdk-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 17:19:47.000000 nuclio_sdk-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-01-15 17:19:12.000000 nuclio_sdk-0.5.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-15 17:19:12.000000 nuclio_sdk-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-01-15 17:19:47.000000 nuclio_sdk-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-01-15 17:19:12.000000 nuclio_sdk-0.5.9/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)    35663 2024-01-15 17:19:34.000000 nuclio_sdk-0.5.9/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-01-15 17:19:12.000000 nuclio_sdk-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 17:19:47.000000 nuclio_sdk-0.5.9/nuclio_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-01-15 17:19:12.000000 nuclio_sdk-0.5.9/nuclio_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-01-15 17:19:12.000000 nuclio_sdk-0.5.9/nuclio_sdk/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-01-15 17:19:12.000000 nuclio_sdk-0.5.9/nuclio_sdk/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-01-15 17:19:12.000000 nuclio_sdk-0.5.9/nuclio_sdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-15 17:19:12.000000 nuclio_sdk-0.5.9/nuclio_sdk/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-01-15 17:19:12.000000 nuclio_sdk-0.5.9/nuclio_sdk/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-01-15 17:19:12.000000 nuclio_sdk-0.5.9/nuclio_sdk/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-01-15 17:19:12.000000 nuclio_sdk-0.5.9/nuclio_sdk/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-01-15 17:19:12.000000 nuclio_sdk-0.5.9/nuclio_sdk/qualified_offset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-01-15 17:19:12.000000 nuclio_sdk-0.5.9/nuclio_sdk/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 17:19:47.000000 nuclio_sdk-0.5.9/nuclio_sdk/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-01-15 17:19:12.000000 nuclio_sdk-0.5.9/nuclio_sdk/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-01-15 17:19:12.000000 nuclio_sdk-0.5.9/nuclio_sdk/test/mock_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-01-15 17:19:12.000000 nuclio_sdk-0.5.9/nuclio_sdk/test/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-01-15 17:19:12.000000 nuclio_sdk-0.5.9/nuclio_sdk/test/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-01-15 17:19:12.000000 nuclio_sdk-0.5.9/nuclio_sdk/test/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-01-15 17:19:12.000000 nuclio_sdk-0.5.9/nuclio_sdk/test/test_qualified_offset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-01-15 17:19:12.000000 nuclio_sdk-0.5.9/nuclio_sdk/test/test_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 17:19:47.000000 nuclio_sdk-0.5.9/nuclio_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-01-15 17:19:47.000000 nuclio_sdk-0.5.9/nuclio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-01-15 17:19:47.000000 nuclio_sdk-0.5.9/nuclio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 17:19:47.000000 nuclio_sdk-0.5.9/nuclio_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-15 17:19:47.000000 nuclio_sdk-0.5.9/nuclio_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-01-15 17:19:12.000000 nuclio_sdk-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-15 17:19:47.000000 nuclio_sdk-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-01-15 17:19:12.000000 nuclio_sdk-0.5.9/setup.py
```

### Comparing `nuclio_sdk-0.5.8/LICENSE.txt` & `nuclio_sdk-0.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.8/PKG-INFO` & `nuclio_sdk-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclio_sdk
-Version: 0.5.8
+Version: 0.5.9
 Summary: Client for the Nuclio serverless platform
 Home-page: https://github.com/nuclio/nuclio-sdk-py
 Author: Eran Duchan
 Author-email: erand@iguazio.com
 License: Apache 2
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `nuclio_sdk-0.5.8/Pipfile` & `nuclio_sdk-0.5.9/Pipfile`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.8/Pipfile.lock` & `nuclio_sdk-0.5.9/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.8/nuclio_sdk/__init__.py` & `nuclio_sdk-0.5.9/nuclio_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.8/nuclio_sdk/context.py` & `nuclio_sdk-0.5.9/nuclio_sdk/context.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.8/nuclio_sdk/event.py` & `nuclio_sdk-0.5.9/nuclio_sdk/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
             url=parsed_data["url"],
             shard_id=parsed_data["shard_id"],
             num_shards=parsed_data["num_shards"],
             _type=parsed_data["type"],
             type_version=parsed_data["type_version"],
             version=parsed_data["version"],
             offset=parsed_data.get("offset", 0),
+            topic=parsed_data.get("topic"),
         )
 
     @staticmethod
     def _from_parsed_data_bytes(parsed_data, body):
         trigger = TriggerInfo(
             parsed_data[b"trigger"][b"kind"], parsed_data[b"trigger"][b"name"]
         )
@@ -82,14 +83,15 @@
             url=parsed_data[b"url"],
             shard_id=parsed_data[b"shard_id"],
             num_shards=parsed_data[b"num_shards"],
             _type=parsed_data[b"type"],
             type_version=parsed_data[b"type_version"],
             version=parsed_data[b"version"],
             offset=parsed_data.get(b"offset", 0),
+            topic=parsed_data.get(b"topic"),
         )
 
 
 class _EventDeserializerMsgPack(_EventDeserializer):
     def __init__(self, raw=False):
 
         # return the concrete function that handled raw/decoded event messages
@@ -158,14 +160,15 @@
         shard_id=None,
         num_shards=None,
         _type=None,
         type_version=None,
         version=None,
         last_in_batch=None,
         offset=None,
+        topic=None,
     ):
         self.body = body
         self.content_type = content_type
         self.trigger = trigger or TriggerInfo()
         self.fields = fields or {}
         self.headers = headers or {}
         self.id = _id
@@ -177,14 +180,15 @@
         self.shard_id = shard_id
         self.num_shards = num_shards
         self.type = _type
         self.type_version = type_version
         self.version = version
         self.last_in_batch = last_in_batch or False
         self.offset = offset or 0
+        self.topic = topic
 
     def to_json(self):
         obj = {}
         for field_name, field_value in vars(self).items():
             # exclude private fields
             if not field_name.startswith("_"):
                 obj[field_name] = field_value
```

### Comparing `nuclio_sdk-0.5.8/nuclio_sdk/exceptions.py` & `nuclio_sdk-0.5.9/nuclio_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.8/nuclio_sdk/helpers.py` & `nuclio_sdk-0.5.9/nuclio_sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.8/nuclio_sdk/json_encoder.py` & `nuclio_sdk-0.5.9/nuclio_sdk/json_encoder.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.8/nuclio_sdk/logger.py` & `nuclio_sdk-0.5.9/nuclio_sdk/logger.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.8/nuclio_sdk/platform.py` & `nuclio_sdk-0.5.9/nuclio_sdk/platform.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,10 +147,10 @@
         """
         When a signal is received, call the termination/drain callback as a hook before exiting
         If not set, the callback will be a no-op
 
         :arg callback_type:str - callback type, can be "termination" or "drain"
         """
         if callback_type == "termination" and self._termination_callback:
-            self._termination_callback()
+            return self._termination_callback()
         elif callback_type == "drain" and self._drain_callback:
-            self._drain_callback()
+            return self._drain_callback()
```

### Comparing `nuclio_sdk-0.5.8/nuclio_sdk/qualified_offset.py` & `nuclio_sdk-0.5.9/nuclio_sdk/qualified_offset.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.8/nuclio_sdk/response.py` & `nuclio_sdk-0.5.9/nuclio_sdk/response.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.8/nuclio_sdk/test/__init__.py` & `nuclio_sdk-0.5.9/nuclio_sdk/test/__init__.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.8/nuclio_sdk/test/mock_platform.py` & `nuclio_sdk-0.5.9/nuclio_sdk/test/mock_platform.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.8/nuclio_sdk/test/test_case.py` & `nuclio_sdk-0.5.9/nuclio_sdk/test/test_case.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.8/nuclio_sdk/test/test_event.py` & `nuclio_sdk-0.5.9/nuclio_sdk/test/test_event.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,27 +31,29 @@
         self.assertEqual(serialized_event.body, "Ynl0ZXMtYm9keQ==")
         self.assertEqual(serialized_event.content_type, "content-type")
         self.assertEqual(serialized_event.method, "GET")
         self.assertDictEqual(
             serialized_event.trigger.__dict__,
             {"kind": "http", "name": "my-http-trigger"},
         )
-        self.assertEqual(serialized_event.last_in_batch, False)
+        self.assertFalse(serialized_event.last_in_batch)
         self.assertEqual(serialized_event.offset, 0)
 
     def test_event_to_json_bytes_non_utf8able_body(self):
         event = nuclio_sdk.Event(body=b"\x80abc")
         serialized_event = self._deserialize_event(event)
         self.assertEqual(serialized_event.body, "gGFiYw==")
 
     def test_event_to_json_string_body(self):
         request_body = "str-body"
-        event = nuclio_sdk.Event(body=request_body)
+        topic = "my-topic"
+        event = nuclio_sdk.Event(body=request_body, topic=topic)
         serialized_event = self._deserialize_event(event)
         self.assertEqual(request_body, serialized_event.body)
+        self.assertEqual(topic, serialized_event.topic)
 
     def test_print_event(self):
         """
         Test that printing an event doesn't raise an exception
         """
         event = nuclio_sdk.Event(body=datetime.datetime(2022, 1, 1))
         print(event)
```

### Comparing `nuclio_sdk-0.5.8/nuclio_sdk/test/test_logger.py` & `nuclio_sdk-0.5.9/nuclio_sdk/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.8/nuclio_sdk/test/test_qualified_offset.py` & `nuclio_sdk-0.5.9/nuclio_sdk/test/test_qualified_offset.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.8/nuclio_sdk/test/test_response.py` & `nuclio_sdk-0.5.9/nuclio_sdk/test/test_response.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.8/nuclio_sdk.egg-info/PKG-INFO` & `nuclio_sdk-0.5.9/nuclio_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclio-sdk
-Version: 0.5.8
+Version: 0.5.9
 Summary: Client for the Nuclio serverless platform
 Home-page: https://github.com/nuclio/nuclio-sdk-py
 Author: Eran Duchan
 Author-email: erand@iguazio.com
 License: Apache 2
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `nuclio_sdk-0.5.8/nuclio_sdk.egg-info/SOURCES.txt` & `nuclio_sdk-0.5.9/nuclio_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.8/setup.py` & `nuclio_sdk-0.5.9/setup.py`

 * *Files identical despite different names*

