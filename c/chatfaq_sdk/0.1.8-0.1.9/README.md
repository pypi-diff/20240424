# Comparing `tmp/chatfaq_sdk-0.1.8.tar.gz` & `tmp/chatfaq_sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatfaq_sdk-0.1.8.tar", max compression
+gzip compressed data, was "chatfaq_sdk-0.1.9.tar", max compression
```

## Comparing `chatfaq_sdk-0.1.8.tar` & `chatfaq_sdk-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    34522 2023-12-13 14:55:14.611002 chatfaq_sdk-0.1.8/LICENSE
--rw-r--r--   0        0        0     4679 2023-12-13 14:55:14.615002 chatfaq_sdk-0.1.8/README.md
--rw-r--r--   0        0        0    13168 2024-01-22 13:18:30.346483 chatfaq_sdk-0.1.8/chatfaq_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-09-26 15:37:06.672838 chatfaq_sdk-0.1.8/chatfaq_sdk/api/__init__.py
--rw-r--r--   0        0        0      421 2024-01-22 12:07:49.241664 chatfaq_sdk-0.1.8/chatfaq_sdk/api/knowledge_items.py
--rw-r--r--   0        0        0      388 2024-01-22 13:17:38.684138 chatfaq_sdk-0.1.8/chatfaq_sdk/api/messages.py
--rw-r--r--   0        0        0      872 2023-09-26 15:37:06.676838 chatfaq_sdk-0.1.8/chatfaq_sdk/conditions/__init__.py
--rw-r--r--   0        0        0      276 2024-01-22 12:55:06.826346 chatfaq_sdk-0.1.8/chatfaq_sdk/data_source_parsers/__init__.py
--rw-r--r--   0        0        0     3533 2023-09-26 15:37:06.676838 chatfaq_sdk-0.1.8/chatfaq_sdk/fsm/__init__.py
--rw-r--r--   0        0        0     2865 2024-01-22 11:13:32.764809 chatfaq_sdk-0.1.8/chatfaq_sdk/layers/__init__.py
--rw-r--r--   0        0        0      371 2023-01-23 15:16:06.664175 chatfaq_sdk-0.1.8/chatfaq_sdk/settings.py
--rw-r--r--   0        0        0      567 2024-01-22 13:43:45.597492 chatfaq_sdk-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5344 1970-01-01 00:00:00.000000 chatfaq_sdk-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    34522 2023-12-13 14:55:14.611002 chatfaq_sdk-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4679 2023-12-13 14:55:14.615002 chatfaq_sdk-0.1.9/README.md
+-rw-r--r--   0        0        0    13218 2024-01-22 13:53:41.551796 chatfaq_sdk-0.1.9/chatfaq_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-26 15:37:06.672838 chatfaq_sdk-0.1.9/chatfaq_sdk/api/__init__.py
+-rw-r--r--   0        0        0      421 2024-01-22 12:07:49.241664 chatfaq_sdk-0.1.9/chatfaq_sdk/api/knowledge_items.py
+-rw-r--r--   0        0        0      388 2024-01-22 13:17:38.684138 chatfaq_sdk-0.1.9/chatfaq_sdk/api/messages.py
+-rw-r--r--   0        0        0      872 2023-09-26 15:37:06.676838 chatfaq_sdk-0.1.9/chatfaq_sdk/conditions/__init__.py
+-rw-r--r--   0        0        0      276 2024-01-22 12:55:06.826346 chatfaq_sdk-0.1.9/chatfaq_sdk/data_source_parsers/__init__.py
+-rw-r--r--   0        0        0     3533 2023-09-26 15:37:06.676838 chatfaq_sdk-0.1.9/chatfaq_sdk/fsm/__init__.py
+-rw-r--r--   0        0        0     2865 2024-01-22 11:13:32.764809 chatfaq_sdk-0.1.9/chatfaq_sdk/layers/__init__.py
+-rw-r--r--   0        0        0      371 2023-01-23 15:16:06.664175 chatfaq_sdk-0.1.9/chatfaq_sdk/settings.py
+-rw-r--r--   0        0        0      567 2024-01-22 13:54:14.482968 chatfaq_sdk-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5344 1970-01-01 00:00:00.000000 chatfaq_sdk-0.1.9/PKG-INFO
```

### Comparing `chatfaq_sdk-0.1.8/LICENSE` & `chatfaq_sdk-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chatfaq_sdk-0.1.8/README.md` & `chatfaq_sdk-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `chatfaq_sdk-0.1.8/chatfaq_sdk/__init__.py` & `chatfaq_sdk-0.1.9/chatfaq_sdk/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import queue
 import urllib.parse
 from logging import getLogger
 from typing import Callable, Optional, Union
 
 import websockets
 from chatfaq_sdk import settings
-from chatfaq_sdk.api.messages import MessageType, RPCNodeType, DataSourceType
+from chatfaq_sdk.api.messages import MessageType, RPCNodeType# , DataSourceType
 from chatfaq_sdk.conditions import Condition
-from chatfaq_sdk.data_source_parsers import DataSourceParser
+# from chatfaq_sdk.data_source_parsers import DataSourceParser
 from chatfaq_sdk.fsm import FSMDefinition
 from chatfaq_sdk.layers import Layer
 
 settings.configure()
 
 logger = getLogger()
 
@@ -32,15 +32,15 @@
 
     def __init__(
         self,
         chatfaq_ws: str,
         token: str,
         fsm_name: Optional[Union[int, str]],
         fsm_definition: Optional[FSMDefinition] = None,
-        data_source_parsers: Optional[dict[DataSourceParser]] = None,
+        # data_source_parsers: Optional[dict[DataSourceParser]] = None,
     ):
         """
         Parameters
         ----------
         chatfaq_ws: str
             The WS address of your ChatFAQ's back-end server
 
@@ -57,15 +57,15 @@
         """
         if fsm_definition is dict and fsm_name is None:
             raise Exception("If you declare a FSM definition you should provide a name")
         self.chatfaq_ws = chatfaq_ws
         self.token = token
         self.fsm_name = fsm_name
         self.fsm_def = fsm_definition
-        self.data_source_parsers = data_source_parsers
+        # self.data_source_parsers = data_source_parsers
         self.rpcs = {}
         # _rpcs is just an auxiliary variable to register the rpcs without the decorator function just so we know if we
         # already registered that rpc under that name and avoid duplicates
         self._rpcs = {}
         self.ws_rpc = None
         self.ws_llm = None
         self.queue_rpc = queue.Queue()
@@ -87,29 +87,29 @@
             MessageType.rpc_request.value: self.rpc_request_callback,
             MessageType.error.value: self.error_callback,
         }
         llm_actions = {
             MessageType.llm_request_result.value: self.llm_request_result_callback,
             MessageType.error.value: self.error_callback,
         }
-        processor_actions = {
-            key: value
-            for key, value in self.data_source_parsers.items()
-        }
-        processor_actions[MessageType.error.value] = self.error_callback
+        # processor_actions = {
+        #     key: value
+        #     for key, value in self.data_source_parsers.items()
+        # }
+        # processor_actions[MessageType.error.value] = self.error_callback
 
         coros_or_futures = [
             self.consumer("rpc", on_connect=self.on_connect_rpc, is_rpc=True),
             self.consumer("llm", on_connect=None),
             self.producer(rpc_actions, is_rpc=True),
             self.producer(llm_actions),
         ]
-        if self.data_source_parsers:
-            self.consumer("processing", on_connect=self.on_connect_processing),
-            coros_or_futures.append(self.producer(processor_actions))
+        # if self.data_source_parsers:
+        #     self.consumer("processing", on_connect=self.on_connect_processing),
+        #     coros_or_futures.append(self.producer(processor_actions))
 
         await asyncio.gather(
             *coros_or_futures,
         )
 
     async def consumer(self, consumer_route, on_connect=None, is_rpc=False):
         uri = urllib.parse.urljoin(self.chatfaq_ws, f"back/ws/broker/{consumer_route}/")
@@ -201,27 +201,27 @@
                             "name": self.fsm_name,
                             "definition": self.fsm_def.to_dict_repr(),
                         },
                     }
                 )
             )
 
-    async def on_connect_processing(self):
-        if self.data_source_parsers is not None:
-            logger.info(f"Registering Data Source Parsers {self.data_source_parsers.keys()}")
-            await self.ws_rpc.send(
-                json.dumps(
-                    {
-                        "type": DataSourceType.data_source_parsers.value,
-                        "data": {
-                            "data_source_parsers": self.data_source_parsers.keys(),
-                        },
-                    }
-                )
-            )
+    # async def on_connect_processing(self):
+    #     if self.data_source_parsers is not None:
+    #         logger.info(f"Registering Data Source Parsers {self.data_source_parsers.keys()}")
+    #         await self.ws_rpc.send(
+    #             json.dumps(
+    #                 {
+    #                     "type": DataSourceType.data_source_parsers.value,
+    #                     "data": {
+    #                         "data_source_parsers": self.data_source_parsers.keys(),
+    #                     },
+    #                 }
+    #             )
+    #         )
 
     async def _disconnect(self):
         logger.info(f"Shutting Down...")
         await self.ws_rpc.close()
         await self.ws_llm.close()
 
     async def rpc_request_callback(self, payload):
```

### Comparing `chatfaq_sdk-0.1.8/chatfaq_sdk/conditions/__init__.py` & `chatfaq_sdk-0.1.9/chatfaq_sdk/conditions/__init__.py`

 * *Files identical despite different names*

### Comparing `chatfaq_sdk-0.1.8/chatfaq_sdk/fsm/__init__.py` & `chatfaq_sdk-0.1.9/chatfaq_sdk/fsm/__init__.py`

 * *Files identical despite different names*

### Comparing `chatfaq_sdk-0.1.8/chatfaq_sdk/layers/__init__.py` & `chatfaq_sdk-0.1.9/chatfaq_sdk/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `chatfaq_sdk-0.1.8/pyproject.toml` & `chatfaq_sdk-0.1.9/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chatfaq_sdk"
-version = "0.1.8"
+version = "0.1.9"
 description = "ChatFAQ SDK"
 authors = ["Hector Soria <hector.soria@with-madrid.com>"]
 readme = "README.md"
 
 packages = [
     { include = "chatfaq_sdk" },
 ]
```

### Comparing `chatfaq_sdk-0.1.8/PKG-INFO` & `chatfaq_sdk-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatfaq_sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: ChatFAQ SDK
 Author: Hector Soria
 Author-email: hector.soria@with-madrid.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

