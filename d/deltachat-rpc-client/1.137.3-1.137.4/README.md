# Comparing `tmp/deltachat_rpc_client-1.137.3.tar.gz` & `tmp/deltachat_rpc_client-1.137.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltachat_rpc_client-1.137.3.tar", last modified: Thu Apr 18 03:06:39 2024, max compression
+gzip compressed data, was "deltachat_rpc_client-1.137.4.tar", last modified: Wed Apr 24 11:40:37 2024, max compression
```

## Comparing `deltachat_rpc_client-1.137.3.tar` & `deltachat_rpc_client-1.137.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:06:39.613222 deltachat_rpc_client-1.137.3/
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-18 03:06:39.613222 deltachat_rpc_client-1.137.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 03:06:39.613222 deltachat_rpc_client-1.137.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:06:39.605222 deltachat_rpc_client-1.137.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:06:39.609222 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13391 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/deltachat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/direct_imap.py
--rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/message.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/pytestplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:06:39.613222 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-18 03:06:39.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-18 03:06:39.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 03:06:39.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-18 03:06:39.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 03:06:39.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 03:06:39.000000 deltachat_rpc_client-1.137.3/src/deltachat_rpc_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:06:39.613222 deltachat_rpc_client-1.137.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/tests/test_chatlist_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    24172 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/tests/test_securejoin.py
--rw-r--r--   0 runner    (1001) docker     (127)    21143 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/tests/test_something.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-18 03:06:33.000000 deltachat_rpc_client-1.137.3/tests/test_webxdc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:40:37.832521 deltachat_rpc_client-1.137.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-24 11:40:28.000000 deltachat_rpc_client-1.137.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-24 11:40:37.832521 deltachat_rpc_client-1.137.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-24 11:40:28.000000 deltachat_rpc_client-1.137.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-24 11:40:28.000000 deltachat_rpc_client-1.137.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 11:40:37.832521 deltachat_rpc_client-1.137.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:40:37.828521 deltachat_rpc_client-1.137.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:40:37.832521 deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-24 11:40:28.000000 deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-24 11:40:28.000000 deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13369 2024-04-24 11:40:28.000000 deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-04-24 11:40:28.000000 deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-24 11:40:28.000000 deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-24 11:40:28.000000 deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-24 11:40:28.000000 deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-24 11:40:28.000000 deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/deltachat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-04-24 11:40:28.000000 deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/direct_imap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-04-24 11:40:28.000000 deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-24 11:40:28.000000 deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-24 11:40:28.000000 deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-24 11:40:28.000000 deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/pytestplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-24 11:40:28.000000 deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:40:37.832521 deltachat_rpc_client-1.137.4/src/deltachat_rpc_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-24 11:40:37.000000 deltachat_rpc_client-1.137.4/src/deltachat_rpc_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-24 11:40:37.000000 deltachat_rpc_client-1.137.4/src/deltachat_rpc_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:40:37.000000 deltachat_rpc_client-1.137.4/src/deltachat_rpc_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-24 11:40:37.000000 deltachat_rpc_client-1.137.4/src/deltachat_rpc_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 11:40:37.000000 deltachat_rpc_client-1.137.4/src/deltachat_rpc_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 11:40:37.000000 deltachat_rpc_client-1.137.4/src/deltachat_rpc_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:40:37.832521 deltachat_rpc_client-1.137.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-04-24 11:40:28.000000 deltachat_rpc_client-1.137.4/tests/test_chatlist_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24172 2024-04-24 11:40:28.000000 deltachat_rpc_client-1.137.4/tests/test_securejoin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22129 2024-04-24 11:40:28.000000 deltachat_rpc_client-1.137.4/tests/test_something.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-24 11:40:28.000000 deltachat_rpc_client-1.137.4/tests/test_webxdc.py
```

### Comparing `deltachat_rpc_client-1.137.3/LICENSE` & `deltachat_rpc_client-1.137.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.137.3/PKG-INFO` & `deltachat_rpc_client-1.137.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat-rpc-client
-Version: 1.137.3
+Version: 1.137.4
 Summary: Python client for Delta Chat core JSON-RPC interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deltachat_rpc_client-1.137.3/README.md` & `deltachat_rpc_client-1.137.4/README.md`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.137.3/pyproject.toml` & `deltachat_rpc_client-1.137.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "deltachat-rpc-client"
-version = "1.137.3"
+version = "1.137.4"
 description = "Python client for Delta Chat core JSON-RPC interface"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
```

### Comparing `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/__init__.py` & `deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/_utils.py` & `deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/_utils.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/account.py` & `deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,15 +240,15 @@
     def secure_join(self, qrdata: str) -> Chat:
         """Continue a Setup-Contact or Verified-Group-Invite protocol started on
         another device.
 
         The function returns immediately and the handshake runs in background, sending
         and receiving several messages.
         Subsequent calls of `secure_join()` will abort previous, unfinished handshakes.
-        See https://securejoin.readthedocs.io/en/latest/new.html for protocol details.
+        See https://securejoin.delta.chat/ for protocol details.
 
         :param qrdata: The text of the scanned QR code.
         """
         return Chat(self, self._rpc.secure_join(self.id, qrdata))
 
     def get_qr_code(self) -> tuple[str, str]:
         """Get Setup-Contact QR Code text and SVG data.
```

### Comparing `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/chat.py` & `deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/chat.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/client.py` & `deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/client.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/const.py` & `deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/const.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/contact.py` & `deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/contact.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/deltachat.py` & `deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/deltachat.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/direct_imap.py` & `deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/direct_imap.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/events.py` & `deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/events.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/message.py` & `deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/message.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/pytestplugin.py` & `deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/pytestplugin.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client/rpc.py` & `deltachat_rpc_client-1.137.4/src/deltachat_rpc_client/rpc.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client.egg-info/PKG-INFO` & `deltachat_rpc_client-1.137.4/src/deltachat_rpc_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat-rpc-client
-Version: 1.137.3
+Version: 1.137.4
 Summary: Python client for Delta Chat core JSON-RPC interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deltachat_rpc_client-1.137.3/src/deltachat_rpc_client.egg-info/SOURCES.txt` & `deltachat_rpc_client-1.137.4/src/deltachat_rpc_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.137.3/tests/test_chatlist_events.py` & `deltachat_rpc_client-1.137.4/tests/test_chatlist_events.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.137.3/tests/test_securejoin.py` & `deltachat_rpc_client-1.137.4/tests/test_securejoin.py`

 * *Files identical despite different names*

### Comparing `deltachat_rpc_client-1.137.3/tests/test_something.py` & `deltachat_rpc_client-1.137.4/tests/test_something.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import subprocess
 import time
 from unittest.mock import MagicMock
 
 import pytest
 from deltachat_rpc_client import Contact, EventType, Message, events
-from deltachat_rpc_client.const import DownloadState
+from deltachat_rpc_client.const import DownloadState, MessageState
 from deltachat_rpc_client.direct_imap import DirectImap
 from deltachat_rpc_client.rpc import JsonRpcError
 
 
 def test_system_info(rpc) -> None:
     system_info = rpc.get_system_info()
     assert "arch" in system_info
@@ -580,7 +580,36 @@
         else:
             # Group contains only Alice and Bob,
             # so partially downloaded messages are
             # hard to distinguish from private replies to group messages.
             #
             # Message may be a private reply, so we assign it to 1:1 chat with Alice.
             assert snapshot.chat == bob_chat_alice
+
+
+def test_markseen_contact_request(acfactory, tmp_path):
+    """
+    Test that seen status is synchronized for contact request messages
+    even though read receipt is not sent.
+    """
+    alice, bob = acfactory.get_online_accounts(2)
+
+    # Bob sets up a second device.
+    bob.export_backup(tmp_path)
+    files = list(tmp_path.glob("*.tar"))
+    bob2 = acfactory.get_unconfigured_account()
+    bob2.import_backup(files[0])
+    bob2.start_io()
+
+    alice_chat_bob = alice.create_chat(bob)
+    alice_chat_bob.send_text("Hello Bob!")
+
+    message = bob.get_message_by_id(bob.wait_for_incoming_msg_event().msg_id)
+    message2 = bob2.get_message_by_id(bob2.wait_for_incoming_msg_event().msg_id)
+    assert message2.get_snapshot().state == MessageState.IN_FRESH
+
+    message.mark_seen()
+    while True:
+        event = bob2.wait_for_event()
+        if event.kind == EventType.MSGS_NOTICED:
+            break
+    assert message2.get_snapshot().state == MessageState.IN_SEEN
```

### Comparing `deltachat_rpc_client-1.137.3/tests/test_webxdc.py` & `deltachat_rpc_client-1.137.4/tests/test_webxdc.py`

 * *Files identical despite different names*

