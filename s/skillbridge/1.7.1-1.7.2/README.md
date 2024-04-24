# Comparing `tmp/skillbridge-1.7.1.tar.gz` & `tmp/skillbridge-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skillbridge-1.7.1.tar", last modified: Thu Apr 11 09:10:48 2024, max compression
+gzip compressed data, was "skillbridge-1.7.2.tar", last modified: Wed Apr 24 07:30:48 2024, max compression
```

## Comparing `skillbridge-1.7.1.tar` & `skillbridge-1.7.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:10:48.320073 skillbridge-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-11 09:10:35.000000 skillbridge-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-11 09:10:35.000000 skillbridge-1.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12733 2024-04-11 09:10:48.320073 skillbridge-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-11 09:10:35.000000 skillbridge-1.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-11 09:10:35.000000 skillbridge-1.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 09:10:48.320073 skillbridge-1.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:10:48.312073 skillbridge-1.7.1/skillbridge/
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:10:48.316073 skillbridge-1.7.1/skillbridge/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/client/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/client/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/client/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/client/hints.py
--rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/client/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/client/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/client/translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/client/var.py
--rw-r--r--   0 runner    (1001) docker     (127)    10754 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/client/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:10:48.316073 skillbridge-1.7.1/skillbridge/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/server/python_server.il
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/server/python_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:10:48.316073 skillbridge-1.7.1/skillbridge/test/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/test/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/test/translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/test/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 09:10:45.000000 skillbridge-1.7.1/skillbridge/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:10:48.320073 skillbridge-1.7.1/skillbridge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12733 2024-04-11 09:10:48.000000 skillbridge-1.7.1/skillbridge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-11 09:10:48.000000 skillbridge-1.7.1/skillbridge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:10:48.000000 skillbridge-1.7.1/skillbridge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-11 09:10:48.000000 skillbridge-1.7.1/skillbridge.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-11 09:10:48.000000 skillbridge-1.7.1/skillbridge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 09:10:48.000000 skillbridge-1.7.1/skillbridge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:10:48.320073 skillbridge-1.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-04-11 09:10:35.000000 skillbridge-1.7.1/tests/test_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-11 09:10:35.000000 skillbridge-1.7.1/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-11 09:10:35.000000 skillbridge-1.7.1/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-11 09:10:35.000000 skillbridge-1.7.1/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-11 09:10:35.000000 skillbridge-1.7.1/tests/test_test_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8367 2024-04-11 09:10:35.000000 skillbridge-1.7.1/tests/test_translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-11 09:10:35.000000 skillbridge-1.7.1/tests/test_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-11 09:10:35.000000 skillbridge-1.7.1/tests/test_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:30:48.816184 skillbridge-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-24 07:30:39.000000 skillbridge-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 07:30:39.000000 skillbridge-1.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12733 2024-04-24 07:30:48.816184 skillbridge-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-24 07:30:39.000000 skillbridge-1.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-24 07:30:39.000000 skillbridge-1.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 07:30:48.816184 skillbridge-1.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:30:48.812184 skillbridge-1.7.2/skillbridge/
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-24 07:30:39.000000 skillbridge-1.7.2/skillbridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-24 07:30:39.000000 skillbridge-1.7.2/skillbridge/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:30:48.812184 skillbridge-1.7.2/skillbridge/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:30:39.000000 skillbridge-1.7.2/skillbridge/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-24 07:30:39.000000 skillbridge-1.7.2/skillbridge/client/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-24 07:30:39.000000 skillbridge-1.7.2/skillbridge/client/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-24 07:30:39.000000 skillbridge-1.7.2/skillbridge/client/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-24 07:30:39.000000 skillbridge-1.7.2/skillbridge/client/hints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-04-24 07:30:39.000000 skillbridge-1.7.2/skillbridge/client/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-24 07:30:39.000000 skillbridge-1.7.2/skillbridge/client/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-04-24 07:30:39.000000 skillbridge-1.7.2/skillbridge/client/translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-24 07:30:39.000000 skillbridge-1.7.2/skillbridge/client/var.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10754 2024-04-24 07:30:39.000000 skillbridge-1.7.2/skillbridge/client/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:30:39.000000 skillbridge-1.7.2/skillbridge/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:30:48.812184 skillbridge-1.7.2/skillbridge/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:30:39.000000 skillbridge-1.7.2/skillbridge/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-24 07:30:39.000000 skillbridge-1.7.2/skillbridge/server/python_server.il
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-04-24 07:30:39.000000 skillbridge-1.7.2/skillbridge/server/python_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:30:48.816184 skillbridge-1.7.2/skillbridge/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-24 07:30:39.000000 skillbridge-1.7.2/skillbridge/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-24 07:30:39.000000 skillbridge-1.7.2/skillbridge/test/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-24 07:30:39.000000 skillbridge-1.7.2/skillbridge/test/translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-24 07:30:39.000000 skillbridge-1.7.2/skillbridge/test/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 07:30:46.000000 skillbridge-1.7.2/skillbridge/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:30:48.816184 skillbridge-1.7.2/skillbridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12733 2024-04-24 07:30:48.000000 skillbridge-1.7.2/skillbridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-24 07:30:48.000000 skillbridge-1.7.2/skillbridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 07:30:48.000000 skillbridge-1.7.2/skillbridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 07:30:48.000000 skillbridge-1.7.2/skillbridge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-24 07:30:48.000000 skillbridge-1.7.2/skillbridge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 07:30:48.000000 skillbridge-1.7.2/skillbridge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:30:48.816184 skillbridge-1.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-04-24 07:30:39.000000 skillbridge-1.7.2/tests/test_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-24 07:30:39.000000 skillbridge-1.7.2/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-24 07:30:39.000000 skillbridge-1.7.2/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-24 07:30:39.000000 skillbridge-1.7.2/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-24 07:30:39.000000 skillbridge-1.7.2/tests/test_test_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8367 2024-04-24 07:30:39.000000 skillbridge-1.7.2/tests/test_translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-24 07:30:39.000000 skillbridge-1.7.2/tests/test_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-24 07:30:39.000000 skillbridge-1.7.2/tests/test_workspace.py
```

### Comparing `skillbridge-1.7.1/LICENSE` & `skillbridge-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/PKG-INFO` & `skillbridge-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skillbridge
-Version: 1.7.1
+Version: 1.7.2
 Summary: A seamless Python remote bridge to Cadence's Skill in Virtuoso
 Author-email: Niels Buwen <dev@niels-buwen.de>, Tobias Markus <tobias_markus@gmx.net>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `skillbridge-1.7.1/README.md` & `skillbridge-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/pyproject.toml` & `skillbridge-1.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/skillbridge/__init__.py` & `skillbridge-1.7.2/skillbridge/__init__.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/skillbridge/__main__.py` & `skillbridge-1.7.2/skillbridge/__main__.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/skillbridge/client/channel.py` & `skillbridge-1.7.2/skillbridge/client/channel.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
             message = b''.join(self._receive_all(length))
         except Exception as e:  # noqa: BLE001
             return e
         return message.decode()
 
     def close(self) -> None:
         if self.connected:
-            self.socket.sendall(b'         5$close')
+            self.socket.sendall(b'         6$close')
             self.socket.close()
             self.connected = False
 
     def flush(self) -> None:
         while True:
             read, _, _ = select([self.socket], [], [], 0.1)
             if read:
```

### Comparing `skillbridge-1.7.1/skillbridge/client/functions.py` & `skillbridge-1.7.2/skillbridge/client/functions.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/skillbridge/client/globals.py` & `skillbridge-1.7.2/skillbridge/client/globals.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/skillbridge/client/hints.py` & `skillbridge-1.7.2/skillbridge/client/hints.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/skillbridge/client/objects.py` & `skillbridge-1.7.2/skillbridge/client/objects.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/skillbridge/client/remote.py` & `skillbridge-1.7.2/skillbridge/client/remote.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/skillbridge/client/translator.py` & `skillbridge-1.7.2/skillbridge/client/translator.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/skillbridge/client/var.py` & `skillbridge-1.7.2/skillbridge/client/var.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/skillbridge/client/workspace.py` & `skillbridge-1.7.2/skillbridge/client/workspace.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/skillbridge/server/python_server.il` & `skillbridge-1.7.2/skillbridge/server/python_server.il`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/skillbridge/server/python_server.py` & `skillbridge-1.7.2/skillbridge/server/python_server.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/skillbridge/test/channel.py` & `skillbridge-1.7.2/skillbridge/test/channel.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/skillbridge/test/translator.py` & `skillbridge-1.7.2/skillbridge/test/translator.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/skillbridge/test/workspace.py` & `skillbridge-1.7.2/skillbridge/test/workspace.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/skillbridge.egg-info/PKG-INFO` & `skillbridge-1.7.2/skillbridge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skillbridge
-Version: 1.7.1
+Version: 1.7.2
 Summary: A seamless Python remote bridge to Cadence's Skill in Virtuoso
 Author-email: Niels Buwen <dev@niels-buwen.de>, Tobias Markus <tobias_markus@gmx.net>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `skillbridge-1.7.1/skillbridge.egg-info/SOURCES.txt` & `skillbridge-1.7.2/skillbridge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/tests/test_channel.py` & `skillbridge-1.7.2/tests/test_channel.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/tests/test_integration.py` & `skillbridge-1.7.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/tests/test_misc.py` & `skillbridge-1.7.2/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/tests/test_server.py` & `skillbridge-1.7.2/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/tests/test_test_channel.py` & `skillbridge-1.7.2/tests/test_test_channel.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/tests/test_translator.py` & `skillbridge-1.7.2/tests/test_translator.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/tests/test_var.py` & `skillbridge-1.7.2/tests/test_var.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.1/tests/test_workspace.py` & `skillbridge-1.7.2/tests/test_workspace.py`

 * *Files identical despite different names*

