# Comparing `tmp/nonebot_adapter_satori-0.9.2.tar.gz` & `tmp/nonebot_adapter_satori-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_satori-0.9.2.tar", last modified: Sun Feb 18 12:46:01 2024, max compression
+gzip compressed data, was "nonebot_adapter_satori-0.9.3.tar", last modified: Mon Feb 19 05:14:32 2024, max compression
```

## Comparing `nonebot_adapter_satori-0.9.2.tar` & `nonebot_adapter_satori-0.9.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1064 2024-02-18 12:45:33.335579 nonebot_adapter_satori-0.9.2/LICENSE
--rw-r--r--   0        0        0     1428 2024-02-18 12:45:33.335579 nonebot_adapter_satori-0.9.2/README.md
--rw-r--r--   0        0        0      210 2024-02-18 12:45:33.335579 nonebot_adapter_satori-0.9.2/nonebot/adapters/satori/__init__.py
--rw-r--r--   0        0        0    10818 2024-02-18 12:45:33.335579 nonebot_adapter_satori-0.9.2/nonebot/adapters/satori/adapter.py
--rw-r--r--   0        0        0    20000 2024-02-18 12:45:33.335579 nonebot_adapter_satori-0.9.2/nonebot/adapters/satori/bot.py
--rw-r--r--   0        0        0      618 2024-02-18 12:45:33.335579 nonebot_adapter_satori-0.9.2/nonebot/adapters/satori/compat.py
--rw-r--r--   0        0        0      800 2024-02-18 12:45:33.335579 nonebot_adapter_satori-0.9.2/nonebot/adapters/satori/config.py
--rw-r--r--   0        0        0    16612 2024-02-18 12:45:33.335579 nonebot_adapter_satori-0.9.2/nonebot/adapters/satori/event.py
--rw-r--r--   0        0        0     1759 2024-02-18 12:45:33.335579 nonebot_adapter_satori-0.9.2/nonebot/adapters/satori/exception.py
--rw-r--r--   0        0        0    19942 2024-02-18 12:45:33.335579 nonebot_adapter_satori-0.9.2/nonebot/adapters/satori/message.py
--rw-r--r--   0        0        0     7251 2024-02-18 12:45:33.335579 nonebot_adapter_satori-0.9.2/nonebot/adapters/satori/models.py
--rw-r--r--   0        0        0     4967 2024-02-18 12:45:33.335579 nonebot_adapter_satori-0.9.2/nonebot/adapters/satori/utils.py
--rw-r--r--   0        0        0     1453 2024-02-18 12:46:01.947524 nonebot_adapter_satori-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     1399 2024-02-18 12:45:33.339579 nonebot_adapter_satori-0.9.2/tests/conftest.py
--rw-r--r--   0        0        0     4808 2024-02-18 12:45:33.339579 nonebot_adapter_satori-0.9.2/tests/fake_server.py
--rw-r--r--   0        0        0     1975 2024-02-18 12:45:33.339579 nonebot_adapter_satori-0.9.2/tests/test_adapter.py
--rw-r--r--   0        0        0     1116 2024-02-18 12:45:33.339579 nonebot_adapter_satori-0.9.2/tests/test_connection.py
--rw-r--r--   0        0        0     1882 1970-01-01 00:00:00.000000 nonebot_adapter_satori-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-02-19 05:14:05.148197 nonebot_adapter_satori-0.9.3/LICENSE
+-rw-r--r--   0        0        0     1428 2024-02-19 05:14:05.148197 nonebot_adapter_satori-0.9.3/README.md
+-rw-r--r--   0        0        0      210 2024-02-19 05:14:05.148197 nonebot_adapter_satori-0.9.3/nonebot/adapters/satori/__init__.py
+-rw-r--r--   0        0        0    10854 2024-02-19 05:14:05.148197 nonebot_adapter_satori-0.9.3/nonebot/adapters/satori/adapter.py
+-rw-r--r--   0        0        0    20096 2024-02-19 05:14:05.152197 nonebot_adapter_satori-0.9.3/nonebot/adapters/satori/bot.py
+-rw-r--r--   0        0        0      618 2024-02-19 05:14:05.152197 nonebot_adapter_satori-0.9.3/nonebot/adapters/satori/compat.py
+-rw-r--r--   0        0        0      800 2024-02-19 05:14:05.152197 nonebot_adapter_satori-0.9.3/nonebot/adapters/satori/config.py
+-rw-r--r--   0        0        0    16768 2024-02-19 05:14:05.152197 nonebot_adapter_satori-0.9.3/nonebot/adapters/satori/event.py
+-rw-r--r--   0        0        0     1759 2024-02-19 05:14:05.152197 nonebot_adapter_satori-0.9.3/nonebot/adapters/satori/exception.py
+-rw-r--r--   0        0        0    19942 2024-02-19 05:14:05.152197 nonebot_adapter_satori-0.9.3/nonebot/adapters/satori/message.py
+-rw-r--r--   0        0        0     7251 2024-02-19 05:14:05.152197 nonebot_adapter_satori-0.9.3/nonebot/adapters/satori/models.py
+-rw-r--r--   0        0        0     4967 2024-02-19 05:14:05.152197 nonebot_adapter_satori-0.9.3/nonebot/adapters/satori/utils.py
+-rw-r--r--   0        0        0     1453 2024-02-19 05:14:32.192168 nonebot_adapter_satori-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     1399 2024-02-19 05:14:05.152197 nonebot_adapter_satori-0.9.3/tests/conftest.py
+-rw-r--r--   0        0        0     4808 2024-02-19 05:14:05.152197 nonebot_adapter_satori-0.9.3/tests/fake_server.py
+-rw-r--r--   0        0        0     1975 2024-02-19 05:14:05.152197 nonebot_adapter_satori-0.9.3/tests/test_adapter.py
+-rw-r--r--   0        0        0     1116 2024-02-19 05:14:05.152197 nonebot_adapter_satori-0.9.3/tests/test_connection.py
+-rw-r--r--   0        0        0     1882 1970-01-01 00:00:00.000000 nonebot_adapter_satori-0.9.3/PKG-INFO
```

### Comparing `nonebot_adapter_satori-0.9.2/LICENSE` & `nonebot_adapter_satori-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_satori-0.9.2/README.md` & `nonebot_adapter_satori-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_satori-0.9.2/nonebot/adapters/satori/adapter.py` & `nonebot_adapter_satori-0.9.3/nonebot/adapters/satori/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import asyncio
 from typing_extensions import override
 from typing import Any, Dict, List, Literal, Optional
 
 from nonebot.utils import escape_tag
 from nonebot.exception import WebSocketClosed
-from nonebot.compat import PYDANTIC_V2, type_validate_python
+from nonebot.compat import PYDANTIC_V2, model_dump, type_validate_python
 from nonebot.drivers import Driver, Request, WebSocket, HTTPClientMixin, WebSocketClientMixin
 
 from nonebot import get_plugin_config
 from nonebot.adapters import Adapter as BaseAdapter
 
 from .bot import Bot
 from .utils import API, log
@@ -267,18 +267,18 @@
                 )
 
     @staticmethod
     def payload_to_event(payload: SatoriEvent) -> Event:
         EventClass = EVENT_CLASSES.get(payload.type, None)
         if EventClass is None:
             log("WARNING", f"Unknown payload type: {payload.type}")
-            event = type_validate_python(Event, payload)
+            event = type_validate_python(Event, model_dump(payload))
             event.__type__ = payload.type  # type: ignore
             return event
-        return type_validate_python(EventClass, payload)
+        return type_validate_python(EventClass, model_dump(payload))
 
     @override
     async def _call_api(self, bot: Bot, api: str, **data: Any) -> Any:
         log("DEBUG", f"Bot {bot.self_id} calling API <y>{api}</y>")
         api_handler: Optional[API] = getattr(bot.__class__, api, None)
         if api_handler is None:
             raise ApiNotAvailable(api)
```

### Comparing `nonebot_adapter_satori-0.9.2/nonebot/adapters/satori/bot.py` & `nonebot_adapter_satori-0.9.3/nonebot/adapters/satori/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,19 +163,22 @@
         return self._self_info
 
     def on_ready(self, user: User) -> None:
         self._self_info = user
 
     def get_authorization_header(self) -> Dict[str, str]:
         """获取当前 Bot 的鉴权信息"""
-        return {
+        header = {
             "Authorization": f"Bearer {self.info.token}",
             "X-Self-ID": self.self_id,
             "X-Platform": self.platform,
         }
+        if not self.info.token:
+            del header["Authorization"]
+        return header
 
     async def handle_event(self, event: Event) -> None:
         if isinstance(event, MessageEvent):
             _check_reply(self, event)
             _check_at_me(self, event)
             _check_nickname(self, event)
         await handle_event(self, event)
```

### Comparing `nonebot_adapter_satori-0.9.2/nonebot/adapters/satori/compat.py` & `nonebot_adapter_satori-0.9.3/nonebot/adapters/satori/compat.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_satori-0.9.2/nonebot/adapters/satori/config.py` & `nonebot_adapter_satori-0.9.3/nonebot/adapters/satori/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_satori-0.9.2/nonebot/adapters/satori/event.py` & `nonebot_adapter_satori-0.9.3/nonebot/adapters/satori/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 from copy import deepcopy
 from typing_extensions import override
 from typing import TYPE_CHECKING, Dict, Type, TypeVar, Optional
 
 from nonebot.utils import escape_tag
-from nonebot.compat import PYDANTIC_V2, type_validate_python
+from nonebot.compat import PYDANTIC_V2, model_dump, type_validate_python
 
 from nonebot.adapters import Event as BaseEvent
 
 from .models import Role, User
 from .compat import model_validator
 from .models import Event as SatoriEvent
 from .message import Message, RenderMessage
@@ -263,39 +263,39 @@
 
 @register_event_class
 class MessageCreatedEvent(MessageEvent):
     __type__ = EventType.MESSAGE_CREATED
 
     def convert(self):
         if self.channel.type == ChannelType.DIRECT:
-            return type_validate_python(PrivateMessageCreatedEvent, self)
+            return type_validate_python(PrivateMessageCreatedEvent, model_dump(self))
         else:
-            return type_validate_python(PublicMessageCreatedEvent, self)
+            return type_validate_python(PublicMessageCreatedEvent, model_dump(self))
 
 
 @register_event_class
 class MessageDeletedEvent(MessageEvent):
     __type__ = EventType.MESSAGE_DELETED
 
     def convert(self):
         if self.channel.type == ChannelType.DIRECT:
-            return type_validate_python(PrivateMessageDeletedEvent, self)
+            return type_validate_python(PrivateMessageDeletedEvent, model_dump(self))
         else:
-            return type_validate_python(PublicMessageDeletedEvent, self)
+            return type_validate_python(PublicMessageDeletedEvent, model_dump(self))
 
 
 @register_event_class
 class MessageUpdatedEvent(MessageEvent):
     __type__ = EventType.MESSAGE_UPDATED
 
     def convert(self):
         if self.channel.type == ChannelType.DIRECT:
-            return type_validate_python(PrivateMessageUpdatedEvent, self)
+            return type_validate_python(PrivateMessageUpdatedEvent, model_dump(self))
         else:
-            return type_validate_python(PublicMessageUpdatedEvent, self)
+            return type_validate_python(PublicMessageUpdatedEvent, model_dump(self))
 
 
 class PrivateMessageEvent(MessageEvent):
     @override
     def is_tome(self) -> bool:
         return True
 
@@ -453,17 +453,17 @@
 
     @override
     def get_event_description(self) -> str:
         return escape_tag(f"Button interacted with button#{self.button.id}")
 
     def convert(self):
         if self.channel and self.user and self.channel.type != ChannelType.DIRECT:
-            return type_validate_python(PublicInteractionButtonEvent, self)
+            return type_validate_python(PublicInteractionButtonEvent, model_dump(self))
         if self.user:
-            return type_validate_python(PrivateInteractionButtonEvent, self)
+            return type_validate_python(PrivateInteractionButtonEvent, model_dump(self))
         return self
 
 
 class PrivateInteractionButtonEvent(InteractionButtonEvent):
     user: User
 
     @override
@@ -532,17 +532,17 @@
         else:
             values["_message"] = Message(cmd)
             values["original_message"] = deepcopy(values["_message"])
         return values
 
     def convert(self):
         if self.channel and self.user and self.channel.type != ChannelType.DIRECT:
-            return type_validate_python(PublicInteractionCommandArgvEvent, self)
+            return type_validate_python(PublicInteractionCommandArgvEvent, model_dump(self))
         if self.user:
-            return type_validate_python(PrivateInteractionCommandArgvEvent, self)
+            return type_validate_python(PrivateInteractionCommandArgvEvent, model_dump(self))
         return self
 
 
 class PrivateInteractionCommandArgvEvent(InteractionCommandArgvEvent):
     user: User
 
     @override
@@ -587,17 +587,17 @@
 
     @override
     def get_event_description(self) -> str:
         return escape_tag(f"Command interacted with {self.get_message()}")
 
     def convert(self):
         if self.channel and self.user and self.channel.type != ChannelType.DIRECT:
-            return type_validate_python(PublicInteractionCommandMessageEvent, self)
+            return type_validate_python(PublicInteractionCommandMessageEvent, model_dump(self))
         if self.user:
-            return type_validate_python(PrivateInteractionCommandMessageEvent, self)
+            return type_validate_python(PrivateInteractionCommandMessageEvent, model_dump(self))
         return self
 
 
 class PrivateInteractionCommandMessageEvent(InteractionCommandMessageEvent):
     user: User
 
     @override
```

### Comparing `nonebot_adapter_satori-0.9.2/nonebot/adapters/satori/exception.py` & `nonebot_adapter_satori-0.9.3/nonebot/adapters/satori/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_satori-0.9.2/nonebot/adapters/satori/message.py` & `nonebot_adapter_satori-0.9.3/nonebot/adapters/satori/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_satori-0.9.2/nonebot/adapters/satori/models.py` & `nonebot_adapter_satori-0.9.3/nonebot/adapters/satori/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_satori-0.9.2/nonebot/adapters/satori/utils.py` & `nonebot_adapter_satori-0.9.3/nonebot/adapters/satori/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_satori-0.9.2/pyproject.toml` & `nonebot_adapter_satori-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-adapter-satori"
-version = "0.9.2"
+version = "0.9.3"
 description = "Satori Protocol Adapter for Nonebot2"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.2.0",
 ]
```

### Comparing `nonebot_adapter_satori-0.9.2/tests/conftest.py` & `nonebot_adapter_satori-0.9.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_satori-0.9.2/tests/fake_server.py` & `nonebot_adapter_satori-0.9.3/tests/fake_server.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_satori-0.9.2/tests/test_adapter.py` & `nonebot_adapter_satori-0.9.3/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_satori-0.9.2/tests/test_connection.py` & `nonebot_adapter_satori-0.9.3/tests/test_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,12 +32,12 @@
                         "platform": "test",
                         "status": 1,
                     }
                 ]
             },
         }
 
-    await asyncio.sleep(2)
+    await asyncio.sleep(5)
     bots = nonebot.get_bots()
     assert "0" in bots
     await adapter.shutdown()
     assert "0" not in nonebot.get_bots()
```

### Comparing `nonebot_adapter_satori-0.9.2/PKG-INFO` & `nonebot_adapter_satori-0.9.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-satori
-Version: 0.9.2
+Version: 0.9.3
 Summary: Satori Protocol Adapter for Nonebot2
 Home-page: https://github.com/nonebot/adapter-satori
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nonebot/adapter-satori
 Project-URL: Repository, https://github.com/nonebot/adapter-satori
 Requires-Python: >=3.8
```

