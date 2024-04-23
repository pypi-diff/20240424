# Comparing `tmp/zcached.py-1.1.1.tar.gz` & `tmp/zcached.py-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zcached.py-1.1.1.tar", last modified: Mon Apr 15 22:47:28 2024, max compression
+gzip compressed data, was "zcached.py-1.2.1.tar", last modified: Tue Apr 23 23:12:21 2024, max compression
```

## Comparing `zcached.py-1.1.1.tar` & `zcached.py-1.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:28.131732 zcached.py-1.1.1/
--rw-rw-rw-   0        0        0     1084 2024-04-08 18:44:53.000000 zcached.py-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     3702 2024-04-15 22:47:28.130226 zcached.py-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      126 2024-04-08 18:44:53.000000 zcached.py-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 22:47:28.131732 zcached.py-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1385 2024-04-15 22:47:05.000000 zcached.py-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:28.110210 zcached.py-1.1.1/tests/
--rw-rw-rw-   0        0        0      589 2024-04-08 18:44:53.000000 zcached.py-1.1.1/tests/test_backoff.py
--rw-rw-rw-   0        0        0     1742 2024-04-15 22:08:29.000000 zcached.py-1.1.1/tests/test_connection.py
--rw-rw-rw-   0        0        0     1338 2024-04-08 18:44:53.000000 zcached.py-1.1.1/tests/test_deserializer.py
--rw-rw-rw-   0        0        0      587 2024-04-08 18:44:53.000000 zcached.py-1.1.1/tests/test_reader.py
--rw-rw-rw-   0        0        0      820 2024-04-15 22:09:01.000000 zcached.py-1.1.1/tests/test_result.py
--rw-rw-rw-   0        0        0     2271 2024-04-08 18:44:53.000000 zcached.py-1.1.1/tests/test_serializer.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:28.120711 zcached.py-1.1.1/zcached/
--rw-rw-rw-   0        0        0      584 2024-04-15 22:37:38.000000 zcached.py-1.1.1/zcached/__init__.py
--rw-rw-rw-   0        0        0     1757 2024-04-08 18:44:53.000000 zcached.py-1.1.1/zcached/backoff.py
--rw-rw-rw-   0        0        0     6175 2024-04-15 22:22:20.000000 zcached.py-1.1.1/zcached/client.py
--rw-rw-rw-   0        0        0     7530 2024-04-15 22:09:11.000000 zcached.py-1.1.1/zcached/connection.py
--rw-rw-rw-   0        0        0     2739 2024-04-15 22:09:01.000000 zcached.py-1.1.1/zcached/deserializer.py
--rw-rw-rw-   0        0        0     1058 2024-04-15 22:09:11.000000 zcached.py-1.1.1/zcached/enums.py
--rw-rw-rw-   0        0        0     2073 2024-04-08 21:02:12.000000 zcached.py-1.1.1/zcached/reader.py
--rw-rw-rw-   0        0        0     2274 2024-04-15 22:09:01.000000 zcached.py-1.1.1/zcached/result.py
--rw-rw-rw-   0        0        0     3324 2024-04-15 22:09:01.000000 zcached.py-1.1.1/zcached/serializer.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:47:28.129229 zcached.py-1.1.1/zcached.py.egg-info/
--rw-rw-rw-   0        0        0     3702 2024-04-15 22:47:27.000000 zcached.py-1.1.1/zcached.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      519 2024-04-15 22:47:27.000000 zcached.py-1.1.1/zcached.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 22:47:27.000000 zcached.py-1.1.1/zcached.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-15 22:47:27.000000 zcached.py-1.1.1/zcached.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-15 22:47:27.000000 zcached.py-1.1.1/zcached.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 23:12:21.700539 zcached.py-1.2.1/
+-rw-rw-rw-   0        0        0     1084 2024-04-08 18:44:53.000000 zcached.py-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     3727 2024-04-23 23:12:21.699145 zcached.py-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      126 2024-04-08 18:44:53.000000 zcached.py-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 23:12:21.701545 zcached.py-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1385 2024-04-23 23:12:10.000000 zcached.py-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 23:12:21.619523 zcached.py-1.2.1/tests/
+-rw-rw-rw-   0        0        0      589 2024-04-08 18:44:53.000000 zcached.py-1.2.1/tests/test_backoff.py
+-rw-rw-rw-   0        0        0     1851 2024-04-23 22:59:22.000000 zcached.py-1.2.1/tests/test_connection.py
+-rw-rw-rw-   0        0        0     1338 2024-04-08 18:44:53.000000 zcached.py-1.2.1/tests/test_deserializer.py
+-rw-rw-rw-   0        0        0      587 2024-04-08 18:44:53.000000 zcached.py-1.2.1/tests/test_reader.py
+-rw-rw-rw-   0        0        0      820 2024-04-15 22:09:01.000000 zcached.py-1.2.1/tests/test_result.py
+-rw-rw-rw-   0        0        0     2271 2024-04-08 18:44:53.000000 zcached.py-1.2.1/tests/test_serializer.py
+drwxrwxrwx   0        0        0        0 2024-04-23 23:12:21.677039 zcached.py-1.2.1/zcached/
+-rw-rw-rw-   0        0        0      585 2024-04-23 23:12:10.000000 zcached.py-1.2.1/zcached/__init__.py
+-rw-rw-rw-   0        0        0     1757 2024-04-23 22:46:05.000000 zcached.py-1.2.1/zcached/backoff.py
+-rw-rw-rw-   0        0        0     7333 2024-04-23 23:06:03.000000 zcached.py-1.2.1/zcached/client.py
+-rw-rw-rw-   0        0        0     8142 2024-04-23 22:59:22.000000 zcached.py-1.2.1/zcached/connection.py
+-rw-rw-rw-   0        0        0     2739 2024-04-15 22:09:01.000000 zcached.py-1.2.1/zcached/deserializer.py
+-rw-rw-rw-   0        0        0     1186 2024-04-23 22:59:22.000000 zcached.py-1.2.1/zcached/enums.py
+-rw-rw-rw-   0        0        0     2073 2024-04-08 21:02:12.000000 zcached.py-1.2.1/zcached/reader.py
+-rw-rw-rw-   0        0        0     2274 2024-04-15 22:09:01.000000 zcached.py-1.2.1/zcached/result.py
+-rw-rw-rw-   0        0        0     3324 2024-04-15 22:09:01.000000 zcached.py-1.2.1/zcached/serializer.py
+drwxrwxrwx   0        0        0        0 2024-04-23 23:12:21.694006 zcached.py-1.2.1/zcached.py.egg-info/
+-rw-rw-rw-   0        0        0     3727 2024-04-23 23:12:21.000000 zcached.py-1.2.1/zcached.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2024-04-23 23:12:21.000000 zcached.py-1.2.1/zcached.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 23:12:21.000000 zcached.py-1.2.1/zcached.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-23 23:12:21.000000 zcached.py-1.2.1/zcached.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-23 23:12:21.000000 zcached.py-1.2.1/zcached.py.egg-info/top_level.txt
```

### Comparing `zcached.py-1.1.1/LICENSE` & `zcached.py-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zcached.py-1.1.1/PKG-INFO` & `zcached.py-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcached.py
-Version: 1.1.1
+Version: 1.2.1
 Summary: A lightweight client-side library for zcached, written in Python.
 Home-page: https://github.com/xXenvy/zcached.py
 Author: xXenvy
 Project-URL: Bug Reports, https://github.com/xXenvy/zcached.py/issues
 Project-URL: Source, https://github.com/xXenvy/zcached.py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -26,31 +26,31 @@
 # Zcached.py - A client-side library for zcached.
 
 ![commits](https://img.shields.io/github/commit-activity/w/xXenvy/zcached.py?style=for-the-badge&color=%2315b328)
 ![license](https://img.shields.io/github/license/xXenvy/zcached.py?style=for-the-badge&color=%2315b328)
 ![release](https://img.shields.io/github/v/release/xXenvy/zcached.py?include_prereleases&style=for-the-badge&color=%2315b328)
 
 ## `📜` Introduction
-Zcached.py is a Python client-side library designed to interact with zcached, a high-performance caching system.
+Zcached.py is a Python client-side library designed to interact with zcached, a high-performance in-memory caching system.
 This library provides developers an easy-to-use interface for integrating zcached into their Python applications, enabling efficient data caching.
 
 For more information, please see [zcached repository](https://github.com/sectasy0/zcached).
 
 ## `🌟` Features
 - **Simplified Caching:** Zcached.py simplifies the process of caching data by providing intuitive functions for storing and retrieving values.
 - **Efficient Communication:** The library optimizes communication with the zcached server, ensuring minimal overhead and efficient data transfer.
 - **Properly Typehinted:** The codebase of zcached.py is properly typehinted, enhancing code readability.
 
 ## `🔧` Installation
 > [!IMPORTANT]  
 > **Library requires python version 3.8 or newer.** (Older also should work, but untested).
 
-Before installing zcached.py, ensure that you have the zcached server. Instructions for installing the server can be found [here](https://github.com/sectasy0/zcached).
+Before installing zcached.py, ensure that you have the zcached server. Instructions for installing and running the server can be found [here](https://github.com/sectasy0/zcached).
 
-Once the zcached server is installed, you can proceed to install zcached.py using pip:
+Once the zcached server is ready to use, you can proceed to install zcached.py using pip:
 ```shell
 pip install -U zcached.py
 ```
 
 ## `🖊️` Usage
 Here's a basic example demonstrating how to use zcached.py in your Python code:
 ```py
```

### Comparing `zcached.py-1.1.1/setup.py` & `zcached.py-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import pathlib
 
-version: str = "1.1.1"
+version: str = "1.2.1"
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="zcached.py",
     version=version,
     description="A lightweight client-side library for zcached, written in Python.",
```

### Comparing `zcached.py-1.1.1/tests/test_backoff.py` & `zcached.py-1.2.1/tests/test_backoff.py`

 * *Files identical despite different names*

### Comparing `zcached.py-1.1.1/tests/test_connection.py` & `zcached.py-1.2.1/tests/test_connection.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,20 +2,26 @@
 from zcached import Connection, Result, ZCached
 
 IS_SERVER_RUNNING = False
 
 
 def test_connection():
     connection = Connection(
-        host="localhost", port=5555, connection_attempts=2, buff_size=2, reconnect=False
+        host="localhost",
+        port=5555,
+        connection_attempts=2,
+        buff_size=512,
+        reconnect=False,
+        timeout_limit=5,
     )
 
     assert connection.host == "localhost"
+    assert connection.timeout_limit == 5
     assert connection.port == 5555
-    assert connection.buff_size == 2
+    assert connection.buff_size == 512
     assert connection.connection_attempts == 2
     assert connection.is_connected is False
     assert connection.socket.getblocking() is True
 
     if not IS_SERVER_RUNNING:
         connection.connect()
         assert not connection.is_connected
```

### Comparing `zcached.py-1.1.1/tests/test_deserializer.py` & `zcached.py-1.2.1/tests/test_deserializer.py`

 * *Files identical despite different names*

### Comparing `zcached.py-1.1.1/tests/test_reader.py` & `zcached.py-1.2.1/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `zcached.py-1.1.1/tests/test_result.py` & `zcached.py-1.2.1/tests/test_result.py`

 * *Files identical despite different names*

### Comparing `zcached.py-1.1.1/tests/test_serializer.py` & `zcached.py-1.2.1/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `zcached.py-1.1.1/zcached/__init__.py` & `zcached.py-1.2.1/zcached/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,11 +15,11 @@
     "ExponentialBackoff",
     "Result",
     "Serializer",
     "SupportedTypes",
     "Deserializer",
     "Reader",
     "Errors",
-    "__version__"
+    "__version__",
 )
 
-__version__: Final[str] = "1.1.1"
+__version__: Final[str] = "1.2.1"
```

### Comparing `zcached.py-1.1.1/zcached/backoff.py` & `zcached.py-1.2.1/zcached/backoff.py`

 * *Files identical despite different names*

### Comparing `zcached.py-1.1.1/zcached/client.py` & `zcached.py-1.2.1/zcached/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,17 +25,20 @@
         while smaller values can be more memory-efficient but slower.
     connection_attempts:
         The maximum number of attempts to establish a connection with the server.
         This value is also considered while reconnecting.
     reconnect:
         Flag indicating whether automatic reconnection attempt should be made
         in case of a broken connection.
+    timeout_limit:
+        The maximum time in seconds to wait for a response from the server.
 
-        .. note::
-            There is an option to do a reconnect manually, using the ``ZCached.connection.try_reconnect()`` method.
+    Notes
+    -----
+    There is a way to do a reconnect manually, using the ``ZCached.connection.try_reconnect()`` method.
 
     Attributes
     ----------
     connection:
         Connection object used by this class.
     """
 
@@ -45,17 +48,23 @@
     def __init__(
         self,
         host: str,
         port: int = 7556,
         buff_size: int = 1024,
         connection_attempts: int = 3,
         reconnect: bool = True,
+        timeout_limit: int = 10,
     ) -> None:
         self.connection: Connection = Connection(
-            host, port, connection_attempts, reconnect, buff_size
+            host=host,
+            port=port,
+            buff_size=buff_size,
+            connection_attempts=connection_attempts,
+            reconnect=reconnect,
+            timeout_limit=timeout_limit,
         )
 
     def __repr__(self) -> str:
         return f"ZCached(connection={self.connection})"
 
     def run(self) -> None:
         """Establishes a connection with the database server."""
@@ -77,14 +86,18 @@
         """Method to save all database records."""
         return self.connection.send(b"*1\r\n$4\r\nSAVE\r\n")
 
     def keys(self) -> Result[List[str]]:
         """Retrieve the keys of the database."""
         return self.connection.send(b"*1\r\n$4\r\nKEYS\r\n")
 
+    def lastsave(self) -> Result[int]:
+        """Method to retrieve the Unix timestamp of the last successful database save."""
+        return self.connection.send(b"*1\r\n$8\r\nLASTSAVE\r\n")
+
     def get(self, key: str) -> Result:
         """
         Method to send a get command to the database.
 
         Parameters
         ----------
         key:
@@ -156,14 +169,31 @@
         ----------
         key:
             Key of the record being deleted.
         """
         command: str = f"*2\r\n$6\r\nDELETE\r\n${len(key)}\r\n{key}\r\n"
         return self.connection.send(command.encode())
 
+    def exists(self, key: str) -> bool:
+        """
+        Checks if the specified key exists in the database.
+
+        Parameters
+        ----------
+        key:
+            The key to check for existence in the database.
+
+        Notes
+        -----
+        **Using this method directly may be unsafe as it does not verify the connection status.**
+        When the key exists in the database, but the connection is broken, the value False will be returned.
+        Because of this it's recommended to use this method only when the connection to the server is guaranteed.
+        """
+        return bool(self.get(key))
+
     def is_alive(self) -> bool:
         """
         Checks if the client is currently connected to the server.
 
         .. note::
             This method sends a ping command to the connected server.
         """
@@ -182,8 +212,9 @@
         """
         return cls(
             host=connection.host,
             port=connection.port,
             buff_size=connection.buff_size,
             connection_attempts=connection.connection_attempts,
             reconnect=connection.reconnect,
+            timeout_limit=connection.timeout_limit,
         )
```

### Comparing `zcached.py-1.1.1/zcached/connection.py` & `zcached.py-1.2.1/zcached/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,51 +26,58 @@
         while smaller values can be more memory-efficient but slower.
     connection_attempts:
         The maximum number of attempts to establish a connection with the server.
         If the maximum number of attempts is exceeded, an error will be raised.
     reconnect:
         Flag indicating whether automatic reconnection attempt should be made
         in case of a broken connection.
+    timeout_limit:
+        The maximum time in seconds to wait for a response from the server.
 
     Attributes
     ----------
     socket:
         The socket object for communicating with the server.
     buff_size:
         The size of the buffer for receiving data from the server.
     connection_attempts:
         The maximum number of attempts to establish a connection with the server.
     reconnect:
         Flag indicating whether automatic reconnection attempt should be made
         in case of a broken connection.
+    timeout_limit:
+        The maximum time in seconds to wait for a response from the server.
     """
 
     __slots__ = (
         "socket",
         "buff_size",
         "connection_attempts",
         "reconnect",
+        "timeout_limit",
         "_backoff",
         "_port",
         "_host",
         "_connected",
     )
 
     def __init__(
         self,
         host: str,
         port: int,
         connection_attempts: int,
         reconnect: bool,
-        buff_size: int = 1024,
+        timeout_limit: int,
+        buff_size: int,
     ):
         self.socket: socket = socket(AF_INET, SOCK_STREAM)
         self.buff_size: int = buff_size
         self.connection_attempts: int = connection_attempts
         self.reconnect: bool = reconnect
+        self.timeout_limit: int = timeout_limit
 
         self._host: str = host
         self._port: int = port
 
         self._connected: bool = False
         self._backoff = ExponentialBackoff(0.5, 2, 3)
 
@@ -124,15 +131,15 @@
         """
         Method to receive the response from the server.
         None if there is no data in the socket yet.
         """
         try:
             data: bytes = self.socket.recv(self.buff_size)
             logging.debug("Received a response -> %s", data)
-        except BlockingIOError:
+        except (BlockingIOError, ConnectionAbortedError):
             return None
 
         return data
 
     def send(self, data: bytes) -> Result:
         """
         Method to send data to the server.
@@ -196,14 +203,20 @@
                     # it means that the data transfer has been completed.
                     transfer_complete = True
                 else:
                     # We haven't received any data yet.
                     logging.debug(
                         f"There is no data in the socket. Timeout: {timeout}s."
                     )
+                    if backoff.total >= float(self.timeout_limit):
+                        logging.error(
+                            "The waiting time limit for a response has been reached."
+                        )
+                        return Result.fail(Errors.TimeoutLimit.value)
+
                     sleep(timeout)
                     continue
 
             if transfer_complete:
                 # If the first byte is "-", it means that the response is an error.
                 if total_bytes.startswith(b"-"):
                     error_message: str = total_bytes.decode()[1::]
```

### Comparing `zcached.py-1.1.1/zcached/deserializer.py` & `zcached.py-1.2.1/zcached/deserializer.py`

 * *Files identical despite different names*

### Comparing `zcached.py-1.1.1/zcached/enums.py` & `zcached.py-1.2.1/zcached/enums.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 
 class Errors(str, Enum):
     ConnectionClosed = "The connection has been terminated."
     ConnectionReestablished = (
         "The connection was terminated, but managed to reestablish it."
     )
     LibraryBug = "This is probably a library bug. Please report it here: https://github.com/xXenvy/zcached.py"
+    TimeoutLimit = "The waiting time limit for a response has been reached."
 
     # Server side errors:
     BadRequest = "ERR bad request"
     UnExpected = "ERR unexpected"
     MaxClientsReached = "ERR max number of clients reached"
     BulkTooLarge = "ERR bulk too large"
     NotWhitelisted = "ERR not whitelisted"
     KeyNotString = "TYPERR key not string"
     NotBoolean = "TYPERR not boolean"
     NotInteger = "TYPERR not integer"
+    SaveFailure = "ERR there is no data to save"
 
     @staticmethod
     def not_found(key: str) -> str:
         """Generates an error message for a key that was not found."""
         return f"ERR '{key}' not found"
 
     @staticmethod
```

### Comparing `zcached.py-1.1.1/zcached/reader.py` & `zcached.py-1.2.1/zcached/reader.py`

 * *Files identical despite different names*

### Comparing `zcached.py-1.1.1/zcached/result.py` & `zcached.py-1.2.1/zcached/result.py`

 * *Files identical despite different names*

### Comparing `zcached.py-1.1.1/zcached/serializer.py` & `zcached.py-1.2.1/zcached/serializer.py`

 * *Files identical despite different names*

### Comparing `zcached.py-1.1.1/zcached.py.egg-info/PKG-INFO` & `zcached.py-1.2.1/zcached.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcached.py
-Version: 1.1.1
+Version: 1.2.1
 Summary: A lightweight client-side library for zcached, written in Python.
 Home-page: https://github.com/xXenvy/zcached.py
 Author: xXenvy
 Project-URL: Bug Reports, https://github.com/xXenvy/zcached.py/issues
 Project-URL: Source, https://github.com/xXenvy/zcached.py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -26,31 +26,31 @@
 # Zcached.py - A client-side library for zcached.
 
 ![commits](https://img.shields.io/github/commit-activity/w/xXenvy/zcached.py?style=for-the-badge&color=%2315b328)
 ![license](https://img.shields.io/github/license/xXenvy/zcached.py?style=for-the-badge&color=%2315b328)
 ![release](https://img.shields.io/github/v/release/xXenvy/zcached.py?include_prereleases&style=for-the-badge&color=%2315b328)
 
 ## `📜` Introduction
-Zcached.py is a Python client-side library designed to interact with zcached, a high-performance caching system.
+Zcached.py is a Python client-side library designed to interact with zcached, a high-performance in-memory caching system.
 This library provides developers an easy-to-use interface for integrating zcached into their Python applications, enabling efficient data caching.
 
 For more information, please see [zcached repository](https://github.com/sectasy0/zcached).
 
 ## `🌟` Features
 - **Simplified Caching:** Zcached.py simplifies the process of caching data by providing intuitive functions for storing and retrieving values.
 - **Efficient Communication:** The library optimizes communication with the zcached server, ensuring minimal overhead and efficient data transfer.
 - **Properly Typehinted:** The codebase of zcached.py is properly typehinted, enhancing code readability.
 
 ## `🔧` Installation
 > [!IMPORTANT]  
 > **Library requires python version 3.8 or newer.** (Older also should work, but untested).
 
-Before installing zcached.py, ensure that you have the zcached server. Instructions for installing the server can be found [here](https://github.com/sectasy0/zcached).
+Before installing zcached.py, ensure that you have the zcached server. Instructions for installing and running the server can be found [here](https://github.com/sectasy0/zcached).
 
-Once the zcached server is installed, you can proceed to install zcached.py using pip:
+Once the zcached server is ready to use, you can proceed to install zcached.py using pip:
 ```shell
 pip install -U zcached.py
 ```
 
 ## `🖊️` Usage
 Here's a basic example demonstrating how to use zcached.py in your Python code:
 ```py
```

### Comparing `zcached.py-1.1.1/zcached.py.egg-info/SOURCES.txt` & `zcached.py-1.2.1/zcached.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

