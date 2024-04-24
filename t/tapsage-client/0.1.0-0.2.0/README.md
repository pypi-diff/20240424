# Comparing `tmp/tapsage_client-0.1.0.tar.gz` & `tmp/tapsage_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tapsage_client-0.1.0.tar", last modified: Wed Apr 24 10:48:04 2024, max compression
+gzip compressed data, was "tapsage_client-0.2.0.tar", last modified: Wed Apr 24 11:52:50 2024, max compression
```

## Comparing `tapsage_client-0.1.0.tar` & `tapsage_client-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-24 10:48:04.169835 tapsage_client-0.1.0/
--rw-rw-r--   0 ali       (1001) ali       (1001)    11357 2024-04-24 02:49:05.000000 tapsage_client-0.1.0/LICENSE
--rw-r--r--   0 ali       (1001) ali       (1001)      585 2024-04-24 10:48:04.165835 tapsage_client-0.1.0/PKG-INFO
--rw-rw-r--   0 ali       (1001) ali       (1001)      160 2024-04-24 02:49:05.000000 tapsage_client-0.1.0/README.md
--rw-rw-r--   0 ali       (1001) ali       (1001)       38 2024-04-24 10:48:04.169835 tapsage_client-0.1.0/setup.cfg
--rw-rw-r--   0 ali       (1001) ali       (1001)     1017 2024-04-24 10:47:56.000000 tapsage_client-0.1.0/setup.py
-drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-24 10:48:04.165835 tapsage_client-0.1.0/tapsage/
--rw-rw-r--   0 ali       (1001) ali       (1001)       49 2024-04-24 10:42:59.000000 tapsage_client-0.1.0/tapsage/__init__.py
--rw-rw-r--   0 ali       (1001) ali       (1001)     5625 2024-04-24 10:42:57.000000 tapsage_client-0.1.0/tapsage/tapsagebot.py
--rw-rw-r--   0 ali       (1001) ali       (1001)     2760 2024-04-24 10:42:56.000000 tapsage_client-0.1.0/tapsage/taptypes.py
--rw-rw-r--   0 ali       (1001) ali       (1001)     1231 2024-04-24 10:41:51.000000 tapsage_client-0.1.0/tapsage/tapuser.py
--rw-rw-r--   0 ali       (1001) ali       (1001)     2065 2024-04-24 10:41:51.000000 tapsage_client-0.1.0/tapsage/test.py
-drwxrwxr-x   0 ali       (1001) ali       (1001)        0 2024-04-24 10:48:04.165835 tapsage_client-0.1.0/tapsage_client.egg-info/
--rw-r--r--   0 ali       (1001) ali       (1001)      585 2024-04-24 10:48:03.000000 tapsage_client-0.1.0/tapsage_client.egg-info/PKG-INFO
--rw-rw-r--   0 ali       (1001) ali       (1001)      312 2024-04-24 10:48:04.000000 tapsage_client-0.1.0/tapsage_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ali       (1001) ali       (1001)        1 2024-04-24 10:48:03.000000 tapsage_client-0.1.0/tapsage_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ali       (1001) ali       (1001)        1 2024-04-24 10:48:03.000000 tapsage_client-0.1.0/tapsage_client.egg-info/not-zip-safe
--rw-rw-r--   0 ali       (1001) ali       (1001)        8 2024-04-24 10:48:03.000000 tapsage_client-0.1.0/tapsage_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:52:50.763165 tapsage_client-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 11:52:43.000000 tapsage_client-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-24 11:52:50.763165 tapsage_client-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-24 11:52:43.000000 tapsage_client-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 11:52:50.763165 tapsage_client-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-24 11:52:43.000000 tapsage_client-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:52:50.763165 tapsage_client-0.2.0/tapsage/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-24 11:52:43.000000 tapsage_client-0.2.0/tapsage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-24 11:52:43.000000 tapsage_client-0.2.0/tapsage/tapsagebot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-24 11:52:43.000000 tapsage_client-0.2.0/tapsage/taptypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-24 11:52:43.000000 tapsage_client-0.2.0/tapsage/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:52:50.763165 tapsage_client-0.2.0/tapsage_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-24 11:52:50.000000 tapsage_client-0.2.0/tapsage_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-24 11:52:50.000000 tapsage_client-0.2.0/tapsage_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:52:50.000000 tapsage_client-0.2.0/tapsage_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:52:50.000000 tapsage_client-0.2.0/tapsage_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 11:52:50.000000 tapsage_client-0.2.0/tapsage_client.egg-info/top_level.txt
```

### Comparing `tapsage_client-0.1.0/LICENSE` & `tapsage_client-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tapsage_client-0.1.0/PKG-INFO` & `tapsage_client-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tapsage_client
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python client for Tapsage to streamline API interactions, enabling easy management and customization of AI-driven chatbots and image models.
 Home-page: https://github.com/mahdikiani/tapsage-python
 Author: Mahdi Kiani
 Author-email: mahdikiany@gmail.com
 License: Apache-2.0
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `tapsage_client-0.1.0/setup.py` & `tapsage_client-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `tapsage_client-0.1.0/tapsage/tapsagebot.py` & `tapsage_client-0.2.0/tapsage/tapsagebot.py`

 * *Files identical despite different names*

### Comparing `tapsage_client-0.1.0/tapsage/taptypes.py` & `tapsage_client-0.2.0/tapsage/taptypes.py`

 * *Files identical despite different names*

### Comparing `tapsage_client-0.1.0/tapsage/test.py` & `tapsage_client-0.2.0/tapsage/test.py`

 * *Files identical despite different names*

### Comparing `tapsage_client-0.1.0/tapsage_client.egg-info/PKG-INFO` & `tapsage_client-0.2.0/tapsage_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tapsage_client
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python client for Tapsage to streamline API interactions, enabling easy management and customization of AI-driven chatbots and image models.
 Home-page: https://github.com/mahdikiani/tapsage-python
 Author: Mahdi Kiani
 Author-email: mahdikiany@gmail.com
 License: Apache-2.0
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

