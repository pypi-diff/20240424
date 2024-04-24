# Comparing `tmp/message-db-py-0.1.2.tar.gz` & `tmp/message_db_py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "message-db-py-0.1.2.tar", max compression
+gzip compressed data, was "message_db_py-0.1.3.tar", max compression
```

## Comparing `message-db-py-0.1.2.tar` & `message_db_py-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0       22 2022-01-27 19:45:47.313148 message-db-py-0.1.2/message_db/__init__.py
--rw-r--r--   0        0        0     7357 2022-01-27 19:43:59.980216 message-db-py-0.1.2/message_db/client.py
--rw-r--r--   0        0        0     1880 2022-01-20 19:19:52.169102 message-db-py-0.1.2/message_db/connection.py
--rw-r--r--   0        0        0      685 2022-01-27 19:45:42.189225 message-db-py-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      670 2022-01-27 19:46:45.258778 message-db-py-0.1.2/setup.py
--rw-r--r--   0        0        0      516 2022-01-27 19:46:45.259325 message-db-py-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-23 22:49:09.333522 message_db_py-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1269 2024-04-23 23:03:47.862606 message_db_py-0.1.3/README.md
+-rw-r--r--   0        0        0      963 2024-04-23 23:52:46.715013 message_db_py-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-23 23:52:46.715427 message_db_py-0.1.3/src/message_db/__init__.py
+-rw-r--r--   0        0        0     7765 2024-04-23 21:56:55.046160 message_db_py-0.1.3/src/message_db/client.py
+-rw-r--r--   0        0        0     1880 2022-01-20 19:19:52.169102 message_db_py-0.1.3/src/message_db/connection.py
+-rw-r--r--   0        0        0     1866 1970-01-01 00:00:00.000000 message_db_py-0.1.3/PKG-INFO
```

### Comparing `message-db-py-0.1.2/message_db/client.py` & `message_db_py-0.1.3/src/message_db/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,33 +32,33 @@
         connection_pool = ConnectionPool.from_url(url, **kwargs)
         return cls(connection_pool=connection_pool)
 
     def __init__(
         self,
         dbname: str = "message_store",
         user: str = "message_store",
-        password: str = None,
+        password: str = "",
         host: str = "localhost",
         port: int = 5432,
-        connection_pool: ConnectionPool = None,
+        connection_pool: ConnectionPool | None = None,
     ) -> None:
         if not connection_pool:
             connection_pool = ConnectionPool(
                 dbname=dbname, user=user, password=password, host=host, port=port
             )
         self.connection_pool = connection_pool
 
     def _write(
         self,
         connection: connection,
         stream_name: str,
         message_type: str,
         data: Dict[str, Any],
-        metadata: Dict[str, Any] = None,
-        expected_version: int = None,
+        metadata: Dict[str, Any] | None = None,
+        expected_version: int | None = None,
     ) -> int:
         try:
             with connection.cursor(cursor_factory=RealDictCursor) as cursor:
                 cursor.execute(
                     (
                         "SELECT message_store.write_message(%(identifier)s, %(stream_name)s, %(type)s, "
                         "%(data)s, %(metadata)s, %(expected_version)s);"
@@ -70,42 +70,46 @@
                         "data": Json(data),
                         "metadata": Json(metadata) if metadata else None,
                         "expected_version": expected_version,
                     },
                 )
 
                 result = cursor.fetchone()
+                if result is None:
+                    raise ValueError("No result returned from the database operation.")
         except Exception as exc:
             raise ValueError(
                 f"{getattr(exc, 'pgcode')}-{getattr(exc, 'pgerror').splitlines()[0]}"
             ) from exc
 
         return result["write_message"]
 
     def write(
         self,
         stream_name: str,
         message_type: str,
         data: Dict,
-        metadata: Dict = None,
-        expected_version: int = None,
+        metadata: Dict | None = None,
+        expected_version: int | None = None,
     ) -> int:
         conn = self.connection_pool.get_connection()
 
         try:
             with conn:
                 position = self._write(
                     conn, stream_name, message_type, data, metadata, expected_version
                 )
         finally:
             self.connection_pool.release(conn)
 
         return position
 
-    def write_batch(self, stream_name, data, expected_version: int = None) -> int:
+    def write_batch(
+        self, stream_name, data, expected_version: int | None = None
+    ) -> int:
         conn = self.connection_pool.get_connection()
 
         try:
             with conn:
                 for record in data:
                     position = self._write(
                         conn,
@@ -121,15 +125,15 @@
             self.connection_pool.release(conn)
 
         return position
 
     def read(
         self,
         stream_name: str,
-        sql: str = None,
+        sql: str | None = None,
         position: int = 0,
         no_of_messages: int = 1000,
     ) -> List[Dict[str, Any]]:
         conn = self.connection_pool.get_connection()
         cursor = conn.cursor(cursor_factory=RealDictCursor)
 
         if not sql:
@@ -167,19 +171,24 @@
 
         conn.commit()
         cursor.close()
         self.connection_pool.release(conn)
 
         messages = []
         for message in raw_messages:
-            message["data"] = json.loads(message["data"])
-            message["metadata"] = (
-                json.loads(message["metadata"]) if message["metadata"] else None
+            processed_message = dict(
+                message
+            )  # Convert each RealDictRow to a dictionary
+            processed_message["data"] = json.loads(processed_message["data"])
+            processed_message["metadata"] = (
+                json.loads(processed_message["metadata"])
+                if processed_message["metadata"]
+                else None
             )
-            messages.append(message)
+            messages.append(processed_message)
 
         return messages
 
     def read_stream(
         self, stream_name: str, position: int = 0, no_of_messages: int = 1000
     ) -> List[Dict[str, Any]]:
         if "-" not in stream_name:
@@ -199,15 +208,15 @@
 
         sql = "SELECT * FROM get_category_messages(%(stream_name)s, %(position)s, %(batch_size)s);"
 
         return self.read(
             category_name, sql=sql, position=position, no_of_messages=no_of_messages
         )
 
-    def read_last_message(self, stream_name) -> Dict[str, Any]:
+    def read_last_message(self, stream_name: str) -> Dict[str, Any] | None:
         conn = self.connection_pool.get_connection()
         cursor = conn.cursor(cursor_factory=RealDictCursor)
 
         cursor.execute(
             "SELECT * from get_last_stream_message(%(stream_name)s);",
             {"stream_name": stream_name},
         )
```

### Comparing `message-db-py-0.1.2/message_db/connection.py` & `message_db_py-0.1.3/src/message_db/connection.py`

 * *Files identical despite different names*

