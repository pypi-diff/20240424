# Comparing `tmp/tapsage_client-0.2.0.tar.gz` & `tmp/tapsage_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tapsage_client-0.2.0.tar", last modified: Wed Apr 24 11:52:50 2024, max compression
+gzip compressed data, was "tapsage_client-0.3.0.tar", last modified: Wed Apr 24 13:18:07 2024, max compression
```

## Comparing `tapsage_client-0.2.0.tar` & `tapsage_client-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:52:50.763165 tapsage_client-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 11:52:43.000000 tapsage_client-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-24 11:52:50.763165 tapsage_client-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-24 11:52:43.000000 tapsage_client-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 11:52:50.763165 tapsage_client-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-24 11:52:43.000000 tapsage_client-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:52:50.763165 tapsage_client-0.2.0/tapsage/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-24 11:52:43.000000 tapsage_client-0.2.0/tapsage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-24 11:52:43.000000 tapsage_client-0.2.0/tapsage/tapsagebot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-24 11:52:43.000000 tapsage_client-0.2.0/tapsage/taptypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-24 11:52:43.000000 tapsage_client-0.2.0/tapsage/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:52:50.763165 tapsage_client-0.2.0/tapsage_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-24 11:52:50.000000 tapsage_client-0.2.0/tapsage_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-24 11:52:50.000000 tapsage_client-0.2.0/tapsage_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:52:50.000000 tapsage_client-0.2.0/tapsage_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:52:50.000000 tapsage_client-0.2.0/tapsage_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 11:52:50.000000 tapsage_client-0.2.0/tapsage_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:18:07.106743 tapsage_client-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 13:18:03.000000 tapsage_client-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-24 13:18:07.106743 tapsage_client-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-24 13:18:03.000000 tapsage_client-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:18:07.106743 tapsage_client-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-24 13:18:03.000000 tapsage_client-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:18:07.102743 tapsage_client-0.3.0/tapsage/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-24 13:18:03.000000 tapsage_client-0.3.0/tapsage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-04-24 13:18:03.000000 tapsage_client-0.3.0/tapsage/tapsagebot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-24 13:18:03.000000 tapsage_client-0.3.0/tapsage/taptypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-24 13:18:03.000000 tapsage_client-0.3.0/tapsage/tapuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-24 13:18:03.000000 tapsage_client-0.3.0/tapsage/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:18:07.106743 tapsage_client-0.3.0/tapsage_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-24 13:18:07.000000 tapsage_client-0.3.0/tapsage_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-24 13:18:07.000000 tapsage_client-0.3.0/tapsage_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:18:07.000000 tapsage_client-0.3.0/tapsage_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:18:06.000000 tapsage_client-0.3.0/tapsage_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 13:18:07.000000 tapsage_client-0.3.0/tapsage_client.egg-info/top_level.txt
```

### Comparing `tapsage_client-0.2.0/LICENSE` & `tapsage_client-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tapsage_client-0.2.0/setup.py` & `tapsage_client-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `tapsage_client-0.2.0/tapsage/tapsagebot.py` & `tapsage_client-0.3.0/tapsage/tapsagebot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import uuid
 
 import requests
-from taptypes import (
+from .taptypes import (
     Message,
     MessageContent,
     MessageRequest,
     MessageStream,
     Session,
     SessionRequest,
     SessionUser,
```

### Comparing `tapsage_client-0.2.0/tapsage/taptypes.py` & `tapsage_client-0.3.0/tapsage/taptypes.py`

 * *Files identical despite different names*

### Comparing `tapsage_client-0.2.0/tapsage/test.py` & `tapsage_client-0.3.0/tapsage/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class TestTapSageBot(unittest.TestCase):
     def __init__(self, *args, **kwargs):
         super(self.__class__, self).__init__(*args, **kwargs)
         api_key = os.getenv("TAPSAGE_API_KEY")
         bot_id = os.getenv("TAPSAGE_BOT_ID")
         self.tapbot = TapSageBot(api_key, bot_id)
-        self.prompt = "Sugegst me a list of 5 gifts for a 30 years boy who is tech-fan."
+        self.prompt = "Suggest me a list of 5 gifts for a 30 years boy who is tech-fan."
 
     def test_message(self):
         print()
         print("test_message")
         session = self.tapbot.create_session()
         message = self.tapbot.send_message(session, self.prompt)
         print(message.content)
```

