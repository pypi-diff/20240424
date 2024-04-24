# Comparing `tmp/asyncmy-0.2.8rc2.tar.gz` & `tmp/asyncmy-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncmy-0.2.8rc2.tar", max compression
+gzip compressed data, was "asyncmy-0.2.9.tar", max compression
```

## Comparing `asyncmy-0.2.8rc2.tar` & `asyncmy-0.2.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1307 2023-05-17 06:17:20.540243 asyncmy-0.2.8rc2/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-05-17 06:17:20.540243 asyncmy-0.2.8rc2/LICENSE
--rw-r--r--   0        0        0     5077 2023-05-17 06:17:20.540243 asyncmy-0.2.8rc2/README.md
--rw-r--r--   0        0        0      106 2023-05-17 06:17:20.540243 asyncmy-0.2.8rc2/asyncmy/__init__.py
--rw-r--r--   0        0        0     6855 2023-05-17 06:17:20.540243 asyncmy-0.2.8rc2/asyncmy/auth.py
--rw-r--r--   0        0        0       50 2023-05-17 06:17:20.540243 asyncmy-0.2.8rc2/asyncmy/charset.pxd
--rw-r--r--   0        0        0    10493 2023-05-17 06:17:20.540243 asyncmy-0.2.8rc2/asyncmy/charset.pyx
--rw-r--r--   0        0        0    49722 2023-05-17 06:17:20.540243 asyncmy-0.2.8rc2/asyncmy/connection.pyx
--rw-r--r--   0        0        0      878 2023-05-17 06:17:20.540243 asyncmy-0.2.8rc2/asyncmy/constants/CLIENT.py
--rw-r--r--   0        0        0      129 2023-05-17 06:17:20.540243 asyncmy-0.2.8rc2/asyncmy/constants/COLUMN.py
--rw-r--r--   0        0        0      679 2023-05-17 06:17:20.540243 asyncmy-0.2.8rc2/asyncmy/constants/COMMAND.py
--rw-r--r--   0        0        0     1927 2023-05-17 06:17:20.540243 asyncmy-0.2.8rc2/asyncmy/constants/CR.py
--rw-r--r--   0        0        0    12296 2023-05-17 06:17:20.540243 asyncmy-0.2.8rc2/asyncmy/constants/ER.py
--rw-r--r--   0        0        0      370 2023-05-17 06:17:20.540243 asyncmy-0.2.8rc2/asyncmy/constants/FIELD_TYPE.py
--rw-r--r--   0        0        0      214 2023-05-17 06:17:20.540243 asyncmy-0.2.8rc2/asyncmy/constants/FLAG.py
--rw-r--r--   0        0        0      333 2023-05-17 06:17:20.540243 asyncmy-0.2.8rc2/asyncmy/constants/SERVER_STATUS.py
--rw-r--r--   0        0        0        0 2023-05-17 06:17:20.540243 asyncmy-0.2.8rc2/asyncmy/constants/__init__.py
--rw-r--r--   0        0        0     2131 2023-05-17 06:17:20.540243 asyncmy-0.2.8rc2/asyncmy/contexts.py
--rw-r--r--   0        0        0     9657 2023-05-17 06:17:20.540243 asyncmy-0.2.8rc2/asyncmy/converters.pyx
--rw-r--r--   0        0        0    17446 2023-05-17 06:17:20.540243 asyncmy-0.2.8rc2/asyncmy/cursors.pyx
--rw-r--r--   0        0        0     4004 2023-05-17 06:17:20.540243 asyncmy-0.2.8rc2/asyncmy/errors.pyx
--rw-r--r--   0        0        0      479 2023-05-17 06:17:20.540243 asyncmy-0.2.8rc2/asyncmy/optionfile.py
--rw-r--r--   0        0        0     6388 2023-05-17 06:17:20.544243 asyncmy-0.2.8rc2/asyncmy/pool.pyx
--rw-r--r--   0        0        0    11582 2023-05-17 06:17:20.544243 asyncmy-0.2.8rc2/asyncmy/protocol.pyx
--rw-r--r--   0        0        0       52 2023-05-17 06:17:20.544243 asyncmy-0.2.8rc2/asyncmy/replication/__init__.py
--rw-r--r--   0        0        0    13427 2023-05-17 06:17:20.544243 asyncmy-0.2.8rc2/asyncmy/replication/binlogstream.py
--rw-r--r--   0        0        0     2189 2023-05-17 06:17:20.544243 asyncmy-0.2.8rc2/asyncmy/replication/bitmap.py
--rw-r--r--   0        0        0     3254 2023-05-17 06:17:20.544243 asyncmy-0.2.8rc2/asyncmy/replication/column.py
--rw-r--r--   0        0        0     1687 2023-05-17 06:17:20.544243 asyncmy-0.2.8rc2/asyncmy/replication/constants.py
--rw-r--r--   0        0        0      277 2023-05-17 06:17:20.544243 asyncmy-0.2.8rc2/asyncmy/replication/errors.py
--rw-r--r--   0        0        0     6697 2023-05-17 06:17:20.544243 asyncmy-0.2.8rc2/asyncmy/replication/events.py
--rw-r--r--   0        0        0     8721 2023-05-17 06:17:20.544243 asyncmy-0.2.8rc2/asyncmy/replication/gtid.py
--rw-r--r--   0        0        0    15555 2023-05-17 06:17:20.544243 asyncmy-0.2.8rc2/asyncmy/replication/packets.py
--rw-r--r--   0        0        0    22843 2023-05-17 06:17:20.544243 asyncmy-0.2.8rc2/asyncmy/replication/row_events.py
--rw-r--r--   0        0        0      944 2023-05-17 06:17:20.544243 asyncmy-0.2.8rc2/asyncmy/replication/table.py
--rw-r--r--   0        0        0      178 2023-05-17 06:17:20.544243 asyncmy-0.2.8rc2/asyncmy/replication/utils.py
--rw-r--r--   0        0        0      455 2023-05-17 06:17:20.544243 asyncmy-0.2.8rc2/asyncmy/structs.py
--rw-r--r--   0        0        0       26 2023-05-17 06:17:20.544243 asyncmy-0.2.8rc2/asyncmy/version.py
--rw-r--r--   0        0        0      400 2023-05-17 06:17:20.544243 asyncmy-0.2.8rc2/build.py
--rw-r--r--   0        0        0     1299 2023-05-17 06:17:20.544243 asyncmy-0.2.8rc2/pyproject.toml
--rw-r--r--   0        0        0     5886 1970-01-01 00:00:00.000000 asyncmy-0.2.8rc2/setup.py
--rw-r--r--   0        0        0     5878 1970-01-01 00:00:00.000000 asyncmy-0.2.8rc2/PKG-INFO
+-rw-r--r--   0        0        0     1545 2023-11-29 02:31:54.649857 asyncmy-0.2.9/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-11-29 02:31:54.649857 asyncmy-0.2.9/LICENSE
+-rw-r--r--   0        0        0     5076 2023-11-29 02:31:54.649857 asyncmy-0.2.9/README.md
+-rw-r--r--   0        0        0      106 2023-11-29 02:31:54.649857 asyncmy-0.2.9/asyncmy/__init__.py
+-rw-r--r--   0        0        0     6855 2023-11-29 02:31:54.649857 asyncmy-0.2.9/asyncmy/auth.py
+-rw-r--r--   0        0        0       50 2023-11-29 02:31:54.649857 asyncmy-0.2.9/asyncmy/charset.pxd
+-rw-r--r--   0        0        0    10493 2023-11-29 02:31:54.649857 asyncmy-0.2.9/asyncmy/charset.pyx
+-rw-r--r--   0        0        0    51742 2023-11-29 02:31:54.649857 asyncmy-0.2.9/asyncmy/connection.pyx
+-rw-r--r--   0        0        0      878 2023-11-29 02:31:54.649857 asyncmy-0.2.9/asyncmy/constants/CLIENT.py
+-rw-r--r--   0        0        0      129 2023-11-29 02:31:54.649857 asyncmy-0.2.9/asyncmy/constants/COLUMN.py
+-rw-r--r--   0        0        0      679 2023-11-29 02:31:54.649857 asyncmy-0.2.9/asyncmy/constants/COMMAND.py
+-rw-r--r--   0        0        0     1927 2023-11-29 02:31:54.649857 asyncmy-0.2.9/asyncmy/constants/CR.py
+-rw-r--r--   0        0        0    12296 2023-11-29 02:31:54.649857 asyncmy-0.2.9/asyncmy/constants/ER.py
+-rw-r--r--   0        0        0      370 2023-11-29 02:31:54.649857 asyncmy-0.2.9/asyncmy/constants/FIELD_TYPE.py
+-rw-r--r--   0        0        0      214 2023-11-29 02:31:54.649857 asyncmy-0.2.9/asyncmy/constants/FLAG.py
+-rw-r--r--   0        0        0      333 2023-11-29 02:31:54.649857 asyncmy-0.2.9/asyncmy/constants/SERVER_STATUS.py
+-rw-r--r--   0        0        0        0 2023-11-29 02:31:54.649857 asyncmy-0.2.9/asyncmy/constants/__init__.py
+-rw-r--r--   0        0        0     2131 2023-11-29 02:31:54.649857 asyncmy-0.2.9/asyncmy/contexts.py
+-rw-r--r--   0        0        0     9658 2023-11-29 02:31:54.649857 asyncmy-0.2.9/asyncmy/converters.pyx
+-rw-r--r--   0        0        0    17446 2023-11-29 02:31:54.653857 asyncmy-0.2.9/asyncmy/cursors.pyx
+-rw-r--r--   0        0        0     4004 2023-11-29 02:31:54.653857 asyncmy-0.2.9/asyncmy/errors.pyx
+-rw-r--r--   0        0        0      479 2023-11-29 02:31:54.653857 asyncmy-0.2.9/asyncmy/optionfile.py
+-rw-r--r--   0        0        0     6388 2023-11-29 02:31:54.653857 asyncmy-0.2.9/asyncmy/pool.pyx
+-rw-r--r--   0        0        0    11582 2023-11-29 02:31:54.653857 asyncmy-0.2.9/asyncmy/protocol.pyx
+-rw-r--r--   0        0        0       52 2023-11-29 02:31:54.653857 asyncmy-0.2.9/asyncmy/replication/__init__.py
+-rw-r--r--   0        0        0    13570 2023-11-29 02:31:54.653857 asyncmy-0.2.9/asyncmy/replication/binlogstream.py
+-rw-r--r--   0        0        0     2189 2023-11-29 02:31:54.653857 asyncmy-0.2.9/asyncmy/replication/bitmap.py
+-rw-r--r--   0        0        0     3254 2023-11-29 02:31:54.653857 asyncmy-0.2.9/asyncmy/replication/column.py
+-rw-r--r--   0        0        0     1687 2023-11-29 02:31:54.653857 asyncmy-0.2.9/asyncmy/replication/constants.py
+-rw-r--r--   0        0        0      201 2023-11-29 02:31:54.653857 asyncmy-0.2.9/asyncmy/replication/errors.py
+-rw-r--r--   0        0        0     6697 2023-11-29 02:31:54.653857 asyncmy-0.2.9/asyncmy/replication/events.py
+-rw-r--r--   0        0        0     8721 2023-11-29 02:31:54.653857 asyncmy-0.2.9/asyncmy/replication/gtid.py
+-rw-r--r--   0        0        0    15555 2023-11-29 02:31:54.653857 asyncmy-0.2.9/asyncmy/replication/packets.py
+-rw-r--r--   0        0        0    22843 2023-11-29 02:31:54.653857 asyncmy-0.2.9/asyncmy/replication/row_events.py
+-rw-r--r--   0        0        0      944 2023-11-29 02:31:54.653857 asyncmy-0.2.9/asyncmy/replication/table.py
+-rw-r--r--   0        0        0      178 2023-11-29 02:31:54.653857 asyncmy-0.2.9/asyncmy/replication/utils.py
+-rw-r--r--   0        0        0      455 2023-11-29 02:31:54.653857 asyncmy-0.2.9/asyncmy/structs.py
+-rw-r--r--   0        0        0       22 2023-11-29 02:31:54.653857 asyncmy-0.2.9/asyncmy/version.py
+-rw-r--r--   0        0        0      400 2023-11-29 02:31:54.653857 asyncmy-0.2.9/build.py
+-rw-r--r--   0        0        0     1282 2023-11-29 02:31:54.653857 asyncmy-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     5882 1970-01-01 00:00:00.000000 asyncmy-0.2.9/setup.py
+-rw-r--r--   0        0        0     5925 1970-01-01 00:00:00.000000 asyncmy-0.2.9/PKG-INFO
```

### Comparing `asyncmy-0.2.8rc2/CHANGELOG.md` & `asyncmy-0.2.9/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 # ChangeLog
 
 ## 0.2
 
-## 0.2.8
+### 0.2.9
+
+- Added support for SSL context creation via `ssl` parameter using a dictionary containing `mysql_ssl_set` parameters. (#64)
+- Fix bug with fallback encoder in the `escape_item()` function. (#65)
+
+### 0.2.8
 
 - Fix sudden loss of float precision. (#56)
 - Fix pool `echo` parameter not apply to create connection. (#62)
+- Fix replication reconnect.
 
 ### 0.2.7
 
 - Fix `No module named 'asyncmy.connection'`.
 
 ### 0.2.6
```

### Comparing `asyncmy-0.2.8rc2/LICENSE` & `asyncmy-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.8rc2/README.md` & `asyncmy-0.2.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 Now you can uninstall previously installed tools.
 
 ## Usage
 
 ### Use `connect`
 
-`asyncmy` provides a way to connect to MySQL database with simple factory function `asyncmy.connnect()`. Use this
+`asyncmy` provides a way to connect to MySQL database with simple factory function `asyncmy.connect()`. Use this
 function if you want just one connection to the database, consider connection pool for multiple connections.
 
 ```py
 from asyncmy import connect
 from asyncmy.cursors import DictCursor
 import asyncio
```

### Comparing `asyncmy-0.2.8rc2/asyncmy/auth.py` & `asyncmy-0.2.9/asyncmy/auth.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.8rc2/asyncmy/charset.pyx` & `asyncmy-0.2.9/asyncmy/charset.pyx`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.8rc2/asyncmy/connection.pyx` & `asyncmy-0.2.9/asyncmy/connection.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         Whether or not to default to unicode strings.
         This option defaults to true.
     :param client_flag: Custom flags to send to MySQL. Find potential values in constants.
     :param cursor_cls: Custom cursor class to use.
     :param init_command: Initial SQL statement to run when connection is established.
     :param connect_timeout: The timeout for connecting to the database in seconds.
         (default: 10, min: 1, max: 31536000)
-    :param ssl: Optional SSL Context to force SSL
+    :param ssl: Optional dict of arguments similar to mysql_ssl_set()'s parameters or SSL Context to force SSL
     :param read_default_group: Group to read from in the configuration file.
     :param autocommit: Autocommit mode. None means use server default. (default: False)
     :param local_infile: Boolean to enable the use of LOAD DATA LOCAL  (default: False)
     :param max_allowed_packet: Max size of packet sent to server in bytes. (default: 16MB)
         Only used to limit size of "LOAD LOCAL INFILE" data packet smaller than default (16KB).
     :param auth_plugin_map: A dict of plugin names to a class that processes that plugin.
         The class will take the Connection object as the argument to the constructor.
@@ -148,18 +148,18 @@
     """
 
     def __init__(
             self,
             *,
             user=None,  # The first four arguments is based on DB-API 2.0 recommendation.
             password="",
-            host='localhost',
+            host=None,
             database=None,
             unix_socket=None,
-            port=3306,
+            port=0,
             charset="",
             sql_mode=None,
             read_default_file=None,
             conv=None,
             use_unicode=True,
             client_flag=0,
             cursor_cls=Cursor,
@@ -213,22 +213,33 @@
             user = _config("user", user)
             password = _config("password", password)
             host = _config("host", host)
             database = _config("database", database)
             unix_socket = _config("socket", unix_socket)
             port = int(_config("port", port))
             charset = _config("default-character-set", charset)
-        self._echo = echo
-        self._last_usage = self._loop.time()
-        self._ssl_context = ssl
+            if not ssl:
+                ssl = {}
+            if isinstance(ssl, dict):
+                for key in ["ca", "capath", "cert", "key", "cipher"]:
+                    value = _config("ssl-" + key, ssl.get(key))
+                    if value:
+                        ssl[key] = value
+        self._ssl_context = None
         if ssl:
+            if not SSL_ENABLED:
+                raise NotImplementedError("SSL module not found")
             client_flag |= SSL
+            self._ssl_context = self._create_ssl_ctx(ssl)
+
+        self._echo = echo
+        self._last_usage = self._loop.time()
 
-        self._host = host
-        self._port = port
+        self._host = host or "localhost"
+        self._port = port or 3306
         if type(self._port) is not int:
             raise ValueError("port should be of type int")
         self._user = user or DEFAULT_USER
         self._password = password or b""
         if isinstance(self._password, str):
             self._password = self._password.encode("latin1")
         self._db = database
@@ -282,14 +293,47 @@
         if program_name:
             self._connect_attrs["program_name"] = program_name
 
         self._connected = False
         self._reader: Optional[StreamReader] = None
         self._writer: Optional[StreamWriter] = None
 
+    def _create_ssl_ctx(self, sslp):
+        if isinstance(sslp, ssl.SSLContext):
+            return sslp
+        ca = sslp.get("ca")
+        capath = sslp.get("capath")
+        hasnoca = ca is None and capath is None
+        ctx = ssl.create_default_context(cafile=ca, capath=capath)
+        ctx.check_hostname = not hasnoca and sslp.get("check_hostname", True)
+        verify_mode_value = sslp.get("verify_mode")
+        if verify_mode_value is None:
+            ctx.verify_mode = ssl.CERT_NONE if hasnoca else ssl.CERT_REQUIRED
+        elif isinstance(verify_mode_value, bool):
+            ctx.verify_mode = ssl.CERT_REQUIRED if verify_mode_value else ssl.CERT_NONE
+        else:
+            if isinstance(verify_mode_value, str):
+                verify_mode_value = verify_mode_value.lower()
+            if verify_mode_value in ("none", "0", "false", "no"):
+                ctx.verify_mode = ssl.CERT_NONE
+            elif verify_mode_value == "optional":
+                ctx.verify_mode = ssl.CERT_OPTIONAL
+            elif verify_mode_value in ("required", "1", "true", "yes"):
+                ctx.verify_mode = ssl.CERT_REQUIRED
+            else:
+                ctx.verify_mode = ssl.CERT_NONE if hasnoca else ssl.CERT_REQUIRED
+        if "cert" in sslp:
+            ctx.load_cert_chain(sslp["cert"], keyfile=sslp.get("key"))
+        if "cipher" in sslp:
+            ctx.set_ciphers(sslp["cipher"])
+        ctx.options |= ssl.OP_NO_SSLv2
+        ctx.options |= ssl.OP_NO_SSLv3
+        return ctx
+
+
     def close(self):
         """Close socket connection"""
         if self._writer:
             self._writer.transport.close()
         self._writer = None
         self._reader = None
 
@@ -1229,18 +1273,18 @@
         finally:
             # send the empty packet to signify we are done sending data
             await conn.write_packet(b"")
 
 
 def connect(user=None,
             password="",
-            host='localhost',
+            host=None,
             database=None,
             unix_socket=None,
-            port=3306,
+            port=0,
             charset="",
             sql_mode=None,
             read_default_file=None,
             conv=None,
             use_unicode=True,
             client_flag=0,
             cursor_cls=Cursor,
```

### Comparing `asyncmy-0.2.8rc2/asyncmy/constants/CLIENT.py` & `asyncmy-0.2.9/asyncmy/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.8rc2/asyncmy/constants/COMMAND.py` & `asyncmy-0.2.9/asyncmy/constants/COMMAND.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.8rc2/asyncmy/constants/CR.py` & `asyncmy-0.2.9/asyncmy/constants/CR.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.8rc2/asyncmy/constants/ER.py` & `asyncmy-0.2.9/asyncmy/constants/ER.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.8rc2/asyncmy/contexts.py` & `asyncmy-0.2.9/asyncmy/contexts.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.8rc2/asyncmy/converters.pyx` & `asyncmy-0.2.9/asyncmy/converters.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -76,16 +76,16 @@
 
 cpdef str escape_bytes_prefixed(bytes value, mapping: dict = None):
     return "_binary'%s'" % value.decode(b"ascii", "surrogateescape").translate(_escape_table)
 
 cpdef str escape_bytes(bytes value, mapping: dict = None):
     return "'%s'" % value.decode(b"ascii", "surrogateescape").translate(_escape_table)
 
-cpdef str escape_str(str value, mapping: dict = None):
-    return "'%s'" % escape_string(value, mapping)
+cpdef str escape_str(value, mapping: dict = None):
+    return "'%s'" % escape_string(str(value), mapping)
 
 cpdef str escape_None(value, mapping: dict = None):
     return "NULL"
 
 cpdef str escape_timedelta(obj: datetime.timedelta, mapping: dict = None):
     seconds = int(obj.seconds) % 60
     minutes = int(obj.seconds // 60) % 60
```

### Comparing `asyncmy-0.2.8rc2/asyncmy/cursors.pyx` & `asyncmy-0.2.9/asyncmy/cursors.pyx`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.8rc2/asyncmy/errors.pyx` & `asyncmy-0.2.9/asyncmy/errors.pyx`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.8rc2/asyncmy/pool.pyx` & `asyncmy-0.2.9/asyncmy/pool.pyx`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.8rc2/asyncmy/protocol.pyx` & `asyncmy-0.2.9/asyncmy/protocol.pyx`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.8rc2/asyncmy/replication/binlogstream.py` & `asyncmy-0.2.9/asyncmy/replication/binlogstream.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import struct
 from typing import Any, Dict, List, Optional, Set, Type, Union
 
 from asyncmy import Connection
 from asyncmy.constants.COMMAND import COM_BINLOG_DUMP, COM_BINLOG_DUMP_GTID, COM_REGISTER_SLAVE
 from asyncmy.cursors import DictCursor
+from asyncmy.errors import OperationalError
 from asyncmy.replication.constants import (
     BINLOG_DUMP_NON_BLOCK,
     BINLOG_THROUGH_GTID,
     MAX_HEARTBEAT,
     ROTATE_EVENT,
     TABLE_MAP_EVENT,
 )
-from asyncmy.replication.errors import BinLogNotEnabledError, StreamClosedError
+from asyncmy.replication.errors import BinLogNotEnabledError
 from asyncmy.replication.events import (
     BeginLoadQueryEvent,
     BinLogEvent,
     ExecuteLoadQueryEvent,
     FormatDescriptionEvent,
     GtidEvent,
     HeartbeatLogEvent,
@@ -89,14 +90,16 @@
             + struct.pack("<H", self._port)
             + struct.pack("<l", 0)
             + struct.pack("<l", master_id)
         )
 
 
 class BinLogStream:
+    MYSQL_EXPECTED_ERROR_CODES = [2013, 2006]
+
     def __init__(
         self,
         connection: Connection,
         ctl_connection: Connection,
         server_id: int,
         slave_uuid: Optional[str] = None,
         slave_heartbeat: Optional[int] = None,
@@ -271,19 +274,26 @@
         if self._connected:
             await self._connection.ensure_closed()
             self._connected = False
 
     async def _read(self):
         if not self._connected:
             await self._connect()
+        try:
+            pkt = await self._connection.read_packet()
+        except OperationalError as e:
+            code, _ = e.args
+            if code in self.MYSQL_EXPECTED_ERROR_CODES:
+                await self.close()
+                return
+            raise e
 
-        pkt = await self._connection.read_packet()
         if pkt.is_eof_packet():
             await self.close()
-            raise StreamClosedError("BinLogStream is closed")
+            return
 
         if not pkt.is_ok_packet():
             return
 
         binlog_event = BinLogPacket(
             pkt,
             self._table_map,
@@ -354,15 +364,12 @@
 
     def __aiter__(self):
         return self
 
     async def __anext__(self):
         if not self._connected:
             await self._connect()
-        try:
+        ret = await self._read()
+        while ret is None:
             ret = await self._read()
-            while ret is None:
-                ret = await self._read()
-                continue
-            return ret
-        except StreamClosedError:
-            raise StopAsyncIteration
+            continue
+        return ret
```

### Comparing `asyncmy-0.2.8rc2/asyncmy/replication/bitmap.py` & `asyncmy-0.2.9/asyncmy/replication/bitmap.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.8rc2/asyncmy/replication/column.py` & `asyncmy-0.2.9/asyncmy/replication/column.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.8rc2/asyncmy/replication/constants.py` & `asyncmy-0.2.9/asyncmy/replication/constants.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.8rc2/asyncmy/replication/events.py` & `asyncmy-0.2.9/asyncmy/replication/events.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.8rc2/asyncmy/replication/gtid.py` & `asyncmy-0.2.9/asyncmy/replication/gtid.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.8rc2/asyncmy/replication/packets.py` & `asyncmy-0.2.9/asyncmy/replication/packets.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.8rc2/asyncmy/replication/row_events.py` & `asyncmy-0.2.9/asyncmy/replication/row_events.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.8rc2/asyncmy/replication/table.py` & `asyncmy-0.2.9/asyncmy/replication/table.py`

 * *Files identical despite different names*

### Comparing `asyncmy-0.2.8rc2/pyproject.toml` & `asyncmy-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,20 @@
 license = "Apache-2.0"
 name = "asyncmy"
 packages = [
     { include = "asyncmy" },
 ]
 readme = "README.md"
 repository = "https://github.com/long2ice/asyncmy.git"
-version = "0.2.8-rc2"
+version = "0.2.9"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 [tool.poetry.group.dev.dependencies]
-bandit = "*"
 black = "*"
 cython = "*"
 flake8 = "*"
 isort = "*"
 mypy = "*"
 rich = "*"
 ruff = "*"
```

### Comparing `asyncmy-0.2.8rc2/setup.py` & `asyncmy-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['asyncmy', 'asyncmy.constants', 'asyncmy.replication']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'asyncmy',
-    'version': '0.2.8rc2',
+    'version': '0.2.9',
     'description': 'A fast asyncio MySQL driver',
-    'long_description': '# asyncmy - A fast asyncio MySQL/MariaDB driver\n\n[![image](https://img.shields.io/pypi/v/asyncmy.svg?style=flat)](https://pypi.python.org/pypi/asyncmy)\n[![image](https://img.shields.io/github/license/long2ice/asyncmy)](https://github.com/long2ice/asyncmy)\n[![pypi](https://github.com/long2ice/asyncmy/actions/workflows/pypi.yml/badge.svg)](https://github.com/long2ice/asyncmy/actions/workflows/pypi.yml)\n[![ci](https://github.com/long2ice/asyncmy/actions/workflows/ci.yml/badge.svg)](https://github.com/long2ice/asyncmy/actions/workflows/ci.yml)\n\n## Introduction\n\n`asyncmy` is a fast asyncio MySQL/MariaDB driver, which reuse most of [pymysql](https://github.com/PyMySQL/PyMySQL)\nand [aiomysql](https://github.com/aio-libs/aiomysql) but rewrite core protocol with [cython](https://cython.org/) to\nspeedup.\n\n## Features\n\n- API compatible with [aiomysql](https://github.com/aio-libs/aiomysql).\n- Faster by [cython](https://cython.org/).\n- MySQL replication protocol support with `asyncio`.\n- Tested both MySQL and MariaDB in [CI](https://github.com/long2ice/asyncmy/blob/dev/.github/workflows/ci.yml).\n\n## Benchmark\n\nThe result comes from [benchmark](./benchmark).\n\n> The device is iMac Pro(2017) i9 3.6GHz 48G and MySQL version is 8.0.26.\n\n![benchmark](./images/benchmark.png)\n\n### Conclusion\n\n- There is no doubt that `mysqlclient` is the fastest MySQL driver.\n- All kinds of drivers have a small gap except `select`.\n- `asyncio` could enhance `insert`.\n- `asyncmy` performs remarkable when compared to other drivers.\n\n## Install\n\n```shell\npip install asyncmy\n```\n\n### Installing on Windows\n\nTo install asyncmy on Windows, you need to install the tools needed to build it.\n\n1. Download *Microsoft C++ Build Tools* from https://visualstudio.microsoft.com/visual-cpp-build-tools/\n2. Run CMD as Admin (not required but recommended) and navigate to the folder when your installer is downloaded\n3. Installer executable should look like this `vs_buildtools__XXXXXXXXX.XXXXXXXXXX.exe`, it will be easier if you rename\n   it to just `vs_buildtools.exe`\n4. Run this command (Make sure you have about 5-6GB of free storage)\n\n```shell\nvs_buildtools.exe --norestart --passive --downloadThenInstall --includeRecommended --add Microsoft.VisualStudio.Workload.NativeDesktop --add Microsoft.VisualStudio.Workload.VCTools --add Microsoft.VisualStudio.Workload.MSBuildTools\n```\n\n5. Wait until the installation is finished\n6. After installation will finish, restart your computer\n7. Install asyncmy via PIP\n\n```shell\npip install asyncmy\n```\n\nNow you can uninstall previously installed tools.\n\n## Usage\n\n### Use `connect`\n\n`asyncmy` provides a way to connect to MySQL database with simple factory function `asyncmy.connnect()`. Use this\nfunction if you want just one connection to the database, consider connection pool for multiple connections.\n\n```py\nfrom asyncmy import connect\nfrom asyncmy.cursors import DictCursor\nimport asyncio\n\n\nasync def run():\n    conn = await connect()\n    async with conn.cursor(cursor=DictCursor) as cursor:\n        await cursor.execute("create database if not exists test")\n        await cursor.execute(\n            """CREATE TABLE if not exists test.asyncmy\n    (\n        `id`       int primary key auto_increment,\n        `decimal`  decimal(10, 2),\n        `date`     date,\n        `datetime` datetime,\n        `float`    float,\n        `string`   varchar(200),\n        `tinyint`  tinyint\n    )"""\n        )\n\n\nif __name__ == \'__main__\':\n    asyncio.run(run())\n```\n\n### Use `pool`\n\n`asyncmy` provides connection pool as well as plain Connection objects.\n\n```py\nimport asyncmy\nimport asyncio\n\n\nasync def run():\n    pool = await asyncmy.create_pool()\n    async with pool.acquire() as conn:\n        async with conn.cursor() as cursor:\n            await cursor.execute("SELECT 1")\n            ret = await cursor.fetchone()\n            assert ret == (1,)\n\n\nif __name__ == \'__main__\':\n    asyncio.run(run())\n```\n\n## Replication\n\n`asyncmy` supports MySQL replication protocol\nlike [python-mysql-replication](https://github.com/noplay/python-mysql-replication), but powered by `asyncio`.\n\n```py\nfrom asyncmy import connect\nfrom asyncmy.replication import BinLogStream\nimport asyncio\n\n\nasync def run():\n    conn = await connect()\n    ctl_conn = await connect()\n\n    stream = BinLogStream(\n        conn,\n        ctl_conn,\n        1,\n        master_log_file="binlog.000172",\n        master_log_position=2235312,\n        resume_stream=True,\n        blocking=True,\n    )\n    async for event in stream:\n        print(event)\n\n\nif __name__ == \'__main__\':\n    asyncio.run(run())\n```\n\n## ThanksTo\n\n> asyncmy is build on top of these awesome projects.\n\n- [pymysql](https://github/pymysql/PyMySQL), a pure python MySQL client.\n- [aiomysql](https://github.com/aio-libs/aiomysql), a library for accessing a MySQL database from the asyncio.\n- [python-mysql-replication](https://github.com/noplay/python-mysql-replication), pure Python Implementation of MySQL\n  replication protocol build on top of PyMYSQL.\n\n## License\n\nThis project is licensed under the [Apache-2.0](./LICENSE) License.\n',
+    'long_description': '# asyncmy - A fast asyncio MySQL/MariaDB driver\n\n[![image](https://img.shields.io/pypi/v/asyncmy.svg?style=flat)](https://pypi.python.org/pypi/asyncmy)\n[![image](https://img.shields.io/github/license/long2ice/asyncmy)](https://github.com/long2ice/asyncmy)\n[![pypi](https://github.com/long2ice/asyncmy/actions/workflows/pypi.yml/badge.svg)](https://github.com/long2ice/asyncmy/actions/workflows/pypi.yml)\n[![ci](https://github.com/long2ice/asyncmy/actions/workflows/ci.yml/badge.svg)](https://github.com/long2ice/asyncmy/actions/workflows/ci.yml)\n\n## Introduction\n\n`asyncmy` is a fast asyncio MySQL/MariaDB driver, which reuse most of [pymysql](https://github.com/PyMySQL/PyMySQL)\nand [aiomysql](https://github.com/aio-libs/aiomysql) but rewrite core protocol with [cython](https://cython.org/) to\nspeedup.\n\n## Features\n\n- API compatible with [aiomysql](https://github.com/aio-libs/aiomysql).\n- Faster by [cython](https://cython.org/).\n- MySQL replication protocol support with `asyncio`.\n- Tested both MySQL and MariaDB in [CI](https://github.com/long2ice/asyncmy/blob/dev/.github/workflows/ci.yml).\n\n## Benchmark\n\nThe result comes from [benchmark](./benchmark).\n\n> The device is iMac Pro(2017) i9 3.6GHz 48G and MySQL version is 8.0.26.\n\n![benchmark](./images/benchmark.png)\n\n### Conclusion\n\n- There is no doubt that `mysqlclient` is the fastest MySQL driver.\n- All kinds of drivers have a small gap except `select`.\n- `asyncio` could enhance `insert`.\n- `asyncmy` performs remarkable when compared to other drivers.\n\n## Install\n\n```shell\npip install asyncmy\n```\n\n### Installing on Windows\n\nTo install asyncmy on Windows, you need to install the tools needed to build it.\n\n1. Download *Microsoft C++ Build Tools* from https://visualstudio.microsoft.com/visual-cpp-build-tools/\n2. Run CMD as Admin (not required but recommended) and navigate to the folder when your installer is downloaded\n3. Installer executable should look like this `vs_buildtools__XXXXXXXXX.XXXXXXXXXX.exe`, it will be easier if you rename\n   it to just `vs_buildtools.exe`\n4. Run this command (Make sure you have about 5-6GB of free storage)\n\n```shell\nvs_buildtools.exe --norestart --passive --downloadThenInstall --includeRecommended --add Microsoft.VisualStudio.Workload.NativeDesktop --add Microsoft.VisualStudio.Workload.VCTools --add Microsoft.VisualStudio.Workload.MSBuildTools\n```\n\n5. Wait until the installation is finished\n6. After installation will finish, restart your computer\n7. Install asyncmy via PIP\n\n```shell\npip install asyncmy\n```\n\nNow you can uninstall previously installed tools.\n\n## Usage\n\n### Use `connect`\n\n`asyncmy` provides a way to connect to MySQL database with simple factory function `asyncmy.connect()`. Use this\nfunction if you want just one connection to the database, consider connection pool for multiple connections.\n\n```py\nfrom asyncmy import connect\nfrom asyncmy.cursors import DictCursor\nimport asyncio\n\n\nasync def run():\n    conn = await connect()\n    async with conn.cursor(cursor=DictCursor) as cursor:\n        await cursor.execute("create database if not exists test")\n        await cursor.execute(\n            """CREATE TABLE if not exists test.asyncmy\n    (\n        `id`       int primary key auto_increment,\n        `decimal`  decimal(10, 2),\n        `date`     date,\n        `datetime` datetime,\n        `float`    float,\n        `string`   varchar(200),\n        `tinyint`  tinyint\n    )"""\n        )\n\n\nif __name__ == \'__main__\':\n    asyncio.run(run())\n```\n\n### Use `pool`\n\n`asyncmy` provides connection pool as well as plain Connection objects.\n\n```py\nimport asyncmy\nimport asyncio\n\n\nasync def run():\n    pool = await asyncmy.create_pool()\n    async with pool.acquire() as conn:\n        async with conn.cursor() as cursor:\n            await cursor.execute("SELECT 1")\n            ret = await cursor.fetchone()\n            assert ret == (1,)\n\n\nif __name__ == \'__main__\':\n    asyncio.run(run())\n```\n\n## Replication\n\n`asyncmy` supports MySQL replication protocol\nlike [python-mysql-replication](https://github.com/noplay/python-mysql-replication), but powered by `asyncio`.\n\n```py\nfrom asyncmy import connect\nfrom asyncmy.replication import BinLogStream\nimport asyncio\n\n\nasync def run():\n    conn = await connect()\n    ctl_conn = await connect()\n\n    stream = BinLogStream(\n        conn,\n        ctl_conn,\n        1,\n        master_log_file="binlog.000172",\n        master_log_position=2235312,\n        resume_stream=True,\n        blocking=True,\n    )\n    async for event in stream:\n        print(event)\n\n\nif __name__ == \'__main__\':\n    asyncio.run(run())\n```\n\n## ThanksTo\n\n> asyncmy is build on top of these awesome projects.\n\n- [pymysql](https://github/pymysql/PyMySQL), a pure python MySQL client.\n- [aiomysql](https://github.com/aio-libs/aiomysql), a library for accessing a MySQL database from the asyncio.\n- [python-mysql-replication](https://github.com/noplay/python-mysql-replication), pure Python Implementation of MySQL\n  replication protocol build on top of PyMYSQL.\n\n## License\n\nThis project is licensed under the [Apache-2.0](./LICENSE) License.\n',
     'author': 'long2ice',
     'author_email': 'long2ice@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/long2ice/asyncmy',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `asyncmy-0.2.8rc2/PKG-INFO` & `asyncmy-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: asyncmy
-Version: 0.2.8rc2
+Version: 0.2.9
 Summary: A fast asyncio MySQL driver
 Home-page: https://github.com/long2ice/asyncmy
 License: Apache-2.0
 Keywords: driver,asyncio,mysql
 Author: long2ice
 Author-email: long2ice@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Project-URL: Documentation, https://github.com/long2ice/asyncmy
 Project-URL: Repository, https://github.com/long2ice/asyncmy.git
 Description-Content-Type: text/markdown
 
 # asyncmy - A fast asyncio MySQL/MariaDB driver
 
 [![image](https://img.shields.io/pypi/v/asyncmy.svg?style=flat)](https://pypi.python.org/pypi/asyncmy)
@@ -84,15 +85,15 @@
 
 Now you can uninstall previously installed tools.
 
 ## Usage
 
 ### Use `connect`
 
-`asyncmy` provides a way to connect to MySQL database with simple factory function `asyncmy.connnect()`. Use this
+`asyncmy` provides a way to connect to MySQL database with simple factory function `asyncmy.connect()`. Use this
 function if you want just one connection to the database, consider connection pool for multiple connections.
 
 ```py
 from asyncmy import connect
 from asyncmy.cursors import DictCursor
 import asyncio
```

