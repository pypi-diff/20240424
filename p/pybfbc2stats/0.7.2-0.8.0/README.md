# Comparing `tmp/pybfbc2stats-0.7.2.tar.gz` & `tmp/pybfbc2stats-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybfbc2stats-0.7.2.tar", last modified: Fri Dec  1 22:19:56 2023, max compression
+gzip compressed data, was "pybfbc2stats-0.8.0.tar", last modified: Tue Apr 23 20:06:08 2024, max compression
```

## Comparing `pybfbc2stats-0.7.2.tar` & `pybfbc2stats-0.8.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 22:19:56.223143 pybfbc2stats-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-12-01 22:19:48.000000 pybfbc2stats-0.7.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    20870 2023-12-01 22:19:56.223143 pybfbc2stats-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20222 2023-12-01 22:19:48.000000 pybfbc2stats-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 22:19:56.223143 pybfbc2stats-0.7.2/pybfbc2stats/
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2023-12-01 22:19:48.000000 pybfbc2stats-0.7.2/pybfbc2stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16899 2023-12-01 22:19:48.000000 pybfbc2stats-0.7.2/pybfbc2stats/asyncio_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2023-12-01 22:19:48.000000 pybfbc2stats-0.7.2/pybfbc2stats/asyncio_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2023-12-01 22:19:48.000000 pybfbc2stats-0.7.2/pybfbc2stats/buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)    43167 2023-12-01 22:19:48.000000 pybfbc2stats-0.7.2/pybfbc2stats/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2023-12-01 22:19:48.000000 pybfbc2stats-0.7.2/pybfbc2stats/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    45835 2023-12-01 22:19:48.000000 pybfbc2stats-0.7.2/pybfbc2stats/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2023-12-01 22:19:48.000000 pybfbc2stats-0.7.2/pybfbc2stats/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-12-01 22:19:48.000000 pybfbc2stats-0.7.2/pybfbc2stats/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    11312 2023-12-01 22:19:48.000000 pybfbc2stats-0.7.2/pybfbc2stats/packet.py
--rw-r--r--   0 runner    (1001) docker     (127)    12992 2023-12-01 22:19:48.000000 pybfbc2stats-0.7.2/pybfbc2stats/payload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 22:19:56.223143 pybfbc2stats-0.7.2/pybfbc2stats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20870 2023-12-01 22:19:56.000000 pybfbc2stats-0.7.2/pybfbc2stats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      549 2023-12-01 22:19:56.000000 pybfbc2stats-0.7.2/pybfbc2stats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-01 22:19:56.000000 pybfbc2stats-0.7.2/pybfbc2stats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-01 22:19:56.000000 pybfbc2stats-0.7.2/pybfbc2stats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-01 22:19:48.000000 pybfbc2stats-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      697 2023-12-01 22:19:56.223143 pybfbc2stats-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-01 22:19:48.000000 pybfbc2stats-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 22:19:56.223143 pybfbc2stats-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2023-12-01 22:19:48.000000 pybfbc2stats-0.7.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10695 2023-12-01 22:19:48.000000 pybfbc2stats-0.7.2/tests/test_packet.py
--rw-r--r--   0 runner    (1001) docker     (127)    44764 2023-12-01 22:19:48.000000 pybfbc2stats-0.7.2/tests/test_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:06:08.895461 pybfbc2stats-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-23 20:06:05.000000 pybfbc2stats-0.8.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    20870 2024-04-23 20:06:08.895461 pybfbc2stats-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20222 2024-04-23 20:06:05.000000 pybfbc2stats-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:06:08.895461 pybfbc2stats-0.8.0/pybfbc2stats/
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-23 20:06:05.000000 pybfbc2stats-0.8.0/pybfbc2stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18405 2024-04-23 20:06:05.000000 pybfbc2stats-0.8.0/pybfbc2stats/asyncio_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-23 20:06:05.000000 pybfbc2stats-0.8.0/pybfbc2stats/asyncio_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-23 20:06:05.000000 pybfbc2stats-0.8.0/pybfbc2stats/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46206 2024-04-23 20:06:05.000000 pybfbc2stats-0.8.0/pybfbc2stats/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-23 20:06:05.000000 pybfbc2stats-0.8.0/pybfbc2stats/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46275 2024-04-23 20:06:05.000000 pybfbc2stats-0.8.0/pybfbc2stats/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-23 20:06:05.000000 pybfbc2stats-0.8.0/pybfbc2stats/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 20:06:05.000000 pybfbc2stats-0.8.0/pybfbc2stats/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11514 2024-04-23 20:06:05.000000 pybfbc2stats-0.8.0/pybfbc2stats/packet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13330 2024-04-23 20:06:05.000000 pybfbc2stats-0.8.0/pybfbc2stats/payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-04-23 20:06:05.000000 pybfbc2stats-0.8.0/pybfbc2stats/rome.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:06:08.895461 pybfbc2stats-0.8.0/pybfbc2stats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20870 2024-04-23 20:06:08.000000 pybfbc2stats-0.8.0/pybfbc2stats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-23 20:06:08.000000 pybfbc2stats-0.8.0/pybfbc2stats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:06:08.000000 pybfbc2stats-0.8.0/pybfbc2stats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 20:06:08.000000 pybfbc2stats-0.8.0/pybfbc2stats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-23 20:06:05.000000 pybfbc2stats-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-23 20:06:08.895461 pybfbc2stats-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 20:06:05.000000 pybfbc2stats-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:06:08.895461 pybfbc2stats-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-23 20:06:05.000000 pybfbc2stats-0.8.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10689 2024-04-23 20:06:05.000000 pybfbc2stats-0.8.0/tests/test_packet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45049 2024-04-23 20:06:05.000000 pybfbc2stats-0.8.0/tests/test_payload.py
```

### Comparing `pybfbc2stats-0.7.2/LICENSE.md` & `pybfbc2stats-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pybfbc2stats-0.7.2/PKG-INFO` & `pybfbc2stats-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybfbc2stats
-Version: 0.7.2
+Version: 0.8.0
 Summary: Python library for retrieving statistics of Battlefield: Bad Company 2 players
 Home-page: https://github.com/cetteup/pybfbc2stats
 Author: cetteup
 Author-email: me@cetteup.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cetteup/pybfbc2stats/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pybfbc2stats-0.7.2/README.md` & `pybfbc2stats-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pybfbc2stats-0.7.2/pybfbc2stats/__init__.py` & `pybfbc2stats-0.8.0/pybfbc2stats/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 from .client import FeslClient, TheaterClient
 from .connection import Connection, SecureConnection
 from .constants import Platform, Namespace, DEFAULT_LEADERBOARD_KEYS, STATS_KEYS, GENERAL_STATS_KEYS, WEAPON_STATS_KEYS, \
     VEHICLE_STATS_KEYS, SERVICE_STARS_STATS_KEYS, AWARDS_STATS_KEYS, SINGLEPLAYER_STATS_KEYS
 from .exceptions import Error, TimeoutError, ParameterError, \
     PlayerNotFoundError, AuthError, ConnectionError, SearchError, \
     NotFoundError, ServerNotFoundError, LobbyNotFoundError, RecordNotFoundError
+from .rome import RomeFeslClient, AsyncRomeFeslClient, RomeTheaterClient, AsyncRomeTheaterClient
 
 """
 pybfbc2stats.
 Python library for retrieving statistics of Battlefield: Bad Company 2 players.
 """
 
-__version__ = '0.7.2'
+__version__ = '0.8.0'
 __author__ = 'cetteup'
 __credits__ = 'nemo, Luigi Auriemma'
 __all__ = ['Connection', 'SecureConnection', 'FeslClient', 'TheaterClient',
            'AsyncConnection', 'AsyncSecureConnection', 'AsyncFeslClient', 'AsyncTheaterClient',
+           'RomeFeslClient', 'AsyncRomeFeslClient', 'RomeTheaterClient', 'AsyncRomeTheaterClient',
            'Platform', 'Namespace', 'DEFAULT_LEADERBOARD_KEYS', 'STATS_KEYS', 'GENERAL_STATS_KEYS', 'WEAPON_STATS_KEYS',
            'VEHICLE_STATS_KEYS', 'SERVICE_STARS_STATS_KEYS', 'AWARDS_STATS_KEYS', 'SINGLEPLAYER_STATS_KEYS',
            'Error', 'ConnectionError', 'ParameterError', 'TimeoutError',
            'AuthError', 'NotFoundError', 'PlayerNotFoundError', 'RecordNotFoundError',
            'ServerNotFoundError', 'LobbyNotFoundError', 'SearchError']
```

### Comparing `pybfbc2stats-0.7.2/pybfbc2stats/asyncio_client.py` & `pybfbc2stats-0.8.0/pybfbc2stats/asyncio_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Tuple, Optional, Union
 
 from .asyncio_connection import AsyncSecureConnection, AsyncConnection
 from .client import Client, FeslClient, TheaterClient
-from .constants import FeslStep, Namespace, BACKEND_DETAILS, Platform, LookupType, DEFAULT_LEADERBOARD_KEYS, STATS_KEYS, \
-    TheaterStep, ENCODING, FeslParseMap, TheaterParseMap
+from .constants import FeslStep, Namespace, Platform, LookupType, DEFAULT_LEADERBOARD_KEYS, STATS_KEYS, \
+    TheaterStep, ENCODING, FeslParseMap, TheaterParseMap, Backend
 from .exceptions import PlayerNotFoundError, AuthError, ConnectionError, TimeoutError
 from .packet import Packet, FeslPacket, TheaterPacket
 from .payload import Payload, StrValue, IntValue, ParseMap
 
 
 class AsyncClient(Client):
     connection: AsyncConnection
@@ -48,48 +48,38 @@
 
 
 class AsyncFeslClient(FeslClient, AsyncClient):
     connection: AsyncSecureConnection
 
     def __init__(self, username: StrValue, password: StrValue, platform: Platform, timeout: float = 3.0,
                  track_steps: bool = True):
-        connection = AsyncSecureConnection(
-            BACKEND_DETAILS[platform]['host'],
-            BACKEND_DETAILS[platform]['port'],
-            FeslPacket,
-            timeout
-        )
+        host, port, client_string = self.get_backend_details(Backend.official, platform)
+        connection = AsyncSecureConnection(host, port, FeslPacket, timeout)
         """
         Multiple inheritance works here, but only if we "skip" the FeslClient constructor. The method resolution here
         is: AsyncFeslClient, FeslClient, AsyncClient, Client. So, by calling super(), we would call the FeslClient
         __init__ function with parameters that make no sense. If we instead use super(FeslClient, self), we call
         FeslClient's super directly - effectively skipping the FeslClient constructor
         """
-        super(FeslClient, self).__init__(
-            connection,
-            platform,
-            BACKEND_DETAILS[platform]['clientString'],
-            timeout,
-            track_steps
-        )
+        super(FeslClient, self).__init__(connection, platform, client_string, timeout, track_steps)
         self.username = username
         self.password = password
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, *excinfo):
         try:
             await self.logout()
         except (ConnectionError, TimeoutError):
             pass
         await self.connection.close()
 
     async def hello(self) -> bytes:
-        if self.track_steps and FeslStep.hello in self.completed_steps:
+        if self.completed_step(FeslStep.hello):
             return bytes(self.completed_steps[FeslStep.hello])
 
         tid = self.get_transaction_id()
         hello_packet = self.build_hello_packet(tid, self.client_string)
         await self.connection.write(hello_packet)
 
         # FESL sends hello response immediately followed initial memcheck => read both and return hello response
@@ -103,80 +93,131 @@
 
         return bytes(response)
 
     async def memcheck(self) -> None:
         memcheck_packet = self.build_memcheck_packet()
         await self.connection.write(memcheck_packet)
 
-    async def login(self) -> bytes:
-        if self.track_steps and FeslStep.login in self.completed_steps:
+    async def login(self, tos_version: Optional[StrValue] = None) -> bytes:
+        if self.completed_step(FeslStep.login):
             return bytes(self.completed_steps[FeslStep.login])
-        elif self.track_steps and FeslStep.hello not in self.completed_steps:
+        elif not self.completed_step(FeslStep.hello):
             await self.hello()
 
         tid = self.get_transaction_id()
-        login_packet = self.build_login_packet(tid, self.username, self.password)
+        login_packet = self.build_login_packet(tid, self.username, self.password, tos_version)
         await self.connection.write(login_packet)
         response = await self.wrapped_read(tid)
 
         response_valid, error_message, code = self.is_valid_login_response(response)
         if not response_valid:
+            # If we received a "TOS Content is out of date" error, fetch current TOS version and try login one more time
+            if code == 260 and tos_version is None and (tos_version := await self.get_tos_version()) != bytes():
+                return await self.login(tos_version)
             raise AuthError(error_message)
 
         self.completed_steps[FeslStep.login] = response
 
         return bytes(response)
 
+    async def login_persona(self, persona_name: Optional[str] = None) -> bytes:
+        if not self.completed_step(FeslStep.login):
+            await self.login()
+
+        # Fetch and use first available persona if none was given
+        if persona_name is None:
+            personas = await self.get_personas()
+            if len(personas) < 1:
+                raise AuthError("No persona available for login")
+
+            persona_name = personas[0]
+
+        tid = self.get_transaction_id()
+        login_persona_packet = self.build_persona_login_packet(tid, persona_name)
+        await self.connection.write(login_persona_packet)
+        response = await self.wrapped_read(tid)
+
+        response_valid, error_message, _ = self.is_valid_login_response(response)
+        if not response_valid:
+            raise AuthError(error_message)
+
+        self.completed_steps[FeslStep.login_persona] = response
+
+        return bytes(response)
+
     async def logout(self) -> Optional[bytes]:
         # Only send logout if client is currently logged in
-        if self.track_steps and FeslStep.login in self.completed_steps:
+        if self.completed_step(FeslStep.login):
             tid = self.get_transaction_id()
             logout_packet = self.build_logout_packet(tid)
             await self.connection.write(logout_packet)
             self.completed_steps.clear()
             return bytes(await self.wrapped_read(tid))
 
     async def ping(self) -> None:
         ping_packet = self.build_ping_packet()
         await self.connection.write(ping_packet)
 
+    async def get_tos_version(self) -> bytes:
+        if not self.completed_step(FeslStep.hello):
+            await self.hello()
+
+        tid = self.get_transaction_id()
+        packet = self.build_tos_packet(tid)
+        await self.connection.write(packet)
+        response = await self.get_response(tid)
+
+        return response.get('version', bytes())
+
     async def get_theater_details(self) -> Tuple[str, int]:
-        if self.track_steps and FeslStep.hello not in self.completed_steps:
+        if not self.completed_step(FeslStep.hello):
             await self.hello()
 
         packet = self.completed_steps[FeslStep.hello]
         payload = packet.get_payload()
 
         # Field is called "ip" but actually contains the hostname
         return payload.get_str('theaterIp', str()), payload.get_int('theaterPort', int())
 
     async def get_lkey(self) -> str:
-        if self.track_steps and FeslStep.login not in self.completed_steps:
+        if not self.completed_step(FeslStep.login):
             await self.login()
 
         packet = self.completed_steps[FeslStep.login]
         payload = packet.get_payload()
 
         return payload.get_str('lkey', str())
 
+    async def get_personas(self) -> List[str]:
+        if not self.completed_step(FeslStep.login):
+            await self.login()
+
+        tid = self.get_transaction_id()
+        packet = self.build_get_personas_packet(tid)
+        await self.connection.write(packet)
+
+        payload = await self.get_response(tid, parse_map=FeslParseMap.Personas)
+        personas = payload.get_list('personas', list())
+        return personas
+
     async def lookup_usernames(self, usernames: List[StrValue], namespace: Namespace) -> List[dict]:
         return await self.lookup_user_identifiers(usernames, namespace, LookupType.byName)
 
     async def lookup_username(self, username: StrValue, namespace: Namespace) -> dict:
         return await self.lookup_user_identifier(username, namespace, LookupType.byName)
 
     async def lookup_user_ids(self, user_ids: List[IntValue], namespace: Namespace) -> List[dict]:
         return await self.lookup_user_identifiers(user_ids, namespace, LookupType.byId)
 
     async def lookup_user_id(self, user_id: IntValue, namespace: Namespace) -> dict:
         return await self.lookup_user_identifier(user_id, namespace, LookupType.byId)
 
     async def lookup_user_identifiers(self, identifiers: List[Union[StrValue, IntValue]], namespace: Namespace,
                                       lookup_type: LookupType) -> List[dict]:
-        if self.track_steps and FeslStep.login not in self.completed_steps:
+        if not self.completed_step(FeslStep.login):
             await self.login()
 
         tid = self.get_transaction_id()
         lookup_packet = self.build_user_lookup_packet(tid, identifiers, namespace, lookup_type)
         await self.connection.write(lookup_packet)
 
         payload = await self.get_response(tid, parse_map=FeslParseMap.UserLookup)
@@ -187,43 +228,43 @@
 
         if len(results) == 0:
             raise PlayerNotFoundError('User lookup did not return any results')
 
         return results.pop()
 
     async def search_name(self, screen_name: StrValue, namespace: Namespace) -> dict:
-        if self.track_steps and FeslStep.login not in self.completed_steps:
+        if not self.completed_step(FeslStep.login):
             await self.login()
 
         tid = self.get_transaction_id()
         search_packet = self.build_search_packet(tid, screen_name, namespace)
         await self.connection.write(search_packet)
 
         payload = await self.get_response(tid, parse_map=FeslParseMap.NameSearch)
         return {
             'namespace': payload.get_str('nameSpaceId', str()),
             'users': payload.get_list('users', list())
         }
 
     async def get_stats(self, userid: IntValue, keys: List[StrValue] = STATS_KEYS) -> dict:
-        if self.track_steps and FeslStep.login not in self.completed_steps:
+        if not self.completed_step(FeslStep.login):
             await self.login()
 
         # Send query in chunks (using the same transaction id for all packets)
         tid = self.get_transaction_id()
         chunk_packets = self.build_stats_query_packets(tid, userid, keys)
         for chunk_packet in chunk_packets:
             await self.connection.write(chunk_packet)
 
         payload = await self.get_response(tid, parse_map=FeslParseMap.Stats)
         return self.dict_list_to_dict(payload.get_list('stats', list()))
 
     async def get_leaderboard(self, min_rank: IntValue = 1, max_rank: IntValue = 50, sort_by: StrValue = 'score',
                               keys: List[StrValue] = DEFAULT_LEADERBOARD_KEYS) -> List[dict]:
-        if self.track_steps and FeslStep.login not in self.completed_steps:
+        if not self.completed_step(FeslStep.login):
             await self.login()
 
         tid = self.get_transaction_id()
         leaderboard_packet = self.build_leaderboard_query_packet(tid, min_rank, max_rank, sort_by, keys)
         await self.connection.write(leaderboard_packet)
 
         payload = await self.get_response(tid, parse_map=FeslParseMap.Leaderboard)
@@ -232,15 +273,15 @@
             {
                 key: Client.dict_list_to_dict(value) if isinstance(value, list) else value
                 for (key, value) in entry.items()
             } for entry in payload.get_list('stats', list())
         ]
 
     async def get_dogtags(self, userid: IntValue) -> List[dict]:
-        if self.track_steps and FeslStep.login not in self.completed_steps:
+        if not self.completed_step(FeslStep.login):
             await self.login()
 
         tid = self.get_transaction_id()
         dogtags_packet = self.build_dogtag_query_packet(tid, userid)
         await self.connection.write(dogtags_packet)
 
         payload = await self.get_response(tid, parse_map=FeslParseMap.Dogtags)
@@ -257,41 +298,36 @@
         return Payload.from_bytes(response, parse_map)
 
 
 class AsyncTheaterClient(TheaterClient, AsyncClient):
     def __init__(self, host: str, port: int, lkey: StrValue, platform: Platform, timeout: float = 3.0,
                  track_steps: bool = True):
         connection = AsyncConnection(host, port, TheaterPacket)
+        _, _, client_string = self.get_backend_details(Backend.official, platform)
         # "Skip" TheaterClient constructor, for details see note in AsyncFeslClient.__init__
-        super(TheaterClient, self).__init__(
-            connection,
-            platform,
-            BACKEND_DETAILS[platform]['clientString'],
-            timeout,
-            track_steps
-        )
+        super(TheaterClient, self).__init__(connection, platform, client_string, timeout, track_steps)
         self.lkey = lkey
 
     async def connect(self) -> bytes:
-        if self.track_steps and TheaterStep.conn in self.completed_steps:
+        if self.completed_step(TheaterStep.conn):
             return bytes(self.completed_steps[TheaterStep.conn])
 
         tid = self.get_transaction_id()
         connect_packet = self.build_conn_packet(tid, self.client_string)
         await self.connection.write(connect_packet)
 
         response = await self.connection.read()
         self.completed_steps[TheaterStep.conn] = response
 
         return bytes(response)
 
     async def authenticate(self) -> bytes:
-        if self.track_steps and TheaterStep.user in self.completed_steps:
+        if self.completed_step(TheaterStep.user):
             return bytes(self.completed_steps[TheaterStep.user])
-        elif self.track_steps and TheaterStep.conn not in self.completed_steps:
+        elif not self.completed_step(TheaterStep.conn):
             await self.connect()
 
         tid = self.get_transaction_id()
         auth_packet = self.build_user_packet(tid, self.lkey)
         await self.connection.write(auth_packet)
 
         response = await self.connection.read()
@@ -304,15 +340,15 @@
         return bytes(response)
 
     async def ping(self) -> None:
         ping_packet = self.build_ping_packet()
         await self.connection.write(ping_packet)
 
     async def get_lobbies(self) -> List[dict]:
-        if self.track_steps and TheaterStep.user not in self.completed_steps:
+        if not self.completed_step(TheaterStep.user):
             await self.authenticate()
 
         tid = self.get_transaction_id()
         lobby_list_packet = self.build_llst_packet(tid)
         await self.connection.write(lobby_list_packet)
 
         # Theater responds with an initial LLST packet, indicating the number of lobbies,
@@ -327,15 +363,15 @@
             ldat_response = await self.wrapped_read(tid)
             ldat = ldat_response.get_payload(TheaterParseMap.LDAT)
             lobbies.append(dict(ldat))
 
         return lobbies
 
     async def get_servers(self, lobby_id: IntValue) -> List[dict]:
-        if self.track_steps and TheaterStep.user not in self.completed_steps:
+        if not self.completed_step(TheaterStep.user):
             await self.authenticate()
 
         tid = self.get_transaction_id()
         server_list_packet = self.build_glst_packet(tid, str(lobby_id).encode(ENCODING))
         await self.connection.write(server_list_packet)
 
         # Again, same procedure: Theater first responds with a GLST packet which indicates the number of games/servers
@@ -364,15 +400,15 @@
     async def get_server_details(self, lobby_id: IntValue, game_id: IntValue) -> Tuple[dict, dict, List[dict]]:
         return await self.get_gdat(LID=lobby_id, GID=game_id)
 
     async def get_current_server(self, user_id: IntValue) -> Tuple[dict, dict, List[dict]]:
         return await self.get_gdat(UID=user_id)
 
     async def get_gdat(self, **kwargs: IntValue) -> Tuple[dict, dict, List[dict]]:
-        if self.track_steps and TheaterStep.user not in self.completed_steps:
+        if not self.completed_step(TheaterStep.user):
             await self.authenticate()
 
         tid = self.get_transaction_id()
         server_details_packet = self.build_gdat_packet(
             tid,
             **kwargs
         )
```

### Comparing `pybfbc2stats-0.7.2/pybfbc2stats/asyncio_connection.py` & `pybfbc2stats-0.8.0/pybfbc2stats/asyncio_connection.py`

 * *Files identical despite different names*

### Comparing `pybfbc2stats-0.7.2/pybfbc2stats/buffer.py` & `pybfbc2stats-0.8.0/pybfbc2stats/buffer.py`

 * *Files identical despite different names*

### Comparing `pybfbc2stats-0.7.2/pybfbc2stats/client.py` & `pybfbc2stats-0.8.0/pybfbc2stats/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import List, Union, Dict, Tuple, Optional, Callable
 from urllib.parse import quote_from_bytes, unquote_to_bytes
 
 from .buffer import Buffer, ByteOrder
 from .connection import SecureConnection, Connection
 from .constants import STATS_KEYS, FRAGMENT_SIZE, FeslStep, Namespace, Platform, BACKEND_DETAILS, LookupType, \
     DEFAULT_LEADERBOARD_KEYS, Step, TheaterStep, FeslTransmissionType, TheaterTransmissionType, StructuredDataType, \
-    EPOCH_START, ENCODING, FeslParseMap, TheaterParseMap
+    EPOCH_START, ENCODING, FeslParseMap, TheaterParseMap, Backend
 from .exceptions import ParameterError, Error, PlayerNotFoundError, \
     SearchError, AuthError, ServerNotFoundError, LobbyNotFoundError, RecordNotFoundError, ConnectionError, TimeoutError
 from .packet import Packet, FeslPacket, TheaterPacket
 from .payload import Payload, StrValue, IntValue, ParseMap
 
 
 class Client:
@@ -44,14 +44,20 @@
 
     def __enter__(self):
         return self
 
     def __exit__(self, *excinfo):
         self.connection.close()
 
+    def completed_step(self, step: Step) -> bool:
+        if not self.track_steps:
+            return False
+
+        return step in self.completed_steps
+
     def wrapped_read(self, tid: int) -> Packet:
         """
         Read a single packet from the connection and automatically respond plus read next packet if the initial packet
         was one that requires an immediate response (memcheck, ping)
         :return: A packet containing "real" data
         """
         initial_packet = self.connection.read()
@@ -95,41 +101,47 @@
         return parsed
 
     @staticmethod
     def dict_list_to_dict(dict_list: List[dict]) -> dict:
         sorted_list = sorted(dict_list, key=lambda x: x['key'])
         return {entry['key']: entry['value'] for entry in sorted_list}
 
+    @staticmethod
+    def get_backend_details(backend: Backend, platform: Platform) -> Tuple[str, int, bytes]:
+        backend_details = BACKEND_DETAILS.get(backend, dict()).get(platform)
+
+        if backend_details is None:
+            raise Error(f'Backend {backend} does not support platform {platform}')
+
+        return backend_details['host'], backend_details['port'], backend_details['clientString']
+
 
 class FeslClient(Client):
     username: StrValue
     password: StrValue
     connection: SecureConnection
     completed_steps: Dict[FeslStep, Packet]
 
     def __init__(self, username: StrValue, password: StrValue, platform: Platform, timeout: float = 3.0,
                  track_steps: bool = True):
-        connection = SecureConnection(
-            BACKEND_DETAILS[platform]['host'],
-            BACKEND_DETAILS[platform]['port'],
-            FeslPacket
-        )
-        super().__init__(connection, platform, BACKEND_DETAILS[platform]['clientString'], timeout, track_steps)
+        host, port, client_string = self.get_backend_details(Backend.official, platform)
+        connection = SecureConnection(host, port, FeslPacket)
+        super().__init__(connection, platform, client_string, timeout, track_steps)
         self.username = username
         self.password = password
 
     def __exit__(self, *excinfo):
         try:
             self.logout()
         except (ConnectionError, TimeoutError):
             pass
         self.connection.close()
 
     def hello(self) -> bytes:
-        if self.track_steps and FeslStep.hello in self.completed_steps:
+        if self.completed_step(FeslStep.hello):
             return bytes(self.completed_steps[FeslStep.hello])
 
         tid = self.get_transaction_id()
         hello_packet = self.build_hello_packet(tid, self.client_string)
         self.connection.write(hello_packet)
 
         # FESL sends hello response immediately followed initial memcheck => read both and return hello response
@@ -143,79 +155,130 @@
 
         return bytes(response)
 
     def memcheck(self) -> None:
         memcheck_packet = self.build_memcheck_packet()
         self.connection.write(memcheck_packet)
 
-    def login(self) -> bytes:
-        if self.track_steps and FeslStep.login in self.completed_steps:
+    def login(self, tos_version: Optional[StrValue] = None) -> bytes:
+        if self.completed_step(FeslStep.login):
             return bytes(self.completed_steps[FeslStep.login])
-        elif self.track_steps and FeslStep.hello not in self.completed_steps:
+        elif not self.completed_step(FeslStep.hello):
             self.hello()
 
         tid = self.get_transaction_id()
-        login_packet = self.build_login_packet(tid, self.username, self.password)
+        login_packet = self.build_login_packet(tid, self.username, self.password, tos_version)
         self.connection.write(login_packet)
         response = self.wrapped_read(tid)
 
         response_valid, error_message, code = self.is_valid_login_response(response)
         if not response_valid:
+            # If we received a "TOS Content is out of date" error, fetch current TOS version and try login one more time
+            if code == 260 and tos_version is None and (tos_version := self.get_tos_version()) != bytes():
+                return self.login(tos_version)
             raise AuthError(error_message)
 
         self.completed_steps[FeslStep.login] = response
 
         return bytes(response)
 
+    def login_persona(self, persona_name: Optional[str] = None) -> bytes:
+        if not self.completed_step(FeslStep.login):
+            self.login()
+
+        # Fetch and use first available persona if none was given
+        if persona_name is None:
+            personas = self.get_personas()
+            if len(personas) < 1:
+                raise AuthError("No persona available for login")
+
+            persona_name = personas[0]
+
+        tid = self.get_transaction_id()
+        login_persona_packet = self.build_persona_login_packet(tid, persona_name)
+        self.connection.write(login_persona_packet)
+        response = self.wrapped_read(tid)
+
+        response_valid, error_message, _ = self.is_valid_login_response(response)
+        if not response_valid:
+            raise AuthError(error_message)
+
+        self.completed_steps[FeslStep.login_persona] = response
+
+        return bytes(response)
+
     def logout(self) -> Optional[bytes]:
-        if self.track_steps and FeslStep.login in self.completed_steps:
+        if self.completed_step(FeslStep.hello):
             tid = self.get_transaction_id()
             logout_packet = self.build_logout_packet(tid)
             self.connection.write(logout_packet)
             self.completed_steps.clear()
             return bytes(self.wrapped_read(tid))
 
     def ping(self) -> None:
         ping_packet = self.build_ping_packet()
         self.connection.write(ping_packet)
 
+    def get_tos_version(self) -> bytes:
+        if not self.completed_step(FeslStep.hello):
+            self.hello()
+
+        tid = self.get_transaction_id()
+        packet = self.build_tos_packet(tid)
+        self.connection.write(packet)
+        response = self.get_response(tid)
+
+        return response.get('version', bytes())
+
     def get_theater_details(self) -> Tuple[str, int]:
-        if self.track_steps and FeslStep.hello not in self.completed_steps:
+        if not self.completed_step(FeslStep.hello):
             self.hello()
 
         packet = self.completed_steps[FeslStep.hello]
         payload = packet.get_payload()
 
         # Field is called "ip" but actually contains the hostname
         return payload.get_str('theaterIp', str()), payload.get_int('theaterPort', int())
 
     def get_lkey(self) -> str:
-        if self.track_steps and FeslStep.login not in self.completed_steps:
+        if not self.completed_step(FeslStep.login):
             self.login()
 
         packet = self.completed_steps[FeslStep.login]
         payload = packet.get_payload()
 
         return payload.get_str('lkey', str())
 
+    def get_personas(self) -> List[str]:
+        if not self.completed_step(FeslStep.login):
+            self.login()
+
+        tid = self.get_transaction_id()
+        packet = self.build_get_personas_packet(tid)
+        self.connection.write(packet)
+
+        payload = self.get_response(tid, parse_map=FeslParseMap.Personas)
+        personas = payload.get_list('personas', list())
+        return personas
+
     def lookup_usernames(self, usernames: List[StrValue], namespace: Namespace) -> List[dict]:
         return self.lookup_user_identifiers(usernames, namespace, LookupType.byName)
 
     def lookup_username(self, username: StrValue, namespace: Namespace) -> dict:
         return self.lookup_user_identifier(username, namespace, LookupType.byName)
 
     def lookup_user_ids(self, user_ids: List[IntValue], namespace: Namespace) -> List[dict]:
         return self.lookup_user_identifiers(user_ids, namespace, LookupType.byId)
 
     def lookup_user_id(self, user_id: IntValue, namespace: Namespace) -> dict:
         return self.lookup_user_identifier(user_id, namespace, LookupType.byId)
 
     def lookup_user_identifiers(self, identifiers: List[Union[StrValue, IntValue]], namespace: Namespace,
                                 lookup_type: LookupType) -> List[dict]:
-        if self.track_steps and FeslStep.login not in self.completed_steps:
+        if not self.completed_step(FeslStep.login):
             self.login()
 
         tid = self.get_transaction_id()
         lookup_packet = self.build_user_lookup_packet(tid, identifiers, namespace, lookup_type)
         self.connection.write(lookup_packet)
 
         payload = self.get_response(tid, parse_map=FeslParseMap.UserLookup)
@@ -227,60 +290,60 @@
 
         if len(results) == 0:
             raise PlayerNotFoundError('User lookup did not return any results')
 
         return results.pop()
 
     def search_name(self, screen_name: StrValue, namespace: Namespace) -> dict:
-        if self.track_steps and FeslStep.login not in self.completed_steps:
+        if not self.completed_step(FeslStep.login):
             self.login()
 
         tid = self.get_transaction_id()
         search_packet = self.build_search_packet(tid, screen_name, namespace)
         self.connection.write(search_packet)
 
         payload = self.get_response(tid, parse_map=FeslParseMap.NameSearch)
         return {
             'namespace': payload.get_str('nameSpaceId', str()),
             'users': payload.get_list('users', list())
         }
 
     def get_stats(self, userid: IntValue, keys: List[StrValue] = STATS_KEYS) -> dict:
-        if self.track_steps and FeslStep.login not in self.completed_steps:
+        if not self.completed_step(FeslStep.login):
             self.login()
 
         # Send query in chunks (using the same transaction id for all packets)
         tid = self.get_transaction_id()
         chunk_packets = self.build_stats_query_packets(tid, userid, keys)
         for chunk_packet in chunk_packets:
             self.connection.write(chunk_packet)
 
         payload = self.get_response(tid, parse_map=FeslParseMap.Stats)
         return self.dict_list_to_dict(payload.get_list('stats', list()))
 
     def get_leaderboard(self, min_rank: IntValue = 1, max_rank: IntValue = 50, sort_by: StrValue = 'score',
                         keys: List[StrValue] = DEFAULT_LEADERBOARD_KEYS) -> List[dict]:
-        if self.track_steps and FeslStep.login not in self.completed_steps:
+        if not self.completed_step(FeslStep.login):
             self.login()
 
         tid = self.get_transaction_id()
         leaderboard_packet = self.build_leaderboard_query_packet(tid, min_rank, max_rank, sort_by, keys)
         self.connection.write(leaderboard_packet)
 
-        payload = self.get_response(tid, parse_map=FeslParseMap.Stats)
+        payload = self.get_response(tid, parse_map=FeslParseMap.Leaderboard)
         # Turn sub lists into dicts and return result
         return [
             {
                 key: Client.dict_list_to_dict(value) if isinstance(value, list) else value
                 for (key, value) in entry.items()
             } for entry in payload.get_list('stats', list())
         ]
 
     def get_dogtags(self, userid: IntValue) -> List[dict]:
-        if self.track_steps and FeslStep.login not in self.completed_steps:
+        if not self.completed_step(FeslStep.login):
             self.login()
 
         tid = self.get_transaction_id()
         dogtags_packet = self.build_dogtag_query_packet(tid, userid)
         self.connection.write(dogtags_packet)
 
         payload = self.get_response(tid, parse_map=FeslParseMap.Dogtags)
@@ -350,23 +413,24 @@
         return FeslPacket.build(
             b'fsys',
             Payload(TXN='MemCheck', result=None),
             FeslTransmissionType.SinglePacketResponse
         )
 
     @staticmethod
-    def build_login_packet(tid: int, username: StrValue, password: StrValue) -> FeslPacket:
+    def build_login_packet(tid: int, username: StrValue, password: StrValue, tos_version: Optional[StrValue] = None) -> FeslPacket:
         return FeslPacket.build(
             b'acct',
             Payload(
                 TXN='Login',
                 returnEncryptedInfo=0,
                 name=username,
                 password=password,
-                macAddr='$000000000000'
+                macAddr='$000000000000',
+                tosVersion=tos_version
             ),
             FeslTransmissionType.SinglePacketRequest,
             tid
         )
 
     @staticmethod
     def build_logout_packet(tid: int) -> FeslPacket:
@@ -382,14 +446,41 @@
         return FeslPacket.build(
             b'fsys',
             Payload(TXN='Ping'),
             FeslTransmissionType.SinglePacketResponse
         )
 
     @staticmethod
+    def build_tos_packet(tid: int) -> FeslPacket:
+        return FeslPacket.build(
+            b'acct',
+            Payload(TXN='NuGetTos'),
+            FeslTransmissionType.SinglePacketRequest,
+            tid
+        )
+
+    @staticmethod
+    def build_get_personas_packet(tid: int) -> FeslPacket:
+        return FeslPacket.build(
+            b'acct',
+            Payload(TXN='NuGetPersonas', namespace=''),
+            FeslTransmissionType.SinglePacketRequest,
+            tid
+        )
+
+    @staticmethod
+    def build_persona_login_packet(tid: int, persona_name: StrValue) -> FeslPacket:
+        return FeslPacket.build(
+            b'acct',
+            Payload(TXN='NuLoginPersona', name=persona_name),
+            FeslTransmissionType.SinglePacketRequest,
+            tid
+        )
+
+    @staticmethod
     def build_user_lookup_packet(
             tid: int,
             user_identifiers: List[Union[StrValue, IntValue]],
             namespace: Union[Namespace, bytes],
             lookup_type: Union[LookupType, bytes]
     ) -> FeslPacket:
         lookups = [
@@ -751,23 +842,24 @@
 class TheaterClient(Client):
     lkey: StrValue
     completed_steps: Dict[TheaterStep, Packet]
 
     def __init__(self, host: str, port: int, lkey: StrValue, platform: Platform, timeout: float = 3.0,
                  track_steps: bool = True):
         connection = Connection(host, port, TheaterPacket)
-        super().__init__(connection, platform, BACKEND_DETAILS[platform]['clientString'], timeout, track_steps)
+        _, _, client_string = self.get_backend_details(Backend.official, platform)
+        super().__init__(connection, platform, client_string, timeout, track_steps)
         self.lkey = lkey
 
     def connect(self) -> bytes:
         """
         Initialize the connection to the Theater backend by sending the initial CONN/hello packet
         :return: Response packet data
         """
-        if self.track_steps and TheaterStep.conn in self.completed_steps:
+        if self.completed_step(TheaterStep.conn):
             return bytes(self.completed_steps[TheaterStep.conn])
 
         tid = self.get_transaction_id()
         connect_packet = self.build_conn_packet(tid, self.client_string)
         self.connection.write(connect_packet)
 
         response = self.connection.read()
@@ -776,17 +868,17 @@
         return bytes(response)
 
     def authenticate(self) -> bytes:
         """
         Authenticate against/log into the Theater backend using the lkey retrieved via FESL
         :return: Response packet data
         """
-        if self.track_steps and TheaterStep.user in self.completed_steps:
+        if self.completed_step(TheaterStep.user):
             return bytes(self.completed_steps[TheaterStep.user])
-        elif self.track_steps and TheaterStep.conn not in self.completed_steps:
+        elif not self.completed_step(TheaterStep.conn):
             self.connect()
 
         tid = self.get_transaction_id()
         auth_packet = self.build_user_packet(tid, self.lkey)
         self.connection.write(auth_packet)
 
         response = self.connection.read()
@@ -803,15 +895,15 @@
         self.connection.write(ping_packet)
 
     def get_lobbies(self) -> List[dict]:
         """
         Retrieve all available game (server) lobbies
         :return: List of lobby details
         """
-        if self.track_steps and TheaterStep.user not in self.completed_steps:
+        if not self.completed_step(TheaterStep.user):
             self.authenticate()
 
         tid = self.get_transaction_id()
         lobby_list_packet = self.build_llst_packet(tid)
         self.connection.write(lobby_list_packet)
 
         # Theater responds with an initial LLST packet, indicating the number of lobbies,
@@ -831,15 +923,15 @@
 
     def get_servers(self, lobby_id: IntValue) -> List[dict]:
         """
         Retrieve all available game servers from the given lobby
         :param lobby_id: Id of the game server lobby
         :return: List of server details
         """
-        if self.track_steps and TheaterStep.user not in self.completed_steps:
+        if not self.completed_step(TheaterStep.user):
             self.authenticate()
 
         tid = self.get_transaction_id()
         server_list_packet = self.build_glst_packet(tid, lobby_id)
         self.connection.write(server_list_packet)
 
         # Again, same procedure: Theater first responds with a GLST packet which indicates the number of games/servers
@@ -887,15 +979,15 @@
         """
         Get GDAT for an individual server
         :param kwargs: Id(s) to identify the game (server):
             a) id of lobby the game server is hosted in (lid) and Id of the game server or (gid)
             b) id of user for which the current server should be returned (uid)
         :return: Tuple of (general server details, extended details, player list)
         """
-        if self.track_steps and TheaterStep.user not in self.completed_steps:
+        if not self.completed_step(TheaterStep.user):
             self.authenticate()
 
         tid = self.get_transaction_id()
         server_details_packet = self.build_gdat_packet(
             tid,
             **kwargs
         )
```

### Comparing `pybfbc2stats-0.7.2/pybfbc2stats/connection.py` & `pybfbc2stats-0.8.0/pybfbc2stats/connection.py`

 * *Files identical despite different names*

### Comparing `pybfbc2stats-0.7.2/pybfbc2stats/constants.py` & `pybfbc2stats-0.8.0/pybfbc2stats/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 class Step(int, Enum):
     pass
 
 
 class FeslStep(Step):
     hello = 1
     login = 2
+    login_persona = 3
 
 
 class TheaterStep(Step):
     conn = 1
     user = 2
 
 
@@ -44,14 +45,19 @@
 
 class Platform(int, Enum):
     pc = 1
     xbox360 = 2
     ps3 = 3
 
 
+class Backend(int, Enum):
+    official = 1
+    rome = 2
+
+
 class TransmissionType(int, Enum):
     pass
 
 
 class FeslTransmissionType(TransmissionType):
     Ping = 1
     SinglePacketResponse = 2
@@ -81,14 +87,17 @@
 
 class ParseMapEnum(dict, Enum):
     def __contains__(self, item):
         return item in self.value
 
 
 class FeslParseMap(ParseMapEnum):
+    Personas = {
+        MagicParseKey.list: str
+    }
     UserLookup = {
         'userId': int,
         'masterUserId': int,
         'xuid': int,
         MagicParseKey.fallback: str
     }
     NameSearch = {
@@ -182,30 +191,39 @@
 HEADER_LENGTH = 12
 HEADER_BYTE_ORDER = 'big'
 ENCODING = 'utf8'
 EPOCH_START = datetime(2008, 1, 1, tzinfo=timezone.utc)
 VALID_HEADER_TYPES_FESL = [b'acct', b'fsys', b'rank', b'recp']
 VALID_HEADER_TYPES_THEATER = [b'CONN', b'USER', b'LLST', b'LDAT', b'GLST', b'GDAT', b'GDET', b'PDAT', b'PING']
 VALID_HEADER_ERROR_INDICATORS = [b'ngam', b'nrom', b'bpar', b'ntfn']
-BACKEND_DETAILS = {
-    Platform.pc: {
-        'host': 'bfbc2-pc-server.fesl.ea.com',
-        'port': 18321,
-        'clientString': b'bfbc2-pc'
-    },
-    Platform.xbox360: {
-        # Xbox 360 FESL (and Theater) resolve to private IP addresses, see DNS_OVERRIDES below for their public IPs
-        'host': 'bfbc2-360-server.fesl.ea.com',
-        'port': 18341,
-        'clientString': b'bfbc2-360'
+BACKEND_DETAILS: Dict[Backend, Dict[Platform, dict]] = {
+    Backend.official: {
+        Platform.pc: {
+            'host': 'bfbc2-pc-server.fesl.ea.com',
+            'port': 18321,
+            'clientString': b'bfbc2-pc'
+        },
+        Platform.xbox360: {
+            # Xbox 360 FESL (and Theater) resolve to private IP addresses, see DNS_OVERRIDES below for their public IPs
+            'host': 'bfbc2-360-server.fesl.ea.com',
+            'port': 18341,
+            'clientString': b'bfbc2-360'
+        },
+        Platform.ps3: {
+            'host': 'bfbc2-ps3-server.fesl.ea.com',
+            'port': 18331,
+            'clientString': b'bfbc2-ps3'
+        }
     },
-    Platform.ps3: {
-        'host': 'bfbc2-ps3-server.fesl.ea.com',
-        'port': 18331,
-        'clientString': b'bfbc2-ps3'
+    Backend.rome: {
+        Platform.pc: {
+            'host': 'bfbc2.emulatornexus.com',
+            'port': 18390,
+            'clientString': b'bfbc2-pc'
+        }
     }
 }
 # Added inactive PC and PS3 overrides for potential future use
 DNS_OVERRIDES = {
     # 'bfbc2-pc-server.fesl.ea.com': '159.153.64.138',
     # 'bfbc2-pc-server.theater.ea.com': '159.153.64.163',
     'bfbc2-360-server.fesl.ea.com': '159.153.64.190',
```

### Comparing `pybfbc2stats-0.7.2/pybfbc2stats/packet.py` & `pybfbc2stats-0.8.0/pybfbc2stats/packet.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         Add any missing header bytes as zero now and update later:
         - transmission type [1 byte]
         - tid [3 bytes, relevant only for FESL]
         - length indicator [4 bytes]
         """
         header = header_stub + b'\x00' * (HEADER_LENGTH - len(header_stub))
         # Add "tail" to body
-        body = bytes(body_data) + b'\x00'
+        body = bytes(body_data) + b'\n\x00'
         self = cls(header, body)
         # Update transaction id if given
         if tid is not None:
             self.set_tid(tid)
         # Update transmission type
         self.set_transmission_type(transmission_type)
         # Update length indicators
@@ -114,17 +114,25 @@
         self.validate_body()
 
     def get_payload(self, parse_map: Optional[ParseMap] = None) -> Payload:
         return Payload.from_bytes(self.get_data(), parse_map)
 
     def get_data(self) -> bytes:
         """
-        Get packet data (body without any trailing \x00 byte)
+        Get packet data (body without any trailing \x00 byte and linebreak)
         """
-        return self.body[:-1] if len(self.body) > 0 and self.body[-1] == 0 else self.body
+        data = self.body
+        # Remove any trailing \x00 byte
+        if len(data) > 0 and data[-1] == 0:
+            data = data[:-1]
+        # Remove any trailing line break
+        if len(data) > 0 and data[-1] == 10:
+            data = data[:-1]
+
+        return data
 
     def get_data_lines(self) -> List[bytes]:
         """
         Get packet data split into lines
         """
         return self.get_data().split(b'\n')
 
@@ -238,15 +246,15 @@
 
 class TheaterPacket(Packet):
     def set_tid(self, tid: int) -> None:
         """
         Set/update the transaction id/packet counter in packet body (requires re-calculation of length indicators)
         """
         # Remove body "tail", add tid and add "tail" again
-        self.body = self.body[:-1] + b'\nTID=' + str(tid).encode(ENCODING) + b'\x00'
+        self.body = self.body[:-2] + b'\nTID=' + str(tid).encode(ENCODING) + b'\n\x00'
 
     def get_tid(self) -> int:
         """
         Get transaction id from packet body
         :return: transaction id as int
         """
         return self.get_payload().get_int('TID', int())
```

### Comparing `pybfbc2stats-0.7.2/pybfbc2stats/payload.py` & `pybfbc2stats-0.8.0/pybfbc2stats/payload.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,21 @@
     def pop(self, key: str) -> PayloadValue:
         return self.data.pop(key)
 
     def keys(self) -> List[str]:
         return list(self.data.keys())
 
     def get(self, key: str, default: Optional[bytes] = None) -> Optional[Union[PayloadValue, PayloadStruct]]:
-        return self.data.get(key, default)
+        value = self.data.get(key, default)
+
+        # Project Rome Theater returns any packet TID with a trailing \x00 byte, waiting for a fix on their end
+        if key == 'TID' and isinstance(value, bytes):
+            value = value.rstrip(b'\x00')
+
+        return value
 
     def get_str(self, key: str, default: Optional[str] = None) -> Optional[str]:
         value = self.get(key)
         if value is None:
             return default
 
         if isinstance(value, bytes):
@@ -296,15 +302,16 @@
         as_str = Payload.parse_str(value)
         return Payload.str_to_bool(as_str)
 
     @staticmethod
     def str_to_bool(value: str) -> bool:
         if value in ['1', 'YES']:
             return True
-        if value in ['0', 'NO']:
+        # Project Rome Theater returns the server PW as an empty field, waiting for fix/clarification
+        if value in ['0', 'NO', '']:
             return False
 
         # Raise error to adhere to behaviour of other parse methods
         raise Error(f'could not convert string to bool: \'{value}\'')
 
     @staticmethod
     def get_struct_length(data: ParsedPayloadStruct, indicator: Union[StructLengthIndicator, str]) -> int:
```

### Comparing `pybfbc2stats-0.7.2/pybfbc2stats.egg-info/PKG-INFO` & `pybfbc2stats-0.8.0/pybfbc2stats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybfbc2stats
-Version: 0.7.2
+Version: 0.8.0
 Summary: Python library for retrieving statistics of Battlefield: Bad Company 2 players
 Home-page: https://github.com/cetteup/pybfbc2stats
 Author: cetteup
 Author-email: me@cetteup.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cetteup/pybfbc2stats/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pybfbc2stats-0.7.2/pybfbc2stats.egg-info/SOURCES.txt` & `pybfbc2stats-0.8.0/pybfbc2stats.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 pybfbc2stats/client.py
 pybfbc2stats/connection.py
 pybfbc2stats/constants.py
 pybfbc2stats/exceptions.py
 pybfbc2stats/logger.py
 pybfbc2stats/packet.py
 pybfbc2stats/payload.py
+pybfbc2stats/rome.py
 pybfbc2stats.egg-info/PKG-INFO
 pybfbc2stats.egg-info/SOURCES.txt
 pybfbc2stats.egg-info/dependency_links.txt
 pybfbc2stats.egg-info/top_level.txt
 tests/test_client.py
 tests/test_packet.py
 tests/test_payload.py
```

### Comparing `pybfbc2stats-0.7.2/setup.cfg` & `pybfbc2stats-0.8.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pybfbc2stats
-version = 0.7.2
+version = 0.8.0
 description = Python library for retrieving statistics of Battlefield: Bad Company 2 players
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cetteup/pybfbc2stats
 project_urls = 
 	Bug Tracker = https://github.com/cetteup/pybfbc2stats/issues
 author = cetteup
```

### Comparing `pybfbc2stats-0.7.2/tests/test_client.py` & `pybfbc2stats-0.8.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pybfbc2stats-0.7.2/tests/test_packet.py` & `pybfbc2stats-0.8.0/tests/test_packet.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,29 +14,29 @@
         transmission_type = FeslTransmissionType.SinglePacketRequest
         tid = 1
 
         # WHEN
         packet = FeslPacket.build(header_stub, body_data, transmission_type, tid)
 
         # THEN
-        expected = FeslPacket(b'fsys\xc0\x00\x00\x01\x00\x00\x00\x16', b'TXN=Hello\x00')
+        expected = FeslPacket(b'fsys\xc0\x00\x00\x01\x00\x00\x00\x17', b'TXN=Hello\n\x00')
         self.assertEqual(expected, packet)
         self.assertIsNone(packet.validate())
 
     def test_build_no_tid(self):
         # GIVEN
         header_stub = b'fsys'
         body_data = b'TXN=MemCheck\nresult='
         transmission_type = FeslTransmissionType.SinglePacketResponse
 
         # WHEN
         packet = FeslPacket.build(header_stub, body_data, transmission_type)
 
         # THEN
-        expected = FeslPacket(b'fsys\x80\x00\x00\x00\x00\x00\x00!', b'TXN=MemCheck\nresult=\x00')
+        expected = FeslPacket(b'fsys\x80\x00\x00\x00\x00\x00\x00"', b'TXN=MemCheck\nresult=\n\x00')
         self.assertEqual(expected, packet)
         self.assertIsNone(packet.validate())
 
     def test_to_bytes(self):
         # GIVEN
         header = b'fsys\x80\x00\x00\x00\x00\x00\x00"'
         body = b'TXN=MemCheck\nresult=\n\x00'
@@ -149,28 +149,28 @@
         payload = packet.get_payload(parse_map)
 
         # THEN
         self.assertEqual(Payload.from_bytes(data, parse_map), payload)
 
     def test_get_data(self):
         # GIVEN
-        expected_data = b'TXN=MemCheck\nresult=\n'
-        packet = FeslPacket(b'fsys\x80\x00\x00\x00\x00\x00\x00"', expected_data + b'\x00')
+        expected_data = b'TXN=MemCheck\nresult='
+        packet = FeslPacket(b'fsys\x80\x00\x00\x00\x00\x00\x00!', expected_data + b'\x00')
         self.assertIsNone(packet.validate())
 
         # WHEN
         data = packet.get_data()
 
         # THEN
         self.assertEqual(expected_data, data)
 
     def test_get_data_lines(self):
         # GIVEN
-        expected_data_lines = [b'TXN=MemCheck', b'result=', b'']
-        packet = FeslPacket(b'fsys\x80\x00\x00\x00\x00\x00\x00"', b'\n'.join(expected_data_lines) + b'\x00')
+        expected_data_lines = [b'TXN=MemCheck', b'result=']
+        packet = FeslPacket(b'fsys\x80\x00\x00\x00\x00\x00\x00!', b'\n'.join(expected_data_lines) + b'\x00')
         self.assertIsNone(packet.validate())
 
         # WHEN
         data_lines = packet.get_data_lines()
 
         # THEN
         self.assertEqual(expected_data_lines, data_lines)
@@ -184,29 +184,29 @@
         transmission_type = TheaterTransmissionType.Request
         tid = 1
 
         # WHEN
         packet = TheaterPacket.build(header_stub, body_data, transmission_type, tid)
 
         # THEN
-        expected = TheaterPacket(b'GDAT@\x00\x00\x00\x00\x00\x00%', b'LID=257\nGID=123456\nTID=1\x00')
+        expected = TheaterPacket(b'GDAT@\x00\x00\x00\x00\x00\x00&', b'LID=257\nGID=123456\nTID=1\n\x00')
         self.assertEqual(expected, packet)
         self.assertIsNone(packet.validate())
 
     def test_build_no_tid(self):
         # GIVEN
         header_stub = b'PING'
         body_data = b'TID=0'
         transmission_type = TheaterTransmissionType.OKResponse
 
         # WHEN
         packet = TheaterPacket.build(header_stub, body_data, transmission_type)
 
         # THEN
-        expected = TheaterPacket(b'PING\x00\x00\x00\x00\x00\x00\x00\x12', b'TID=0\x00')
+        expected = TheaterPacket(b'PING\x00\x00\x00\x00\x00\x00\x00\x13', b'TID=0\n\x00')
         self.assertEqual(expected, packet)
         self.assertIsNone(packet.validate())
 
     def test_to_bytes(self):
         # GIVEN
         header = b'GDAT@\x00\x00\x00\x00\x00\x00&'
         body = b'LID=257\nGID=123456\nTID=1\n\x00'
@@ -315,28 +315,28 @@
         body_length = packet.indicated_body_length()
 
         # THEN
         self.assertEqual(expected_length, body_length)
 
     def test_get_data(self):
         # GIVEN
-        expected_data = b'LID=257\nGID=123456\nTID=1\n'
-        packet = TheaterPacket(b'GDAT@\x00\x00\x00\x00\x00\x00&', expected_data + b'\x00')
+        expected_data = b'LID=257\nGID=123456\nTID=1'
+        packet = TheaterPacket(b'GDAT@\x00\x00\x00\x00\x00\x00%', expected_data + b'\x00')
         self.assertIsNone(packet.validate())
 
         # WHEN
         data = packet.get_data()
 
         # THEN
         self.assertEqual(expected_data, data)
 
     def test_get_data_lines(self):
         # GIVEN
-        expected_data_lines = [b'LID=257', b'GID=123456', b'TID=1', b'']
-        packet = TheaterPacket(b'GDAT@\x00\x00\x00\x00\x00\x00&', b'\n'.join(expected_data_lines) + b'\x00')
+        expected_data_lines = [b'LID=257', b'GID=123456', b'TID=1']
+        packet = TheaterPacket(b'GDAT@\x00\x00\x00\x00\x00\x00%', b'\n'.join(expected_data_lines) + b'\x00')
         self.assertIsNone(packet.validate())
 
         # WHEN
         data_lines = packet.get_data_lines()
 
         # THEN
         self.assertEqual(expected_data_lines, data_lines)
```

### Comparing `pybfbc2stats-0.7.2/tests/test_payload.py` & `pybfbc2stats-0.8.0/tests/test_payload.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,25 +198,25 @@
 
         # THEN
         self.assertEqual([1.0, -1.0, 3.22E7, 3.22E-7], payload.data.get('float'))
 
     def test_from_bytes_list_parsed_bool(self):
         # GIVEN
         data = join_data([
-            b'bool.0=1', b'bool.1=0', b'bool.2=YES', b'bool.3=NO', b'bool.[]=4',
+            b'bool.0=1', b'bool.1=0', b'bool.2=YES', b'bool.3=NO', b'bool.4=', b'bool.[]=5',
         ])
         parse_map = {
             MagicParseKey.list: bool
         }
 
         # WHEN
         payload = Payload.from_bytes(data, parse_map)
 
         # THEN
-        self.assertEqual([True, False, True, False], payload.data.get('bool'))
+        self.assertEqual([True, False, True, False, False], payload.data.get('bool'))
 
     def test_from_bytes_list_parsed_nested(self):
         # GIVEN
         data = join_data([
             b'nested.0.0=1', b'nested.0.1=2', b'nested.0.2=3', b'nested.0.3=4', b'nested.0.4=5',
             b'nested.0.[]=5', b'nested.[]=1',
         ])
@@ -321,29 +321,31 @@
             'c-key': 3.22E7,
             'd-key': 3.22E-7
         }, payload.data.get('float'))
 
     def test_from_bytes_map_parsed_bool(self):
         # GIVEN
         data = join_data([
-            b'bool.{a-key}=1', b'bool.{b-key}=0', b'bool.{c-key}=YES', b'bool.{d-key}=NO', b'bool.{}=4',
+            b'bool.{a-key}=1', b'bool.{b-key}=0', b'bool.{c-key}=YES', b'bool.{d-key}=NO', b'bool.{e-key}=',
+            b'bool.{}=5',
         ])
         parse_map = {
             MagicParseKey.map: bool
         }
 
         # WHEN
         payload = Payload.from_bytes(data, parse_map)
 
         # THEN
         self.assertEqual({
             'a-key': True,
             'b-key': False,
             'c-key': True,
-            'd-key': False
+            'd-key': False,
+            'e-key': False
         }, payload.data.get('bool'))
 
     def test_from_bytes_map_parsed_nested(self):
         # GIVEN
         data = join_data([
             b'nested.{a-key}.{aa-key}=1', b'nested.{a-key}.{ab-key}=2', b'nested.{a-key}.{ac-key}=3',
             b'nested.{a-key}.{ad-key}=4', b'nested.{a-key}.{ae-key}=5',
@@ -1342,7 +1344,17 @@
         self.assertEqual('PC', payload.get_str('PL'))
         self.assertEqual(1000, payload.get_int('B-U-elo'))
         self.assertEqual(0, payload.get_int('B-maxObservers'))
         self.assertEqual(0, payload.get_int('PW'))
         self.assertEqual(19, payload.get_int('TID'))
         self.assertEqual('NO', payload.get_str('B-U-coralsea'))
         self.assertEqual(0, payload.get_int('AP'))
+
+    def test_tid_with_nil_byte(self):
+        # GIVEN
+        payload = Payload.from_bytes(b'TID=1\x00')
+
+        # WHEN
+        tid = payload.get_int('TID')
+
+        # THEN
+        self.assertEqual(1, tid)
```

