# Comparing `tmp/websocket-client-1.6.4.tar.gz` & `tmp/websocket-client-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "websocket-client-1.6.4.tar", last modified: Sun Oct  8 09:41:26 2023, max compression
+gzip compressed data, was "websocket-client-1.7.0.tar", last modified: Sun Dec  3 15:55:59 2023, max compression
```

## Comparing `websocket-client-1.6.4.tar` & `websocket-client-1.7.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwxr-x   0 engn33r   (1000) engn33r   (1000)        0 2023-10-08 09:41:26.570065 websocket-client-1.6.4/
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)    18014 2023-10-08 09:39:41.000000 websocket-client-1.6.4/ChangeLog
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)    11339 2023-08-07 03:14:24.000000 websocket-client-1.6.4/LICENSE
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)       81 2023-08-07 03:14:24.000000 websocket-client-1.6.4/MANIFEST.in
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     7436 2023-10-08 09:41:26.570065 websocket-client-1.6.4/PKG-INFO
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     5997 2023-08-07 03:14:24.000000 websocket-client-1.6.4/README.md
-drwxrwxr-x   0 engn33r   (1000) engn33r   (1000)        0 2023-10-08 09:41:26.566065 websocket-client-1.6.4/examples/
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)      344 2023-08-07 03:14:24.000000 websocket-client-1.6.4/examples/echo_client.py
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     1009 2023-08-07 03:14:24.000000 websocket-client-1.6.4/examples/echoapp_client.py
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)      351 2023-08-07 03:14:24.000000 websocket-client-1.6.4/examples/rel_client.py
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)       59 2023-10-08 09:41:26.570065 websocket-client-1.6.4/setup.cfg
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     2721 2023-10-08 09:40:19.000000 websocket-client-1.6.4/setup.py
-drwxrwxr-x   0 engn33r   (1000) engn33r   (1000)        0 2023-10-08 09:41:26.570065 websocket-client-1.6.4/websocket/
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)      801 2023-10-08 09:40:32.000000 websocket-client-1.6.4/websocket/__init__.py
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)    13769 2023-09-11 03:47:25.000000 websocket-client-1.6.4/websocket/_abnf.py
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)    21595 2023-09-11 03:47:25.000000 websocket-client-1.6.4/websocket/_app.py
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     2203 2023-09-11 03:47:25.000000 websocket-client-1.6.4/websocket/_cookiejar.py
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)    20181 2023-09-11 03:47:25.000000 websocket-client-1.6.4/websocket/_core.py
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     2116 2023-08-07 03:14:24.000000 websocket-client-1.6.4/websocket/_exceptions.py
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     6770 2023-09-21 20:30:20.000000 websocket-client-1.6.4/websocket/_handshake.py
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)    12242 2023-08-22 15:11:12.000000 websocket-client-1.6.4/websocket/_http.py
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     2220 2023-08-07 03:14:24.000000 websocket-client-1.6.4/websocket/_logging.py
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     5060 2023-09-11 03:47:25.000000 websocket-client-1.6.4/websocket/_socket.py
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     1122 2023-08-07 03:14:24.000000 websocket-client-1.6.4/websocket/_ssl_compat.py
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     4904 2023-09-11 03:47:25.000000 websocket-client-1.6.4/websocket/_url.py
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     3713 2023-09-11 03:47:25.000000 websocket-client-1.6.4/websocket/_utils.py
--rwxrwxr-x   0 engn33r   (1000) engn33r   (1000)     7106 2023-08-07 03:14:24.000000 websocket-client-1.6.4/websocket/_wsdump.py
-drwxrwxr-x   0 engn33r   (1000) engn33r   (1000)        0 2023-10-08 09:41:26.570065 websocket-client-1.6.4/websocket/tests/
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)        0 2023-08-07 03:14:24.000000 websocket-client-1.6.4/websocket/tests/__init__.py
-drwxrwxr-x   0 engn33r   (1000) engn33r   (1000)        0 2023-10-08 09:41:26.570065 websocket-client-1.6.4/websocket/tests/data/
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)      163 2023-08-07 03:14:24.000000 websocket-client-1.6.4/websocket/tests/data/header01.txt
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)      161 2023-08-07 03:14:24.000000 websocket-client-1.6.4/websocket/tests/data/header02.txt
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)      216 2023-08-07 03:14:24.000000 websocket-client-1.6.4/websocket/tests/data/header03.txt
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)      486 2023-08-07 03:14:24.000000 websocket-client-1.6.4/websocket/tests/echo-server.py
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     4175 2023-08-07 03:14:24.000000 websocket-client-1.6.4/websocket/tests/test_abnf.py
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)    11795 2023-08-15 03:26:19.000000 websocket-client-1.6.4/websocket/tests/test_app.py
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     4325 2023-08-07 03:14:24.000000 websocket-client-1.6.4/websocket/tests/test_cookiejar.py
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     9623 2023-08-22 15:11:12.000000 websocket-client-1.6.4/websocket/tests/test_http.py
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)    15737 2023-08-07 03:14:24.000000 websocket-client-1.6.4/websocket/tests/test_url.py
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)    18072 2023-08-07 03:14:24.000000 websocket-client-1.6.4/websocket/tests/test_websocket.py
-drwxrwxr-x   0 engn33r   (1000) engn33r   (1000)        0 2023-10-08 09:41:26.570065 websocket-client-1.6.4/websocket_client.egg-info/
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     7436 2023-10-08 09:41:26.000000 websocket-client-1.6.4/websocket_client.egg-info/PKG-INFO
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     1014 2023-10-08 09:41:26.000000 websocket-client-1.6.4/websocket_client.egg-info/SOURCES.txt
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)        1 2023-10-08 09:41:26.000000 websocket-client-1.6.4/websocket_client.egg-info/dependency_links.txt
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)       51 2023-10-08 09:41:26.000000 websocket-client-1.6.4/websocket_client.egg-info/entry_points.txt
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)       96 2023-10-08 09:41:26.000000 websocket-client-1.6.4/websocket_client.egg-info/requires.txt
--rw-rw-r--   0 engn33r   (1000) engn33r   (1000)       10 2023-10-08 09:41:26.000000 websocket-client-1.6.4/websocket_client.egg-info/top_level.txt
+drwxrwxr-x   0 engn33r   (1000) engn33r   (1000)        0 2023-12-03 15:55:59.329127 websocket-client-1.7.0/
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)    18460 2023-12-03 15:44:37.000000 websocket-client-1.7.0/ChangeLog
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)    11339 2023-08-07 03:14:24.000000 websocket-client-1.7.0/LICENSE
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)       81 2023-08-07 03:14:24.000000 websocket-client-1.7.0/MANIFEST.in
+-rw-r--r--   0 engn33r   (1000) engn33r   (1000)     7880 2023-12-03 15:55:59.329127 websocket-client-1.7.0/PKG-INFO
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     6225 2023-12-03 08:05:38.000000 websocket-client-1.7.0/README.md
+drwxrwxr-x   0 engn33r   (1000) engn33r   (1000)        0 2023-12-03 15:55:59.329127 websocket-client-1.7.0/examples/
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)      342 2023-12-03 06:44:41.000000 websocket-client-1.7.0/examples/echo_client.py
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)      928 2023-12-03 08:01:38.000000 websocket-client-1.7.0/examples/echoapp_client.py
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)      352 2023-12-03 08:01:38.000000 websocket-client-1.7.0/examples/rel_client.py
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)      178 2023-12-03 15:55:59.329127 websocket-client-1.7.0/setup.cfg
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     2709 2023-12-03 15:45:16.000000 websocket-client-1.7.0/setup.py
+drwxrwxr-x   0 engn33r   (1000) engn33r   (1000)        0 2023-12-03 15:55:59.329127 websocket-client-1.7.0/websocket/
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)      801 2023-12-03 15:45:29.000000 websocket-client-1.7.0/websocket/__init__.py
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)    14333 2023-12-03 15:22:11.000000 websocket-client-1.7.0/websocket/_abnf.py
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)    23614 2023-12-03 12:07:51.000000 websocket-client-1.7.0/websocket/_app.py
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     2418 2023-12-03 10:39:23.000000 websocket-client-1.7.0/websocket/_cookiejar.py
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)    20819 2023-12-03 12:06:24.000000 websocket-client-1.7.0/websocket/_core.py
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     2178 2023-12-03 07:54:06.000000 websocket-client-1.7.0/websocket/_exceptions.py
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     6508 2023-12-03 12:07:51.000000 websocket-client-1.7.0/websocket/_handshake.py
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)    12660 2023-12-03 11:52:11.000000 websocket-client-1.7.0/websocket/_http.py
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     2228 2023-12-03 07:54:06.000000 websocket-client-1.7.0/websocket/_logging.py
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     5043 2023-12-03 12:07:40.000000 websocket-client-1.7.0/websocket/_socket.py
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     1085 2023-12-03 08:01:38.000000 websocket-client-1.7.0/websocket/_ssl_compat.py
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     5086 2023-12-03 11:26:13.000000 websocket-client-1.7.0/websocket/_url.py
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     6961 2023-12-03 11:36:57.000000 websocket-client-1.7.0/websocket/_utils.py
+-rwxrwxr-x   0 engn33r   (1000) engn33r   (1000)     7010 2023-12-03 08:01:38.000000 websocket-client-1.7.0/websocket/_wsdump.py
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)        0 2023-12-03 05:53:16.000000 websocket-client-1.7.0/websocket/py.typed
+drwxrwxr-x   0 engn33r   (1000) engn33r   (1000)        0 2023-12-03 15:55:59.329127 websocket-client-1.7.0/websocket/tests/
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)        0 2023-08-07 03:14:24.000000 websocket-client-1.7.0/websocket/tests/__init__.py
+drwxrwxr-x   0 engn33r   (1000) engn33r   (1000)        0 2023-12-03 15:55:59.329127 websocket-client-1.7.0/websocket/tests/data/
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)      163 2023-08-07 03:14:24.000000 websocket-client-1.7.0/websocket/tests/data/header01.txt
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)      161 2023-08-07 03:14:24.000000 websocket-client-1.7.0/websocket/tests/data/header02.txt
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)      216 2023-08-07 03:14:24.000000 websocket-client-1.7.0/websocket/tests/data/header03.txt
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)      488 2023-12-03 08:01:38.000000 websocket-client-1.7.0/websocket/tests/echo-server.py
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     4658 2023-12-03 15:22:49.000000 websocket-client-1.7.0/websocket/tests/test_abnf.py
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)    12317 2023-12-03 08:01:38.000000 websocket-client-1.7.0/websocket/tests/test_app.py
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     4392 2023-12-03 08:01:38.000000 websocket-client-1.7.0/websocket/tests/test_cookiejar.py
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)    12427 2023-12-03 08:02:27.000000 websocket-client-1.7.0/websocket/tests/test_http.py
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)    17203 2023-12-03 08:02:27.000000 websocket-client-1.7.0/websocket/tests/test_url.py
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)    18434 2023-12-03 08:01:38.000000 websocket-client-1.7.0/websocket/tests/test_websocket.py
+drwxrwxr-x   0 engn33r   (1000) engn33r   (1000)        0 2023-12-03 15:55:59.329127 websocket-client-1.7.0/websocket_client.egg-info/
+-rw-r--r--   0 engn33r   (1000) engn33r   (1000)     7880 2023-12-03 15:55:59.000000 websocket-client-1.7.0/websocket_client.egg-info/PKG-INFO
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)     1033 2023-12-03 15:55:59.000000 websocket-client-1.7.0/websocket_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)        1 2023-12-03 15:55:59.000000 websocket-client-1.7.0/websocket_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)       50 2023-12-03 15:55:59.000000 websocket-client-1.7.0/websocket_client.egg-info/entry_points.txt
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)       96 2023-12-03 15:55:59.000000 websocket-client-1.7.0/websocket_client.egg-info/requires.txt
+-rw-rw-r--   0 engn33r   (1000) engn33r   (1000)       10 2023-12-03 15:55:59.000000 websocket-client-1.7.0/websocket_client.egg-info/top_level.txt
```

### Comparing `websocket-client-1.6.4/ChangeLog` & `websocket-client-1.7.0/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 ChangeLog
 ============
 
+- 1.7.0
+  - Renamed `mask` variable in ABNF to prevent name collision with `mask()` function (9b51f73)
+  - Fixed old http import of HTTPStatus in _handshake.py (9b51f73)
+  - Add `send_text()` and `send_bytes()` to _app.py (#953)
+  - Improved typehint support (#953, 9b51f73, 8b73d00)
+  - General readability improvements, made all string concatenations use f-strings (#909, 780584f, 3eabc6e)
+  - Applied black formatting style to code (da7f286)
+
 - 1.6.4
   - Fix #952, add support for HTTP 307 and 308 redirect codes (69468ad)
 
 - 1.6.3
   - Fix type hints issues (#949)
   - Add support for Python beta release 3.12 in CI (#946)
   - Add maintainer email in setup.py (3d464fc)
```

### Comparing `websocket-client-1.6.4/LICENSE` & `websocket-client-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `websocket-client-1.6.4/PKG-INFO` & `websocket-client-1.7.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,14 @@
-Metadata-Version: 2.1
-Name: websocket-client
-Version: 1.6.4
-Summary: WebSocket client for Python with low level API options
-Home-page: https://github.com/websocket-client/websocket-client.git
-Author: liris
-Author-email: liris.pp@gmail.com
-Maintainer: engn33r
-Maintainer-email: websocket.client@proton.me
-License: Apache-2.0
-Download-URL: https://github.com/websocket-client/websocket-client/releases
-Project-URL: Documentation, https://websocket-client.readthedocs.io/
-Project-URL: Source, https://github.com/websocket-client/websocket-client/
-Keywords: websockets client
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: optional
-Provides-Extra: test
-License-File: LICENSE
-
 [![docs](https://readthedocs.org/projects/websocket-client/badge/?style=flat)](https://websocket-client.readthedocs.io/)
 [![Build Status](https://github.com/websocket-client/websocket-client/actions/workflows/build.yml/badge.svg)](https://github.com/websocket-client/websocket-client/actions/workflows/build.yml)
 [![codecov](https://codecov.io/gh/websocket-client/websocket-client/branch/master/graph/badge.svg?token=pcXhUQwiL3)](https://codecov.io/gh/websocket-client/websocket-client)
 [![PyPI Downloads](https://pepy.tech/badge/websocket-client)](https://pepy.tech/project/websocket-client)
 [![PyPI version](https://img.shields.io/pypi/v/websocket_client)](https://pypi.org/project/websocket_client/)
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # websocket-client
 
 websocket-client is a WebSocket client for Python. It provides access
 to low level APIs for WebSockets. websocket-client implements version
 [hybi-13](https://tools.ietf.org/html/draft-ietf-hybi-thewebsocketprotocol-13)
 of the WebSocket protocol. This client does not currently support the
@@ -171,9 +137,7 @@
 ws.send("Hello, World")
 print("Sent")
 print("Receiving...")
 result =  ws.recv()
 print("Received '%s'" % result)
 ws.close()
 ```
-
-
```

### Comparing `websocket-client-1.6.4/README.md` & `websocket-client-1.7.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,54 @@
+Metadata-Version: 2.1
+Name: websocket-client
+Version: 1.7.0
+Summary: WebSocket client for Python with low level API options
+Home-page: https://github.com/websocket-client/websocket-client.git
+Download-URL: https://github.com/websocket-client/websocket-client/releases
+Author: liris
+Author-email: liris.pp@gmail.com
+Maintainer: engn33r
+Maintainer-email: websocket.client@proton.me
+License: Apache-2.0
+Project-URL: Documentation, https://websocket-client.readthedocs.io/
+Project-URL: Source, https://github.com/websocket-client/websocket-client/
+Keywords: websockets client
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Provides-Extra: test
+Requires-Dist: websockets; extra == "test"
+Provides-Extra: optional
+Requires-Dist: python-socks; extra == "optional"
+Requires-Dist: wsaccel; extra == "optional"
+Provides-Extra: docs
+Requires-Dist: Sphinx>=6.0; extra == "docs"
+Requires-Dist: sphinx_rtd_theme>=1.1.0; extra == "docs"
+
 [![docs](https://readthedocs.org/projects/websocket-client/badge/?style=flat)](https://websocket-client.readthedocs.io/)
 [![Build Status](https://github.com/websocket-client/websocket-client/actions/workflows/build.yml/badge.svg)](https://github.com/websocket-client/websocket-client/actions/workflows/build.yml)
 [![codecov](https://codecov.io/gh/websocket-client/websocket-client/branch/master/graph/badge.svg?token=pcXhUQwiL3)](https://codecov.io/gh/websocket-client/websocket-client)
 [![PyPI Downloads](https://pepy.tech/badge/websocket-client)](https://pepy.tech/project/websocket-client)
 [![PyPI version](https://img.shields.io/pypi/v/websocket_client)](https://pypi.org/project/websocket_client/)
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # websocket-client
 
 websocket-client is a WebSocket client for Python. It provides access
 to low level APIs for WebSockets. websocket-client implements version
 [hybi-13](https://tools.ietf.org/html/draft-ietf-hybi-thewebsocketprotocol-13)
 of the WebSocket protocol. This client does not currently support the
```

### Comparing `websocket-client-1.6.4/examples/echoapp_client.py` & `websocket-client-1.7.0/examples/echoapp_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import websocket
-from threading import Thread
-import time
 import sys
+import time
+from threading import Thread
+
+import websocket
 
 
 def on_message(ws, message):
     print(message)
 
 
 def on_error(ws, error):
@@ -34,13 +35,12 @@
 
 if __name__ == "__main__":
     websocket.enableTrace(True)
     if len(sys.argv) < 2:
         host = "ws://echo.websocket.events/"
     else:
         host = sys.argv[1]
-    ws = websocket.WebSocketApp(host,
-                                on_message=on_message,
-                                on_error=on_error,
-                                on_close=on_close)
+    ws = websocket.WebSocketApp(
+        host, on_message=on_message, on_error=on_error, on_close=on_close
+    )
     ws.on_open = on_open
     ws.run_forever()
```

### Comparing `websocket-client-1.6.4/setup.py` & `websocket-client-1.7.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sys
+
 import pkg_resources
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 """
 setup.py
 websocket - WebSocket client library for Python
 
 Copyright 2023 engn33r
 
@@ -17,33 +18,33 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-VERSION = "1.6.4"
+VERSION = "1.7.0"
 
 install_requires = []
 tests_require = []
 
 setup(
     name="websocket-client",
     version=VERSION,
     description="WebSocket client for Python with low level API options",
     long_description=open("README.md").read(),
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     author="liris",
     author_email="liris.pp@gmail.com",
     maintainer="engn33r",
     maintainer_email="websocket.client@proton.me",
     license="Apache-2.0",
     url="https://github.com/websocket-client/websocket-client.git",
-    download_url='https://github.com/websocket-client/websocket-client/releases',
-    python_requires='>=3.8',
+    download_url="https://github.com/websocket-client/websocket-client/releases",
+    python_requires=">=3.8",
     extras_require={
         "test": ["websockets"],
         "optional": ["python-socks", "wsaccel"],
         "docs": ["Sphinx >= 6.0", "sphinx_rtd_theme >= 1.1.0"],
     },
     classifiers=[
         "Development Status :: 4 - Beta",
@@ -58,24 +59,22 @@
         "Operating System :: POSIX",
         "Operating System :: Microsoft :: Windows",
         "Topic :: Internet",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Intended Audience :: Developers",
     ],
     project_urls={
-        'Documentation': 'https://websocket-client.readthedocs.io/',
-        'Source': 'https://github.com/websocket-client/websocket-client/',
+        "Documentation": "https://websocket-client.readthedocs.io/",
+        "Source": "https://github.com/websocket-client/websocket-client/",
     },
-    keywords='websockets client',
+    keywords="websockets client",
     entry_points={
-        'console_scripts': [
-            'wsdump=websocket._wsdump:main',
+        "console_scripts": [
+            "wsdump=websocket._wsdump:main",
         ],
     },
     install_requires=install_requires,
     packages=find_packages(),
-    package_data={
-        'websocket.tests': ['data/*.txt']
-    },
+    package_data={"websocket.tests": ["data/*.txt"]},
     tests_require=tests_require,
-    test_suite="websocket.tests"
+    test_suite="websocket.tests",
 )
```

### Comparing `websocket-client-1.6.4/websocket/__init__.py` & `websocket-client-1.7.0/websocket/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 from ._abnf import *
 from ._app import WebSocketApp, setReconnect
 from ._core import *
 from ._exceptions import *
 from ._logging import *
 from ._socket import *
 
-__version__ = "1.6.4"
+__version__ = "1.7.0"
```

### Comparing `websocket-client-1.6.4/websocket/_abnf.py` & `websocket-client-1.7.0/websocket/_abnf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import array
 import os
 import struct
 import sys
-
 from threading import Lock
-from typing import Callable, Union
+from typing import Callable, Optional, Union
 
 from ._exceptions import *
 from ._utils import validate_utf8
 
 """
 _abnf.py
 websocket - WebSocket client library for Python
@@ -31,43 +30,48 @@
 try:
     # If wsaccel is available, use compiled routines to mask data.
     # wsaccel only provides around a 10% speed boost compared
     # to the websocket-client _mask() implementation.
     # Note that wsaccel is unmaintained.
     from wsaccel.xormask import XorMaskerSimple
 
-    def _mask(_m, _d) -> bytes:
-        return XorMaskerSimple(_m).process(_d)
+    def _mask(mask_value: array.array, data_value: array.array) -> bytes:
+        mask_result: bytes = XorMaskerSimple(mask_value).process(data_value)
+        return mask_result
 
 except ImportError:
     # wsaccel is not available, use websocket-client _mask()
     native_byteorder = sys.byteorder
 
     def _mask(mask_value: array.array, data_value: array.array) -> bytes:
         datalen = len(data_value)
         int_data_value = int.from_bytes(data_value, native_byteorder)
-        int_mask_value = int.from_bytes(mask_value * (datalen // 4) + mask_value[: datalen % 4], native_byteorder)
+        int_mask_value = int.from_bytes(
+            mask_value * (datalen // 4) + mask_value[: datalen % 4], native_byteorder
+        )
         return (int_data_value ^ int_mask_value).to_bytes(datalen, native_byteorder)
 
 
 __all__ = [
-    'ABNF', 'continuous_frame', 'frame_buffer',
-    'STATUS_NORMAL',
-    'STATUS_GOING_AWAY',
-    'STATUS_PROTOCOL_ERROR',
-    'STATUS_UNSUPPORTED_DATA_TYPE',
-    'STATUS_STATUS_NOT_AVAILABLE',
-    'STATUS_ABNORMAL_CLOSED',
-    'STATUS_INVALID_PAYLOAD',
-    'STATUS_POLICY_VIOLATION',
-    'STATUS_MESSAGE_TOO_BIG',
-    'STATUS_INVALID_EXTENSION',
-    'STATUS_UNEXPECTED_CONDITION',
-    'STATUS_BAD_GATEWAY',
-    'STATUS_TLS_HANDSHAKE_ERROR',
+    "ABNF",
+    "continuous_frame",
+    "frame_buffer",
+    "STATUS_NORMAL",
+    "STATUS_GOING_AWAY",
+    "STATUS_PROTOCOL_ERROR",
+    "STATUS_UNSUPPORTED_DATA_TYPE",
+    "STATUS_STATUS_NOT_AVAILABLE",
+    "STATUS_ABNORMAL_CLOSED",
+    "STATUS_INVALID_PAYLOAD",
+    "STATUS_POLICY_VIOLATION",
+    "STATUS_MESSAGE_TOO_BIG",
+    "STATUS_INVALID_EXTENSION",
+    "STATUS_UNEXPECTED_CONDITION",
+    "STATUS_BAD_GATEWAY",
+    "STATUS_TLS_HANDSHAKE_ERROR",
 ]
 
 # closing frame status codes.
 STATUS_NORMAL = 1000
 STATUS_GOING_AWAY = 1001
 STATUS_PROTOCOL_ERROR = 1002
 STATUS_UNSUPPORTED_DATA_TYPE = 1003
@@ -108,46 +112,60 @@
 
     # operation code values.
     OPCODE_CONT = 0x0
     OPCODE_TEXT = 0x1
     OPCODE_BINARY = 0x2
     OPCODE_CLOSE = 0x8
     OPCODE_PING = 0x9
-    OPCODE_PONG = 0xa
+    OPCODE_PONG = 0xA
 
     # available operation code value tuple
-    OPCODES = (OPCODE_CONT, OPCODE_TEXT, OPCODE_BINARY, OPCODE_CLOSE,
-               OPCODE_PING, OPCODE_PONG)
+    OPCODES = (
+        OPCODE_CONT,
+        OPCODE_TEXT,
+        OPCODE_BINARY,
+        OPCODE_CLOSE,
+        OPCODE_PING,
+        OPCODE_PONG,
+    )
 
     # opcode human readable string
     OPCODE_MAP = {
         OPCODE_CONT: "cont",
         OPCODE_TEXT: "text",
         OPCODE_BINARY: "binary",
         OPCODE_CLOSE: "close",
         OPCODE_PING: "ping",
-        OPCODE_PONG: "pong"
+        OPCODE_PONG: "pong",
     }
 
     # data length threshold.
-    LENGTH_7 = 0x7e
+    LENGTH_7 = 0x7E
     LENGTH_16 = 1 << 16
     LENGTH_63 = 1 << 63
 
-    def __init__(self, fin: int = 0, rsv1: int = 0, rsv2: int = 0, rsv3: int = 0,
-                 opcode: int = OPCODE_TEXT, mask: int = 1, data: Union[str, bytes] = "") -> None:
+    def __init__(
+        self,
+        fin: int = 0,
+        rsv1: int = 0,
+        rsv2: int = 0,
+        rsv3: int = 0,
+        opcode: int = OPCODE_TEXT,
+        mask_value: int = 1,
+        data: Union[str, bytes, None] = "",
+    ) -> None:
         """
         Constructor for ABNF. Please check RFC for arguments.
         """
         self.fin = fin
         self.rsv1 = rsv1
         self.rsv2 = rsv2
         self.rsv3 = rsv3
         self.opcode = opcode
-        self.mask = mask
+        self.mask_value = mask_value
         if data is None:
             data = ""
         self.data = data
         self.get_mask_key = os.urandom
 
     def validate(self, skip_utf8_validation: bool = False) -> None:
         """
@@ -171,29 +189,27 @@
             if not l:
                 return
             if l == 1 or l >= 126:
                 raise WebSocketProtocolException("Invalid close frame.")
             if l > 2 and not skip_utf8_validation and not validate_utf8(self.data[2:]):
                 raise WebSocketProtocolException("Invalid close frame.")
 
-            code = 256 * self.data[0] + self.data[1]
+            code = 256 * int(self.data[0]) + int(self.data[1])
             if not self._is_valid_close_status(code):
                 raise WebSocketProtocolException("Invalid close opcode %r", code)
 
     @staticmethod
     def _is_valid_close_status(code: int) -> bool:
         return code in VALID_CLOSE_STATUS or (3000 <= code < 5000)
 
     def __str__(self) -> str:
-        return "fin=" + str(self.fin) \
-            + " opcode=" + str(self.opcode) \
-            + " data=" + str(self.data)
+        return f"fin={self.fin} opcode={self.opcode} data={self.data}"
 
     @staticmethod
-    def create_frame(data: Union[bytes, str], opcode: int, fin: int = 1) -> 'ABNF':
+    def create_frame(data: Union[bytes, str], opcode: int, fin: int = 1) -> "ABNF":
         """
         Create frame to send text, binary and other data.
 
         Parameters
         ----------
         data: str
             data to send. This is string value(byte array).
@@ -217,37 +233,42 @@
             raise ValueError("not 0 or 1")
         if self.opcode not in ABNF.OPCODES:
             raise ValueError("Invalid OPCODE")
         length = len(self.data)
         if length >= ABNF.LENGTH_63:
             raise ValueError("data is too long")
 
-        frame_header = chr(self.fin << 7 |
-                           self.rsv1 << 6 | self.rsv2 << 5 | self.rsv3 << 4 |
-                           self.opcode).encode('latin-1')
+        frame_header = chr(
+            self.fin << 7
+            | self.rsv1 << 6
+            | self.rsv2 << 5
+            | self.rsv3 << 4
+            | self.opcode
+        ).encode("latin-1")
         if length < ABNF.LENGTH_7:
-            frame_header += chr(self.mask << 7 | length).encode('latin-1')
+            frame_header += chr(self.mask_value << 7 | length).encode("latin-1")
         elif length < ABNF.LENGTH_16:
-            frame_header += chr(self.mask << 7 | 0x7e).encode('latin-1')
+            frame_header += chr(self.mask_value << 7 | 0x7E).encode("latin-1")
             frame_header += struct.pack("!H", length)
         else:
-            frame_header += chr(self.mask << 7 | 0x7f).encode('latin-1')
+            frame_header += chr(self.mask_value << 7 | 0x7F).encode("latin-1")
             frame_header += struct.pack("!Q", length)
 
-        if not self.mask:
+        if not self.mask_value:
+            if isinstance(self.data, str):
+                self.data = self.data.encode("utf-8")
             return frame_header + self.data
-        else:
-            mask_key = self.get_mask_key(4)
-            return frame_header + self._get_masked(mask_key)
+        mask_key = self.get_mask_key(4)
+        return frame_header + self._get_masked(mask_key)
 
     def _get_masked(self, mask_key: Union[str, bytes]) -> bytes:
         s = ABNF.mask(mask_key, self.data)
 
         if isinstance(mask_key, str):
-            mask_key = mask_key.encode('utf-8')
+            mask_key = mask_key.encode("utf-8")
 
         return mask_key + s
 
     @staticmethod
     def mask(mask_key: Union[str, bytes], data: Union[str, bytes]) -> bytes:
         """
         Mask or unmask data. Just do xor for each byte
@@ -259,105 +280,107 @@
         data: bytes or str
             data to mask/unmask.
         """
         if data is None:
             data = ""
 
         if isinstance(mask_key, str):
-            mask_key = mask_key.encode('latin-1')
+            mask_key = mask_key.encode("latin-1")
 
         if isinstance(data, str):
-            data = data.encode('latin-1')
+            data = data.encode("latin-1")
 
         return _mask(array.array("B", mask_key), array.array("B", data))
 
 
 class frame_buffer:
     _HEADER_MASK_INDEX = 5
     _HEADER_LENGTH_INDEX = 6
 
-    def __init__(self, recv_fn: Callable[[int], int], skip_utf8_validation: bool) -> None:
+    def __init__(
+        self, recv_fn: Callable[[int], int], skip_utf8_validation: bool
+    ) -> None:
         self.recv = recv_fn
         self.skip_utf8_validation = skip_utf8_validation
         # Buffers over the packets from the layer beneath until desired amount
         # bytes of bytes are received.
-        self.recv_buffer = []
+        self.recv_buffer: list = []
         self.clear()
         self.lock = Lock()
 
     def clear(self) -> None:
-        self.header = None
-        self.length = None
-        self.mask = None
+        self.header: Optional[tuple] = None
+        self.length: Optional[int] = None
+        self.mask_value: Union[bytes, str, None] = None
 
     def has_received_header(self) -> bool:
         return self.header is None
 
     def recv_header(self) -> None:
         header = self.recv_strict(2)
         b1 = header[0]
         fin = b1 >> 7 & 1
         rsv1 = b1 >> 6 & 1
         rsv2 = b1 >> 5 & 1
         rsv3 = b1 >> 4 & 1
-        opcode = b1 & 0xf
+        opcode = b1 & 0xF
         b2 = header[1]
         has_mask = b2 >> 7 & 1
-        length_bits = b2 & 0x7f
+        length_bits = b2 & 0x7F
 
         self.header = (fin, rsv1, rsv2, rsv3, opcode, has_mask, length_bits)
 
     def has_mask(self) -> Union[bool, int]:
         if not self.header:
             return False
-        return self.header[frame_buffer._HEADER_MASK_INDEX]
+        header_val: int = self.header[frame_buffer._HEADER_MASK_INDEX]
+        return header_val
 
     def has_received_length(self) -> bool:
         return self.length is None
 
     def recv_length(self) -> None:
         bits = self.header[frame_buffer._HEADER_LENGTH_INDEX]
-        length_bits = bits & 0x7f
-        if length_bits == 0x7e:
+        length_bits = bits & 0x7F
+        if length_bits == 0x7E:
             v = self.recv_strict(2)
             self.length = struct.unpack("!H", v)[0]
-        elif length_bits == 0x7f:
+        elif length_bits == 0x7F:
             v = self.recv_strict(8)
             self.length = struct.unpack("!Q", v)[0]
         else:
             self.length = length_bits
 
     def has_received_mask(self) -> bool:
-        return self.mask is None
+        return self.mask_value is None
 
     def recv_mask(self) -> None:
-        self.mask = self.recv_strict(4) if self.has_mask() else ""
+        self.mask_value = self.recv_strict(4) if self.has_mask() else ""
 
     def recv_frame(self) -> ABNF:
-
         with self.lock:
             # Header
             if self.has_received_header():
                 self.recv_header()
             (fin, rsv1, rsv2, rsv3, opcode, has_mask, _) = self.header
 
             # Frame length
             if self.has_received_length():
                 self.recv_length()
             length = self.length
 
             # Mask
             if self.has_received_mask():
                 self.recv_mask()
-            mask = self.mask
+            mask_value = self.mask_value
 
             # Payload
             payload = self.recv_strict(length)
             if has_mask:
-                payload = ABNF.mask(mask, payload)
+                payload = ABNF.mask(mask_value, payload)
 
             # Reset for next frame
             self.clear()
 
             frame = ABNF(fin, rsv1, rsv2, rsv3, opcode, has_mask, payload)
             frame.validate(self.skip_utf8_validation)
 
@@ -383,26 +406,27 @@
             return unified
         else:
             self.recv_buffer = [unified[bufsize:]]
             return unified[:bufsize]
 
 
 class continuous_frame:
-
     def __init__(self, fire_cont_frame: bool, skip_utf8_validation: bool) -> None:
         self.fire_cont_frame = fire_cont_frame
         self.skip_utf8_validation = skip_utf8_validation
-        self.cont_data = None
-        self.recving_frames = None
+        self.cont_data: Optional[list] = None
+        self.recving_frames: Optional[int] = None
 
     def validate(self, frame: ABNF) -> None:
         if not self.recving_frames and frame.opcode == ABNF.OPCODE_CONT:
             raise WebSocketProtocolException("Illegal frame")
-        if self.recving_frames and \
-                frame.opcode in (ABNF.OPCODE_TEXT, ABNF.OPCODE_BINARY):
+        if self.recving_frames and frame.opcode in (
+            ABNF.OPCODE_TEXT,
+            ABNF.OPCODE_BINARY,
+        ):
             raise WebSocketProtocolException("Illegal frame")
 
     def add(self, frame: ABNF) -> None:
         if self.cont_data:
             self.cont_data[1] += frame.data
         else:
             if frame.opcode in (ABNF.OPCODE_TEXT, ABNF.OPCODE_BINARY):
@@ -411,16 +435,19 @@
 
         if frame.fin:
             self.recving_frames = None
 
     def is_fire(self, frame: ABNF) -> Union[bool, int]:
         return frame.fin or self.fire_cont_frame
 
-    def extract(self, frame: ABNF) -> list:
+    def extract(self, frame: ABNF) -> tuple:
         data = self.cont_data
         self.cont_data = None
         frame.data = data[1]
-        if not self.fire_cont_frame and data[0] == ABNF.OPCODE_TEXT and not self.skip_utf8_validation and not validate_utf8(frame.data):
-            raise WebSocketPayloadException(
-                "cannot decode: " + repr(frame.data))
-
-        return [data[0], frame]
+        if (
+            not self.fire_cont_frame
+            and data[0] == ABNF.OPCODE_TEXT
+            and not self.skip_utf8_validation
+            and not validate_utf8(frame.data)
+        ):
+            raise WebSocketPayloadException(f"cannot decode: {repr(frame.data)}")
+        return data[0], frame
```

### Comparing `websocket-client-1.6.4/websocket/_app.py` & `websocket-client-1.7.0/websocket/_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import inspect
 import selectors
 import socket
-import sys
 import threading
 import time
-import traceback
-
 from typing import Any, Callable, Optional, Union
 
 from . import _logging
 from ._abnf import ABNF
-from ._url import parse_url
 from ._core import WebSocket, getdefaulttimeout
-from ._exceptions import *
+from ._exceptions import (
+    WebSocketConnectionClosedException,
+    WebSocketException,
+    WebSocketTimeoutException,
+)
+from ._url import parse_url
 
 """
 _app.py
 websocket - WebSocket client library for Python
 
 Copyright 2023 engn33r
 
@@ -43,114 +44,144 @@
     RECONNECT = reconnectInterval
 
 
 class DispatcherBase:
     """
     DispatcherBase
     """
-    def __init__(self, app: Any, ping_timeout: float) -> None:
+
+    def __init__(self, app: Any, ping_timeout: Union[float, int, None]) -> None:
         self.app = app
         self.ping_timeout = ping_timeout
 
-    def timeout(self, seconds: int, callback: Callable) -> None:
+    def timeout(self, seconds: Union[float, int, None], callback: Callable) -> None:
         time.sleep(seconds)
         callback()
 
     def reconnect(self, seconds: int, reconnector: Callable) -> None:
         try:
-            _logging.info("reconnect() - retrying in {seconds_count} seconds [{frame_count} frames in stack]".format(
-                seconds_count=seconds, frame_count=len(inspect.stack())))
+            _logging.info(
+                f"reconnect() - retrying in {seconds} seconds [{len(inspect.stack())} frames in stack]"
+            )
             time.sleep(seconds)
             reconnector(reconnecting=True)
         except KeyboardInterrupt as e:
-            _logging.info("User exited {err}".format(err=e))
+            _logging.info(f"User exited {e}")
             raise e
 
 
 class Dispatcher(DispatcherBase):
     """
     Dispatcher
     """
-    def read(self, sock: socket.socket, read_callback: Callable, check_callback: Callable) -> None:
+
+    def read(
+        self,
+        sock: socket.socket,
+        read_callback: Callable,
+        check_callback: Callable,
+    ) -> None:
         sel = selectors.DefaultSelector()
         sel.register(self.app.sock.sock, selectors.EVENT_READ)
         try:
             while self.app.keep_running:
-                r = sel.select(self.ping_timeout)
-                if r:
+                if sel.select(self.ping_timeout):
                     if not read_callback():
                         break
                 check_callback()
         finally:
             sel.close()
 
 
 class SSLDispatcher(DispatcherBase):
     """
     SSLDispatcher
     """
-    def read(self, sock: socket.socket, read_callback: Callable, check_callback: Callable) -> None:
+
+    def read(
+        self,
+        sock: socket.socket,
+        read_callback: Callable,
+        check_callback: Callable,
+    ) -> None:
         sock = self.app.sock.sock
         sel = selectors.DefaultSelector()
         sel.register(sock, selectors.EVENT_READ)
         try:
             while self.app.keep_running:
-                r = self.select(sock, sel)
-                if r:
+                if self.select(sock, sel):
                     if not read_callback():
                         break
                 check_callback()
         finally:
             sel.close()
 
-    def select(self, sock, sel:selectors.DefaultSelector):
+    def select(self, sock, sel: selectors.DefaultSelector):
         sock = self.app.sock.sock
         if sock.pending():
-            return [sock,]
+            return [
+                sock,
+            ]
 
         r = sel.select(self.ping_timeout)
 
         if len(r) > 0:
             return r[0][0]
 
 
 class WrappedDispatcher:
     """
     WrappedDispatcher
     """
-    def __init__(self, app, ping_timeout: float, dispatcher: Dispatcher) -> None:
+
+    def __init__(self, app, ping_timeout: Union[float, int, None], dispatcher) -> None:
         self.app = app
         self.ping_timeout = ping_timeout
         self.dispatcher = dispatcher
         dispatcher.signal(2, dispatcher.abort)  # keyboard interrupt
 
-    def read(self, sock: socket.socket, read_callback: Callable, check_callback: Callable) -> None:
+    def read(
+        self,
+        sock: socket.socket,
+        read_callback: Callable,
+        check_callback: Callable,
+    ) -> None:
         self.dispatcher.read(sock, read_callback)
         self.ping_timeout and self.timeout(self.ping_timeout, check_callback)
 
-    def timeout(self, seconds: int, callback: Callable) -> None:
+    def timeout(self, seconds: float, callback: Callable) -> None:
         self.dispatcher.timeout(seconds, callback)
 
     def reconnect(self, seconds: int, reconnector: Callable) -> None:
         self.timeout(seconds, reconnector)
 
 
 class WebSocketApp:
     """
     Higher level of APIs are provided. The interface is like JavaScript WebSocket object.
     """
 
-    def __init__(self, url: str, header: Union[list, dict, Callable] = None,
-                 on_open: Callable = None, on_message: Callable = None, on_error: Callable = None,
-                 on_close: Callable = None, on_ping: Callable = None, on_pong: Callable = None,
-                 on_cont_message: Callable = None,
-                 keep_running: bool = True, get_mask_key: Callable = None, cookie: str = None,
-                 subprotocols: list = None,
-                 on_data: Callable = None,
-                 socket: socket.socket = None) -> None:
+    def __init__(
+        self,
+        url: str,
+        header: Union[list, dict, Callable, None] = None,
+        on_open: Optional[Callable[[WebSocket], None]] = None,
+        on_message: Optional[Callable[[WebSocket, Any], None]] = None,
+        on_error: Optional[Callable[[WebSocket, Any], None]] = None,
+        on_close: Optional[Callable[[WebSocket, Any, Any], None]] = None,
+        on_ping: Optional[Callable] = None,
+        on_pong: Optional[Callable] = None,
+        on_cont_message: Optional[Callable] = None,
+        keep_running: bool = True,
+        get_mask_key: Optional[Callable] = None,
+        cookie: Optional[str] = None,
+        subprotocols: Optional[list] = None,
+        on_data: Optional[Callable] = None,
+        socket: Optional[socket.socket] = None,
+    ) -> None:
         """
         WebSocketApp initialization
 
         Parameters
         ----------
         url: str
             Websocket url.
@@ -218,89 +249,113 @@
         self.on_error = on_error
         self.on_close = on_close
         self.on_ping = on_ping
         self.on_pong = on_pong
         self.on_cont_message = on_cont_message
         self.keep_running = False
         self.get_mask_key = get_mask_key
-        self.sock = None
-        self.last_ping_tm = 0
-        self.last_pong_tm = 0
-        self.ping_thread = None
-        self.stop_ping = None
-        self.ping_interval = 0
-        self.ping_timeout = None
+        self.sock: Optional[WebSocket] = None
+        self.last_ping_tm = float(0)
+        self.last_pong_tm = float(0)
+        self.ping_thread: Optional[threading.Thread] = None
+        self.stop_ping: Optional[threading.Event] = None
+        self.ping_interval = float(0)
+        self.ping_timeout: Union[float, int, None] = None
         self.ping_payload = ""
         self.subprotocols = subprotocols
         self.prepared_socket = socket
         self.has_errored = False
         self.has_done_teardown = False
         self.has_done_teardown_lock = threading.Lock()
 
-    def send(self, data: str, opcode: int = ABNF.OPCODE_TEXT) -> None:
+    def send(self, data: Union[bytes, str], opcode: int = ABNF.OPCODE_TEXT) -> None:
         """
         send message
 
         Parameters
         ----------
         data: str
             Message to send. If you set opcode to OPCODE_TEXT,
             data must be utf-8 string or unicode.
         opcode: int
             Operation code of data. Default is OPCODE_TEXT.
         """
 
         if not self.sock or self.sock.send(data, opcode) == 0:
-            raise WebSocketConnectionClosedException(
-                "Connection is already closed.")
+            raise WebSocketConnectionClosedException("Connection is already closed.")
+
+    def send_text(self, text_data: str) -> None:
+        """
+        Sends UTF-8 encoded text.
+        """
+        if not self.sock or self.sock.send(text_data, ABNF.OPCODE_TEXT) == 0:
+            raise WebSocketConnectionClosedException("Connection is already closed.")
+
+    def send_bytes(self, data: Union[bytes, bytearray]) -> None:
+        """
+        Sends a sequence of bytes.
+        """
+        if not self.sock or self.sock.send(data, ABNF.OPCODE_BINARY) == 0:
+            raise WebSocketConnectionClosedException("Connection is already closed.")
 
     def close(self, **kwargs) -> None:
         """
         Close websocket connection.
         """
         self.keep_running = False
         if self.sock:
             self.sock.close(**kwargs)
             self.sock = None
 
     def _start_ping_thread(self) -> None:
-        self.last_ping_tm = self.last_pong_tm = 0
+        self.last_ping_tm = self.last_pong_tm = float(0)
         self.stop_ping = threading.Event()
         self.ping_thread = threading.Thread(target=self._send_ping)
         self.ping_thread.daemon = True
         self.ping_thread.start()
 
     def _stop_ping_thread(self) -> None:
         if self.stop_ping:
             self.stop_ping.set()
         if self.ping_thread and self.ping_thread.is_alive():
             self.ping_thread.join(3)
-        self.last_ping_tm = self.last_pong_tm = 0
+        self.last_ping_tm = self.last_pong_tm = float(0)
 
     def _send_ping(self) -> None:
         if self.stop_ping.wait(self.ping_interval) or self.keep_running is False:
             return
         while not self.stop_ping.wait(self.ping_interval) and self.keep_running is True:
             if self.sock:
                 self.last_ping_tm = time.time()
                 try:
                     _logging.debug("Sending ping")
                     self.sock.ping(self.ping_payload)
                 except Exception as e:
-                    _logging.debug("Failed to send ping: {err}".format(err=e))
+                    _logging.debug(f"Failed to send ping: {e}")
 
-    def run_forever(self, sockopt: tuple = None, sslopt: dict = None,
-                    ping_interval: float = 0, ping_timeout: Optional[float] = None,
-                    ping_payload: str = "",
-                    http_proxy_host: str = None, http_proxy_port: Union[int, str] = None,
-                    http_no_proxy: list = None, http_proxy_auth: tuple = None,
-                    http_proxy_timeout: float = None,
-                    skip_utf8_validation: bool = False,
-                    host: str = None, origin: str = None, dispatcher: Dispatcher = None,
-                    suppress_origin: bool = False, proxy_type: str = None, reconnect: int = None) -> bool:
+    def run_forever(
+        self,
+        sockopt: tuple = None,
+        sslopt: dict = None,
+        ping_interval: Union[float, int] = 0,
+        ping_timeout: Union[float, int, None] = None,
+        ping_payload: str = "",
+        http_proxy_host: str = None,
+        http_proxy_port: Union[int, str] = None,
+        http_no_proxy: list = None,
+        http_proxy_auth: tuple = None,
+        http_proxy_timeout: Optional[float] = None,
+        skip_utf8_validation: bool = False,
+        host: str = None,
+        origin: str = None,
+        dispatcher=None,
+        suppress_origin: bool = False,
+        proxy_type: str = None,
+        reconnect: int = None,
+    ) -> bool:
         """
         Run event loop for WebSocket framework.
 
         This loop is an infinite loop and is alive while websocket is available.
 
         Parameters
         ----------
@@ -356,15 +411,15 @@
         if ping_timeout is not None and ping_timeout <= 0:
             raise WebSocketException("Ensure ping_timeout > 0")
         if ping_interval is not None and ping_interval < 0:
             raise WebSocketException("Ensure ping_interval >= 0")
         if ping_timeout and ping_interval and ping_interval <= ping_timeout:
             raise WebSocketException("Ensure ping_interval > ping_timeout")
         if not sockopt:
-            sockopt = []
+            sockopt = ()
         if not sslopt:
             sslopt = {}
         if self.sock:
             raise WebSocketException("socket is already opened")
 
         self.ping_interval = ping_interval
         self.ping_timeout = ping_timeout
@@ -390,169 +445,221 @@
                 self.has_done_teardown = True
 
             self._stop_ping_thread()
             self.keep_running = False
             if self.sock:
                 self.sock.close()
             close_status_code, close_reason = self._get_close_args(
-                close_frame if close_frame else None)
+                close_frame if close_frame else None
+            )
             self.sock = None
 
             # Finally call the callback AFTER all teardown is complete
             self._callback(self.on_close, close_status_code, close_reason)
 
         def setSock(reconnecting: bool = False) -> None:
             if reconnecting and self.sock:
                 self.sock.shutdown()
 
             self.sock = WebSocket(
-                self.get_mask_key, sockopt=sockopt, sslopt=sslopt,
+                self.get_mask_key,
+                sockopt=sockopt,
+                sslopt=sslopt,
                 fire_cont_frame=self.on_cont_message is not None,
                 skip_utf8_validation=skip_utf8_validation,
-                enable_multithread=True)
+                enable_multithread=True,
+            )
 
             self.sock.settimeout(getdefaulttimeout())
             try:
-
                 header = self.header() if callable(self.header) else self.header
 
                 self.sock.connect(
-                    self.url, header=header, cookie=self.cookie,
+                    self.url,
+                    header=header,
+                    cookie=self.cookie,
                     http_proxy_host=http_proxy_host,
-                    http_proxy_port=http_proxy_port, http_no_proxy=http_no_proxy,
-                    http_proxy_auth=http_proxy_auth, http_proxy_timeout=http_proxy_timeout,
+                    http_proxy_port=http_proxy_port,
+                    http_no_proxy=http_no_proxy,
+                    http_proxy_auth=http_proxy_auth,
+                    http_proxy_timeout=http_proxy_timeout,
                     subprotocols=self.subprotocols,
-                    host=host, origin=origin, suppress_origin=suppress_origin,
-                    proxy_type=proxy_type, socket=self.prepared_socket)
+                    host=host,
+                    origin=origin,
+                    suppress_origin=suppress_origin,
+                    proxy_type=proxy_type,
+                    socket=self.prepared_socket,
+                )
 
                 _logging.info("Websocket connected")
 
                 if self.ping_interval:
                     self._start_ping_thread()
 
                 self._callback(self.on_open)
 
                 dispatcher.read(self.sock.sock, read, check)
-            except (WebSocketConnectionClosedException, ConnectionRefusedError, KeyboardInterrupt, SystemExit, Exception) as e:
+            except (
+                WebSocketConnectionClosedException,
+                ConnectionRefusedError,
+                KeyboardInterrupt,
+                SystemExit,
+                Exception,
+            ) as e:
                 handleDisconnect(e, reconnecting)
 
         def read() -> bool:
             if not self.keep_running:
                 return teardown()
 
             try:
                 op_code, frame = self.sock.recv_data_frame(True)
-            except (WebSocketConnectionClosedException, KeyboardInterrupt) as e:
+            except (
+                WebSocketConnectionClosedException,
+                KeyboardInterrupt,
+            ) as e:
                 if custom_dispatcher:
                     return handleDisconnect(e)
                 else:
                     raise e
 
             if op_code == ABNF.OPCODE_CLOSE:
                 return teardown(frame)
             elif op_code == ABNF.OPCODE_PING:
                 self._callback(self.on_ping, frame.data)
             elif op_code == ABNF.OPCODE_PONG:
                 self.last_pong_tm = time.time()
                 self._callback(self.on_pong, frame.data)
             elif op_code == ABNF.OPCODE_CONT and self.on_cont_message:
-                self._callback(self.on_data, frame.data,
-                               frame.opcode, frame.fin)
-                self._callback(self.on_cont_message,
-                               frame.data, frame.fin)
+                self._callback(self.on_data, frame.data, frame.opcode, frame.fin)
+                self._callback(self.on_cont_message, frame.data, frame.fin)
             else:
                 data = frame.data
                 if op_code == ABNF.OPCODE_TEXT and not skip_utf8_validation:
                     data = data.decode("utf-8")
                 self._callback(self.on_data, data, frame.opcode, True)
                 self._callback(self.on_message, data)
 
             return True
 
         def check() -> bool:
-            if (self.ping_timeout):
-                has_timeout_expired = time.time() - self.last_ping_tm > self.ping_timeout
-                has_pong_not_arrived_after_last_ping = self.last_pong_tm - self.last_ping_tm < 0
-                has_pong_arrived_too_late = self.last_pong_tm - self.last_ping_tm > self.ping_timeout
-
-                if (self.last_ping_tm and
-                        has_timeout_expired and
-                        (has_pong_not_arrived_after_last_ping or has_pong_arrived_too_late)):
+            if self.ping_timeout:
+                has_timeout_expired = (
+                    time.time() - self.last_ping_tm > self.ping_timeout
+                )
+                has_pong_not_arrived_after_last_ping = (
+                    self.last_pong_tm - self.last_ping_tm < 0
+                )
+                has_pong_arrived_too_late = (
+                    self.last_pong_tm - self.last_ping_tm > self.ping_timeout
+                )
+
+                if (
+                    self.last_ping_tm
+                    and has_timeout_expired
+                    and (
+                        has_pong_not_arrived_after_last_ping
+                        or has_pong_arrived_too_late
+                    )
+                ):
                     raise WebSocketTimeoutException("ping/pong timed out")
             return True
 
-        def handleDisconnect(e: Exception, reconnecting: bool = False) -> bool:
+        def handleDisconnect(
+            e: Union[
+                WebSocketConnectionClosedException,
+                ConnectionRefusedError,
+                KeyboardInterrupt,
+                SystemExit,
+                Exception,
+            ],
+            reconnecting: bool = False,
+        ) -> bool:
             self.has_errored = True
             self._stop_ping_thread()
             if not reconnecting:
                 self._callback(self.on_error, e)
 
             if isinstance(e, (KeyboardInterrupt, SystemExit)):
                 teardown()
                 # Propagate further
                 raise
 
             if reconnect:
-                _logging.info("{err} - reconnect".format(err=e))
+                _logging.info(f"{e} - reconnect")
                 if custom_dispatcher:
-                    _logging.debug("Calling custom dispatcher reconnect [{frame_count} frames in stack]".format(frame_count=len(inspect.stack())))
+                    _logging.debug(
+                        f"Calling custom dispatcher reconnect [{len(inspect.stack())} frames in stack]"
+                    )
                     dispatcher.reconnect(reconnect, setSock)
             else:
-                _logging.error("{err} - goodbye".format(err=e))
+                _logging.error(f"{e} - goodbye")
                 teardown()
 
         custom_dispatcher = bool(dispatcher)
-        dispatcher = self.create_dispatcher(ping_timeout, dispatcher, parse_url(self.url)[3])
+        dispatcher = self.create_dispatcher(
+            ping_timeout, dispatcher, parse_url(self.url)[3]
+        )
 
         try:
             setSock()
             if not custom_dispatcher and reconnect:
                 while self.keep_running:
-                    _logging.debug("Calling dispatcher reconnect [{frame_count} frames in stack]".format(frame_count=len(inspect.stack())))
+                    _logging.debug(
+                        f"Calling dispatcher reconnect [{len(inspect.stack())} frames in stack]"
+                    )
                     dispatcher.reconnect(reconnect, setSock)
         except (KeyboardInterrupt, Exception) as e:
-            _logging.info("tearing down on exception {err}".format(err=e))
+            _logging.info(f"tearing down on exception {e}")
             teardown()
         finally:
             if not custom_dispatcher:
                 # Ensure teardown was called before returning from run_forever
                 teardown()
 
         return self.has_errored
 
-    def create_dispatcher(self, ping_timeout: int, dispatcher: Dispatcher = None, is_ssl: bool = False) -> DispatcherBase:
+    def create_dispatcher(
+        self,
+        ping_timeout: Union[float, int, None],
+        dispatcher: Optional[DispatcherBase] = None,
+        is_ssl: bool = False,
+    ) -> Union[Dispatcher, SSLDispatcher, WrappedDispatcher]:
         if dispatcher:  # If custom dispatcher is set, use WrappedDispatcher
             return WrappedDispatcher(self, ping_timeout, dispatcher)
         timeout = ping_timeout or 10
         if is_ssl:
             return SSLDispatcher(self, timeout)
-
         return Dispatcher(self, timeout)
 
     def _get_close_args(self, close_frame: ABNF) -> list:
         """
         _get_close_args extracts the close code and reason from the close body
         if it exists (RFC6455 says WebSocket Connection Close Code is optional)
         """
         # Need to catch the case where close_frame is None
         # Otherwise the following if statement causes an error
         if not self.on_close or not close_frame:
             return [None, None]
 
         # Extract close frame status code
         if close_frame.data and len(close_frame.data) >= 2:
-            close_status_code = 256 * close_frame.data[0] + close_frame.data[1]
-            reason = close_frame.data[2:].decode('utf-8')
+            close_status_code = 256 * int(close_frame.data[0]) + int(
+                close_frame.data[1]
+            )
+            reason = close_frame.data[2:]
+            if isinstance(reason, bytes):
+                reason = reason.decode("utf-8")
             return [close_status_code, reason]
         else:
             # Most likely reached this because len(close_frame_data.data) < 2
             return [None, None]
 
     def _callback(self, callback, *args) -> None:
         if callback:
             try:
                 callback(self, *args)
 
             except Exception as e:
-                _logging.error("error from callback {callback}: {err}".format(callback=callback, err=e))
+                _logging.error(f"error from callback {callback}: {e}")
                 if self.on_error:
                     self.on_error(self, e)
```

### Comparing `websocket-client-1.6.4/websocket/_cookiejar.py` & `websocket-client-1.7.0/websocket/_cookiejar.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import http.cookies
-
 from typing import Optional
 
 """
 _cookiejar.py
 websocket - WebSocket client library for Python
 
 Copyright 2023 engn33r
@@ -20,47 +19,57 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 
 class SimpleCookieJar:
     def __init__(self) -> None:
-        self.jar = dict()
+        self.jar: dict = dict()
 
     def add(self, set_cookie: Optional[str]) -> None:
         if set_cookie:
             simpleCookie = http.cookies.SimpleCookie(set_cookie)
 
             for k, v in simpleCookie.items():
-                domain = v.get("domain")
-                if domain:
+                if domain := v.get("domain"):
                     if not domain.startswith("."):
-                        domain = "." + domain
-                    cookie = self.jar.get(domain) if self.jar.get(domain) else http.cookies.SimpleCookie()
+                        domain = f".{domain}"
+                    cookie = (
+                        self.jar.get(domain)
+                        if self.jar.get(domain)
+                        else http.cookies.SimpleCookie()
+                    )
                     cookie.update(simpleCookie)
                     self.jar[domain.lower()] = cookie
 
     def set(self, set_cookie: str) -> None:
         if set_cookie:
             simpleCookie = http.cookies.SimpleCookie(set_cookie)
 
             for k, v in simpleCookie.items():
-                domain = v.get("domain")
-                if domain:
+                if domain := v.get("domain"):
                     if not domain.startswith("."):
-                        domain = "." + domain
+                        domain = f".{domain}"
                     self.jar[domain.lower()] = simpleCookie
 
     def get(self, host: str) -> str:
         if not host:
             return ""
 
         cookies = []
         for domain, simpleCookie in self.jar.items():
             host = host.lower()
             if host.endswith(domain) or host == domain[1:]:
                 cookies.append(self.jar.get(domain))
 
-        return "; ".join(filter(
-            None, sorted(
-                ["%s=%s" % (k, v.value) for cookie in filter(None, cookies) for k, v in cookie.items()]
-            )))
+        return "; ".join(
+            filter(
+                None,
+                sorted(
+                    [
+                        "%s=%s" % (k, v.value)
+                        for cookie in filter(None, cookies)
+                        for k, v in cookie.items()
+                    ]
+                ),
+            )
+        )
```

### Comparing `websocket-client-1.6.4/websocket/_core.py` & `websocket-client-1.7.0/websocket/_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import socket
 import struct
 import threading
 import time
-
 from typing import Optional, Union
 
 # websocket modules
 from ._abnf import *
 from ._exceptions import *
 from ._handshake import *
 from ._http import *
@@ -30,15 +29,15 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-__all__ = ['WebSocket', 'create_connection']
+__all__ = ["WebSocket", "create_connection"]
 
 
 class WebSocket:
     """
     Low level WebSocket interface.
 
     This class is based on the WebSocket protocol `draft-hixie-thewebsocketprotocol-76 <http://tools.ietf.org/html/draft-hixie-thewebsocketprotocol-76>`_
@@ -71,35 +70,41 @@
         Fire recv event for each cont frame. Default is False.
     enable_multithread: bool
         If set to True, lock send method.
     skip_utf8_validation: bool
         Skip utf8 validation.
     """
 
-    def __init__(self, get_mask_key=None, sockopt=None, sslopt=None,
-                 fire_cont_frame: bool = False, enable_multithread: bool = True,
-                 skip_utf8_validation: bool = False, **_):
+    def __init__(
+        self,
+        get_mask_key=None,
+        sockopt=None,
+        sslopt=None,
+        fire_cont_frame: bool = False,
+        enable_multithread: bool = True,
+        skip_utf8_validation: bool = False,
+        **_,
+    ):
         """
         Initialize WebSocket object.
 
         Parameters
         ----------
         sslopt: dict
             Optional dict object for ssl socket options. See FAQ for details.
         """
         self.sock_opt = sock_opt(sockopt, sslopt)
         self.handshake_response = None
-        self.sock = None
+        self.sock: Optional[socket.socket] = None
 
         self.connected = False
         self.get_mask_key = get_mask_key
         # These buffer over the build-up of a single frame.
         self.frame_buffer = frame_buffer(self._recv, skip_utf8_validation)
-        self.cont_frame = continuous_frame(
-            fire_cont_frame, skip_utf8_validation)
+        self.cont_frame = continuous_frame(fire_cont_frame, skip_utf8_validation)
 
         if enable_multithread:
             self.lock = threading.Lock()
             self.readlock = threading.Lock()
         else:
             self.lock = NoLock()
             self.readlock = NoLock()
@@ -131,26 +136,26 @@
             callable object. the func takes 1 argument as integer.
             The argument means length of mask key.
             This func must return string(byte array),
             which length is argument specified.
         """
         self.get_mask_key = func
 
-    def gettimeout(self) -> float:
+    def gettimeout(self) -> Union[float, int, None]:
         """
         Get the websocket timeout (in seconds) as an int or float
 
         Returns
         ----------
         timeout: int or float
              returns timeout value (in seconds). This value could be either float/integer.
         """
         return self.sock_opt.timeout
 
-    def settimeout(self, timeout: Optional[float]):
+    def settimeout(self, timeout: Union[float, int, None]):
         """
         Set the timeout to the websocket.
 
         Parameters
         ----------
         timeout: int or float
             timeout time (in seconds). This value could be either float/integer.
@@ -243,27 +248,34 @@
         redirect_limit: int
             Number of redirects to follow.
         subprotocols: list
             List of available subprotocols. Default is None.
         socket: socket
             Pre-initialized stream socket.
         """
-        self.sock_opt.timeout = options.get('timeout', self.sock_opt.timeout)
-        self.sock, addrs = connect(url, self.sock_opt, proxy_info(**options),
-                                   options.pop('socket', None))
+        self.sock_opt.timeout = options.get("timeout", self.sock_opt.timeout)
+        self.sock, addrs = connect(
+            url, self.sock_opt, proxy_info(**options), options.pop("socket", None)
+        )
 
         try:
             self.handshake_response = handshake(self.sock, url, *addrs, **options)
-            for attempt in range(options.pop('redirect_limit', 3)):
+            for attempt in range(options.pop("redirect_limit", 3)):
                 if self.handshake_response.status in SUPPORTED_REDIRECT_STATUSES:
-                    url = self.handshake_response.headers['location']
+                    url = self.handshake_response.headers["location"]
                     self.sock.close()
-                    self.sock, addrs = connect(url, self.sock_opt, proxy_info(**options),
-                                               options.pop('socket', None))
-                    self.handshake_response = handshake(self.sock, url, *addrs, **options)
+                    self.sock, addrs = connect(
+                        url,
+                        self.sock_opt,
+                        proxy_info(**options),
+                        options.pop("socket", None),
+                    )
+                    self.handshake_response = handshake(
+                        self.sock, url, *addrs, **options
+                    )
             self.connected = True
         except:
             if self.sock:
                 self.sock.close()
                 self.sock = None
             raise
 
@@ -280,14 +292,26 @@
         opcode: int
             Operation code (opcode) to send.
         """
 
         frame = ABNF.create_frame(payload, opcode)
         return self.send_frame(frame)
 
+    def send_text(self, text_data: str) -> int:
+        """
+        Sends UTF-8 encoded text.
+        """
+        return self.send(text_data, ABNF.OPCODE_TEXT)
+
+    def send_bytes(self, data: Union[bytes, bytearray]) -> int:
+        """
+        Sends a sequence of bytes.
+        """
+        return self.send(data, ABNF.OPCODE_BINARY)
+
     def send_frame(self, frame) -> int:
         """
         Send the data frame.
 
         >>> ws = create_connection("ws://echo.websocket.events")
         >>> frame = ABNF.create_frame("Hello", ABNF.OPCODE_TEXT)
         >>> ws.send_frame(frame)
@@ -301,17 +325,17 @@
         frame: ABNF frame
             frame data created by ABNF.create_frame
         """
         if self.get_mask_key:
             frame.get_mask_key = self.get_mask_key
         data = frame.format()
         length = len(data)
-        if (isEnabledForTrace()):
-            trace("++Sent raw: " + repr(data))
-            trace("++Sent decoded: " + frame.__str__())
+        if isEnabledForTrace():
+            trace(f"++Sent raw: {repr(data)}")
+            trace(f"++Sent decoded: {frame.__str__()}")
         with self.lock:
             while data:
                 l = self._send(data)
                 data = data[l:]
 
         return length
 
@@ -359,19 +383,24 @@
         Returns
         ----------
         data: string (byte array) value.
         """
         with self.readlock:
             opcode, data = self.recv_data()
         if opcode == ABNF.OPCODE_TEXT:
-            return data.decode("utf-8")
-        elif opcode == ABNF.OPCODE_TEXT or opcode == ABNF.OPCODE_BINARY:
-            return data
+            data_received: Union[bytes, str] = data
+            if isinstance(data_received, bytes):
+                return data_received.decode("utf-8")
+            elif isinstance(data_received, str):
+                return data_received
+        elif opcode == ABNF.OPCODE_BINARY:
+            data_binary: bytes = data
+            return data_binary
         else:
-            return ''
+            return ""
 
     def recv_data(self, control_frame: bool = False) -> tuple:
         """
         Receive data with operation code.
 
         Parameters
         ----------
@@ -383,15 +412,15 @@
         -------
         opcode, frame.data: tuple
             tuple of operation code and string(byte array) value.
         """
         opcode, frame = self.recv_data_frame(control_frame)
         return opcode, frame.data
 
-    def recv_data_frame(self, control_frame: bool = False):
+    def recv_data_frame(self, control_frame: bool = False) -> tuple:
         """
         Receive data with operation code.
 
         If a valid ping message is received, a pong response is sent.
 
         Parameters
         ----------
@@ -402,38 +431,40 @@
         Returns
         -------
         frame.opcode, frame: tuple
             tuple of operation code and string(byte array) value.
         """
         while True:
             frame = self.recv_frame()
-            if (isEnabledForTrace()):
-                trace("++Rcv raw: " + repr(frame.format()))
-                trace("++Rcv decoded: " + frame.__str__())
+            if isEnabledForTrace():
+                trace(f"++Rcv raw: {repr(frame.format())}")
+                trace(f"++Rcv decoded: {frame.__str__()}")
             if not frame:
                 # handle error:
                 # 'NoneType' object has no attribute 'opcode'
-                raise WebSocketProtocolException(
-                    "Not a valid frame {frame}".format(frame=frame))
-            elif frame.opcode in (ABNF.OPCODE_TEXT, ABNF.OPCODE_BINARY, ABNF.OPCODE_CONT):
+                raise WebSocketProtocolException(f"Not a valid frame {frame}")
+            elif frame.opcode in (
+                ABNF.OPCODE_TEXT,
+                ABNF.OPCODE_BINARY,
+                ABNF.OPCODE_CONT,
+            ):
                 self.cont_frame.validate(frame)
                 self.cont_frame.add(frame)
 
                 if self.cont_frame.is_fire(frame):
                     return self.cont_frame.extract(frame)
 
             elif frame.opcode == ABNF.OPCODE_CLOSE:
                 self.send_close()
                 return frame.opcode, frame
             elif frame.opcode == ABNF.OPCODE_PING:
                 if len(frame.data) < 126:
                     self.pong(frame.data)
                 else:
-                    raise WebSocketProtocolException(
-                        "Ping message is too long")
+                    raise WebSocketProtocolException("Ping message is too long")
                 if control_frame:
                     return frame.opcode, frame
             elif frame.opcode == ABNF.OPCODE_PONG:
                 if control_frame:
                     return frame.opcode, frame
 
     def recv_frame(self):
@@ -456,60 +487,61 @@
             Status code to send. See STATUS_XXX.
         reason: str or bytes
             The reason to close. This must be string or UTF-8 bytes.
         """
         if status < 0 or status >= ABNF.LENGTH_16:
             raise ValueError("code is invalid range")
         self.connected = False
-        self.send(struct.pack('!H', status) + reason, ABNF.OPCODE_CLOSE)
+        self.send(struct.pack("!H", status) + reason, ABNF.OPCODE_CLOSE)
 
-    def close(self, status: int = STATUS_NORMAL, reason: bytes = b"", timeout: float = 3):
+    def close(self, status: int = STATUS_NORMAL, reason: bytes = b"", timeout: int = 3):
         """
         Close Websocket object
 
         Parameters
         ----------
         status: int
             Status code to send. See VALID_CLOSE_STATUS in ABNF.
         reason: bytes
             The reason to close in UTF-8.
         timeout: int or float
             Timeout until receive a close frame.
             If None, it will wait forever until receive a close frame.
         """
-        if self.connected:
-            if status < 0 or status >= ABNF.LENGTH_16:
-                raise ValueError("code is invalid range")
+        if not self.connected:
+            return
+        if status < 0 or status >= ABNF.LENGTH_16:
+            raise ValueError("code is invalid range")
 
-            try:
-                self.connected = False
-                self.send(struct.pack('!H', status) + reason, ABNF.OPCODE_CLOSE)
-                sock_timeout = self.sock.gettimeout()
-                self.sock.settimeout(timeout)
-                start_time = time.time()
-                while timeout is None or time.time() - start_time < timeout:
-                    try:
-                        frame = self.recv_frame()
-                        if frame.opcode != ABNF.OPCODE_CLOSE:
-                            continue
-                        if isEnabledForError():
-                            recv_status = struct.unpack("!H", frame.data[0:2])[0]
-                            if recv_status >= 3000 and recv_status <= 4999:
-                                debug("close status: " + repr(recv_status))
-                            elif recv_status != STATUS_NORMAL:
-                                error("close status: " + repr(recv_status))
-                        break
-                    except:
-                        break
-                self.sock.settimeout(sock_timeout)
-                self.sock.shutdown(socket.SHUT_RDWR)
-            except:
-                pass
+        try:
+            self.connected = False
+            self.send(struct.pack("!H", status) + reason, ABNF.OPCODE_CLOSE)
+            sock_timeout = self.sock.gettimeout()
+            self.sock.settimeout(timeout)
+            start_time = time.time()
+            while timeout is None or time.time() - start_time < timeout:
+                try:
+                    frame = self.recv_frame()
+                    if frame.opcode != ABNF.OPCODE_CLOSE:
+                        continue
+                    if isEnabledForError():
+                        recv_status = struct.unpack("!H", frame.data[0:2])[0]
+                        if recv_status >= 3000 and recv_status <= 4999:
+                            debug(f"close status: {repr(recv_status)}")
+                        elif recv_status != STATUS_NORMAL:
+                            error(f"close status: {repr(recv_status)}")
+                    break
+                except:
+                    break
+            self.sock.settimeout(sock_timeout)
+            self.sock.shutdown(socket.SHUT_RDWR)
+        except:
+            pass
 
-            self.shutdown()
+        self.shutdown()
 
     def abort(self):
         """
         Low-level asynchronous abort, wakes up other threads that are waiting in recv_*
         """
         if self.connected:
             self.sock.shutdown(socket.SHUT_RDWR)
@@ -598,14 +630,18 @@
         Pre-initialized stream socket.
     """
     sockopt = options.pop("sockopt", [])
     sslopt = options.pop("sslopt", {})
     fire_cont_frame = options.pop("fire_cont_frame", False)
     enable_multithread = options.pop("enable_multithread", True)
     skip_utf8_validation = options.pop("skip_utf8_validation", False)
-    websock = class_(sockopt=sockopt, sslopt=sslopt,
-                     fire_cont_frame=fire_cont_frame,
-                     enable_multithread=enable_multithread,
-                     skip_utf8_validation=skip_utf8_validation, **options)
+    websock = class_(
+        sockopt=sockopt,
+        sslopt=sslopt,
+        fire_cont_frame=fire_cont_frame,
+        enable_multithread=enable_multithread,
+        skip_utf8_validation=skip_utf8_validation,
+        **options,
+    )
     websock.settimeout(timeout if timeout is not None else getdefaulttimeout())
     websock.connect(url, **options)
     return websock
```

### Comparing `websocket-client-1.6.4/websocket/_exceptions.py` & `websocket-client-1.7.0/websocket/_exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,63 +18,77 @@
 """
 
 
 class WebSocketException(Exception):
     """
     WebSocket exception class.
     """
+
     pass
 
 
 class WebSocketProtocolException(WebSocketException):
     """
     If the WebSocket protocol is invalid, this exception will be raised.
     """
+
     pass
 
 
 class WebSocketPayloadException(WebSocketException):
     """
     If the WebSocket payload is invalid, this exception will be raised.
     """
+
     pass
 
 
 class WebSocketConnectionClosedException(WebSocketException):
     """
     If remote host closed the connection or some network error happened,
     this exception will be raised.
     """
+
     pass
 
 
 class WebSocketTimeoutException(WebSocketException):
     """
     WebSocketTimeoutException will be raised at socket timeout during read/write data.
     """
+
     pass
 
 
 class WebSocketProxyException(WebSocketException):
     """
     WebSocketProxyException will be raised when proxy error occurred.
     """
+
     pass
 
 
 class WebSocketBadStatusException(WebSocketException):
     """
     WebSocketBadStatusException will be raised when we get bad handshake status code.
     """
 
-    def __init__(self, message: str, status_code: int, status_message=None, resp_headers=None, resp_body=None):
+    def __init__(
+        self,
+        message: str,
+        status_code: int,
+        status_message=None,
+        resp_headers=None,
+        resp_body=None,
+    ):
         super().__init__(message)
         self.status_code = status_code
         self.resp_headers = resp_headers
         self.resp_body = resp_body
 
 
 class WebSocketAddressException(WebSocketException):
     """
     If the websocket address info cannot be found, this exception will be raised.
     """
+
     pass
```

### Comparing `websocket-client-1.6.4/websocket/_handshake.py` & `websocket-client-1.7.0/websocket/_handshake.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,42 +16,50 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import hashlib
 import hmac
 import os
 from base64 import encodebytes as base64encode
-from http import client as HTTPStatus
+from http import HTTPStatus
+
 from ._cookiejar import SimpleCookieJar
 from ._exceptions import *
 from ._http import *
 from ._logging import *
 from ._socket import *
 
 __all__ = ["handshake_response", "handshake", "SUPPORTED_REDIRECT_STATUSES"]
 
 # websocket supported version.
 VERSION = 13
 
-SUPPORTED_REDIRECT_STATUSES = (HTTPStatus.MOVED_PERMANENTLY, HTTPStatus.FOUND, HTTPStatus.SEE_OTHER, HTTPStatus.TEMPORARY_REDIRECT, HTTPStatus.PERMANENT_REDIRECT)
+SUPPORTED_REDIRECT_STATUSES = (
+    HTTPStatus.MOVED_PERMANENTLY,
+    HTTPStatus.FOUND,
+    HTTPStatus.SEE_OTHER,
+    HTTPStatus.TEMPORARY_REDIRECT,
+    HTTPStatus.PERMANENT_REDIRECT,
+)
 SUCCESS_STATUSES = SUPPORTED_REDIRECT_STATUSES + (HTTPStatus.SWITCHING_PROTOCOLS,)
 
 CookieJar = SimpleCookieJar()
 
 
 class handshake_response:
-
     def __init__(self, status: int, headers: dict, subprotocol):
         self.status = status
         self.headers = headers
         self.subprotocol = subprotocol
         CookieJar.add(headers.get("set-cookie"))
 
 
-def handshake(sock, url: str, hostname: str, port: int, resource: str, **options):
+def handshake(
+    sock, url: str, hostname: str, port: int, resource: str, **options
+) -> handshake_response:
     headers, key = _get_handshake_headers(resource, url, hostname, port, options)
 
     header_str = "\r\n".join(headers)
     send(sock, header_str)
     dump("request header", header_str)
 
     status, resp = _get_resp_headers(sock)
@@ -62,136 +70,133 @@
         raise WebSocketException("Invalid WebSocket Header")
 
     return handshake_response(status, resp, subproto)
 
 
 def _pack_hostname(hostname: str) -> str:
     # IPv6 address
-    if ':' in hostname:
-        return '[' + hostname + ']'
-
+    if ":" in hostname:
+        return f"[{hostname}]"
     return hostname
 
 
-def _get_handshake_headers(resource: str, url: str, host: str, port: int, options: dict):
-    headers = [
-        "GET {resource} HTTP/1.1".format(resource=resource),
-        "Upgrade: websocket"
-    ]
-    if port == 80 or port == 443:
+def _get_handshake_headers(
+    resource: str, url: str, host: str, port: int, options: dict
+) -> tuple:
+    headers = [f"GET {resource} HTTP/1.1", "Upgrade: websocket"]
+    if port in [80, 443]:
         hostport = _pack_hostname(host)
     else:
-        hostport = "{h}:{p}".format(h=_pack_hostname(host), p=port)
+        hostport = f"{_pack_hostname(host)}:{port}"
     if options.get("host"):
-        headers.append("Host: {h}".format(h=options["host"]))
+        headers.append(f'Host: {options["host"]}')
     else:
-        headers.append("Host: {hp}".format(hp=hostport))
+        headers.append(f"Host: {hostport}")
 
     # scheme indicates whether http or https is used in Origin
     # The same approach is used in parse_url of _url.py to set default port
     scheme, url = url.split(":", 1)
     if not options.get("suppress_origin"):
         if "origin" in options and options["origin"] is not None:
-            headers.append("Origin: {origin}".format(origin=options["origin"]))
+            headers.append(f'Origin: {options["origin"]}')
         elif scheme == "wss":
-            headers.append("Origin: https://{hp}".format(hp=hostport))
+            headers.append(f"Origin: https://{hostport}")
         else:
-            headers.append("Origin: http://{hp}".format(hp=hostport))
+            headers.append(f"Origin: http://{hostport}")
 
     key = _create_sec_websocket_key()
 
     # Append Sec-WebSocket-Key & Sec-WebSocket-Version if not manually specified
-    if not options.get('header') or 'Sec-WebSocket-Key' not in options['header']:
-        headers.append("Sec-WebSocket-Key: {key}".format(key=key))
+    if not options.get("header") or "Sec-WebSocket-Key" not in options["header"]:
+        headers.append(f"Sec-WebSocket-Key: {key}")
     else:
-        key = options['header']['Sec-WebSocket-Key']
+        key = options["header"]["Sec-WebSocket-Key"]
 
-    if not options.get('header') or 'Sec-WebSocket-Version' not in options['header']:
-        headers.append("Sec-WebSocket-Version: {version}".format(version=VERSION))
+    if not options.get("header") or "Sec-WebSocket-Version" not in options["header"]:
+        headers.append(f"Sec-WebSocket-Version: {VERSION}")
 
-    if not options.get('connection'):
-        headers.append('Connection: Upgrade')
+    if not options.get("connection"):
+        headers.append("Connection: Upgrade")
     else:
-        headers.append(options['connection'])
+        headers.append(options["connection"])
 
-    subprotocols = options.get("subprotocols")
-    if subprotocols:
-        headers.append("Sec-WebSocket-Protocol: {protocols}".format(protocols=",".join(subprotocols)))
+    if subprotocols := options.get("subprotocols"):
+        headers.append(f'Sec-WebSocket-Protocol: {",".join(subprotocols)}')
 
-    header = options.get("header")
-    if header:
+    if header := options.get("header"):
         if isinstance(header, dict):
-            header = [
-                ": ".join([k, v])
-                for k, v in header.items()
-                if v is not None
-            ]
+            header = [": ".join([k, v]) for k, v in header.items() if v is not None]
         headers.extend(header)
 
     server_cookie = CookieJar.get(host)
     client_cookie = options.get("cookie", None)
 
-    cookie = "; ".join(filter(None, [server_cookie, client_cookie]))
-
-    if cookie:
-        headers.append("Cookie: {cookie}".format(cookie=cookie))
+    if cookie := "; ".join(filter(None, [server_cookie, client_cookie])):
+        headers.append(f"Cookie: {cookie}")
 
     headers.extend(("", ""))
     return headers, key
 
 
 def _get_resp_headers(sock, success_statuses: tuple = SUCCESS_STATUSES) -> tuple:
     status, resp_headers, status_message = read_headers(sock)
     if status not in success_statuses:
-        content_len = resp_headers.get('content-length')
+        content_len = resp_headers.get("content-length")
         if content_len:
-            response_body = sock.recv(int(content_len))  # read the body of the HTTP error message response and include it in the exception
+            response_body = sock.recv(
+                int(content_len)
+            )  # read the body of the HTTP error message response and include it in the exception
         else:
             response_body = None
-        raise WebSocketBadStatusException("Handshake status {status} {message} -+-+- {headers} -+-+- {body}".format(status=status, message=status_message, headers=resp_headers, body=response_body), status, status_message, resp_headers, response_body)
+        raise WebSocketBadStatusException(
+            f"Handshake status {status} {status_message} -+-+- {resp_headers} -+-+- {response_body}",
+            status,
+            status_message,
+            resp_headers,
+            response_body,
+        )
     return status, resp_headers
 
 
 _HEADERS_TO_CHECK = {
     "upgrade": "websocket",
     "connection": "upgrade",
 }
 
 
-def _validate(headers, key: str, subprotocols):
+def _validate(headers, key: str, subprotocols) -> tuple:
     subproto = None
     for k, v in _HEADERS_TO_CHECK.items():
         r = headers.get(k, None)
         if not r:
             return False, None
-        r = [x.strip().lower() for x in r.split(',')]
+        r = [x.strip().lower() for x in r.split(",")]
         if v not in r:
             return False, None
 
     if subprotocols:
         subproto = headers.get("sec-websocket-protocol", None)
         if not subproto or subproto.lower() not in [s.lower() for s in subprotocols]:
-            error("Invalid subprotocol: " + str(subprotocols))
+            error(f"Invalid subprotocol: {subprotocols}")
             return False, None
         subproto = subproto.lower()
 
     result = headers.get("sec-websocket-accept", None)
     if not result:
         return False, None
     result = result.lower()
 
     if isinstance(result, str):
-        result = result.encode('utf-8')
+        result = result.encode("utf-8")
 
-    value = (key + "258EAFA5-E914-47DA-95CA-C5AB0DC85B11").encode('utf-8')
+    value = f"{key}258EAFA5-E914-47DA-95CA-C5AB0DC85B11".encode("utf-8")
     hashed = base64encode(hashlib.sha1(value).digest()).strip().lower()
-    success = hmac.compare_digest(hashed, result)
 
-    if success:
+    if hmac.compare_digest(hashed, result):
         return True, subproto
     else:
         return False, None
 
 
 def _create_sec_websocket_key() -> str:
     randomness = os.urandom(16)
-    return base64encode(randomness).decode('utf-8').strip()
+    return base64encode(randomness).decode("utf-8").strip()
```

### Comparing `websocket-client-1.6.4/websocket/_http.py` & `websocket-client-1.7.0/websocket/_http.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import errno
 import os
 import socket
+from base64 import encodebytes as base64encode
 
 from ._exceptions import *
 from ._logging import *
 from ._socket import *
 from ._ssl_compat import *
 from ._url import *
 
-from base64 import encodebytes as base64encode
-
 __all__ = ["proxy_info", "connect", "read_headers"]
 
 try:
-    from python_socks.sync import Proxy
     from python_socks._errors import *
     from python_socks._types import ProxyType
+    from python_socks.sync import Proxy
+
     HAVE_PYTHON_SOCKS = True
 except:
     HAVE_PYTHON_SOCKS = False
 
     class ProxyError(Exception):
         pass
 
@@ -45,88 +45,100 @@
         pass
 
     class ProxyConnectionError(Exception):
         pass
 
 
 class proxy_info:
-
     def __init__(self, **options):
         self.proxy_host = options.get("http_proxy_host", None)
         if self.proxy_host:
             self.proxy_port = options.get("http_proxy_port", 0)
             self.auth = options.get("http_proxy_auth", None)
             self.no_proxy = options.get("http_no_proxy", None)
             self.proxy_protocol = options.get("proxy_type", "http")
             # Note: If timeout not specified, default python-socks timeout is 60 seconds
             self.proxy_timeout = options.get("http_proxy_timeout", None)
-            if self.proxy_protocol not in ['http', 'socks4', 'socks4a', 'socks5', 'socks5h']:
-                raise ProxyError("Only http, socks4, socks5 proxy protocols are supported")
+            if self.proxy_protocol not in [
+                "http",
+                "socks4",
+                "socks4a",
+                "socks5",
+                "socks5h",
+            ]:
+                raise ProxyError(
+                    "Only http, socks4, socks5 proxy protocols are supported"
+                )
         else:
             self.proxy_port = 0
             self.auth = None
             self.no_proxy = None
             self.proxy_protocol = "http"
 
 
-def _start_proxied_socket(url: str, options, proxy):
+def _start_proxied_socket(url: str, options, proxy) -> tuple:
     if not HAVE_PYTHON_SOCKS:
-        raise WebSocketException("Python Socks is needed for SOCKS proxying but is not available")
+        raise WebSocketException(
+            "Python Socks is needed for SOCKS proxying but is not available"
+        )
 
     hostname, port, resource, is_secure = parse_url(url)
 
-    if proxy.proxy_protocol == "socks5":
-        rdns = False
-        proxy_type = ProxyType.SOCKS5
     if proxy.proxy_protocol == "socks4":
         rdns = False
         proxy_type = ProxyType.SOCKS4
-    # socks5h and socks4a send DNS through proxy
-    if proxy.proxy_protocol == "socks5h":
+    # socks4a sends DNS through proxy
+    elif proxy.proxy_protocol == "socks4a":
         rdns = True
+        proxy_type = ProxyType.SOCKS4
+    elif proxy.proxy_protocol == "socks5":
+        rdns = False
         proxy_type = ProxyType.SOCKS5
-    if proxy.proxy_protocol == "socks4a":
+    # socks5h sends DNS through proxy
+    elif proxy.proxy_protocol == "socks5h":
         rdns = True
-        proxy_type = ProxyType.SOCKS4
+        proxy_type = ProxyType.SOCKS5
 
     ws_proxy = Proxy.create(
         proxy_type=proxy_type,
         host=proxy.proxy_host,
         port=int(proxy.proxy_port),
         username=proxy.auth[0] if proxy.auth else None,
         password=proxy.auth[1] if proxy.auth else None,
-        rdns=rdns)
+        rdns=rdns,
+    )
 
     sock = ws_proxy.connect(hostname, port, timeout=proxy.proxy_timeout)
 
-    if is_secure and HAVE_SSL:
-        sock = _ssl_socket(sock, options.sslopt, hostname)
-    elif is_secure:
-        raise WebSocketException("SSL not available.")
+    if is_secure:
+        if HAVE_SSL:
+            sock = _ssl_socket(sock, options.sslopt, hostname)
+        else:
+            raise WebSocketException("SSL not available.")
 
     return sock, (hostname, port, resource)
 
 
 def connect(url: str, options, proxy, socket):
     # Use _start_proxied_socket() only for socks4 or socks5 proxy
     # Use _tunnel() for http proxy
     # TODO: Use python-socks for http protocol also, to standardize flow
-    if proxy.proxy_host and not socket and not (proxy.proxy_protocol == "http"):
+    if proxy.proxy_host and not socket and proxy.proxy_protocol != "http":
         return _start_proxied_socket(url, options, proxy)
 
     hostname, port_from_url, resource, is_secure = parse_url(url)
 
     if socket:
         return socket, (hostname, port_from_url, resource)
 
     addrinfo_list, need_tunnel, auth = _get_addrinfo_list(
-        hostname, port_from_url, is_secure, proxy)
+        hostname, port_from_url, is_secure, proxy
+    )
     if not addrinfo_list:
-        raise WebSocketException(
-            "Host not found.: " + hostname + ":" + str(port_from_url))
+        raise WebSocketException(f"Host not found.: {hostname}:{port_from_url}")
 
     sock = None
     try:
         sock = _open_socket(addrinfo_list, options.sockopt, options.timeout)
         if need_tunnel:
             sock = _tunnel(sock, hostname, port_from_url, auth)
 
@@ -139,32 +151,41 @@
         return sock, (hostname, port_from_url, resource)
     except:
         if sock:
             sock.close()
         raise
 
 
-def _get_addrinfo_list(hostname, port, is_secure, proxy):
+def _get_addrinfo_list(hostname, port: int, is_secure: bool, proxy) -> tuple:
     phost, pport, pauth = get_proxy_info(
-        hostname, is_secure, proxy.proxy_host, proxy.proxy_port, proxy.auth, proxy.no_proxy)
+        hostname,
+        is_secure,
+        proxy.proxy_host,
+        proxy.proxy_port,
+        proxy.auth,
+        proxy.no_proxy,
+    )
     try:
         # when running on windows 10, getaddrinfo without socktype returns a socktype 0.
         # This generates an error exception: `_on_error: exception Socket type must be stream or datagram, not 0`
         # or `OSError: [Errno 22] Invalid argument` when creating socket. Force the socket type to SOCK_STREAM.
         if not phost:
             addrinfo_list = socket.getaddrinfo(
-                hostname, port, 0, socket.SOCK_STREAM, socket.SOL_TCP)
+                hostname, port, 0, socket.SOCK_STREAM, socket.SOL_TCP
+            )
             return addrinfo_list, False, None
         else:
             pport = pport and pport or 80
             # when running on windows 10, the getaddrinfo used above
             # returns a socktype 0. This generates an error exception:
             # _on_error: exception Socket type must be stream or datagram, not 0
             # Force the socket type to SOCK_STREAM
-            addrinfo_list = socket.getaddrinfo(phost, pport, 0, socket.SOCK_STREAM, socket.SOL_TCP)
+            addrinfo_list = socket.getaddrinfo(
+                phost, pport, 0, socket.SOCK_STREAM, socket.SOL_TCP
+            )
             return addrinfo_list, True, pauth
     except socket.gaierror as e:
         raise WebSocketAddressException(e)
 
 
 def _open_socket(addrinfo_list, sockopt, timeout):
     err = None
@@ -182,159 +203,167 @@
         while not err:
             try:
                 sock.connect(address)
             except socket.error as error:
                 sock.close()
                 error.remote_ip = str(address[0])
                 try:
-                    eConnRefused = (errno.ECONNREFUSED, errno.WSAECONNREFUSED, errno.ENETUNREACH)
+                    eConnRefused = (
+                        errno.ECONNREFUSED,
+                        errno.WSAECONNREFUSED,
+                        errno.ENETUNREACH,
+                    )
                 except AttributeError:
                     eConnRefused = (errno.ECONNREFUSED, errno.ENETUNREACH)
-                if error.errno in eConnRefused:
-                    err = error
-                    continue
-                else:
+                if error.errno not in eConnRefused:
                     raise error
+                err = error
+                continue
             else:
                 break
         else:
             continue
         break
     else:
         if err:
             raise err
 
     return sock
 
 
-def _wrap_sni_socket(sock, sslopt, hostname, check_hostname):
-    context = sslopt.get('context', None)
+def _wrap_sni_socket(sock: socket.socket, sslopt: dict, hostname, check_hostname):
+    context = sslopt.get("context", None)
     if not context:
-        context = ssl.SSLContext(sslopt.get('ssl_version', ssl.PROTOCOL_TLS_CLIENT))
+        context = ssl.SSLContext(sslopt.get("ssl_version", ssl.PROTOCOL_TLS_CLIENT))
         # Non default context need to manually enable SSLKEYLOGFILE support by setting the keylog_filename attribute.
         # For more details see also:
         # * https://docs.python.org/3.8/library/ssl.html?highlight=sslkeylogfile#context-creation
         # * https://docs.python.org/3.8/library/ssl.html?highlight=sslkeylogfile#ssl.SSLContext.keylog_filename
         context.keylog_filename = os.environ.get("SSLKEYLOGFILE", None)
 
-        if sslopt.get('cert_reqs', ssl.CERT_NONE) != ssl.CERT_NONE:
-            cafile = sslopt.get('ca_certs', None)
-            capath = sslopt.get('ca_cert_path', None)
+        if sslopt.get("cert_reqs", ssl.CERT_NONE) != ssl.CERT_NONE:
+            cafile = sslopt.get("ca_certs", None)
+            capath = sslopt.get("ca_cert_path", None)
             if cafile or capath:
                 context.load_verify_locations(cafile=cafile, capath=capath)
-            elif hasattr(context, 'load_default_certs'):
+            elif hasattr(context, "load_default_certs"):
                 context.load_default_certs(ssl.Purpose.SERVER_AUTH)
-        if sslopt.get('certfile', None):
+        if sslopt.get("certfile", None):
             context.load_cert_chain(
-                sslopt['certfile'],
-                sslopt.get('keyfile', None),
-                sslopt.get('password', None),
+                sslopt["certfile"],
+                sslopt.get("keyfile", None),
+                sslopt.get("password", None),
             )
 
         # Python 3.10 switch to PROTOCOL_TLS_CLIENT defaults to "cert_reqs = ssl.CERT_REQUIRED" and "check_hostname = True"
         # If both disabled, set check_hostname before verify_mode
         # see https://github.com/liris/websocket-client/commit/b96a2e8fa765753e82eea531adb19716b52ca3ca#commitcomment-10803153
-        if sslopt.get('cert_reqs', ssl.CERT_NONE) == ssl.CERT_NONE and not sslopt.get('check_hostname', False):
+        if sslopt.get("cert_reqs", ssl.CERT_NONE) == ssl.CERT_NONE and not sslopt.get(
+            "check_hostname", False
+        ):
             context.check_hostname = False
             context.verify_mode = ssl.CERT_NONE
         else:
-            context.check_hostname = sslopt.get('check_hostname', True)
-            context.verify_mode = sslopt.get('cert_reqs', ssl.CERT_REQUIRED)
+            context.check_hostname = sslopt.get("check_hostname", True)
+            context.verify_mode = sslopt.get("cert_reqs", ssl.CERT_REQUIRED)
 
-        if 'ciphers' in sslopt:
-            context.set_ciphers(sslopt['ciphers'])
-        if 'cert_chain' in sslopt:
-            certfile, keyfile, password = sslopt['cert_chain']
+        if "ciphers" in sslopt:
+            context.set_ciphers(sslopt["ciphers"])
+        if "cert_chain" in sslopt:
+            certfile, keyfile, password = sslopt["cert_chain"]
             context.load_cert_chain(certfile, keyfile, password)
-        if 'ecdh_curve' in sslopt:
-            context.set_ecdh_curve(sslopt['ecdh_curve'])
+        if "ecdh_curve" in sslopt:
+            context.set_ecdh_curve(sslopt["ecdh_curve"])
 
     return context.wrap_socket(
         sock,
-        do_handshake_on_connect=sslopt.get('do_handshake_on_connect', True),
-        suppress_ragged_eofs=sslopt.get('suppress_ragged_eofs', True),
+        do_handshake_on_connect=sslopt.get("do_handshake_on_connect", True),
+        suppress_ragged_eofs=sslopt.get("suppress_ragged_eofs", True),
         server_hostname=hostname,
     )
 
 
-def _ssl_socket(sock, user_sslopt, hostname):
-    sslopt = dict(cert_reqs=ssl.CERT_REQUIRED)
+def _ssl_socket(sock: socket.socket, user_sslopt: dict, hostname):
+    sslopt: dict = dict(cert_reqs=ssl.CERT_REQUIRED)
     sslopt.update(user_sslopt)
 
-    certPath = os.environ.get('WEBSOCKET_CLIENT_CA_BUNDLE')
-    if certPath and os.path.isfile(certPath) \
-            and user_sslopt.get('ca_certs', None) is None:
-        sslopt['ca_certs'] = certPath
-    elif certPath and os.path.isdir(certPath) \
-            and user_sslopt.get('ca_cert_path', None) is None:
-        sslopt['ca_cert_path'] = certPath
+    certPath = os.environ.get("WEBSOCKET_CLIENT_CA_BUNDLE")
+    if (
+        certPath
+        and os.path.isfile(certPath)
+        and user_sslopt.get("ca_certs", None) is None
+    ):
+        sslopt["ca_certs"] = certPath
+    elif (
+        certPath
+        and os.path.isdir(certPath)
+        and user_sslopt.get("ca_cert_path", None) is None
+    ):
+        sslopt["ca_cert_path"] = certPath
 
-    if sslopt.get('server_hostname', None):
-        hostname = sslopt['server_hostname']
+    if sslopt.get("server_hostname", None):
+        hostname = sslopt["server_hostname"]
 
-    check_hostname = sslopt.get('check_hostname', True)
+    check_hostname = sslopt.get("check_hostname", True)
     sock = _wrap_sni_socket(sock, sslopt, hostname, check_hostname)
 
     return sock
 
 
-def _tunnel(sock, host, port, auth):
+def _tunnel(sock: socket.socket, host, port: int, auth) -> socket.socket:
     debug("Connecting proxy...")
-    connect_header = "CONNECT {h}:{p} HTTP/1.1\r\n".format(h=host, p=port)
-    connect_header += "Host: {h}:{p}\r\n".format(h=host, p=port)
+    connect_header = f"CONNECT {host}:{port} HTTP/1.1\r\n"
+    connect_header += f"Host: {host}:{port}\r\n"
 
     # TODO: support digest auth.
     if auth and auth[0]:
         auth_str = auth[0]
         if auth[1]:
-            auth_str += ":" + auth[1]
-        encoded_str = base64encode(auth_str.encode()).strip().decode().replace('\n', '')
-        connect_header += "Proxy-Authorization: Basic {str}\r\n".format(str=encoded_str)
+            auth_str += f":{auth[1]}"
+        encoded_str = base64encode(auth_str.encode()).strip().decode().replace("\n", "")
+        connect_header += f"Proxy-Authorization: Basic {encoded_str}\r\n"
     connect_header += "\r\n"
     dump("request header", connect_header)
 
     send(sock, connect_header)
 
     try:
         status, resp_headers, status_message = read_headers(sock)
     except Exception as e:
         raise WebSocketProxyException(str(e))
 
     if status != 200:
-        raise WebSocketProxyException(
-            "failed CONNECT via proxy status: {status}".format(status=status))
+        raise WebSocketProxyException(f"failed CONNECT via proxy status: {status}")
 
     return sock
 
 
-def read_headers(sock):
+def read_headers(sock: socket.socket) -> tuple:
     status = None
     status_message = None
-    headers = {}
+    headers: dict = {}
     trace("--- response header ---")
 
     while True:
         line = recv_line(sock)
-        line = line.decode('utf-8').strip()
+        line = line.decode("utf-8").strip()
         if not line:
             break
         trace(line)
         if not status:
-
             status_info = line.split(" ", 2)
             status = int(status_info[1])
             if len(status_info) > 2:
                 status_message = status_info[2]
         else:
             kv = line.split(":", 1)
-            if len(kv) == 2:
-                key, value = kv
-                if key.lower() == "set-cookie" and headers.get("set-cookie"):
-                    headers["set-cookie"] = headers.get("set-cookie") + "; " + value.strip()
-                else:
-                    headers[key.lower()] = value.strip()
-            else:
+            if len(kv) != 2:
                 raise WebSocketException("Invalid header")
+            key, value = kv
+            if key.lower() == "set-cookie" and headers.get("set-cookie"):
+                headers["set-cookie"] = headers.get("set-cookie") + "; " + value.strip()
+            else:
+                headers[key.lower()] = value.strip()
 
     trace("-----------------------")
 
     return status, headers, status_message
```

### Comparing `websocket-client-1.6.4/websocket/_logging.py` & `websocket-client-1.7.0/websocket/_logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,33 +15,46 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-_logger = logging.getLogger('websocket')
+_logger = logging.getLogger("websocket")
 try:
     from logging import NullHandler
 except ImportError:
+
     class NullHandler(logging.Handler):
         def emit(self, record) -> None:
             pass
 
+
 _logger.addHandler(NullHandler())
 
 _traceEnabled = False
 
-__all__ = ["enableTrace", "dump", "error", "warning", "debug", "trace",
-           "isEnabledForError", "isEnabledForDebug", "isEnabledForTrace"]
-
-
-def enableTrace(traceable: bool,
-                handler: logging.StreamHandler = logging.StreamHandler(),
-                level: str = "DEBUG") -> None:
+__all__ = [
+    "enableTrace",
+    "dump",
+    "error",
+    "warning",
+    "debug",
+    "trace",
+    "isEnabledForError",
+    "isEnabledForDebug",
+    "isEnabledForTrace",
+]
+
+
+def enableTrace(
+    traceable: bool,
+    handler: logging.StreamHandler = logging.StreamHandler(),
+    level: str = "DEBUG",
+) -> None:
     """
     Turn on/off the traceability.
 
     Parameters
     ----------
     traceable: bool
         If set to True, traceability is enabled.
@@ -51,15 +64,15 @@
     if traceable:
         _logger.addHandler(handler)
         _logger.setLevel(getattr(logging, level))
 
 
 def dump(title: str, message: str) -> None:
     if _traceEnabled:
-        _logger.debug("--- " + title + " ---")
+        _logger.debug(f"--- {title} ---")
         _logger.debug(message)
         _logger.debug("-----------------------")
 
 
 def error(msg: str) -> None:
     _logger.error(msg)
```

### Comparing `websocket-client-1.6.4/websocket/_socket.py` & `websocket-client-1.7.0/websocket/_socket.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import errno
 import selectors
 import socket
-
 from typing import Union
 
 from ._exceptions import *
 from ._ssl_compat import *
 from ._utils import *
 
 """
@@ -35,20 +34,26 @@
 if hasattr(socket, "TCP_KEEPINTVL"):
     DEFAULT_SOCKET_OPTION.append((socket.SOL_TCP, socket.TCP_KEEPINTVL, 10))
 if hasattr(socket, "TCP_KEEPCNT"):
     DEFAULT_SOCKET_OPTION.append((socket.SOL_TCP, socket.TCP_KEEPCNT, 3))
 
 _default_timeout = None
 
-__all__ = ["DEFAULT_SOCKET_OPTION", "sock_opt", "setdefaulttimeout", "getdefaulttimeout",
-           "recv", "recv_line", "send"]
+__all__ = [
+    "DEFAULT_SOCKET_OPTION",
+    "sock_opt",
+    "setdefaulttimeout",
+    "getdefaulttimeout",
+    "recv",
+    "recv_line",
+    "send",
+]
 
 
 class sock_opt:
-
     def __init__(self, sockopt: list, sslopt: dict) -> None:
         if sockopt is None:
             sockopt = []
         if sslopt is None:
             sslopt = {}
         self.sockopt = sockopt
         self.sslopt = sslopt
@@ -87,15 +92,15 @@
     def _recv():
         try:
             return sock.recv(bufsize)
         except SSLWantReadError:
             pass
         except socket.error as exc:
             error_code = extract_error_code(exc)
-            if error_code != errno.EAGAIN and error_code != errno.EWOULDBLOCK:
+            if error_code not in [errno.EAGAIN, errno.EWOULDBLOCK]:
                 raise
 
         sel = selectors.DefaultSelector()
         sel.register(sock, selectors.EVENT_READ)
 
         r = sel.select(sock.gettimeout())
         sel.close()
@@ -111,53 +116,52 @@
     except TimeoutError:
         raise WebSocketTimeoutException("Connection timed out")
     except socket.timeout as e:
         message = extract_err_message(e)
         raise WebSocketTimeoutException(message)
     except SSLError as e:
         message = extract_err_message(e)
-        if isinstance(message, str) and 'timed out' in message:
+        if isinstance(message, str) and "timed out" in message:
             raise WebSocketTimeoutException(message)
         else:
             raise
 
     if not bytes_:
-        raise WebSocketConnectionClosedException(
-            "Connection to remote host was lost.")
+        raise WebSocketConnectionClosedException("Connection to remote host was lost.")
 
     return bytes_
 
 
 def recv_line(sock: socket.socket) -> bytes:
     line = []
     while True:
         c = recv(sock, 1)
         line.append(c)
-        if c == b'\n':
+        if c == b"\n":
             break
-    return b''.join(line)
+    return b"".join(line)
 
 
 def send(sock: socket.socket, data: Union[bytes, str]) -> int:
     if isinstance(data, str):
-        data = data.encode('utf-8')
+        data = data.encode("utf-8")
 
     if not sock:
         raise WebSocketConnectionClosedException("socket is already closed.")
 
     def _send():
         try:
             return sock.send(data)
         except SSLWantWriteError:
             pass
         except socket.error as exc:
             error_code = extract_error_code(exc)
             if error_code is None:
                 raise
-            if error_code != errno.EAGAIN and error_code != errno.EWOULDBLOCK:
+            if error_code not in [errno.EAGAIN, errno.EWOULDBLOCK]:
                 raise
 
         sel = selectors.DefaultSelector()
         sel.register(sock, selectors.EVENT_WRITE)
 
         w = sel.select(sock.gettimeout())
         sel.close()
```

### Comparing `websocket-client-1.6.4/websocket/_ssl_compat.py` & `websocket-client-1.7.0/websocket/_ssl_compat.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,17 +16,16 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 __all__ = ["HAVE_SSL", "ssl", "SSLError", "SSLWantReadError", "SSLWantWriteError"]
 
 try:
     import ssl
-    from ssl import SSLError
-    from ssl import SSLWantReadError
-    from ssl import SSLWantWriteError
+    from ssl import SSLError, SSLWantReadError, SSLWantWriteError
+
     HAVE_SSL = True
 except ImportError:
     # dummy class of SSLError for environment without ssl support
     class SSLError(Exception):
         pass
 
     class SSLWantReadError(Exception):
```

### Comparing `websocket-client-1.6.4/websocket/_url.py` & `websocket-client-1.7.0/websocket/_url.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import socket
 import struct
-
 from typing import Optional
 from urllib.parse import unquote, urlparse
 
 """
 _url.py
 websocket - WebSocket client library for Python
 
@@ -64,15 +63,15 @@
 
     if parsed.path:
         resource = parsed.path
     else:
         resource = "/"
 
     if parsed.query:
-        resource += "?" + parsed.query
+        resource += f"?{parsed.query}"
 
     return hostname, port, resource, is_secure
 
 
 DEFAULT_NO_PROXY_HOST = ["localhost", "127.0.0.1"]
 
 
@@ -90,45 +89,58 @@
         addr, netmask = hostname.split("/")
         return _is_ip_address(addr) and 0 <= int(netmask) < 32
     except ValueError:
         return False
 
 
 def _is_address_in_network(ip: str, net: str) -> bool:
-    ipaddr = struct.unpack('!I', socket.inet_aton(ip))[0]
-    netaddr, netmask = net.split('/')
-    netaddr = struct.unpack('!I', socket.inet_aton(netaddr))[0]
+    ipaddr: int = struct.unpack("!I", socket.inet_aton(ip))[0]
+    netaddr, netmask = net.split("/")
+    netaddr: int = struct.unpack("!I", socket.inet_aton(netaddr))[0]
 
     netmask = (0xFFFFFFFF << (32 - int(netmask))) & 0xFFFFFFFF
     return ipaddr & netmask == netaddr
 
 
 def _is_no_proxy_host(hostname: str, no_proxy: Optional[list]) -> bool:
     if not no_proxy:
-        v = os.environ.get("no_proxy", os.environ.get("NO_PROXY", "")).replace(" ", "")
-        if v:
+        if v := os.environ.get("no_proxy", os.environ.get("NO_PROXY", "")).replace(
+            " ", ""
+        ):
             no_proxy = v.split(",")
     if not no_proxy:
         no_proxy = DEFAULT_NO_PROXY_HOST
 
-    if '*' in no_proxy:
+    if "*" in no_proxy:
         return True
     if hostname in no_proxy:
         return True
     if _is_ip_address(hostname):
-        return any([_is_address_in_network(hostname, subnet) for subnet in no_proxy if _is_subnet_address(subnet)])
-    for domain in [domain for domain in no_proxy if domain.startswith('.')]:
+        return any(
+            [
+                _is_address_in_network(hostname, subnet)
+                for subnet in no_proxy
+                if _is_subnet_address(subnet)
+            ]
+        )
+    for domain in [domain for domain in no_proxy if domain.startswith(".")]:
         if hostname.endswith(domain):
             return True
     return False
 
 
 def get_proxy_info(
-        hostname: str, is_secure: bool, proxy_host: Optional[str] = None, proxy_port: int = 0, proxy_auth: Optional[tuple] = None,
-        no_proxy: Optional[list] = None, proxy_type: str = 'http') -> tuple:
+    hostname: str,
+    is_secure: bool,
+    proxy_host: Optional[str] = None,
+    proxy_port: int = 0,
+    proxy_auth: Optional[tuple] = None,
+    no_proxy: Optional[list] = None,
+    proxy_type: str = "http",
+) -> tuple:
     """
     Try to retrieve proxy host and port from environment
     if not provided in options.
     Result is (proxy_host, proxy_port, proxy_auth).
     proxy_auth is tuple of username and password
     of proxy authentication information.
 
@@ -156,14 +168,20 @@
 
     if proxy_host:
         port = proxy_port
         auth = proxy_auth
         return proxy_host, port, auth
 
     env_key = "https_proxy" if is_secure else "http_proxy"
-    value = os.environ.get(env_key, os.environ.get(env_key.upper(), "")).replace(" ", "")
+    value = os.environ.get(env_key, os.environ.get(env_key.upper(), "")).replace(
+        " ", ""
+    )
     if value:
         proxy = urlparse(value)
-        auth = (unquote(proxy.username), unquote(proxy.password)) if proxy.username else None
+        auth = (
+            (unquote(proxy.username), unquote(proxy.password))
+            if proxy.username
+            else None
+        )
         return proxy.hostname, proxy.port, auth
 
     return None, 0, None
```

### Comparing `websocket-client-1.6.4/websocket/_wsdump.py` & `websocket-client-1.7.0/websocket/_wsdump.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import argparse
 import code
+import gzip
+import ssl
 import sys
 import threading
 import time
-import ssl
-import gzip
 import zlib
 from urllib.parse import urlparse
 
 import websocket
 
 try:
     import readline
@@ -46,83 +46,92 @@
 
 
 OPCODE_DATA = (websocket.ABNF.OPCODE_TEXT, websocket.ABNF.OPCODE_BINARY)
 ENCODING = get_encoding()
 
 
 class VAction(argparse.Action):
-
-    def __call__(self, parser: argparse.Namespace, args: tuple, values: str, option_string: str = None) -> None:
+    def __call__(
+        self,
+        parser: argparse.Namespace,
+        args: tuple,
+        values: str,
+        option_string: str = None,
+    ) -> None:
         if values is None:
             values = "1"
         try:
             values = int(values)
         except ValueError:
             values = values.count("v") + 1
         setattr(args, self.dest, values)
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(description="WebSocket Simple Dump Tool")
-    parser.add_argument("url", metavar="ws_url",
-                        help="websocket url. ex. ws://echo.websocket.events/")
-    parser.add_argument("-p", "--proxy",
-                        help="proxy url. ex. http://127.0.0.1:8080")
-    parser.add_argument("-v", "--verbose", default=0, nargs='?', action=VAction,
-                        dest="verbose",
-                        help="set verbose mode. If set to 1, show opcode. "
-                        "If set to 2, enable to trace  websocket module")
-    parser.add_argument("-n", "--nocert", action='store_true',
-                        help="Ignore invalid SSL cert")
-    parser.add_argument("-r", "--raw", action="store_true",
-                        help="raw output")
-    parser.add_argument("-s", "--subprotocols", nargs='*',
-                        help="Set subprotocols")
-    parser.add_argument("-o", "--origin",
-                        help="Set origin")
-    parser.add_argument("--eof-wait", default=0, type=int,
-                        help="wait time(second) after 'EOF' received.")
-    parser.add_argument("-t", "--text",
-                        help="Send initial text")
-    parser.add_argument("--timings", action="store_true",
-                        help="Print timings in seconds")
-    parser.add_argument("--headers",
-                        help="Set custom headers. Use ',' as separator")
+    parser.add_argument(
+        "url", metavar="ws_url", help="websocket url. ex. ws://echo.websocket.events/"
+    )
+    parser.add_argument("-p", "--proxy", help="proxy url. ex. http://127.0.0.1:8080")
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        default=0,
+        nargs="?",
+        action=VAction,
+        dest="verbose",
+        help="set verbose mode. If set to 1, show opcode. "
+        "If set to 2, enable to trace  websocket module",
+    )
+    parser.add_argument(
+        "-n", "--nocert", action="store_true", help="Ignore invalid SSL cert"
+    )
+    parser.add_argument("-r", "--raw", action="store_true", help="raw output")
+    parser.add_argument("-s", "--subprotocols", nargs="*", help="Set subprotocols")
+    parser.add_argument("-o", "--origin", help="Set origin")
+    parser.add_argument(
+        "--eof-wait",
+        default=0,
+        type=int,
+        help="wait time(second) after 'EOF' received.",
+    )
+    parser.add_argument("-t", "--text", help="Send initial text")
+    parser.add_argument(
+        "--timings", action="store_true", help="Print timings in seconds"
+    )
+    parser.add_argument("--headers", help="Set custom headers. Use ',' as separator")
 
     return parser.parse_args()
 
 
 class RawInput:
-
     def raw_input(self, prompt: str = "") -> str:
         line = input(prompt)
 
         if ENCODING and ENCODING != "utf-8" and not isinstance(line, str):
             line = line.decode(ENCODING).encode("utf-8")
         elif isinstance(line, str):
             line = line.encode("utf-8")
 
         return line
 
 
 class InteractiveConsole(RawInput, code.InteractiveConsole):
-
     def write(self, data: str) -> None:
         sys.stdout.write("\033[2K\033[E")
         # sys.stdout.write("\n")
         sys.stdout.write("\033[34m< " + data + "\033[39m")
         sys.stdout.write("\n> ")
         sys.stdout.flush()
 
     def read(self) -> str:
         return self.raw_input("> ")
 
 
 class NonInteractive(RawInput):
-
     def write(self, data: str) -> None:
         sys.stdout.write(data)
         sys.stdout.write("\n")
         sys.stdout.flush()
 
     def read(self) -> str:
         return self.raw_input("")
@@ -142,29 +151,29 @@
         options["origin"] = args.origin
     if args.subprotocols:
         options["subprotocols"] = args.subprotocols
     opts = {}
     if args.nocert:
         opts = {"cert_reqs": ssl.CERT_NONE, "check_hostname": False}
     if args.headers:
-        options['header'] = list(map(str.strip, args.headers.split(',')))
+        options["header"] = list(map(str.strip, args.headers.split(",")))
     ws = websocket.create_connection(args.url, sslopt=opts, **options)
     if args.raw:
         console = NonInteractive()
     else:
         console = InteractiveConsole()
         print("Press Ctrl+C to quit")
 
     def recv() -> tuple:
         try:
             frame = ws.recv_frame()
         except websocket.WebSocketException:
             return websocket.ABNF.OPCODE_CLOSE, ""
         if not frame:
-            raise websocket.WebSocketException("Not a valid frame {frame}".format(frame=frame))
+            raise websocket.WebSocketException(f"Not a valid frame {frame}")
         elif frame.opcode in OPCODE_DATA:
             return frame.opcode, frame.data
         elif frame.opcode == websocket.ABNF.OPCODE_CLOSE:
             ws.send_close()
             return frame.opcode, ""
         elif frame.opcode == websocket.ABNF.OPCODE_PING:
             ws.pong(frame.data)
@@ -174,36 +183,40 @@
 
     def recv_ws() -> None:
         while True:
             opcode, data = recv()
             msg = None
             if opcode == websocket.ABNF.OPCODE_TEXT and isinstance(data, bytes):
                 data = str(data, "utf-8")
-            if isinstance(data, bytes) and len(data) > 2 and data[:2] == b'\037\213':  # gzip magick
+            if (
+                isinstance(data, bytes) and len(data) > 2 and data[:2] == b"\037\213"
+            ):  # gzip magick
                 try:
                     data = "[gzip] " + str(gzip.decompress(data), "utf-8")
                 except:
                     pass
             elif isinstance(data, bytes):
                 try:
-                    data = "[zlib] " + str(zlib.decompress(data, -zlib.MAX_WBITS), "utf-8")
+                    data = "[zlib] " + str(
+                        zlib.decompress(data, -zlib.MAX_WBITS), "utf-8"
+                    )
                 except:
                     pass
 
             if isinstance(data, bytes):
                 data = repr(data)
 
             if args.verbose:
-                msg = "{opcode}: {data}".format(opcode=websocket.ABNF.OPCODE_MAP.get(opcode), data=data)
+                msg = f"{websocket.ABNF.OPCODE_MAP.get(opcode)}: {data}"
             else:
                 msg = data
 
             if msg is not None:
                 if args.timings:
-                    console.write(str(time.time() - start_time) + ": " + msg)
+                    console.write(f"{time.time() - start_time}: {msg}")
                 else:
                     console.write(msg)
 
             if opcode == websocket.ABNF.OPCODE_CLOSE:
                 break
 
     thread = threading.Thread(target=recv_ws)
```

### Comparing `websocket-client-1.6.4/websocket/tests/test_abnf.py` & `websocket-client-1.7.0/websocket/tests/test_abnf.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 #
+import unittest
+
 import websocket as ws
 from websocket._abnf import *
-import unittest
 
 """
 test_abnf.py
 websocket - WebSocket client library for Python
 
 Copyright 2023 engn33r
 
@@ -21,69 +22,104 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 
 class ABNFTest(unittest.TestCase):
-
     def testInit(self):
-        a = ABNF(0,0,0,0, opcode=ABNF.OPCODE_PING)
+        a = ABNF(0, 0, 0, 0, opcode=ABNF.OPCODE_PING)
         self.assertEqual(a.fin, 0)
         self.assertEqual(a.rsv1, 0)
         self.assertEqual(a.rsv2, 0)
         self.assertEqual(a.rsv3, 0)
         self.assertEqual(a.opcode, 9)
-        self.assertEqual(a.data, '')
-        a_bad = ABNF(0,1,0,0, opcode=77)
+        self.assertEqual(a.data, "")
+        a_bad = ABNF(0, 1, 0, 0, opcode=77)
         self.assertEqual(a_bad.rsv1, 1)
         self.assertEqual(a_bad.opcode, 77)
 
     def testValidate(self):
-        a_invalid_ping = ABNF(0,0,0,0, opcode=ABNF.OPCODE_PING)
-        self.assertRaises(ws._exceptions.WebSocketProtocolException, a_invalid_ping.validate, skip_utf8_validation=False)
-        a_bad_rsv_value = ABNF(0,1,0,0, opcode=ABNF.OPCODE_TEXT)
-        self.assertRaises(ws._exceptions.WebSocketProtocolException, a_bad_rsv_value.validate, skip_utf8_validation=False)
-        a_bad_opcode = ABNF(0,0,0,0, opcode=77)
-        self.assertRaises(ws._exceptions.WebSocketProtocolException, a_bad_opcode.validate, skip_utf8_validation=False)
-        a_bad_close_frame = ABNF(0,0,0,0, opcode=ABNF.OPCODE_CLOSE, data=b'\x01')
-        self.assertRaises(ws._exceptions.WebSocketProtocolException, a_bad_close_frame.validate, skip_utf8_validation=False)
-        a_bad_close_frame_2 = ABNF(0,0,0,0, opcode=ABNF.OPCODE_CLOSE, data=b'\x01\x8a\xaa\xff\xdd')
-        self.assertRaises(ws._exceptions.WebSocketProtocolException, a_bad_close_frame_2.validate, skip_utf8_validation=False)
-        a_bad_close_frame_3 = ABNF(0,0,0,0, opcode=ABNF.OPCODE_CLOSE, data=b'\x03\xe7')
-        self.assertRaises(ws._exceptions.WebSocketProtocolException, a_bad_close_frame_3.validate, skip_utf8_validation=True)
+        a_invalid_ping = ABNF(0, 0, 0, 0, opcode=ABNF.OPCODE_PING)
+        self.assertRaises(
+            ws._exceptions.WebSocketProtocolException,
+            a_invalid_ping.validate,
+            skip_utf8_validation=False,
+        )
+        a_bad_rsv_value = ABNF(0, 1, 0, 0, opcode=ABNF.OPCODE_TEXT)
+        self.assertRaises(
+            ws._exceptions.WebSocketProtocolException,
+            a_bad_rsv_value.validate,
+            skip_utf8_validation=False,
+        )
+        a_bad_opcode = ABNF(0, 0, 0, 0, opcode=77)
+        self.assertRaises(
+            ws._exceptions.WebSocketProtocolException,
+            a_bad_opcode.validate,
+            skip_utf8_validation=False,
+        )
+        a_bad_close_frame = ABNF(0, 0, 0, 0, opcode=ABNF.OPCODE_CLOSE, data=b"\x01")
+        self.assertRaises(
+            ws._exceptions.WebSocketProtocolException,
+            a_bad_close_frame.validate,
+            skip_utf8_validation=False,
+        )
+        a_bad_close_frame_2 = ABNF(
+            0, 0, 0, 0, opcode=ABNF.OPCODE_CLOSE, data=b"\x01\x8a\xaa\xff\xdd"
+        )
+        self.assertRaises(
+            ws._exceptions.WebSocketProtocolException,
+            a_bad_close_frame_2.validate,
+            skip_utf8_validation=False,
+        )
+        a_bad_close_frame_3 = ABNF(
+            0, 0, 0, 0, opcode=ABNF.OPCODE_CLOSE, data=b"\x03\xe7"
+        )
+        self.assertRaises(
+            ws._exceptions.WebSocketProtocolException,
+            a_bad_close_frame_3.validate,
+            skip_utf8_validation=True,
+        )
 
     def testMask(self):
-        abnf_none_data = ABNF(0,0,0,0, opcode=ABNF.OPCODE_PING, mask=1, data=None)
+        abnf_none_data = ABNF(
+            0, 0, 0, 0, opcode=ABNF.OPCODE_PING, mask_value=1, data=None
+        )
         bytes_val = b"aaaa"
         self.assertEqual(abnf_none_data._get_masked(bytes_val), bytes_val)
-        abnf_str_data = ABNF(0,0,0,0, opcode=ABNF.OPCODE_PING, mask=1, data="a")
-        self.assertEqual(abnf_str_data._get_masked(bytes_val), b'aaaa\x00')
+        abnf_str_data = ABNF(
+            0, 0, 0, 0, opcode=ABNF.OPCODE_PING, mask_value=1, data="a"
+        )
+        self.assertEqual(abnf_str_data._get_masked(bytes_val), b"aaaa\x00")
 
     def testFormat(self):
-        abnf_bad_rsv_bits = ABNF(2,0,0,0, opcode=ABNF.OPCODE_TEXT)
+        abnf_bad_rsv_bits = ABNF(2, 0, 0, 0, opcode=ABNF.OPCODE_TEXT)
         self.assertRaises(ValueError, abnf_bad_rsv_bits.format)
-        abnf_bad_opcode = ABNF(0,0,0,0, opcode=5)
+        abnf_bad_opcode = ABNF(0, 0, 0, 0, opcode=5)
         self.assertRaises(ValueError, abnf_bad_opcode.format)
-        abnf_length_10 = ABNF(0,0,0,0, opcode=ABNF.OPCODE_TEXT, data="abcdefghij")
-        self.assertEqual(b'\x01', abnf_length_10.format()[0].to_bytes(1, 'big'))
-        self.assertEqual(b'\x8a', abnf_length_10.format()[1].to_bytes(1, 'big'))
+        abnf_length_10 = ABNF(0, 0, 0, 0, opcode=ABNF.OPCODE_TEXT, data="abcdefghij")
+        self.assertEqual(b"\x01", abnf_length_10.format()[0].to_bytes(1, "big"))
+        self.assertEqual(b"\x8a", abnf_length_10.format()[1].to_bytes(1, "big"))
         self.assertEqual("fin=0 opcode=1 data=abcdefghij", abnf_length_10.__str__())
-        abnf_length_20 = ABNF(0,0,0,0, opcode=ABNF.OPCODE_BINARY, data="abcdefghijabcdefghij")
-        self.assertEqual(b'\x02', abnf_length_20.format()[0].to_bytes(1, 'big'))
-        self.assertEqual(b'\x94', abnf_length_20.format()[1].to_bytes(1, 'big'))
-        abnf_no_mask = ABNF(0,0,0,0, opcode=ABNF.OPCODE_TEXT, mask=0, data=b'\x01\x8a\xcc')
-        self.assertEqual(b'\x01\x03\x01\x8a\xcc', abnf_no_mask.format())
+        abnf_length_20 = ABNF(
+            0, 0, 0, 0, opcode=ABNF.OPCODE_BINARY, data="abcdefghijabcdefghij"
+        )
+        self.assertEqual(b"\x02", abnf_length_20.format()[0].to_bytes(1, "big"))
+        self.assertEqual(b"\x94", abnf_length_20.format()[1].to_bytes(1, "big"))
+        abnf_no_mask = ABNF(
+            0, 0, 0, 0, opcode=ABNF.OPCODE_TEXT, mask_value=0, data=b"\x01\x8a\xcc"
+        )
+        self.assertEqual(b"\x01\x03\x01\x8a\xcc", abnf_no_mask.format())
 
     def testFrameBuffer(self):
         fb = frame_buffer(0, True)
         self.assertEqual(fb.recv, 0)
         self.assertEqual(fb.skip_utf8_validation, True)
         fb.clear
         self.assertEqual(fb.header, None)
         self.assertEqual(fb.length, None)
-        self.assertEqual(fb.mask, None)
+        self.assertEqual(fb.mask_value, None)
         self.assertEqual(fb.has_mask(), False)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `websocket-client-1.6.4/websocket/tests/test_app.py` & `websocket-client-1.7.0/websocket/tests/test_app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
 #
 import os
 import os.path
-import threading
-import websocket as ws
 import ssl
+import threading
 import unittest
 
+import websocket as ws
+
 """
 test_app.py
 websocket - WebSocket client library for Python
 
 Copyright 2023 engn33r
 
 Licensed under the Apache License, Version 2.0 (the "License");
@@ -23,26 +24,24 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # Skip test to access the internet unless TEST_WITH_INTERNET == 1
-TEST_WITH_INTERNET = os.environ.get('TEST_WITH_INTERNET', '0') == '1'
+TEST_WITH_INTERNET = os.environ.get("TEST_WITH_INTERNET", "0") == "1"
 # Skip tests relying on local websockets server unless LOCAL_WS_SERVER_PORT != -1
-LOCAL_WS_SERVER_PORT = os.environ.get('LOCAL_WS_SERVER_PORT', '-1')
-TEST_WITH_LOCAL_SERVER = LOCAL_WS_SERVER_PORT != '-1'
+LOCAL_WS_SERVER_PORT = os.environ.get("LOCAL_WS_SERVER_PORT", "-1")
+TEST_WITH_LOCAL_SERVER = LOCAL_WS_SERVER_PORT != "-1"
 TRACEABLE = True
 
 
 class WebSocketAppTest(unittest.TestCase):
-
     class NotSetYet:
-        """ A marker class for signalling that a value hasn't been set yet.
-        """
+        """A marker class for signalling that a value hasn't been set yet."""
 
     def setUp(self):
         ws.enableTrace(TRACEABLE)
 
         WebSocketAppTest.keep_running_open = WebSocketAppTest.NotSetYet()
         WebSocketAppTest.keep_running_close = WebSocketAppTest.NotSetYet()
         WebSocketAppTest.get_mask_key_id = WebSocketAppTest.NotSetYet()
@@ -50,172 +49,212 @@
 
     def tearDown(self):
         WebSocketAppTest.keep_running_open = WebSocketAppTest.NotSetYet()
         WebSocketAppTest.keep_running_close = WebSocketAppTest.NotSetYet()
         WebSocketAppTest.get_mask_key_id = WebSocketAppTest.NotSetYet()
         WebSocketAppTest.on_error_data = WebSocketAppTest.NotSetYet()
 
-    @unittest.skipUnless(TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled")
+    @unittest.skipUnless(
+        TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled"
+    )
     def testKeepRunning(self):
-        """ A WebSocketApp should keep running as long as its self.keep_running
+        """A WebSocketApp should keep running as long as its self.keep_running
         is not False (in the boolean context).
         """
 
         def on_open(self, *args, **kwargs):
-            """ Set the keep_running flag for later inspection and immediately
+            """Set the keep_running flag for later inspection and immediately
             close the connection.
             """
             self.send("hello!")
             WebSocketAppTest.keep_running_open = self.keep_running
             self.keep_running = False
 
         def on_message(wsapp, message):
             print(message)
             self.close()
 
         def on_close(self, *args, **kwargs):
-            """ Set the keep_running flag for the test to use.
-            """
+            """Set the keep_running flag for the test to use."""
             WebSocketAppTest.keep_running_close = self.keep_running
 
-        app = ws.WebSocketApp('ws://127.0.0.1:' + LOCAL_WS_SERVER_PORT, on_open=on_open, on_close=on_close, on_message=on_message)
+        app = ws.WebSocketApp(
+            f"ws://127.0.0.1:{LOCAL_WS_SERVER_PORT}",
+            on_open=on_open,
+            on_close=on_close,
+            on_message=on_message,
+        )
         app.run_forever()
 
-#    @unittest.skipUnless(TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled")
+    #    @unittest.skipUnless(TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled")
     @unittest.skipUnless(False, "Test disabled for now (requires rel)")
     def testRunForeverDispatcher(self):
-        """ A WebSocketApp should keep running as long as its self.keep_running
+        """A WebSocketApp should keep running as long as its self.keep_running
         is not False (in the boolean context).
         """
 
         def on_open(self, *args, **kwargs):
-            """ Send a message, receive, and send one more
-            """
+            """Send a message, receive, and send one more"""
             self.send("hello!")
             self.recv()
             self.send("goodbye!")
 
         def on_message(wsapp, message):
             print(message)
             self.close()
 
-        app = ws.WebSocketApp('ws://127.0.0.1:' + LOCAL_WS_SERVER_PORT, on_open=on_open, on_message=on_message)
+        app = ws.WebSocketApp(
+            f"ws://127.0.0.1:{LOCAL_WS_SERVER_PORT}",
+            on_open=on_open,
+            on_message=on_message,
+        )
         app.run_forever(dispatcher="Dispatcher")  # doesn't work
-#        app.run_forever(dispatcher=rel)          # would work
-#        rel.dispatch()
 
-    @unittest.skipUnless(TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled")
+    #        app.run_forever(dispatcher=rel)          # would work
+    #        rel.dispatch()
+
+    @unittest.skipUnless(
+        TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled"
+    )
     def testRunForeverTeardownCleanExit(self):
-        """ The WebSocketApp.run_forever() method should return `False` when the application ends gracefully.
-        """
-        app = ws.WebSocketApp('ws://127.0.0.1:' + LOCAL_WS_SERVER_PORT)
+        """The WebSocketApp.run_forever() method should return `False` when the application ends gracefully."""
+        app = ws.WebSocketApp(f"ws://127.0.0.1:{LOCAL_WS_SERVER_PORT}")
         threading.Timer(interval=0.2, function=app.close).start()
         teardown = app.run_forever()
         self.assertEqual(teardown, False)
 
     @unittest.skipUnless(TEST_WITH_INTERNET, "Internet-requiring tests are disabled")
     def testSockMaskKey(self):
-        """ A WebSocketApp should forward the received mask_key function down
+        """A WebSocketApp should forward the received mask_key function down
         to the actual socket.
         """
 
         def my_mask_key_func():
             return "\x00\x00\x00\x00"
 
-        app = ws.WebSocketApp('wss://api-pub.bitfinex.com/ws/1', get_mask_key=my_mask_key_func)
+        app = ws.WebSocketApp(
+            "wss://api-pub.bitfinex.com/ws/1", get_mask_key=my_mask_key_func
+        )
 
         # if numpy is installed, this assertion fail
         # Note: We can't use 'is' for comparing the functions directly, need to use 'id'.
         self.assertEqual(id(app.get_mask_key), id(my_mask_key_func))
 
     @unittest.skipUnless(TEST_WITH_INTERNET, "Internet-requiring tests are disabled")
     def testInvalidPingIntervalPingTimeout(self):
-        """ Test exception handling if ping_interval < ping_timeout
-        """
+        """Test exception handling if ping_interval < ping_timeout"""
 
         def on_ping(app, msg):
             print("Got a ping!")
             app.close()
 
         def on_pong(app, msg):
             print("Got a pong! No need to respond")
             app.close()
 
-        app = ws.WebSocketApp('wss://api-pub.bitfinex.com/ws/1', on_ping=on_ping, on_pong=on_pong)
-        self.assertRaises(ws.WebSocketException, app.run_forever, ping_interval=1, ping_timeout=2, sslopt={"cert_reqs": ssl.CERT_NONE})
+        app = ws.WebSocketApp(
+            "wss://api-pub.bitfinex.com/ws/1", on_ping=on_ping, on_pong=on_pong
+        )
+        self.assertRaises(
+            ws.WebSocketException,
+            app.run_forever,
+            ping_interval=1,
+            ping_timeout=2,
+            sslopt={"cert_reqs": ssl.CERT_NONE},
+        )
 
     @unittest.skipUnless(TEST_WITH_INTERNET, "Internet-requiring tests are disabled")
     def testPingInterval(self):
-        """ Test WebSocketApp proper ping functionality
-        """
+        """Test WebSocketApp proper ping functionality"""
 
         def on_ping(app, msg):
             print("Got a ping!")
             app.close()
 
         def on_pong(app, msg):
             print("Got a pong! No need to respond")
             app.close()
 
-        app = ws.WebSocketApp('wss://api-pub.bitfinex.com/ws/1', on_ping=on_ping, on_pong=on_pong)
-        app.run_forever(ping_interval=2, ping_timeout=1, sslopt={"cert_reqs": ssl.CERT_NONE})
+        app = ws.WebSocketApp(
+            "wss://api-pub.bitfinex.com/ws/1", on_ping=on_ping, on_pong=on_pong
+        )
+        app.run_forever(
+            ping_interval=2, ping_timeout=1, sslopt={"cert_reqs": ssl.CERT_NONE}
+        )
 
     @unittest.skipUnless(TEST_WITH_INTERNET, "Internet-requiring tests are disabled")
     def testOpcodeClose(self):
-        """ Test WebSocketApp close opcode
-        """
+        """Test WebSocketApp close opcode"""
 
-        app = ws.WebSocketApp('wss://tsock.us1.twilio.com/v3/wsconnect')
+        app = ws.WebSocketApp("wss://tsock.us1.twilio.com/v3/wsconnect")
         app.run_forever(ping_interval=2, ping_timeout=1, ping_payload="Ping payload")
 
     # This is commented out because the URL no longer responds in the expected way
     # @unittest.skipUnless(TEST_WITH_INTERNET, "Internet-requiring tests are disabled")
     # def testOpcodeBinary(self):
     #     """ Test WebSocketApp binary opcode
     #     """
     #     app = ws.WebSocketApp('wss://streaming.vn.teslamotors.com/streaming/')
     #     app.run_forever(ping_interval=2, ping_timeout=1, ping_payload="Ping payload")
 
     @unittest.skipUnless(TEST_WITH_INTERNET, "Internet-requiring tests are disabled")
     def testBadPingInterval(self):
-        """ A WebSocketApp handling of negative ping_interval
-        """
-        app = ws.WebSocketApp('wss://api-pub.bitfinex.com/ws/1')
-        self.assertRaises(ws.WebSocketException, app.run_forever, ping_interval=-5, sslopt={"cert_reqs": ssl.CERT_NONE})
+        """A WebSocketApp handling of negative ping_interval"""
+        app = ws.WebSocketApp("wss://api-pub.bitfinex.com/ws/1")
+        self.assertRaises(
+            ws.WebSocketException,
+            app.run_forever,
+            ping_interval=-5,
+            sslopt={"cert_reqs": ssl.CERT_NONE},
+        )
 
     @unittest.skipUnless(TEST_WITH_INTERNET, "Internet-requiring tests are disabled")
     def testBadPingTimeout(self):
-        """ A WebSocketApp handling of negative ping_timeout
-        """
-        app = ws.WebSocketApp('wss://api-pub.bitfinex.com/ws/1')
-        self.assertRaises(ws.WebSocketException, app.run_forever, ping_timeout=-3, sslopt={"cert_reqs": ssl.CERT_NONE})
+        """A WebSocketApp handling of negative ping_timeout"""
+        app = ws.WebSocketApp("wss://api-pub.bitfinex.com/ws/1")
+        self.assertRaises(
+            ws.WebSocketException,
+            app.run_forever,
+            ping_timeout=-3,
+            sslopt={"cert_reqs": ssl.CERT_NONE},
+        )
 
     @unittest.skipUnless(TEST_WITH_INTERNET, "Internet-requiring tests are disabled")
     def testCloseStatusCode(self):
-        """ Test extraction of close frame status code and close reason in WebSocketApp
-        """
+        """Test extraction of close frame status code and close reason in WebSocketApp"""
+
         def on_close(wsapp, close_status_code, close_msg):
             print("on_close reached")
 
-        app = ws.WebSocketApp('wss://tsock.us1.twilio.com/v3/wsconnect', on_close=on_close)
-        closeframe = ws.ABNF(opcode=ws.ABNF.OPCODE_CLOSE, data=b'\x03\xe8no-init-from-client')
-        self.assertEqual([1000, 'no-init-from-client'], app._get_close_args(closeframe))
+        app = ws.WebSocketApp(
+            "wss://tsock.us1.twilio.com/v3/wsconnect", on_close=on_close
+        )
+        closeframe = ws.ABNF(
+            opcode=ws.ABNF.OPCODE_CLOSE, data=b"\x03\xe8no-init-from-client"
+        )
+        self.assertEqual([1000, "no-init-from-client"], app._get_close_args(closeframe))
 
-        closeframe = ws.ABNF(opcode=ws.ABNF.OPCODE_CLOSE, data=b'')
+        closeframe = ws.ABNF(opcode=ws.ABNF.OPCODE_CLOSE, data=b"")
         self.assertEqual([None, None], app._get_close_args(closeframe))
 
-        app2 = ws.WebSocketApp('wss://tsock.us1.twilio.com/v3/wsconnect')
-        closeframe = ws.ABNF(opcode=ws.ABNF.OPCODE_CLOSE, data=b'')
+        app2 = ws.WebSocketApp("wss://tsock.us1.twilio.com/v3/wsconnect")
+        closeframe = ws.ABNF(opcode=ws.ABNF.OPCODE_CLOSE, data=b"")
         self.assertEqual([None, None], app2._get_close_args(closeframe))
 
-        self.assertRaises(ws.WebSocketConnectionClosedException, app.send, data="test if connection is closed")
-
-    @unittest.skipUnless(TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled")
+        self.assertRaises(
+            ws.WebSocketConnectionClosedException,
+            app.send,
+            data="test if connection is closed",
+        )
+
+    @unittest.skipUnless(
+        TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled"
+    )
     def testCallbackFunctionException(self):
-        """ Test callback function exception handling """
+        """Test callback function exception handling"""
 
         exc = None
         passed_app = None
 
         def on_open(app):
             raise RuntimeError("Callback failed")
 
@@ -224,34 +263,41 @@
             passed_app = app
             nonlocal exc
             exc = err
 
         def on_pong(app, msg):
             app.close()
 
-        app = ws.WebSocketApp('ws://127.0.0.1:' + LOCAL_WS_SERVER_PORT, on_open=on_open, on_error=on_error, on_pong=on_pong)
+        app = ws.WebSocketApp(
+            f"ws://127.0.0.1:{LOCAL_WS_SERVER_PORT}",
+            on_open=on_open,
+            on_error=on_error,
+            on_pong=on_pong,
+        )
         app.run_forever(ping_interval=2, ping_timeout=1)
 
         self.assertEqual(passed_app, app)
         self.assertIsInstance(exc, RuntimeError)
         self.assertEqual(str(exc), "Callback failed")
 
-    @unittest.skipUnless(TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled")
+    @unittest.skipUnless(
+        TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled"
+    )
     def testCallbackMethodException(self):
-        """ Test callback method exception handling """
+        """Test callback method exception handling"""
 
         class Callbacks:
             def __init__(self):
                 self.exc = None
                 self.passed_app = None
                 self.app = ws.WebSocketApp(
-                    'ws://127.0.0.1:' + LOCAL_WS_SERVER_PORT,
+                    f"ws://127.0.0.1:{LOCAL_WS_SERVER_PORT}",
                     on_open=self.on_open,
                     on_error=self.on_error,
-                    on_pong=self.on_pong
+                    on_pong=self.on_pong,
                 )
                 self.app.run_forever(ping_interval=2, ping_timeout=1)
 
             def on_open(self, app):
                 raise RuntimeError("Callback failed")
 
             def on_error(self, app, err):
@@ -263,17 +309,19 @@
 
         callbacks = Callbacks()
 
         self.assertEqual(callbacks.passed_app, callbacks.app)
         self.assertIsInstance(callbacks.exc, RuntimeError)
         self.assertEqual(str(callbacks.exc), "Callback failed")
 
-    @unittest.skipUnless(TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled")
+    @unittest.skipUnless(
+        TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled"
+    )
     def testReconnect(self):
-        """ Test reconnect """
+        """Test reconnect"""
         pong_count = 0
         exc = None
 
         def on_error(app, err):
             nonlocal exc
             exc = err
 
@@ -283,15 +331,17 @@
             if pong_count == 1:
                 # First pong, shutdown socket, enforce read error
                 app.sock.shutdown()
             if pong_count >= 2:
                 # Got second pong after reconnect
                 app.close()
 
-        app = ws.WebSocketApp('ws://127.0.0.1:' + LOCAL_WS_SERVER_PORT, on_pong=on_pong, on_error=on_error)
+        app = ws.WebSocketApp(
+            f"ws://127.0.0.1:{LOCAL_WS_SERVER_PORT}", on_pong=on_pong, on_error=on_error
+        )
         app.run_forever(ping_interval=2, ping_timeout=1, reconnect=3)
 
         self.assertEqual(pong_count, 2)
         self.assertIsInstance(exc, ws.WebSocketTimeoutException)
         self.assertEqual(str(exc), "ping/pong timed out")
```

### Comparing `websocket-client-1.6.4/websocket/tests/test_cookiejar.py` & `websocket-client-1.7.0/websocket/tests/test_cookiejar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+
 from websocket._cookiejar import SimpleCookieJar
 
 """
 test_cookiejar.py
 websocket - WebSocket client library for Python
 
 Copyright 2023 engn33r
@@ -21,19 +22,23 @@
 """
 
 
 class CookieJarTest(unittest.TestCase):
     def testAdd(self):
         cookie_jar = SimpleCookieJar()
         cookie_jar.add("")
-        self.assertFalse(cookie_jar.jar, "Cookie with no domain should not be added to the jar")
+        self.assertFalse(
+            cookie_jar.jar, "Cookie with no domain should not be added to the jar"
+        )
 
         cookie_jar = SimpleCookieJar()
         cookie_jar.add("a=b")
-        self.assertFalse(cookie_jar.jar, "Cookie with no domain should not be added to the jar")
+        self.assertFalse(
+            cookie_jar.jar, "Cookie with no domain should not be added to the jar"
+        )
 
         cookie_jar = SimpleCookieJar()
         cookie_jar.add("a=b; domain=.abc")
         self.assertTrue(".abc" in cookie_jar.jar)
 
         cookie_jar = SimpleCookieJar()
         cookie_jar.add("a=b; domain=abc")
@@ -61,15 +66,17 @@
         self.assertEqual(cookie_jar.get("abc"), "a=b; c=d")
         self.assertEqual(cookie_jar.get("xyz"), "e=f")
         self.assertEqual(cookie_jar.get("something"), "")
 
     def testSet(self):
         cookie_jar = SimpleCookieJar()
         cookie_jar.set("a=b")
-        self.assertFalse(cookie_jar.jar, "Cookie with no domain should not be added to the jar")
+        self.assertFalse(
+            cookie_jar.jar, "Cookie with no domain should not be added to the jar"
+        )
 
         cookie_jar = SimpleCookieJar()
         cookie_jar.set("a=b; domain=.abc")
         self.assertTrue(".abc" in cookie_jar.jar)
 
         cookie_jar = SimpleCookieJar()
         cookie_jar.set("a=b; domain=abc")
```

### Comparing `websocket-client-1.6.4/websocket/tests/test_http.py` & `websocket-client-1.7.0/websocket/tests/test_http.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 # -*- coding: utf-8 -*-
 #
 import os
 import os.path
-import websocket as ws
-from websocket._http import proxy_info, read_headers, _start_proxied_socket, _tunnel, _get_addrinfo_list, connect
-import unittest
+import socket
 import ssl
+import unittest
+
 import websocket
-import socket
+import websocket as ws
+from websocket._http import (
+    _get_addrinfo_list,
+    _start_proxied_socket,
+    _tunnel,
+    connect,
+    proxy_info,
+    read_headers,
+)
 
 """
 test_http.py
 websocket - WebSocket client library for Python
 
 Copyright 2023 engn33r
 
@@ -25,24 +33,24 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 try:
-    from python_socks._errors import ProxyError, ProxyTimeoutError, ProxyConnectionError
+    from python_socks._errors import ProxyConnectionError, ProxyError, ProxyTimeoutError
 except:
-    from websocket._http import ProxyError, ProxyTimeoutError, ProxyConnectionError
+    from websocket._http import ProxyConnectionError, ProxyError, ProxyTimeoutError
 
 # Skip test to access the internet unless TEST_WITH_INTERNET == 1
-TEST_WITH_INTERNET = os.environ.get('TEST_WITH_INTERNET', '0') == '1'
-TEST_WITH_PROXY = os.environ.get('TEST_WITH_PROXY', '0') == '1'
+TEST_WITH_INTERNET = os.environ.get("TEST_WITH_INTERNET", "0") == "1"
+TEST_WITH_PROXY = os.environ.get("TEST_WITH_PROXY", "0") == "1"
 # Skip tests relying on local websockets server unless LOCAL_WS_SERVER_PORT != -1
-LOCAL_WS_SERVER_PORT = os.environ.get('LOCAL_WS_SERVER_PORT', '-1')
-TEST_WITH_LOCAL_SERVER = LOCAL_WS_SERVER_PORT != '-1'
+LOCAL_WS_SERVER_PORT = os.environ.get("LOCAL_WS_SERVER_PORT", "-1")
+TEST_WITH_LOCAL_SERVER = LOCAL_WS_SERVER_PORT != "-1"
 
 
 class SockMock:
     def __init__(self):
         self.data = []
         self.sent = []
 
@@ -66,77 +74,222 @@
         return len(data)
 
     def close(self):
         pass
 
 
 class HeaderSockMock(SockMock):
-
     def __init__(self, fname):
         SockMock.__init__(self)
         path = os.path.join(os.path.dirname(__file__), fname)
         with open(path, "rb") as f:
             self.add_packet(f.read())
 
 
-class OptsList():
-
+class OptsList:
     def __init__(self):
         self.timeout = 1
         self.sockopt = []
         self.sslopt = {"cert_reqs": ssl.CERT_NONE}
 
 
 class HttpTest(unittest.TestCase):
-
     def testReadHeader(self):
-        status, header, status_message = read_headers(HeaderSockMock("data/header01.txt"))
+        status, header, status_message = read_headers(
+            HeaderSockMock("data/header01.txt")
+        )
         self.assertEqual(status, 101)
         self.assertEqual(header["connection"], "Upgrade")
         # header02.txt is intentionally malformed
-        self.assertRaises(ws.WebSocketException, read_headers, HeaderSockMock("data/header02.txt"))
+        self.assertRaises(
+            ws.WebSocketException, read_headers, HeaderSockMock("data/header02.txt")
+        )
 
     def testTunnel(self):
-        self.assertRaises(ws.WebSocketProxyException, _tunnel, HeaderSockMock("data/header01.txt"), "example.com", 80, ("username", "password"))
-        self.assertRaises(ws.WebSocketProxyException, _tunnel, HeaderSockMock("data/header02.txt"), "example.com", 80, ("username", "password"))
+        self.assertRaises(
+            ws.WebSocketProxyException,
+            _tunnel,
+            HeaderSockMock("data/header01.txt"),
+            "example.com",
+            80,
+            ("username", "password"),
+        )
+        self.assertRaises(
+            ws.WebSocketProxyException,
+            _tunnel,
+            HeaderSockMock("data/header02.txt"),
+            "example.com",
+            80,
+            ("username", "password"),
+        )
 
     @unittest.skipUnless(TEST_WITH_INTERNET, "Internet-requiring tests are disabled")
     def testConnect(self):
         # Not currently testing an actual proxy connection, so just check whether proxy errors are raised. This requires internet for a DNS lookup
         if ws._http.HAVE_PYTHON_SOCKS:
             # Need this check, otherwise case where python_socks is not installed triggers
             # websocket._exceptions.WebSocketException: Python Socks is needed for SOCKS proxying but is not available
-            self.assertRaises((ProxyTimeoutError, OSError), _start_proxied_socket, "wss://example.com", OptsList(), proxy_info(http_proxy_host="example.com", http_proxy_port="8080", proxy_type="socks4", http_proxy_timeout=1))
-            self.assertRaises((ProxyTimeoutError, OSError), _start_proxied_socket, "wss://example.com", OptsList(), proxy_info(http_proxy_host="example.com", http_proxy_port="8080", proxy_type="socks4a", http_proxy_timeout=1))
-            self.assertRaises((ProxyTimeoutError, OSError), _start_proxied_socket, "wss://example.com", OptsList(), proxy_info(http_proxy_host="example.com", http_proxy_port="8080", proxy_type="socks5", http_proxy_timeout=1))
-            self.assertRaises((ProxyTimeoutError, OSError), _start_proxied_socket, "wss://example.com", OptsList(), proxy_info(http_proxy_host="example.com", http_proxy_port="8080", proxy_type="socks5h", http_proxy_timeout=1))
-            self.assertRaises(ProxyConnectionError, connect, "wss://example.com", OptsList(), proxy_info(http_proxy_host="127.0.0.1", http_proxy_port=9999, proxy_type="socks4", http_proxy_timeout=1), None)
-
-        self.assertRaises(TypeError, _get_addrinfo_list, None, 80, True, proxy_info(http_proxy_host="127.0.0.1", http_proxy_port="9999", proxy_type="http"))
-        self.assertRaises(TypeError, _get_addrinfo_list, None, 80, True, proxy_info(http_proxy_host="127.0.0.1", http_proxy_port="9999", proxy_type="http"))
-        self.assertRaises(socket.timeout, connect, "wss://google.com", OptsList(), proxy_info(http_proxy_host="8.8.8.8", http_proxy_port=9999, proxy_type="http", http_proxy_timeout=1), None)
+            self.assertRaises(
+                (ProxyTimeoutError, OSError),
+                _start_proxied_socket,
+                "wss://example.com",
+                OptsList(),
+                proxy_info(
+                    http_proxy_host="example.com",
+                    http_proxy_port="8080",
+                    proxy_type="socks4",
+                    http_proxy_timeout=1,
+                ),
+            )
+            self.assertRaises(
+                (ProxyTimeoutError, OSError),
+                _start_proxied_socket,
+                "wss://example.com",
+                OptsList(),
+                proxy_info(
+                    http_proxy_host="example.com",
+                    http_proxy_port="8080",
+                    proxy_type="socks4a",
+                    http_proxy_timeout=1,
+                ),
+            )
+            self.assertRaises(
+                (ProxyTimeoutError, OSError),
+                _start_proxied_socket,
+                "wss://example.com",
+                OptsList(),
+                proxy_info(
+                    http_proxy_host="example.com",
+                    http_proxy_port="8080",
+                    proxy_type="socks5",
+                    http_proxy_timeout=1,
+                ),
+            )
+            self.assertRaises(
+                (ProxyTimeoutError, OSError),
+                _start_proxied_socket,
+                "wss://example.com",
+                OptsList(),
+                proxy_info(
+                    http_proxy_host="example.com",
+                    http_proxy_port="8080",
+                    proxy_type="socks5h",
+                    http_proxy_timeout=1,
+                ),
+            )
+            self.assertRaises(
+                ProxyConnectionError,
+                connect,
+                "wss://example.com",
+                OptsList(),
+                proxy_info(
+                    http_proxy_host="127.0.0.1",
+                    http_proxy_port=9999,
+                    proxy_type="socks4",
+                    http_proxy_timeout=1,
+                ),
+                None,
+            )
+
+        self.assertRaises(
+            TypeError,
+            _get_addrinfo_list,
+            None,
+            80,
+            True,
+            proxy_info(
+                http_proxy_host="127.0.0.1", http_proxy_port="9999", proxy_type="http"
+            ),
+        )
+        self.assertRaises(
+            TypeError,
+            _get_addrinfo_list,
+            None,
+            80,
+            True,
+            proxy_info(
+                http_proxy_host="127.0.0.1", http_proxy_port="9999", proxy_type="http"
+            ),
+        )
+        self.assertRaises(
+            socket.timeout,
+            connect,
+            "wss://google.com",
+            OptsList(),
+            proxy_info(
+                http_proxy_host="8.8.8.8",
+                http_proxy_port=9999,
+                proxy_type="http",
+                http_proxy_timeout=1,
+            ),
+            None,
+        )
         self.assertEqual(
-            connect("wss://google.com", OptsList(), proxy_info(http_proxy_host="8.8.8.8", http_proxy_port=8080, proxy_type="http"), True),
-            (True, ("google.com", 443, "/")))
+            connect(
+                "wss://google.com",
+                OptsList(),
+                proxy_info(
+                    http_proxy_host="8.8.8.8", http_proxy_port=8080, proxy_type="http"
+                ),
+                True,
+            ),
+            (True, ("google.com", 443, "/")),
+        )
         # The following test fails on Mac OS with a gaierror, not an OverflowError
         # self.assertRaises(OverflowError, connect, "wss://example.com", OptsList(), proxy_info(http_proxy_host="127.0.0.1", http_proxy_port=99999, proxy_type="socks4", timeout=2), False)
 
     @unittest.skipUnless(TEST_WITH_INTERNET, "Internet-requiring tests are disabled")
-    @unittest.skipUnless(TEST_WITH_PROXY, "This test requires a HTTP proxy to be running on port 8899")
-    @unittest.skipUnless(TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled")
+    @unittest.skipUnless(
+        TEST_WITH_PROXY, "This test requires a HTTP proxy to be running on port 8899"
+    )
+    @unittest.skipUnless(
+        TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled"
+    )
     def testProxyConnect(self):
         ws = websocket.WebSocket()
-        ws.connect("ws://127.0.0.1:" + LOCAL_WS_SERVER_PORT, http_proxy_host="127.0.0.1", http_proxy_port="8899", proxy_type="http")
+        ws.connect(
+            f"ws://127.0.0.1:{LOCAL_WS_SERVER_PORT}",
+            http_proxy_host="127.0.0.1",
+            http_proxy_port="8899",
+            proxy_type="http",
+        )
         ws.send("Hello, Server")
         server_response = ws.recv()
         self.assertEqual(server_response, "Hello, Server")
         # self.assertEqual(_start_proxied_socket("wss://api.bitfinex.com/ws/2", OptsList(), proxy_info(http_proxy_host="127.0.0.1", http_proxy_port="8899", proxy_type="http"))[1], ("api.bitfinex.com", 443, '/ws/2'))
-        self.assertEqual(_get_addrinfo_list("api.bitfinex.com", 443, True, proxy_info(http_proxy_host="127.0.0.1", http_proxy_port="8899", proxy_type="http")),
-                         (socket.getaddrinfo("127.0.0.1", 8899, 0, socket.SOCK_STREAM, socket.SOL_TCP), True, None))
-        self.assertEqual(connect("wss://api.bitfinex.com/ws/2", OptsList(), proxy_info(http_proxy_host="127.0.0.1", http_proxy_port=8899, proxy_type="http"), None)[1], ("api.bitfinex.com", 443, '/ws/2'))
+        self.assertEqual(
+            _get_addrinfo_list(
+                "api.bitfinex.com",
+                443,
+                True,
+                proxy_info(
+                    http_proxy_host="127.0.0.1",
+                    http_proxy_port="8899",
+                    proxy_type="http",
+                ),
+            ),
+            (
+                socket.getaddrinfo(
+                    "127.0.0.1", 8899, 0, socket.SOCK_STREAM, socket.SOL_TCP
+                ),
+                True,
+                None,
+            ),
+        )
+        self.assertEqual(
+            connect(
+                "wss://api.bitfinex.com/ws/2",
+                OptsList(),
+                proxy_info(
+                    http_proxy_host="127.0.0.1", http_proxy_port=8899, proxy_type="http"
+                ),
+                None,
+            )[1],
+            ("api.bitfinex.com", 443, "/ws/2"),
+        )
         # TODO: Test SOCKS4 and SOCK5 proxies with unit tests
 
     @unittest.skipUnless(TEST_WITH_INTERNET, "Internet-requiring tests are disabled")
     def testSSLopt(self):
         ssloptions = {
             "check_hostname": False,
             "server_hostname": "ServerName",
@@ -147,30 +300,72 @@
                         ECDHE-ECDSA-CHACHA20-POLY1305:ECDHE-RSA-CHACHA20-POLY1305:\
                         DHE-RSA-CHACHA20-POLY1305:ECDHE-ECDSA-AES128-GCM-SHA256:\
                         ECDHE-RSA-AES128-GCM-SHA256:DHE-RSA-AES128-GCM-SHA256:\
                         ECDHE-ECDSA-AES256-SHA384:ECDHE-RSA-AES256-SHA384:\
                         DHE-RSA-AES256-SHA256:ECDHE-ECDSA-AES128-SHA256:\
                         ECDHE-RSA-AES128-SHA256:DHE-RSA-AES128-SHA256:\
                         ECDHE-ECDSA-AES256-SHA:ECDHE-RSA-AES256-SHA",
-            "ecdh_curve": "prime256v1"
+            "ecdh_curve": "prime256v1",
         }
         ws_ssl1 = websocket.WebSocket(sslopt=ssloptions)
         ws_ssl1.connect("wss://api.bitfinex.com/ws/2")
         ws_ssl1.send("Hello")
         ws_ssl1.close()
 
         ws_ssl2 = websocket.WebSocket(sslopt={"check_hostname": True})
         ws_ssl2.connect("wss://api.bitfinex.com/ws/2")
         ws_ssl2.close
 
     def testProxyInfo(self):
-        self.assertEqual(proxy_info(http_proxy_host="127.0.0.1", http_proxy_port="8080", proxy_type="http").proxy_protocol, "http")
-        self.assertRaises(ProxyError, proxy_info, http_proxy_host="127.0.0.1", http_proxy_port="8080", proxy_type="badval")
-        self.assertEqual(proxy_info(http_proxy_host="example.com", http_proxy_port="8080", proxy_type="http").proxy_host, "example.com")
-        self.assertEqual(proxy_info(http_proxy_host="127.0.0.1", http_proxy_port="8080", proxy_type="http").proxy_port, "8080")
-        self.assertEqual(proxy_info(http_proxy_host="127.0.0.1", http_proxy_port="8080", proxy_type="http").auth, None)
-        self.assertEqual(proxy_info(http_proxy_host="127.0.0.1", http_proxy_port="8080", proxy_type="http", http_proxy_auth=("my_username123", "my_pass321")).auth[0], "my_username123")
-        self.assertEqual(proxy_info(http_proxy_host="127.0.0.1", http_proxy_port="8080", proxy_type="http", http_proxy_auth=("my_username123", "my_pass321")).auth[1], "my_pass321")
+        self.assertEqual(
+            proxy_info(
+                http_proxy_host="127.0.0.1", http_proxy_port="8080", proxy_type="http"
+            ).proxy_protocol,
+            "http",
+        )
+        self.assertRaises(
+            ProxyError,
+            proxy_info,
+            http_proxy_host="127.0.0.1",
+            http_proxy_port="8080",
+            proxy_type="badval",
+        )
+        self.assertEqual(
+            proxy_info(
+                http_proxy_host="example.com", http_proxy_port="8080", proxy_type="http"
+            ).proxy_host,
+            "example.com",
+        )
+        self.assertEqual(
+            proxy_info(
+                http_proxy_host="127.0.0.1", http_proxy_port="8080", proxy_type="http"
+            ).proxy_port,
+            "8080",
+        )
+        self.assertEqual(
+            proxy_info(
+                http_proxy_host="127.0.0.1", http_proxy_port="8080", proxy_type="http"
+            ).auth,
+            None,
+        )
+        self.assertEqual(
+            proxy_info(
+                http_proxy_host="127.0.0.1",
+                http_proxy_port="8080",
+                proxy_type="http",
+                http_proxy_auth=("my_username123", "my_pass321"),
+            ).auth[0],
+            "my_username123",
+        )
+        self.assertEqual(
+            proxy_info(
+                http_proxy_host="127.0.0.1",
+                http_proxy_port="8080",
+                proxy_type="http",
+                http_proxy_auth=("my_username123", "my_pass321"),
+            ).auth[1],
+            "my_pass321",
+        )
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `websocket-client-1.6.4/websocket/tests/test_url.py` & `websocket-client-1.7.0/websocket/tests/test_url.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # -*- coding: utf-8 -*-
 #
 import os
 import unittest
-from websocket._url import get_proxy_info, parse_url, _is_address_in_network, _is_no_proxy_host
+
+from websocket._url import (
+    _is_address_in_network,
+    _is_no_proxy_host,
+    get_proxy_info,
+    parse_url,
+)
 
 """
 test_url.py
 websocket - WebSocket client library for Python
 
 Copyright 2023 engn33r
 
@@ -21,19 +27,18 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 
 class UrlTest(unittest.TestCase):
-
     def test_address_in_network(self):
-        self.assertTrue(_is_address_in_network('127.0.0.1', '127.0.0.0/8'))
-        self.assertTrue(_is_address_in_network('127.1.0.1', '127.0.0.0/8'))
-        self.assertFalse(_is_address_in_network('127.1.0.1', '127.0.0.0/24'))
+        self.assertTrue(_is_address_in_network("127.0.0.1", "127.0.0.0/8"))
+        self.assertTrue(_is_address_in_network("127.1.0.1", "127.0.0.0/8"))
+        self.assertFalse(_is_address_in_network("127.1.0.1", "127.0.0.0/24"))
 
     def testParseUrl(self):
         p = parse_url("ws://www.example.com/r")
         self.assertEqual(p[0], "www.example.com")
         self.assertEqual(p[1], 80)
         self.assertEqual(p[2], "/r")
         self.assertEqual(p[3], False)
@@ -122,65 +127,79 @@
     def tearDown(self):
         if self.no_proxy:
             os.environ["no_proxy"] = self.no_proxy
         elif "no_proxy" in os.environ:
             del os.environ["no_proxy"]
 
     def testMatchAll(self):
-        self.assertTrue(_is_no_proxy_host("any.websocket.org", ['*']))
-        self.assertTrue(_is_no_proxy_host("192.168.0.1", ['*']))
-        self.assertTrue(_is_no_proxy_host("any.websocket.org", ['other.websocket.org', '*']))
-        os.environ['no_proxy'] = '*'
+        self.assertTrue(_is_no_proxy_host("any.websocket.org", ["*"]))
+        self.assertTrue(_is_no_proxy_host("192.168.0.1", ["*"]))
+        self.assertTrue(
+            _is_no_proxy_host("any.websocket.org", ["other.websocket.org", "*"])
+        )
+        os.environ["no_proxy"] = "*"
         self.assertTrue(_is_no_proxy_host("any.websocket.org", None))
         self.assertTrue(_is_no_proxy_host("192.168.0.1", None))
-        os.environ['no_proxy'] = 'other.websocket.org, *'
+        os.environ["no_proxy"] = "other.websocket.org, *"
         self.assertTrue(_is_no_proxy_host("any.websocket.org", None))
 
     def testIpAddress(self):
-        self.assertTrue(_is_no_proxy_host("127.0.0.1", ['127.0.0.1']))
-        self.assertFalse(_is_no_proxy_host("127.0.0.2", ['127.0.0.1']))
-        self.assertTrue(_is_no_proxy_host("127.0.0.1", ['other.websocket.org', '127.0.0.1']))
-        self.assertFalse(_is_no_proxy_host("127.0.0.2", ['other.websocket.org', '127.0.0.1']))
-        os.environ['no_proxy'] = '127.0.0.1'
+        self.assertTrue(_is_no_proxy_host("127.0.0.1", ["127.0.0.1"]))
+        self.assertFalse(_is_no_proxy_host("127.0.0.2", ["127.0.0.1"]))
+        self.assertTrue(
+            _is_no_proxy_host("127.0.0.1", ["other.websocket.org", "127.0.0.1"])
+        )
+        self.assertFalse(
+            _is_no_proxy_host("127.0.0.2", ["other.websocket.org", "127.0.0.1"])
+        )
+        os.environ["no_proxy"] = "127.0.0.1"
         self.assertTrue(_is_no_proxy_host("127.0.0.1", None))
         self.assertFalse(_is_no_proxy_host("127.0.0.2", None))
-        os.environ['no_proxy'] = 'other.websocket.org, 127.0.0.1'
+        os.environ["no_proxy"] = "other.websocket.org, 127.0.0.1"
         self.assertTrue(_is_no_proxy_host("127.0.0.1", None))
         self.assertFalse(_is_no_proxy_host("127.0.0.2", None))
 
     def testIpAddressInRange(self):
-        self.assertTrue(_is_no_proxy_host("127.0.0.1", ['127.0.0.0/8']))
-        self.assertTrue(_is_no_proxy_host("127.0.0.2", ['127.0.0.0/8']))
-        self.assertFalse(_is_no_proxy_host("127.1.0.1", ['127.0.0.0/24']))
-        os.environ['no_proxy'] = '127.0.0.0/8'
+        self.assertTrue(_is_no_proxy_host("127.0.0.1", ["127.0.0.0/8"]))
+        self.assertTrue(_is_no_proxy_host("127.0.0.2", ["127.0.0.0/8"]))
+        self.assertFalse(_is_no_proxy_host("127.1.0.1", ["127.0.0.0/24"]))
+        os.environ["no_proxy"] = "127.0.0.0/8"
         self.assertTrue(_is_no_proxy_host("127.0.0.1", None))
         self.assertTrue(_is_no_proxy_host("127.0.0.2", None))
-        os.environ['no_proxy'] = '127.0.0.0/24'
+        os.environ["no_proxy"] = "127.0.0.0/24"
         self.assertFalse(_is_no_proxy_host("127.1.0.1", None))
 
     def testHostnameMatch(self):
-        self.assertTrue(_is_no_proxy_host("my.websocket.org", ['my.websocket.org']))
-        self.assertTrue(_is_no_proxy_host("my.websocket.org", ['other.websocket.org', 'my.websocket.org']))
-        self.assertFalse(_is_no_proxy_host("my.websocket.org", ['other.websocket.org']))
-        os.environ['no_proxy'] = 'my.websocket.org'
+        self.assertTrue(_is_no_proxy_host("my.websocket.org", ["my.websocket.org"]))
+        self.assertTrue(
+            _is_no_proxy_host(
+                "my.websocket.org", ["other.websocket.org", "my.websocket.org"]
+            )
+        )
+        self.assertFalse(_is_no_proxy_host("my.websocket.org", ["other.websocket.org"]))
+        os.environ["no_proxy"] = "my.websocket.org"
         self.assertTrue(_is_no_proxy_host("my.websocket.org", None))
         self.assertFalse(_is_no_proxy_host("other.websocket.org", None))
-        os.environ['no_proxy'] = 'other.websocket.org, my.websocket.org'
+        os.environ["no_proxy"] = "other.websocket.org, my.websocket.org"
         self.assertTrue(_is_no_proxy_host("my.websocket.org", None))
 
     def testHostnameMatchDomain(self):
-        self.assertTrue(_is_no_proxy_host("any.websocket.org", ['.websocket.org']))
-        self.assertTrue(_is_no_proxy_host("my.other.websocket.org", ['.websocket.org']))
-        self.assertTrue(_is_no_proxy_host("any.websocket.org", ['my.websocket.org', '.websocket.org']))
-        self.assertFalse(_is_no_proxy_host("any.websocket.com", ['.websocket.org']))
-        os.environ['no_proxy'] = '.websocket.org'
+        self.assertTrue(_is_no_proxy_host("any.websocket.org", [".websocket.org"]))
+        self.assertTrue(_is_no_proxy_host("my.other.websocket.org", [".websocket.org"]))
+        self.assertTrue(
+            _is_no_proxy_host(
+                "any.websocket.org", ["my.websocket.org", ".websocket.org"]
+            )
+        )
+        self.assertFalse(_is_no_proxy_host("any.websocket.com", [".websocket.org"]))
+        os.environ["no_proxy"] = ".websocket.org"
         self.assertTrue(_is_no_proxy_host("any.websocket.org", None))
         self.assertTrue(_is_no_proxy_host("my.other.websocket.org", None))
         self.assertFalse(_is_no_proxy_host("any.websocket.com", None))
-        os.environ['no_proxy'] = 'my.websocket.org, .websocket.org'
+        os.environ["no_proxy"] = "my.websocket.org, .websocket.org"
         self.assertTrue(_is_no_proxy_host("any.websocket.org", None))
 
 
 class ProxyInfoTest(unittest.TestCase):
     def setUp(self):
         self.http_proxy = os.environ.get("http_proxy", None)
         self.https_proxy = os.environ.get("https_proxy", None)
@@ -205,104 +224,213 @@
 
         if self.no_proxy:
             os.environ["no_proxy"] = self.no_proxy
         elif "no_proxy" in os.environ:
             del os.environ["no_proxy"]
 
     def testProxyFromArgs(self):
-        self.assertEqual(get_proxy_info("echo.websocket.events", False, proxy_host="localhost"), ("localhost", 0, None))
-        self.assertEqual(get_proxy_info("echo.websocket.events", False, proxy_host="localhost", proxy_port=3128),
-                         ("localhost", 3128, None))
-        self.assertEqual(get_proxy_info("echo.websocket.events", True, proxy_host="localhost"), ("localhost", 0, None))
-        self.assertEqual(get_proxy_info("echo.websocket.events", True, proxy_host="localhost", proxy_port=3128),
-                         ("localhost", 3128, None))
-
-        self.assertEqual(get_proxy_info("echo.websocket.events", False, proxy_host="localhost", proxy_auth=("a", "b")),
-                         ("localhost", 0, ("a", "b")))
-        self.assertEqual(
-            get_proxy_info("echo.websocket.events", False, proxy_host="localhost", proxy_port=3128, proxy_auth=("a", "b")),
-            ("localhost", 3128, ("a", "b")))
-        self.assertEqual(get_proxy_info("echo.websocket.events", True, proxy_host="localhost", proxy_auth=("a", "b")),
-                         ("localhost", 0, ("a", "b")))
-        self.assertEqual(
-            get_proxy_info("echo.websocket.events", True, proxy_host="localhost", proxy_port=3128, proxy_auth=("a", "b")),
-            ("localhost", 3128, ("a", "b")))
-
-        self.assertEqual(get_proxy_info("echo.websocket.events", True, proxy_host="localhost", proxy_port=3128,
-                                        no_proxy=["example.com"], proxy_auth=("a", "b")),
-                         ("localhost", 3128, ("a", "b")))
-        self.assertEqual(get_proxy_info("echo.websocket.events", True, proxy_host="localhost", proxy_port=3128,
-                                        no_proxy=["echo.websocket.events"], proxy_auth=("a", "b")),
-                         (None, 0, None))
+        self.assertEqual(
+            get_proxy_info("echo.websocket.events", False, proxy_host="localhost"),
+            ("localhost", 0, None),
+        )
+        self.assertEqual(
+            get_proxy_info(
+                "echo.websocket.events", False, proxy_host="localhost", proxy_port=3128
+            ),
+            ("localhost", 3128, None),
+        )
+        self.assertEqual(
+            get_proxy_info("echo.websocket.events", True, proxy_host="localhost"),
+            ("localhost", 0, None),
+        )
+        self.assertEqual(
+            get_proxy_info(
+                "echo.websocket.events", True, proxy_host="localhost", proxy_port=3128
+            ),
+            ("localhost", 3128, None),
+        )
+
+        self.assertEqual(
+            get_proxy_info(
+                "echo.websocket.events",
+                False,
+                proxy_host="localhost",
+                proxy_auth=("a", "b"),
+            ),
+            ("localhost", 0, ("a", "b")),
+        )
+        self.assertEqual(
+            get_proxy_info(
+                "echo.websocket.events",
+                False,
+                proxy_host="localhost",
+                proxy_port=3128,
+                proxy_auth=("a", "b"),
+            ),
+            ("localhost", 3128, ("a", "b")),
+        )
+        self.assertEqual(
+            get_proxy_info(
+                "echo.websocket.events",
+                True,
+                proxy_host="localhost",
+                proxy_auth=("a", "b"),
+            ),
+            ("localhost", 0, ("a", "b")),
+        )
+        self.assertEqual(
+            get_proxy_info(
+                "echo.websocket.events",
+                True,
+                proxy_host="localhost",
+                proxy_port=3128,
+                proxy_auth=("a", "b"),
+            ),
+            ("localhost", 3128, ("a", "b")),
+        )
+
+        self.assertEqual(
+            get_proxy_info(
+                "echo.websocket.events",
+                True,
+                proxy_host="localhost",
+                proxy_port=3128,
+                no_proxy=["example.com"],
+                proxy_auth=("a", "b"),
+            ),
+            ("localhost", 3128, ("a", "b")),
+        )
+        self.assertEqual(
+            get_proxy_info(
+                "echo.websocket.events",
+                True,
+                proxy_host="localhost",
+                proxy_port=3128,
+                no_proxy=["echo.websocket.events"],
+                proxy_auth=("a", "b"),
+            ),
+            (None, 0, None),
+        )
 
     def testProxyFromEnv(self):
         os.environ["http_proxy"] = "http://localhost/"
-        self.assertEqual(get_proxy_info("echo.websocket.events", False), ("localhost", None, None))
+        self.assertEqual(
+            get_proxy_info("echo.websocket.events", False), ("localhost", None, None)
+        )
         os.environ["http_proxy"] = "http://localhost:3128/"
-        self.assertEqual(get_proxy_info("echo.websocket.events", False), ("localhost", 3128, None))
+        self.assertEqual(
+            get_proxy_info("echo.websocket.events", False), ("localhost", 3128, None)
+        )
 
         os.environ["http_proxy"] = "http://localhost/"
         os.environ["https_proxy"] = "http://localhost2/"
-        self.assertEqual(get_proxy_info("echo.websocket.events", False), ("localhost", None, None))
+        self.assertEqual(
+            get_proxy_info("echo.websocket.events", False), ("localhost", None, None)
+        )
         os.environ["http_proxy"] = "http://localhost:3128/"
         os.environ["https_proxy"] = "http://localhost2:3128/"
-        self.assertEqual(get_proxy_info("echo.websocket.events", False), ("localhost", 3128, None))
+        self.assertEqual(
+            get_proxy_info("echo.websocket.events", False), ("localhost", 3128, None)
+        )
 
         os.environ["http_proxy"] = "http://localhost/"
         os.environ["https_proxy"] = "http://localhost2/"
-        self.assertEqual(get_proxy_info("echo.websocket.events", True), ("localhost2", None, None))
+        self.assertEqual(
+            get_proxy_info("echo.websocket.events", True), ("localhost2", None, None)
+        )
         os.environ["http_proxy"] = "http://localhost:3128/"
         os.environ["https_proxy"] = "http://localhost2:3128/"
-        self.assertEqual(get_proxy_info("echo.websocket.events", True), ("localhost2", 3128, None))
+        self.assertEqual(
+            get_proxy_info("echo.websocket.events", True), ("localhost2", 3128, None)
+        )
 
         os.environ["http_proxy"] = ""
         os.environ["https_proxy"] = "http://localhost2/"
-        self.assertEqual(get_proxy_info("echo.websocket.events", True), ("localhost2", None, None))
-        self.assertEqual(get_proxy_info("echo.websocket.events", False), (None, 0, None))
+        self.assertEqual(
+            get_proxy_info("echo.websocket.events", True), ("localhost2", None, None)
+        )
+        self.assertEqual(
+            get_proxy_info("echo.websocket.events", False), (None, 0, None)
+        )
         os.environ["http_proxy"] = ""
         os.environ["https_proxy"] = "http://localhost2:3128/"
-        self.assertEqual(get_proxy_info("echo.websocket.events", True), ("localhost2", 3128, None))
-        self.assertEqual(get_proxy_info("echo.websocket.events", False), (None, 0, None))
+        self.assertEqual(
+            get_proxy_info("echo.websocket.events", True), ("localhost2", 3128, None)
+        )
+        self.assertEqual(
+            get_proxy_info("echo.websocket.events", False), (None, 0, None)
+        )
 
         os.environ["http_proxy"] = "http://localhost/"
         os.environ["https_proxy"] = ""
         self.assertEqual(get_proxy_info("echo.websocket.events", True), (None, 0, None))
-        self.assertEqual(get_proxy_info("echo.websocket.events", False), ("localhost", None, None))
+        self.assertEqual(
+            get_proxy_info("echo.websocket.events", False), ("localhost", None, None)
+        )
         os.environ["http_proxy"] = "http://localhost:3128/"
         os.environ["https_proxy"] = ""
         self.assertEqual(get_proxy_info("echo.websocket.events", True), (None, 0, None))
-        self.assertEqual(get_proxy_info("echo.websocket.events", False), ("localhost", 3128, None))
+        self.assertEqual(
+            get_proxy_info("echo.websocket.events", False), ("localhost", 3128, None)
+        )
 
         os.environ["http_proxy"] = "http://a:b@localhost/"
-        self.assertEqual(get_proxy_info("echo.websocket.events", False), ("localhost", None, ("a", "b")))
+        self.assertEqual(
+            get_proxy_info("echo.websocket.events", False),
+            ("localhost", None, ("a", "b")),
+        )
         os.environ["http_proxy"] = "http://a:b@localhost:3128/"
-        self.assertEqual(get_proxy_info("echo.websocket.events", False), ("localhost", 3128, ("a", "b")))
+        self.assertEqual(
+            get_proxy_info("echo.websocket.events", False),
+            ("localhost", 3128, ("a", "b")),
+        )
 
         os.environ["http_proxy"] = "http://a:b@localhost/"
         os.environ["https_proxy"] = "http://a:b@localhost2/"
-        self.assertEqual(get_proxy_info("echo.websocket.events", False), ("localhost", None, ("a", "b")))
+        self.assertEqual(
+            get_proxy_info("echo.websocket.events", False),
+            ("localhost", None, ("a", "b")),
+        )
         os.environ["http_proxy"] = "http://a:b@localhost:3128/"
         os.environ["https_proxy"] = "http://a:b@localhost2:3128/"
-        self.assertEqual(get_proxy_info("echo.websocket.events", False), ("localhost", 3128, ("a", "b")))
+        self.assertEqual(
+            get_proxy_info("echo.websocket.events", False),
+            ("localhost", 3128, ("a", "b")),
+        )
 
         os.environ["http_proxy"] = "http://a:b@localhost/"
         os.environ["https_proxy"] = "http://a:b@localhost2/"
-        self.assertEqual(get_proxy_info("echo.websocket.events", True), ("localhost2", None, ("a", "b")))
+        self.assertEqual(
+            get_proxy_info("echo.websocket.events", True),
+            ("localhost2", None, ("a", "b")),
+        )
         os.environ["http_proxy"] = "http://a:b@localhost:3128/"
         os.environ["https_proxy"] = "http://a:b@localhost2:3128/"
-        self.assertEqual(get_proxy_info("echo.websocket.events", True), ("localhost2", 3128, ("a", "b")))
-
-        os.environ["http_proxy"] = "http://john%40example.com:P%40SSWORD@localhost:3128/"
-        os.environ["https_proxy"] = "http://john%40example.com:P%40SSWORD@localhost2:3128/"
-        self.assertEqual(get_proxy_info("echo.websocket.events", True), ("localhost2", 3128, ("john@example.com", "P@SSWORD")))
+        self.assertEqual(
+            get_proxy_info("echo.websocket.events", True),
+            ("localhost2", 3128, ("a", "b")),
+        )
+
+        os.environ[
+            "http_proxy"
+        ] = "http://john%40example.com:P%40SSWORD@localhost:3128/"
+        os.environ[
+            "https_proxy"
+        ] = "http://john%40example.com:P%40SSWORD@localhost2:3128/"
+        self.assertEqual(
+            get_proxy_info("echo.websocket.events", True),
+            ("localhost2", 3128, ("john@example.com", "P@SSWORD")),
+        )
 
         os.environ["http_proxy"] = "http://a:b@localhost/"
         os.environ["https_proxy"] = "http://a:b@localhost2/"
         os.environ["no_proxy"] = "example1.com,example2.com"
-        self.assertEqual(get_proxy_info("example.1.com", True), ("localhost2", None, ("a", "b")))
+        self.assertEqual(
+            get_proxy_info("example.1.com", True), ("localhost2", None, ("a", "b"))
+        )
         os.environ["http_proxy"] = "http://a:b@localhost:3128/"
         os.environ["https_proxy"] = "http://a:b@localhost2:3128/"
         os.environ["no_proxy"] = "example1.com,example2.com, echo.websocket.events"
         self.assertEqual(get_proxy_info("echo.websocket.events", True), (None, 0, None))
         os.environ["http_proxy"] = "http://a:b@localhost:3128/"
         os.environ["https_proxy"] = "http://a:b@localhost2:3128/"
         os.environ["no_proxy"] = "example1.com,example2.com, .websocket.events"
```

### Comparing `websocket-client-1.6.4/websocket/tests/test_websocket.py` & `websocket-client-1.7.0/websocket/tests/test_websocket.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # -*- coding: utf-8 -*-
 #
 import os
 import os.path
 import socket
-import websocket as ws
 import unittest
-from websocket._handshake import _create_sec_websocket_key, \
-    _validate as _validate_header
+from base64 import decodebytes as base64decode
+
+import websocket as ws
+from websocket._handshake import _create_sec_websocket_key
+from websocket._handshake import _validate as _validate_header
 from websocket._http import read_headers
 from websocket._utils import validate_utf8
-from base64 import decodebytes as base64decode
 
 """
 test_websocket.py
 websocket - WebSocket client library for Python
 
 Copyright 2023 engn33r
 
@@ -34,19 +35,20 @@
     import ssl
     from ssl import SSLError
 except ImportError:
     # dummy class of SSLError for ssl none-support environment.
     class SSLError(Exception):
         pass
 
+
 # Skip test to access the internet unless TEST_WITH_INTERNET == 1
-TEST_WITH_INTERNET = os.environ.get('TEST_WITH_INTERNET', '0') == '1'
+TEST_WITH_INTERNET = os.environ.get("TEST_WITH_INTERNET", "0") == "1"
 # Skip tests relying on local websockets server unless LOCAL_WS_SERVER_PORT != -1
-LOCAL_WS_SERVER_PORT = os.environ.get('LOCAL_WS_SERVER_PORT', '-1')
-TEST_WITH_LOCAL_SERVER = LOCAL_WS_SERVER_PORT != '-1'
+LOCAL_WS_SERVER_PORT = os.environ.get("LOCAL_WS_SERVER_PORT", "-1")
+TEST_WITH_LOCAL_SERVER = LOCAL_WS_SERVER_PORT != "-1"
 TRACEABLE = True
 
 
 def create_mask_key(_):
     return "abcd"
 
 
@@ -75,15 +77,14 @@
         return len(data)
 
     def close(self):
         pass
 
 
 class HeaderSockMock(SockMock):
-
     def __init__(self, fname):
         SockMock.__init__(self)
         path = os.path.join(os.path.dirname(__file__), fname)
         with open(path, "rb") as f:
             self.add_packet(f.read())
 
 
@@ -99,29 +100,29 @@
         ws.setdefaulttimeout(10)
         self.assertEqual(ws.getdefaulttimeout(), 10)
         ws.setdefaulttimeout(None)
 
     def testWSKey(self):
         key = _create_sec_websocket_key()
         self.assertTrue(key != 24)
-        self.assertTrue(str("¥n") not in key)
+        self.assertTrue("¥n" not in key)
 
     def testNonce(self):
-        """ WebSocket key should be a random 16-byte nonce.
-        """
+        """WebSocket key should be a random 16-byte nonce."""
         key = _create_sec_websocket_key()
         nonce = base64decode(key.encode("utf-8"))
         self.assertEqual(16, len(nonce))
 
     def testWsUtils(self):
         key = "c6b8hTg4EeGb2gQMztV1/g=="
         required_header = {
             "upgrade": "websocket",
             "connection": "upgrade",
-            "sec-websocket-accept": "Kxep+hNu9n51529fGidYu7a3wO0="}
+            "sec-websocket-accept": "Kxep+hNu9n51529fGidYu7a3wO0=",
+        }
         self.assertEqual(_validate_header(required_header, key, None), (True, None))
 
         header = required_header.copy()
         header["upgrade"] = "http"
         self.assertEqual(_validate_header(header, key, None), (False, None))
         del header["upgrade"]
         self.assertEqual(_validate_header(header, key, None), (False, None))
@@ -136,147 +137,162 @@
         header["sec-websocket-accept"] = "something"
         self.assertEqual(_validate_header(header, key, None), (False, None))
         del header["sec-websocket-accept"]
         self.assertEqual(_validate_header(header, key, None), (False, None))
 
         header = required_header.copy()
         header["sec-websocket-protocol"] = "sub1"
-        self.assertEqual(_validate_header(header, key, ["sub1", "sub2"]), (True, "sub1"))
+        self.assertEqual(
+            _validate_header(header, key, ["sub1", "sub2"]), (True, "sub1")
+        )
         # This case will print out a logging error using the error() function, but that is expected
         self.assertEqual(_validate_header(header, key, ["sub2", "sub3"]), (False, None))
 
         header = required_header.copy()
         header["sec-websocket-protocol"] = "sUb1"
-        self.assertEqual(_validate_header(header, key, ["Sub1", "suB2"]), (True, "sub1"))
+        self.assertEqual(
+            _validate_header(header, key, ["Sub1", "suB2"]), (True, "sub1")
+        )
 
         header = required_header.copy()
         # This case will print out a logging error using the error() function, but that is expected
         self.assertEqual(_validate_header(header, key, ["Sub1", "suB2"]), (False, None))
 
     def testReadHeader(self):
-        status, header, status_message = read_headers(HeaderSockMock("data/header01.txt"))
+        status, header, status_message = read_headers(
+            HeaderSockMock("data/header01.txt")
+        )
         self.assertEqual(status, 101)
         self.assertEqual(header["connection"], "Upgrade")
 
-        status, header, status_message = read_headers(HeaderSockMock("data/header03.txt"))
+        status, header, status_message = read_headers(
+            HeaderSockMock("data/header03.txt")
+        )
         self.assertEqual(status, 101)
         self.assertEqual(header["connection"], "Upgrade, Keep-Alive")
 
         HeaderSockMock("data/header02.txt")
-        self.assertRaises(ws.WebSocketException, read_headers, HeaderSockMock("data/header02.txt"))
+        self.assertRaises(
+            ws.WebSocketException, read_headers, HeaderSockMock("data/header02.txt")
+        )
 
     def testSend(self):
         # TODO: add longer frame data
         sock = ws.WebSocket()
         sock.set_mask_key(create_mask_key)
         s = sock.sock = HeaderSockMock("data/header01.txt")
         sock.send("Hello")
-        self.assertEqual(s.sent[0], b'\x81\x85abcd)\x07\x0f\x08\x0e')
+        self.assertEqual(s.sent[0], b"\x81\x85abcd)\x07\x0f\x08\x0e")
 
         sock.send("こんにちは")
-        self.assertEqual(s.sent[1], b'\x81\x8fabcd\x82\xe3\xf0\x87\xe3\xf1\x80\xe5\xca\x81\xe2\xc5\x82\xe3\xcc')
+        self.assertEqual(
+            s.sent[1],
+            b"\x81\x8fabcd\x82\xe3\xf0\x87\xe3\xf1\x80\xe5\xca\x81\xe2\xc5\x82\xe3\xcc",
+        )
 
-#        sock.send("x" * 5000)
-#        self.assertEqual(s.sent[1], b'\x81\x8fabcd\x82\xe3\xf0\x87\xe3\xf1\x80\xe5\xca\x81\xe2\xc5\x82\xe3\xcc")
+        #        sock.send("x" * 5000)
+        #        self.assertEqual(s.sent[1], b'\x81\x8fabcd\x82\xe3\xf0\x87\xe3\xf1\x80\xe5\xca\x81\xe2\xc5\x82\xe3\xcc")
 
-        self.assertEqual(sock.send_binary(b'1111111111101'), 19)
+        self.assertEqual(sock.send_binary(b"1111111111101"), 19)
 
     def testRecv(self):
         # TODO: add longer frame data
         sock = ws.WebSocket()
         s = sock.sock = SockMock()
-        something = b'\x81\x8fabcd\x82\xe3\xf0\x87\xe3\xf1\x80\xe5\xca\x81\xe2\xc5\x82\xe3\xcc'
+        something = (
+            b"\x81\x8fabcd\x82\xe3\xf0\x87\xe3\xf1\x80\xe5\xca\x81\xe2\xc5\x82\xe3\xcc"
+        )
         s.add_packet(something)
         data = sock.recv()
         self.assertEqual(data, "こんにちは")
 
-        s.add_packet(b'\x81\x85abcd)\x07\x0f\x08\x0e')
+        s.add_packet(b"\x81\x85abcd)\x07\x0f\x08\x0e")
         data = sock.recv()
         self.assertEqual(data, "Hello")
 
     @unittest.skipUnless(TEST_WITH_INTERNET, "Internet-requiring tests are disabled")
     def testIter(self):
         count = 2
-        s = ws.create_connection('wss://api.bitfinex.com/ws/2')
+        s = ws.create_connection("wss://api.bitfinex.com/ws/2")
         s.send('{"event": "subscribe", "channel": "ticker"}')
         for _ in s:
             count -= 1
             if count == 0:
                 break
 
     @unittest.skipUnless(TEST_WITH_INTERNET, "Internet-requiring tests are disabled")
     def testNext(self):
-        sock = ws.create_connection('wss://api.bitfinex.com/ws/2')
+        sock = ws.create_connection("wss://api.bitfinex.com/ws/2")
         self.assertEqual(str, type(next(sock)))
 
     def testInternalRecvStrict(self):
         sock = ws.WebSocket()
         s = sock.sock = SockMock()
-        s.add_packet(b'foo')
+        s.add_packet(b"foo")
         s.add_packet(socket.timeout())
-        s.add_packet(b'bar')
+        s.add_packet(b"bar")
         # s.add_packet(SSLError("The read operation timed out"))
-        s.add_packet(b'baz')
+        s.add_packet(b"baz")
         with self.assertRaises(ws.WebSocketTimeoutException):
             sock.frame_buffer.recv_strict(9)
         #     with self.assertRaises(SSLError):
         #         data = sock._recv_strict(9)
         data = sock.frame_buffer.recv_strict(9)
-        self.assertEqual(data, b'foobarbaz')
+        self.assertEqual(data, b"foobarbaz")
         with self.assertRaises(ws.WebSocketConnectionClosedException):
             sock.frame_buffer.recv_strict(1)
 
     def testRecvTimeout(self):
         sock = ws.WebSocket()
         s = sock.sock = SockMock()
-        s.add_packet(b'\x81')
+        s.add_packet(b"\x81")
         s.add_packet(socket.timeout())
-        s.add_packet(b'\x8dabcd\x29\x07\x0f\x08\x0e')
+        s.add_packet(b"\x8dabcd\x29\x07\x0f\x08\x0e")
         s.add_packet(socket.timeout())
-        s.add_packet(b'\x4e\x43\x33\x0e\x10\x0f\x00\x40')
+        s.add_packet(b"\x4e\x43\x33\x0e\x10\x0f\x00\x40")
         with self.assertRaises(ws.WebSocketTimeoutException):
             sock.recv()
         with self.assertRaises(ws.WebSocketTimeoutException):
             sock.recv()
         data = sock.recv()
         self.assertEqual(data, "Hello, World!")
         with self.assertRaises(ws.WebSocketConnectionClosedException):
             sock.recv()
 
     def testRecvWithSimpleFragmentation(self):
         sock = ws.WebSocket()
         s = sock.sock = SockMock()
         # OPCODE=TEXT, FIN=0, MSG="Brevity is "
-        s.add_packet(b'\x01\x8babcd#\x10\x06\x12\x08\x16\x1aD\x08\x11C')
+        s.add_packet(b"\x01\x8babcd#\x10\x06\x12\x08\x16\x1aD\x08\x11C")
         # OPCODE=CONT, FIN=1, MSG="the soul of wit"
-        s.add_packet(b'\x80\x8fabcd\x15\n\x06D\x12\r\x16\x08A\r\x05D\x16\x0b\x17')
+        s.add_packet(b"\x80\x8fabcd\x15\n\x06D\x12\r\x16\x08A\r\x05D\x16\x0b\x17")
         data = sock.recv()
         self.assertEqual(data, "Brevity is the soul of wit")
         with self.assertRaises(ws.WebSocketConnectionClosedException):
             sock.recv()
 
     def testRecvWithFireEventOfFragmentation(self):
         sock = ws.WebSocket(fire_cont_frame=True)
         s = sock.sock = SockMock()
         # OPCODE=TEXT, FIN=0, MSG="Brevity is "
-        s.add_packet(b'\x01\x8babcd#\x10\x06\x12\x08\x16\x1aD\x08\x11C')
+        s.add_packet(b"\x01\x8babcd#\x10\x06\x12\x08\x16\x1aD\x08\x11C")
         # OPCODE=CONT, FIN=0, MSG="Brevity is "
-        s.add_packet(b'\x00\x8babcd#\x10\x06\x12\x08\x16\x1aD\x08\x11C')
+        s.add_packet(b"\x00\x8babcd#\x10\x06\x12\x08\x16\x1aD\x08\x11C")
         # OPCODE=CONT, FIN=1, MSG="the soul of wit"
-        s.add_packet(b'\x80\x8fabcd\x15\n\x06D\x12\r\x16\x08A\r\x05D\x16\x0b\x17')
+        s.add_packet(b"\x80\x8fabcd\x15\n\x06D\x12\r\x16\x08A\r\x05D\x16\x0b\x17")
 
         _, data = sock.recv_data()
-        self.assertEqual(data, b'Brevity is ')
+        self.assertEqual(data, b"Brevity is ")
         _, data = sock.recv_data()
-        self.assertEqual(data, b'Brevity is ')
+        self.assertEqual(data, b"Brevity is ")
         _, data = sock.recv_data()
-        self.assertEqual(data, b'the soul of wit')
+        self.assertEqual(data, b"the soul of wit")
 
         # OPCODE=CONT, FIN=0, MSG="Brevity is "
-        s.add_packet(b'\x80\x8babcd#\x10\x06\x12\x08\x16\x1aD\x08\x11C')
+        s.add_packet(b"\x80\x8babcd#\x10\x06\x12\x08\x16\x1aD\x08\x11C")
 
         with self.assertRaises(ws.WebSocketException):
             sock.recv_data()
 
         with self.assertRaises(ws.WebSocketConnectionClosedException):
             sock.recv()
 
@@ -284,172 +300,208 @@
         sock = ws.WebSocket()
         sock.connected = True
         sock.close
 
         sock = ws.WebSocket()
         s = sock.sock = SockMock()
         sock.connected = True
-        s.add_packet(b'\x88\x80\x17\x98p\x84')
+        s.add_packet(b"\x88\x80\x17\x98p\x84")
         sock.recv()
         self.assertEqual(sock.connected, False)
 
     def testRecvContFragmentation(self):
         sock = ws.WebSocket()
         s = sock.sock = SockMock()
         # OPCODE=CONT, FIN=1, MSG="the soul of wit"
-        s.add_packet(b'\x80\x8fabcd\x15\n\x06D\x12\r\x16\x08A\r\x05D\x16\x0b\x17')
+        s.add_packet(b"\x80\x8fabcd\x15\n\x06D\x12\r\x16\x08A\r\x05D\x16\x0b\x17")
         self.assertRaises(ws.WebSocketException, sock.recv)
 
     def testRecvWithProlongedFragmentation(self):
         sock = ws.WebSocket()
         s = sock.sock = SockMock()
         # OPCODE=TEXT, FIN=0, MSG="Once more unto the breach, "
-        s.add_packet(b'\x01\x9babcd.\x0c\x00\x01A\x0f\x0c\x16\x04B\x16\n\x15\rC\x10\t\x07C\x06\x13\x07\x02\x07\tNC')
+        s.add_packet(
+            b"\x01\x9babcd.\x0c\x00\x01A\x0f\x0c\x16\x04B\x16\n\x15\rC\x10\t\x07C\x06\x13\x07\x02\x07\tNC"
+        )
         # OPCODE=CONT, FIN=0, MSG="dear friends, "
-        s.add_packet(b'\x00\x8eabcd\x05\x07\x02\x16A\x04\x11\r\x04\x0c\x07\x17MB')
+        s.add_packet(b"\x00\x8eabcd\x05\x07\x02\x16A\x04\x11\r\x04\x0c\x07\x17MB")
         # OPCODE=CONT, FIN=1, MSG="once more"
-        s.add_packet(b'\x80\x89abcd\x0e\x0c\x00\x01A\x0f\x0c\x16\x04')
+        s.add_packet(b"\x80\x89abcd\x0e\x0c\x00\x01A\x0f\x0c\x16\x04")
         data = sock.recv()
-        self.assertEqual(
-            data,
-            "Once more unto the breach, dear friends, once more")
+        self.assertEqual(data, "Once more unto the breach, dear friends, once more")
         with self.assertRaises(ws.WebSocketConnectionClosedException):
             sock.recv()
 
     def testRecvWithFragmentationAndControlFrame(self):
         sock = ws.WebSocket()
         sock.set_mask_key(create_mask_key)
         s = sock.sock = SockMock()
         # OPCODE=TEXT, FIN=0, MSG="Too much "
-        s.add_packet(b'\x01\x89abcd5\r\x0cD\x0c\x17\x00\x0cA')
+        s.add_packet(b"\x01\x89abcd5\r\x0cD\x0c\x17\x00\x0cA")
         # OPCODE=PING, FIN=1, MSG="Please PONG this"
-        s.add_packet(b'\x89\x90abcd1\x0e\x06\x05\x12\x07C4.,$D\x15\n\n\x17')
+        s.add_packet(b"\x89\x90abcd1\x0e\x06\x05\x12\x07C4.,$D\x15\n\n\x17")
         # OPCODE=CONT, FIN=1, MSG="of a good thing"
-        s.add_packet(b'\x80\x8fabcd\x0e\x04C\x05A\x05\x0c\x0b\x05B\x17\x0c\x08\x0c\x04')
+        s.add_packet(b"\x80\x8fabcd\x0e\x04C\x05A\x05\x0c\x0b\x05B\x17\x0c\x08\x0c\x04")
         data = sock.recv()
         self.assertEqual(data, "Too much of a good thing")
         with self.assertRaises(ws.WebSocketConnectionClosedException):
             sock.recv()
         self.assertEqual(
-            s.sent[0],
-            b'\x8a\x90abcd1\x0e\x06\x05\x12\x07C4.,$D\x15\n\n\x17')
+            s.sent[0], b"\x8a\x90abcd1\x0e\x06\x05\x12\x07C4.,$D\x15\n\n\x17"
+        )
 
-    @unittest.skipUnless(TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled")
+    @unittest.skipUnless(
+        TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled"
+    )
     def testWebSocket(self):
-        s = ws.create_connection("ws://127.0.0.1:" + LOCAL_WS_SERVER_PORT)
+        s = ws.create_connection(f"ws://127.0.0.1:{LOCAL_WS_SERVER_PORT}")
         self.assertNotEqual(s, None)
         s.send("Hello, World")
         result = s.next()
         s.fileno()
         self.assertEqual(result, "Hello, World")
 
         s.send("こにゃにゃちは、世界")
         result = s.recv()
         self.assertEqual(result, "こにゃにゃちは、世界")
         self.assertRaises(ValueError, s.send_close, -1, "")
         s.close()
 
-    @unittest.skipUnless(TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled")
+    @unittest.skipUnless(
+        TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled"
+    )
     def testPingPong(self):
-        s = ws.create_connection("ws://127.0.0.1:" + LOCAL_WS_SERVER_PORT)
+        s = ws.create_connection(f"ws://127.0.0.1:{LOCAL_WS_SERVER_PORT}")
         self.assertNotEqual(s, None)
         s.ping("Hello")
         s.pong("Hi")
         s.close()
 
     @unittest.skipUnless(TEST_WITH_INTERNET, "Internet-requiring tests are disabled")
     def testSupportRedirect(self):
         s = ws.WebSocket()
-        self.assertRaises(ws._exceptions.WebSocketBadStatusException, s.connect, "ws://google.com/")
+        self.assertRaises(
+            ws._exceptions.WebSocketBadStatusException, s.connect, "ws://google.com/"
+        )
         # Need to find a URL that has a redirect code leading to a websocket
 
     @unittest.skipUnless(TEST_WITH_INTERNET, "Internet-requiring tests are disabled")
     def testSecureWebSocket(self):
         import ssl
+
         s = ws.create_connection("wss://api.bitfinex.com/ws/2")
         self.assertNotEqual(s, None)
         self.assertTrue(isinstance(s.sock, ssl.SSLSocket))
         self.assertEqual(s.getstatus(), 101)
         self.assertNotEqual(s.getheaders(), None)
         s.settimeout(10)
         self.assertEqual(s.gettimeout(), 10)
         self.assertEqual(s.getsubprotocol(), None)
         s.abort()
 
-    @unittest.skipUnless(TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled")
+    @unittest.skipUnless(
+        TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled"
+    )
     def testWebSocketWithCustomHeader(self):
-        s = ws.create_connection("ws://127.0.0.1:" + LOCAL_WS_SERVER_PORT,
-                                 headers={"User-Agent": "PythonWebsocketClient"})
+        s = ws.create_connection(
+            f"ws://127.0.0.1:{LOCAL_WS_SERVER_PORT}",
+            headers={"User-Agent": "PythonWebsocketClient"},
+        )
         self.assertNotEqual(s, None)
         self.assertEqual(s.getsubprotocol(), None)
         s.send("Hello, World")
         result = s.recv()
         self.assertEqual(result, "Hello, World")
         self.assertRaises(ValueError, s.close, -1, "")
         s.close()
 
-    @unittest.skipUnless(TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled")
+    @unittest.skipUnless(
+        TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled"
+    )
     def testAfterClose(self):
-        s = ws.create_connection("ws://127.0.0.1:" + LOCAL_WS_SERVER_PORT)
+        s = ws.create_connection(f"ws://127.0.0.1:{LOCAL_WS_SERVER_PORT}")
         self.assertNotEqual(s, None)
         s.close()
         self.assertRaises(ws.WebSocketConnectionClosedException, s.send, "Hello")
         self.assertRaises(ws.WebSocketConnectionClosedException, s.recv)
 
 
 class SockOptTest(unittest.TestCase):
-    @unittest.skipUnless(TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled")
+    @unittest.skipUnless(
+        TEST_WITH_LOCAL_SERVER, "Tests using local websocket server are disabled"
+    )
     def testSockOpt(self):
         sockopt = ((socket.IPPROTO_TCP, socket.TCP_NODELAY, 1),)
-        s = ws.create_connection("ws://127.0.0.1:" + LOCAL_WS_SERVER_PORT, sockopt=sockopt)
-        self.assertNotEqual(s.sock.getsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY), 0)
+        s = ws.create_connection(
+            f"ws://127.0.0.1:{LOCAL_WS_SERVER_PORT}", sockopt=sockopt
+        )
+        self.assertNotEqual(
+            s.sock.getsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY), 0
+        )
         s.close()
 
 
 class UtilsTest(unittest.TestCase):
     def testUtf8Validator(self):
-        state = validate_utf8(b'\xf0\x90\x80\x80')
+        state = validate_utf8(b"\xf0\x90\x80\x80")
         self.assertEqual(state, True)
-        state = validate_utf8(b'\xce\xba\xe1\xbd\xb9\xcf\x83\xce\xbc\xce\xb5\xed\xa0\x80edited')
+        state = validate_utf8(
+            b"\xce\xba\xe1\xbd\xb9\xcf\x83\xce\xbc\xce\xb5\xed\xa0\x80edited"
+        )
         self.assertEqual(state, False)
-        state = validate_utf8(b'')
+        state = validate_utf8(b"")
         self.assertEqual(state, True)
 
 
 class HandshakeTest(unittest.TestCase):
     @unittest.skipUnless(TEST_WITH_INTERNET, "Internet-requiring tests are disabled")
     def test_http_SSL(self):
-        websock1 = ws.WebSocket(sslopt={"cert_chain": ssl.get_default_verify_paths().capath}, enable_multithread=False)
-        self.assertRaises(ValueError,
-                          websock1.connect, "wss://api.bitfinex.com/ws/2")
+        websock1 = ws.WebSocket(
+            sslopt={"cert_chain": ssl.get_default_verify_paths().capath},
+            enable_multithread=False,
+        )
+        self.assertRaises(ValueError, websock1.connect, "wss://api.bitfinex.com/ws/2")
         websock2 = ws.WebSocket(sslopt={"certfile": "myNonexistentCertFile"})
-        self.assertRaises(FileNotFoundError,
-                          websock2.connect, "wss://api.bitfinex.com/ws/2")
+        self.assertRaises(
+            FileNotFoundError, websock2.connect, "wss://api.bitfinex.com/ws/2"
+        )
 
     @unittest.skipUnless(TEST_WITH_INTERNET, "Internet-requiring tests are disabled")
     def testManualHeaders(self):
-        websock3 = ws.WebSocket(sslopt={"ca_certs": ssl.get_default_verify_paths().cafile,
-                                        "ca_cert_path": ssl.get_default_verify_paths().capath})
-        self.assertRaises(ws._exceptions.WebSocketBadStatusException,
-                          websock3.connect, "wss://api.bitfinex.com/ws/2", cookie="chocolate",
-                          origin="testing_websockets.com",
-                          host="echo.websocket.events/websocket-client-test",
-                          subprotocols=["testproto"],
-                          connection="Upgrade",
-                          header={"CustomHeader1":"123",
-                                  "Cookie":"TestValue",
-                                  "Sec-WebSocket-Key":"k9kFAUWNAMmf5OEMfTlOEA==",
-                                  "Sec-WebSocket-Protocol":"newprotocol"})
+        websock3 = ws.WebSocket(
+            sslopt={
+                "ca_certs": ssl.get_default_verify_paths().cafile,
+                "ca_cert_path": ssl.get_default_verify_paths().capath,
+            }
+        )
+        self.assertRaises(
+            ws._exceptions.WebSocketBadStatusException,
+            websock3.connect,
+            "wss://api.bitfinex.com/ws/2",
+            cookie="chocolate",
+            origin="testing_websockets.com",
+            host="echo.websocket.events/websocket-client-test",
+            subprotocols=["testproto"],
+            connection="Upgrade",
+            header={
+                "CustomHeader1": "123",
+                "Cookie": "TestValue",
+                "Sec-WebSocket-Key": "k9kFAUWNAMmf5OEMfTlOEA==",
+                "Sec-WebSocket-Protocol": "newprotocol",
+            },
+        )
 
     def testIPv6(self):
         websock2 = ws.WebSocket()
         self.assertRaises(ValueError, websock2.connect, "2001:4860:4860::8888")
 
     def testBadURLs(self):
         websock3 = ws.WebSocket()
         self.assertRaises(ValueError, websock3.connect, "ws//example.com")
-        self.assertRaises(ws.WebSocketAddressException, websock3.connect, "ws://example")
+        self.assertRaises(
+            ws.WebSocketAddressException, websock3.connect, "ws://example"
+        )
         self.assertRaises(ValueError, websock3.connect, "example.com")
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `websocket-client-1.6.4/websocket_client.egg-info/PKG-INFO` & `websocket-client-1.7.0/websocket_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: websocket-client
-Version: 1.6.4
+Version: 1.7.0
 Summary: WebSocket client for Python with low level API options
 Home-page: https://github.com/websocket-client/websocket-client.git
+Download-URL: https://github.com/websocket-client/websocket-client/releases
 Author: liris
 Author-email: liris.pp@gmail.com
 Maintainer: engn33r
 Maintainer-email: websocket.client@proton.me
 License: Apache-2.0
-Download-URL: https://github.com/websocket-client/websocket-client/releases
 Project-URL: Documentation, https://websocket-client.readthedocs.io/
 Project-URL: Source, https://github.com/websocket-client/websocket-client/
 Keywords: websockets client
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -25,24 +24,31 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: optional
-Provides-Extra: test
 License-File: LICENSE
+Provides-Extra: test
+Requires-Dist: websockets; extra == "test"
+Provides-Extra: optional
+Requires-Dist: python-socks; extra == "optional"
+Requires-Dist: wsaccel; extra == "optional"
+Provides-Extra: docs
+Requires-Dist: Sphinx>=6.0; extra == "docs"
+Requires-Dist: sphinx_rtd_theme>=1.1.0; extra == "docs"
 
 [![docs](https://readthedocs.org/projects/websocket-client/badge/?style=flat)](https://websocket-client.readthedocs.io/)
 [![Build Status](https://github.com/websocket-client/websocket-client/actions/workflows/build.yml/badge.svg)](https://github.com/websocket-client/websocket-client/actions/workflows/build.yml)
 [![codecov](https://codecov.io/gh/websocket-client/websocket-client/branch/master/graph/badge.svg?token=pcXhUQwiL3)](https://codecov.io/gh/websocket-client/websocket-client)
 [![PyPI Downloads](https://pepy.tech/badge/websocket-client)](https://pepy.tech/project/websocket-client)
 [![PyPI version](https://img.shields.io/pypi/v/websocket_client)](https://pypi.org/project/websocket_client/)
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # websocket-client
 
 websocket-client is a WebSocket client for Python. It provides access
 to low level APIs for WebSockets. websocket-client implements version
 [hybi-13](https://tools.ietf.org/html/draft-ietf-hybi-thewebsocketprotocol-13)
 of the WebSocket protocol. This client does not currently support the
@@ -171,9 +177,7 @@
 ws.send("Hello, World")
 print("Sent")
 print("Receiving...")
 result =  ws.recv()
 print("Received '%s'" % result)
 ws.close()
 ```
-
-
```

### Comparing `websocket-client-1.6.4/websocket_client.egg-info/SOURCES.txt` & `websocket-client-1.7.0/websocket_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 websocket/_http.py
 websocket/_logging.py
 websocket/_socket.py
 websocket/_ssl_compat.py
 websocket/_url.py
 websocket/_utils.py
 websocket/_wsdump.py
+websocket/py.typed
 websocket/tests/__init__.py
 websocket/tests/echo-server.py
 websocket/tests/test_abnf.py
 websocket/tests/test_app.py
 websocket/tests/test_cookiejar.py
 websocket/tests/test_http.py
 websocket/tests/test_url.py
```

