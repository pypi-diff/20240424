# Comparing `tmp/aiomqtt-2.0.1.tar.gz` & `tmp/aiomqtt-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomqtt-2.0.1.tar", max compression
+gzip compressed data, was "aiomqtt-2.1.0.tar", max compression
```

## Comparing `aiomqtt-2.0.1.tar` & `aiomqtt-2.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1464 2024-03-13 22:09:34.630488 aiomqtt-2.0.1/LICENSE
--rw-r--r--   0        0        0     5565 2024-03-13 22:09:34.630488 aiomqtt-2.0.1/README.md
--rw-r--r--   0        0        0      722 2024-03-13 22:10:10.778290 aiomqtt-2.0.1/aiomqtt/__init__.py
--rw-r--r--   0        0        0    30372 2024-03-13 22:09:34.630488 aiomqtt-2.0.1/aiomqtt/client.py
--rw-r--r--   0        0        0     1687 2024-03-13 22:09:34.630488 aiomqtt-2.0.1/aiomqtt/exceptions.py
--rw-r--r--   0        0        0     2350 2024-03-13 22:09:34.630488 aiomqtt-2.0.1/aiomqtt/message.py
--rw-r--r--   0        0        0        0 2024-03-13 22:09:34.630488 aiomqtt-2.0.1/aiomqtt/py.typed
--rw-r--r--   0        0        0     3346 2024-03-13 22:09:34.630488 aiomqtt-2.0.1/aiomqtt/topic.py
--rw-r--r--   0        0        0      901 2024-03-13 22:09:34.630488 aiomqtt-2.0.1/aiomqtt/types.py
--rw-r--r--   0        0        0     4623 2024-03-13 22:10:10.778290 aiomqtt-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     6772 1970-01-01 00:00:00.000000 aiomqtt-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1464 2024-04-24 16:56:39.000731 aiomqtt-2.1.0/LICENSE
+-rw-r--r--   0        0        0     5570 2024-04-24 16:56:39.000731 aiomqtt-2.1.0/README.md
+-rw-r--r--   0        0        0      722 2024-04-24 16:56:58.968810 aiomqtt-2.1.0/aiomqtt/__init__.py
+-rw-r--r--   0        0        0    30858 2024-04-24 16:56:39.000731 aiomqtt-2.1.0/aiomqtt/client.py
+-rw-r--r--   0        0        0     1734 2024-04-24 16:56:39.000731 aiomqtt-2.1.0/aiomqtt/exceptions.py
+-rw-r--r--   0        0        0     2389 2024-04-24 16:56:39.000731 aiomqtt-2.1.0/aiomqtt/message.py
+-rw-r--r--   0        0        0        0 2024-04-24 16:56:39.000731 aiomqtt-2.1.0/aiomqtt/py.typed
+-rw-r--r--   0        0        0     3346 2024-04-24 16:56:39.000731 aiomqtt-2.1.0/aiomqtt/topic.py
+-rw-r--r--   0        0        0      891 2024-04-24 16:56:39.000731 aiomqtt-2.1.0/aiomqtt/types.py
+-rw-r--r--   0        0        0     4769 2024-04-24 16:56:58.968810 aiomqtt-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6777 1970-01-01 00:00:00.000000 aiomqtt-2.1.0/PKG-INFO
```

### Comparing `aiomqtt-2.0.1/LICENSE` & `aiomqtt-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiomqtt-2.0.1/README.md` & `aiomqtt-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 asyncio.run(main())
 ```
 
 ## License
 
 This project is licensed under the [BSD 3-clause License](https://opensource.org/licenses/BSD-3-Clause).
 
-Note that the underlying paho-mqtt library is dual-licensed. One of the licenses is the [Eclipse Distribution License v1.0](https://www.eclipse.org/org/documents/edl-v10.php), which is almost identical to the BSD 3-clause License. The differences are:
+Note that the underlying paho-mqtt library is dual-licensed. One of the licenses is the [Eclipse Distribution License v1.0](https://www.eclipse.org/org/documents/edl-v10.php), which is almost identical to the BSD 3-clause License. The only differences are:
 
 - One use of "COPYRIGHT OWNER" (EDL) instead of "COPYRIGHT HOLDER" (BSD)
 - One use of "Eclipse Foundation, Inc." (EDL) instead of "copyright holder" (BSD)
 
 ## Contributing
 
 We're very happy about contributions to aiomqtt! ✨ You can get started by reading [CONTRIBUTING.md](https://github.com/sbtinstruments/aiomqtt/blob/main/CONTRIBUTING.md).
```

#### html2text {}

```diff
@@ -27,18 +27,18 @@
 "nt": from asyncio import set_event_loop_policy, WindowsSelectorEventLoopPolicy
 set_event_loop_policy(WindowsSelectorEventLoopPolicy()) # Run your async
 application as usual asyncio.run(main()) ``` ## License This project is
 licensed under the [BSD 3-clause License](https://opensource.org/licenses/BSD-
 3-Clause). Note that the underlying paho-mqtt library is dual-licensed. One of
 the licenses is the [Eclipse Distribution License v1.0](https://
 www.eclipse.org/org/documents/edl-v10.php), which is almost identical to the
-BSD 3-clause License. The differences are: - One use of "COPYRIGHT OWNER" (EDL)
-instead of "COPYRIGHT HOLDER" (BSD) - One use of "Eclipse Foundation, Inc."
-(EDL) instead of "copyright holder" (BSD) ## Contributing We're very happy
-about contributions to aiomqtt! â¨ You can get started by reading
+BSD 3-clause License. The only differences are: - One use of "COPYRIGHT OWNER"
+(EDL) instead of "COPYRIGHT HOLDER" (BSD) - One use of "Eclipse Foundation,
+Inc." (EDL) instead of "copyright holder" (BSD) ## Contributing We're very
+happy about contributions to aiomqtt! â¨ You can get started by reading
 [CONTRIBUTING.md](https://github.com/sbtinstruments/aiomqtt/blob/main/
 CONTRIBUTING.md). ## Versioning This project adheres to [Semantic Versioning]
 (https://semver.org/spec/v2.0.0.html). Breaking changes will only occur in
 major `X.0.0` releases. ## Changelog The changelog lives in [CHANGELOG.md]
 (https://github.com/sbtinstruments/aiomqtt/blob/main/CHANGELOG.md). It follows
 the principles of [Keep a Changelog](https://keepachangelog.com/en/1.0.0/). ##
 Related projects Is aiomqtt not what you're looking for? There are a few other
```

### Comparing `aiomqtt-2.0.1/aiomqtt/__init__.py` & `aiomqtt-2.1.0/aiomqtt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Will,
 )
 from .exceptions import MqttCodeError, MqttError, MqttReentrantError
 from .message import Message
 from .topic import Topic, TopicLike, Wildcard, WildcardLike
 
 # These are placeholders that are managed by poetry-dynamic-versioning
-__version__ = "2.0.1"
-__version_tuple__ = (2, 0, 1)
+__version__ = "2.1.0"
+__version_tuple__ = (2, 1, 0)
 
 __all__ = [
     "__version__",
     "__version_tuple__",
     "Client",
     "Message",
     "ProtocolVersion",
```

### Comparing `aiomqtt-2.0.1/aiomqtt/client.py` & `aiomqtt-2.1.0/aiomqtt/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,24 @@
     AsyncGenerator,
     Awaitable,
     Callable,
     Coroutine,
     Generator,
     Iterable,
     Iterator,
+    Literal,
     TypeVar,
     cast,
 )
 
 import paho.mqtt.client as mqtt
+from paho.mqtt.enums import CallbackAPIVersion
+from paho.mqtt.properties import Properties
+from paho.mqtt.reasoncodes import ReasonCode
+from paho.mqtt.subscribeoptions import SubscribeOptions
 
 from .exceptions import MqttCodeError, MqttConnectError, MqttError, MqttReentrantError
 from .message import Message
 from .types import (
     P,
     PayloadType,
     SocketOption,
@@ -112,15 +117,15 @@
 
 @dataclasses.dataclass(frozen=True)
 class Will:
     topic: str
     payload: PayloadType | None = None
     qos: int = 0
     retain: bool = False
-    properties: mqtt.Properties | None = None
+    properties: Properties | None = None
 
 
 class Client:
     """The async context manager that manages the connection to the broker.
 
     Args:
         hostname: The hostname or IP address of the remote broker.
@@ -181,25 +186,25 @@
         password: str | None = None,
         logger: logging.Logger | None = None,
         identifier: str | None = None,
         queue_type: type[asyncio.Queue[Message]] | None = None,
         protocol: ProtocolVersion | None = None,
         will: Will | None = None,
         clean_session: bool | None = None,
-        transport: str = "tcp",
+        transport: Literal["tcp", "websockets"] = "tcp",
         timeout: float | None = None,
         keepalive: int = 60,
         bind_address: str = "",
         bind_port: int = 0,
-        clean_start: int = mqtt.MQTT_CLEAN_START_FIRST_ONLY,
+        clean_start: mqtt.CleanStartOption = mqtt.MQTT_CLEAN_START_FIRST_ONLY,
         max_queued_incoming_messages: int | None = None,
         max_queued_outgoing_messages: int | None = None,
         max_inflight_messages: int | None = None,
         max_concurrent_outgoing_calls: int | None = None,
-        properties: mqtt.Properties | None = None,
+        properties: Properties | None = None,
         tls_context: ssl.SSLContext | None = None,
         tls_params: TLSParameters | None = None,
         tls_insecure: bool | None = None,
         proxy: ProxySettings | None = None,
         socket_options: Iterable[SocketOption] | None = None,
         websocket_path: str | None = None,
         websocket_headers: WebSocketHeaders | None = None,
@@ -216,15 +221,15 @@
         # Connection state
         self._connected: asyncio.Future[None] = asyncio.Future()
         self._disconnected: asyncio.Future[None] = asyncio.Future()
         self._lock: asyncio.Lock = asyncio.Lock()
 
         # Pending subscribe, unsubscribe, and publish calls
         self._pending_subscribes: dict[
-            int, asyncio.Future[tuple[int] | list[mqtt.ReasonCodes]]
+            int, asyncio.Future[tuple[int, ...] | list[ReasonCode]]
         ] = {}
         self._pending_unsubscribes: dict[int, asyncio.Event] = {}
         self._pending_publishes: dict[int, asyncio.Event] = {}
         self.pending_calls_threshold: int = 10
         self._misc_task: asyncio.Task[None] | None = None
 
         # Queue that holds incoming messages
@@ -243,15 +248,16 @@
             self._outgoing_calls_sem = None
 
         if protocol is None:
             protocol = ProtocolVersion.V311
 
         # Create the underlying paho-mqtt client instance
         self._client: mqtt.Client = mqtt.Client(
-            client_id=identifier,
+            callback_api_version=CallbackAPIVersion.VERSION1,
+            client_id=identifier,  # type: ignore[arg-type]
             protocol=protocol,
             clean_session=clean_session,
             transport=transport,
             reconnect_on_failure=False,
         )
         self._client.on_connect = self._on_connect
         self._client.on_disconnect = self._on_disconnect
@@ -318,35 +324,35 @@
     @property
     def identifier(self) -> str:
         """Return the client identifier.
 
         Note that paho-mqtt stores the client ID as `bytes` internally. We assume that
         the client ID is a UTF8-encoded string and decode it first.
         """
-        return cast(bytes, self._client._client_id).decode()  # type: ignore[attr-defined] # noqa: SLF001
+        return self._client._client_id.decode()  # noqa: SLF001
 
     @property
     def _pending_calls(self) -> Generator[int, None, None]:
         """Yield all message IDs with pending calls."""
         yield from self._pending_subscribes.keys()
         yield from self._pending_unsubscribes.keys()
         yield from self._pending_publishes.keys()
 
     @_outgoing_call
     async def subscribe(  # noqa: PLR0913
         self,
         /,
         topic: SubscribeTopic,
         qos: int = 0,
-        options: mqtt.SubscribeOptions | None = None,
-        properties: mqtt.Properties | None = None,
+        options: SubscribeOptions | None = None,
+        properties: Properties | None = None,
         *args: Any,
         timeout: float | None = None,
         **kwargs: Any,
-    ) -> tuple[int] | list[mqtt.ReasonCodes]:
+    ) -> tuple[int, ...] | list[ReasonCode]:
         """Subscribe to a topic or wildcard.
 
         Args:
             topic: The topic or wildcard to subscribe to.
             qos: The requested QoS level for the subscription.
             options: (MQTT v5.0 only) Optional paho-mqtt subscription options.
             properties: (MQTT v5.0 only) Optional paho-mqtt properties.
@@ -358,30 +364,30 @@
                 method.
 
         """
         result, mid = self._client.subscribe(
             topic, qos, options, properties, *args, **kwargs
         )
         # Early out on error
-        if result != mqtt.MQTT_ERR_SUCCESS:
+        if result != mqtt.MQTT_ERR_SUCCESS or mid is None:
             raise MqttCodeError(result, "Could not subscribe to topic")
         # Create future for when the on_subscribe callback is called
         callback_result: asyncio.Future[
-            tuple[int] | list[mqtt.ReasonCodes]
+            tuple[int, ...] | list[ReasonCode]
         ] = asyncio.Future()
         with self._pending_call(mid, callback_result, self._pending_subscribes):
             # Wait for callback_result
             return await self._wait_for(callback_result, timeout=timeout)
 
     @_outgoing_call
     async def unsubscribe(
         self,
         /,
         topic: str | list[str],
-        properties: mqtt.Properties | None = None,
+        properties: Properties | None = None,
         *args: Any,
         timeout: float | None = None,
         **kwargs: Any,
     ) -> None:
         """Unsubscribe from a topic or wildcard.
 
         Args:
@@ -390,17 +396,17 @@
             *args: Additional positional arguments to pass to paho-mqtt's unsubscribe
                 method.
             timeout: The maximum time in seconds to wait for the unsubscription to
                 complete. Use ``math.inf`` to wait indefinitely.
             **kwargs: Additional keyword arguments to pass to paho-mqtt's unsubscribe
                 method.
         """
-        result, mid = self._client.unsubscribe(topic, properties, *args, **kwargs)
+        result, mid = self._client.unsubscribe(topic, properties, *args, **kwargs)  # type: ignore[arg-type]
         # Early out on error
-        if result != mqtt.MQTT_ERR_SUCCESS:
+        if result != mqtt.MQTT_ERR_SUCCESS or mid is None:
             raise MqttCodeError(result, "Could not unsubscribe from topic")
         # Create event for when the on_unsubscribe callback is called
         confirmation = asyncio.Event()
         with self._pending_call(mid, confirmation, self._pending_unsubscribes):
             # Wait for confirmation
             await self._wait_for(confirmation.wait(), timeout=timeout)
 
@@ -408,15 +414,15 @@
     async def publish(  # noqa: PLR0913
         self,
         /,
         topic: str,
         payload: PayloadType = None,
         qos: int = 0,
         retain: bool = False,
-        properties: mqtt.Properties | None = None,
+        properties: Properties | None = None,
         *args: Any,
         timeout: float | None = None,
         **kwargs: Any,
     ) -> None:
         """Publish a message to the broker.
 
         Args:
@@ -514,35 +520,36 @@
                 pass
 
     def _on_connect(  # noqa: PLR0913
         self,
         client: mqtt.Client,
         userdata: Any,
         flags: dict[str, int],
-        rc: int | mqtt.ReasonCodes,
-        properties: mqtt.Properties | None = None,
+        rc: int | ReasonCode,
+        properties: Properties | None = None,
     ) -> None:
         """Called when we receive a CONNACK message from the broker."""
         # Return early if already connected. Sometimes, paho-mqtt calls _on_connect
         # multiple times. Maybe because we receive multiple CONNACK messages
         # from the server. In any case, we return early so that we don't set
         # self._connected twice (as it raises an asyncio.InvalidStateError).
         if self._connected.done():
             return
         if rc == mqtt.CONNACK_ACCEPTED:
             self._connected.set_result(None)
         else:
+            # We received a negative CONNACK response
             self._connected.set_exception(MqttConnectError(rc))
 
     def _on_disconnect(
         self,
         client: mqtt.Client,
         userdata: Any,
-        rc: int | mqtt.ReasonCodes | None,
-        properties: mqtt.Properties | None = None,
+        rc: int | ReasonCode | None,
+        properties: Properties | None = None,
     ) -> None:
         # Return early if the disconnect is already acknowledged.
         # Sometimes (e.g., due to timeouts), paho-mqtt calls _on_disconnect
         # twice. We return early to avoid setting self._disconnected twice
         # (as it raises an asyncio.InvalidStateError).
         if self._disconnected.done():
             return
@@ -565,34 +572,36 @@
             )
 
     def _on_subscribe(  # noqa: PLR0913
         self,
         client: mqtt.Client,
         userdata: Any,
         mid: int,
-        granted_qos: tuple[int] | list[mqtt.ReasonCodes],
-        properties: mqtt.Properties | None = None,
+        granted_qos: tuple[int, ...] | list[ReasonCode],
+        properties: Properties | None = None,
     ) -> None:
+        """Called when we receive a SUBACK message from the broker."""
         try:
             fut = self._pending_subscribes.pop(mid)
             if not fut.done():
                 fut.set_result(granted_qos)
         except KeyError:
             self._logger.exception(
                 'Unexpected message ID "%d" in on_subscribe callback', mid
             )
 
     def _on_unsubscribe(  # noqa: PLR0913
         self,
         client: mqtt.Client,
         userdata: Any,
         mid: int,
-        properties: mqtt.Properties | None = None,
-        reason_codes: list[mqtt.ReasonCodes] | mqtt.ReasonCodes | None = None,
+        properties: Properties | None = None,
+        reason_codes: list[ReasonCode] | ReasonCode | None = None,
     ) -> None:
+        """Called when we receive an UNSUBACK message from the broker."""
         try:
             self._pending_unsubscribes.pop(mid).set()
         except KeyError:
             self._logger.exception(
                 'Unexpected message ID "%d" in on_unsubscribe callback', mid
             )
 
@@ -700,15 +709,15 @@
         # See: https://github.com/eclipse/paho.mqtt.python/blob/v1.5.0/src/paho/mqtt/client.py#L1770
         except (OSError, mqtt.WebsocketConnectionError) as exc:
             self._lock.release()
             raise MqttError(str(exc)) from None
         try:
             await self._wait_for(self._connected, timeout=None)
         except MqttError:
-            # Reset internal state if the connection attempt times out
+            # Reset state if connection attempt times out or CONNACK returns negative
             self._lock.release()
             self._connected = asyncio.Future()
             raise
         # Reset `_disconnected` if it's already in completed state after connecting
         if self._disconnected.done():
             self._disconnected = asyncio.Future()
         return self
```

### Comparing `aiomqtt-2.0.1/aiomqtt/exceptions.py` & `aiomqtt-2.1.0/aiomqtt/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # SPDX-License-Identifier: BSD-3-Clause
 from __future__ import annotations
 
 from typing import Any
 
 import paho.mqtt.client as mqtt
+from paho.mqtt.reasoncodes import ReasonCode
 
 
 class MqttError(Exception):
     pass
 
 
 class MqttCodeError(MqttError):
-    def __init__(self, rc: int | mqtt.ReasonCodes | None, *args: Any) -> None:
+    def __init__(self, rc: int | ReasonCode | None, *args: Any) -> None:
         super().__init__(*args)
         self.rc = rc
 
     def __str__(self) -> str:
-        if isinstance(self.rc, mqtt.ReasonCodes):
+        if isinstance(self.rc, ReasonCode):
             return f"[code:{self.rc.value}] {self.rc!s}"
         if isinstance(self.rc, int):
-            return f"[code:{self.rc}] {mqtt.error_string(self.rc)}"
+            return f"[code:{self.rc}] {mqtt.error_string(self.rc)}"  # type: ignore[arg-type]
         return f"[code:{self.rc}] {super().__str__()}"
 
 
 class MqttConnectError(MqttCodeError):
-    def __init__(self, rc: int | mqtt.ReasonCodes) -> None:
-        if isinstance(rc, mqtt.ReasonCodes):
+    def __init__(self, rc: int | ReasonCode) -> None:
+        if isinstance(rc, ReasonCode):
             super().__init__(rc)
             return
         msg = "Connection refused"
         try:
             msg += f": {_CONNECT_RC_STRINGS[rc]}"
         except KeyError:
             pass
```

### Comparing `aiomqtt-2.0.1/aiomqtt/message.py` & `aiomqtt-2.1.0/aiomqtt/message.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # SPDX-License-Identifier: BSD-3-Clause
 from __future__ import annotations
 
 import sys
 
 import paho.mqtt.client as mqtt
+from paho.mqtt.properties import Properties
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
 from .topic import Topic, TopicLike
@@ -46,15 +47,15 @@
     def __init__(  # noqa: PLR0913
         self,
         topic: TopicLike,
         payload: PayloadType,
         qos: int,
         retain: bool,
         mid: int,
-        properties: mqtt.Properties | None,
+        properties: Properties | None,
     ) -> None:
         self.topic = Topic(topic) if not isinstance(topic, Topic) else topic
         self.payload = payload
         self.qos = qos
         self.retain = retain
         self.mid = mid
         self.properties = properties
```

### Comparing `aiomqtt-2.0.1/aiomqtt/topic.py` & `aiomqtt-2.1.0/aiomqtt/topic.py`

 * *Files identical despite different names*

### Comparing `aiomqtt-2.0.1/aiomqtt/types.py` & `aiomqtt-2.1.0/aiomqtt/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 from __future__ import annotations
 
 import socket
 import ssl
 import sys
 from typing import Any, Callable, TypeVar
 
-import paho.mqtt.client as mqtt
+from paho.mqtt.subscribeoptions import SubscribeOptions
 
 if sys.version_info >= (3, 10):
     from typing import ParamSpec, TypeAlias
 else:
     from typing_extensions import ParamSpec, TypeAlias
 
 
 T = TypeVar("T")
 P = ParamSpec("P")
 
 PayloadType: TypeAlias = "str | bytes | bytearray | int | float | None"
-SubscribeTopic: TypeAlias = "str | tuple[str, mqtt.SubscribeOptions] | list[tuple[str, mqtt.SubscribeOptions]] | list[tuple[str, int]]"
+SubscribeTopic: TypeAlias = "str | tuple[str, SubscribeOptions] | list[tuple[str, SubscribeOptions]] | list[tuple[str, int]]"
 WebSocketHeaders: TypeAlias = (
     "dict[str, str] | Callable[[dict[str, str]], dict[str, str]]"
 )
-_PahoSocket: TypeAlias = "socket.socket | ssl.SSLSocket | mqtt.WebsocketWrapper | Any"
+_PahoSocket: TypeAlias = "socket.socket | ssl.SSLSocket | Any"
 # See the overloads of `socket.setsockopt` for details.
 SocketOption: TypeAlias = "tuple[int, int, int | bytes] | tuple[int, int, None, int]"
```

### Comparing `aiomqtt-2.0.1/pyproject.toml` & `aiomqtt-2.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiomqtt"
-version = "2.0.1"  # Placeholder: Managed by poetry-dynamic-versioning
+version = "2.1.0"  # Placeholder: Managed by poetry-dynamic-versioning
 description = "The idiomatic asyncio MQTT client, wrapped around paho-mqtt"
 license = "BSD-3-Clause"
 authors = ["Frederik Aalund <fpa@sbtinstruments.com>", "Felix Böhm <felix@felixboehm.dev>", "Jonathan Plasse <jonathan.plasse@live.fr>"]
 readme = "README.md"
 packages = [{include = "aiomqtt"}]
 repository = "https://github.com/sbtinstruments/aiomqtt"
 documentation = "https://sbtinstruments.github.io/aiomqtt"
@@ -16,24 +16,23 @@
 ]
 
 [tool.poetry.urls]
 "Issue tracker" = "https://github.com/sbtinstruments/aiomqtt/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-paho-mqtt = "^1.6.0"
+paho-mqtt = "^2.0.0"
 typing-extensions = {version = "^4.4.0", markers = "python_version < '3.10'"}
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-mypy = "^1.8.0"
+mypy = "^1.9.0"
 ruff = "^0.1.9"
-types-paho-mqtt = "^1.6.0.7"
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 anyio = "^3.6.2"
 furo = "^2023.3.27"
 sphinx-autobuild = "^2021.3.14"
 myst-parser = "^1.0.0"
 sphinx-copybutton = "^0.5.2"
@@ -133,14 +132,16 @@
 show_error_context = true
 pretty = true
 
 [tool.pytest.ini_options] # https://docs.pytest.org/en/latest/reference/reference.html#ini-options-ref
 filterwarnings = [
     "error",
     "ignore:ssl.PROTOCOL_TLS is deprecated:DeprecationWarning",
+    # TODO(jonathan): Remove these once we finish the migration to the new API
+    "ignore:Callback API version 1 is deprecated, update to latest version:DeprecationWarning",
 ]
 markers = [
     "network: tests that requires network access"
 ]
 xfail_strict = true
 
 [tool.coverage.run] # https://coverage.readthedocs.io/en/latest/config.html#run
```

### Comparing `aiomqtt-2.0.1/PKG-INFO` & `aiomqtt-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomqtt
-Version: 2.0.1
+Version: 2.1.0
 Summary: The idiomatic asyncio MQTT client, wrapped around paho-mqtt
 Home-page: https://github.com/sbtinstruments/aiomqtt
 License: BSD-3-Clause
 Keywords: mqtt,iot,internet-of-things,asyncio,paho-mqtt,mqttv5
 Author: Frederik Aalund
 Author-email: fpa@sbtinstruments.com
 Requires-Python: >=3.8,<4.0
@@ -14,15 +14,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: paho-mqtt (>=1.6.0,<2.0.0)
+Requires-Dist: paho-mqtt (>=2.0.0,<3.0.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0) ; python_version < "3.10"
 Project-URL: Documentation, https://sbtinstruments.github.io/aiomqtt
 Project-URL: Issue tracker, https://github.com/sbtinstruments/aiomqtt/issues
 Project-URL: Repository, https://github.com/sbtinstruments/aiomqtt
 Description-Content-Type: text/markdown
 
 <h1 align="center">The idiomatic asyncio MQTT client 🙌</h1>
@@ -100,15 +100,15 @@
 asyncio.run(main())
 ```
 
 ## License
 
 This project is licensed under the [BSD 3-clause License](https://opensource.org/licenses/BSD-3-Clause).
 
-Note that the underlying paho-mqtt library is dual-licensed. One of the licenses is the [Eclipse Distribution License v1.0](https://www.eclipse.org/org/documents/edl-v10.php), which is almost identical to the BSD 3-clause License. The differences are:
+Note that the underlying paho-mqtt library is dual-licensed. One of the licenses is the [Eclipse Distribution License v1.0](https://www.eclipse.org/org/documents/edl-v10.php), which is almost identical to the BSD 3-clause License. The only differences are:
 
 - One use of "COPYRIGHT OWNER" (EDL) instead of "COPYRIGHT HOLDER" (BSD)
 - One use of "Eclipse Foundation, Inc." (EDL) instead of "copyright holder" (BSD)
 
 ## Contributing
 
 We're very happy about contributions to aiomqtt! ✨ You can get started by reading [CONTRIBUTING.md](https://github.com/sbtinstruments/aiomqtt/blob/main/CONTRIBUTING.md).
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: aiomqtt Version: 2.0.1 Summary: The idiomatic
+Metadata-Version: 2.1 Name: aiomqtt Version: 2.1.0 Summary: The idiomatic
 asyncio MQTT client, wrapped around paho-mqtt Home-page: https://github.com/
 sbtinstruments/aiomqtt License: BSD-3-Clause Keywords: mqtt,iot,internet-of-
 things,asyncio,paho-mqtt,mqttv5 Author: Frederik Aalund Author-email:
 fpa@sbtinstruments.com Requires-Python: >=3.8,<4.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Requires-Dist: paho-mqtt (>=1.6.0,<2.0.0) Requires-Dist: typing-
+Python :: 3.12 Requires-Dist: paho-mqtt (>=2.0.0,<3.0.0) Requires-Dist: typing-
 extensions (>=4.4.0,<5.0.0) ; python_version < "3.10" Project-URL:
 Documentation, https://sbtinstruments.github.io/aiomqtt Project-URL: Issue
 tracker, https://github.com/sbtinstruments/aiomqtt/issues Project-URL:
 Repository, https://github.com/sbtinstruments/aiomqtt Description-Content-Type:
 text/markdown
              ************ TThhee iiddiioommaattiicc aassyynncciioo MMQQTTTT cclliieenntt ?ð??? ************
                        ((ffoorrmmeerrllyy kknnoowwnn aass aassyynncciioo--mmqqtttt))
@@ -44,18 +44,18 @@
 "nt": from asyncio import set_event_loop_policy, WindowsSelectorEventLoopPolicy
 set_event_loop_policy(WindowsSelectorEventLoopPolicy()) # Run your async
 application as usual asyncio.run(main()) ``` ## License This project is
 licensed under the [BSD 3-clause License](https://opensource.org/licenses/BSD-
 3-Clause). Note that the underlying paho-mqtt library is dual-licensed. One of
 the licenses is the [Eclipse Distribution License v1.0](https://
 www.eclipse.org/org/documents/edl-v10.php), which is almost identical to the
-BSD 3-clause License. The differences are: - One use of "COPYRIGHT OWNER" (EDL)
-instead of "COPYRIGHT HOLDER" (BSD) - One use of "Eclipse Foundation, Inc."
-(EDL) instead of "copyright holder" (BSD) ## Contributing We're very happy
-about contributions to aiomqtt! â¨ You can get started by reading
+BSD 3-clause License. The only differences are: - One use of "COPYRIGHT OWNER"
+(EDL) instead of "COPYRIGHT HOLDER" (BSD) - One use of "Eclipse Foundation,
+Inc." (EDL) instead of "copyright holder" (BSD) ## Contributing We're very
+happy about contributions to aiomqtt! â¨ You can get started by reading
 [CONTRIBUTING.md](https://github.com/sbtinstruments/aiomqtt/blob/main/
 CONTRIBUTING.md). ## Versioning This project adheres to [Semantic Versioning]
 (https://semver.org/spec/v2.0.0.html). Breaking changes will only occur in
 major `X.0.0` releases. ## Changelog The changelog lives in [CHANGELOG.md]
 (https://github.com/sbtinstruments/aiomqtt/blob/main/CHANGELOG.md). It follows
 the principles of [Keep a Changelog](https://keepachangelog.com/en/1.0.0/). ##
 Related projects Is aiomqtt not what you're looking for? There are a few other
```

