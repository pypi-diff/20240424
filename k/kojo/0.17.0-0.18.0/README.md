# Comparing `tmp/kojo-0.17.0.tar.gz` & `tmp/kojo-0.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kojo-0.17.0.tar", last modified: Sun May 21 11:07:53 2023, max compression
+gzip compressed data, was "kojo-0.18.0.tar", last modified: Tue Apr 23 12:08:42 2024, max compression
```

## Comparing `kojo-0.17.0.tar` & `kojo-0.18.0.tar`

### file list

```diff
@@ -1,12 +1,9 @@
-drwxr-xr-x   0 olaf       (501) staff       (20)        0 2023-05-21 11:07:53.000000 kojo-0.17.0/
-drwxr-xr-x   0 olaf       (501) staff       (20)        0 2023-05-21 11:07:53.000000 kojo-0.17.0/kojo/
--rw-r--r--   0 olaf       (501) staff       (20)      454 2023-05-20 06:51:50.000000 kojo-0.17.0/kojo/duplicatefinder.py
--rw-r--r--   0 olaf       (501) staff       (20)     2188 2023-05-20 19:17:09.000000 kojo-0.17.0/kojo/io.py
--rw-r--r--   0 olaf       (501) staff       (20)      142 2023-05-20 06:51:50.000000 kojo-0.17.0/kojo/__init__.py
--rw-r--r--   0 olaf       (501) staff       (20)      947 2023-05-20 06:51:50.000000 kojo-0.17.0/kojo/jsonschemavalidator.py
--rw-r--r--   0 olaf       (501) staff       (20)     1314 2023-05-21 10:39:01.000000 kojo-0.17.0/kojo/process.py
--rw-r--r--   0 olaf       (501) staff       (20)     1844 2023-05-20 06:51:50.000000 kojo-0.17.0/kojo/propertiesconverter.py
--rw-r--r--   0 olaf       (501) staff       (20)     4108 2023-05-20 07:57:15.000000 kojo-0.17.0/kojo/item.py
--rw-r--r--   0 olaf       (501) staff       (20)      561 2023-05-21 11:07:53.000000 kojo-0.17.0/PKG-INFO
--rw-r--r--   0 olaf       (501) staff       (20)      693 2023-05-21 11:02:26.000000 kojo-0.17.0/setup.py
--rw-r--r--   0 olaf       (501) staff       (20)       39 2023-05-20 06:51:50.000000 kojo-0.17.0/setup.cfg
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-23 12:08:42.103149 kojo-0.18.0/
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      561 2024-04-23 12:08:42.103149 kojo-0.18.0/PKG-INFO
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-23 12:08:42.103149 kojo-0.18.0/kojo/
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      142 2023-04-27 08:51:59.007066 kojo-0.18.0/kojo/__init__.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     2188 2023-05-22 08:05:06.162114 kojo-0.18.0/kojo/io.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     4886 2024-04-23 12:07:56.515686 kojo-0.18.0/kojo/item.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     1718 2024-04-23 12:07:56.515686 kojo-0.18.0/kojo/process.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)       39 2023-04-27 08:31:58.877706 kojo-0.18.0/setup.cfg
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      693 2024-04-23 12:07:56.515686 kojo-0.18.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `kojo-0.17.0/kojo/io.py` & `kojo-0.18.0/kojo/io.py`

 * *Files identical despite different names*

### Comparing `kojo-0.17.0/kojo/item.py` & `kojo-0.18.0/kojo/item.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,147 +1,168 @@
+from __future__ import annotations
 import copy
 import json
 import logging
+from typing import Any
 
 
-def flatten(item, prefix=""):
+def _flatten(item: dict[str, Any], prefix: str = "") -> dict[str, Any]:
     flat_dict = {}
     for k, v in item.items():
         kk = k
         if prefix:
             kk = prefix + "." + k
 
         if type(v) is dict:
-            for ksub, vsub in flatten(v, kk).items():
+            for ksub, vsub in _flatten(v, kk).items():
                 flat_dict[ksub] = vsub
         else:
             flat_dict[kk] = v
     return flat_dict
 
 
 class ItemLogEntry:
-    def __init__(self, _level, _message, **details):
+    level: int  # logging.NOTSET .. logging.CRITICAL
+    message: str
+    details: dict[str, Any]
+
+    def __init__(self, _level: int, _message: str, **details: Any):
         self.level = _level
         self.message = _message
         self.details = details
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         d = "".join([", {}={}".format(k, repr(v)) for k, v in self.details.items()])
         return "ItemLogEntry(logging.{}, {}{})".format(
             logging.getLevelName(self.level), repr(self.message), d
         )
 
-    def __contains__(self, key):
+    def __contains__(self, key: str) -> bool:
         return key in self.details
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: str) -> Any:
         return self.details[key]
 
 
 class ItemLog:
-    def __init__(self):
+    level: int  # logging.NOTSET .. logging.CRITICAL
+    entries: list[ItemLogEntry]
+
+    def __init__(self) -> None:
         self.level = logging.NOTSET
         self.entries = []
 
-    def log(self, _level, _message, **details):
+    def log(self, _level: int, _message: str, **details: Any) -> None:
         entry = ItemLogEntry(_level, _message, **details)
         self.entries.append(entry)
         if _level > self.level:
             self.level = _level
 
-    def debug(self, _message, **details):
+    def debug(self, _message: str, **details: Any) -> None:
         self.log(logging.DEBUG, _message, **details)
 
-    def info(self, _message, **details):
+    def info(self, _message: str, **details: Any) -> None:
         self.log(logging.INFO, _message, **details)
 
-    def warning(self, _message, **details):
+    def warning(self, _message: str, **details: Any) -> None:
         self.log(logging.WARNING, _message, **details)
 
-    def error(self, _message, **details):
+    def error(self, _message: str, **details: Any) -> None:
         self.log(logging.ERROR, _message, **details)
 
-    def critical(self, _message, **details):
+    def critical(self, _message: str, **details: Any) -> None:
         self.log(logging.CRITICAL, _message, **details)
 
-    def clone(self):
+    def clone(self) -> ItemLog:
         log = ItemLog()
         log.level = self.level
         log.entries = copy.copy(self.entries)
         return log
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "ItemLog(" + ", ".join([repr(entry) for entry in self.entries]) + ")"
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self.entries)
 
-    def __add__(self, other):
-        if type(other) != ItemLog:
+    def __add__(self, other: ItemLog) -> ItemLog:
+        if type(other) is not ItemLog:
             raise TypeError(
                 "TypeError: unsupported operand type(s) for +: 'ItemLog' and '{}'".format(
                     type(other).__name__
                 )
             )
         log = ItemLog()
-        for entry in self:
+        for entry in self.entries:
             log.log(entry.level, entry.message, **entry.details)
-        for entry in other:
+        for entry in other.entries:
             log.log(entry.level, entry.message, **entry.details)
         return log
 
-    def __getitem__(self, index):
+    def __getitem__(self, index: int) -> ItemLogEntry:
         return self.entries[index]
 
 
-class Item(dict):
+class Item(dict[str, Any]):
     """
     Item extends the dictionary class.
 
     Item behaves like a dict but provides additional functionality
 
     Each Item has an log list to report comments and incidents found while
     transforming, for example validation errors or import notes.
 
     Each Item has an empty dict of meta when being created. meta is
     used to track import information as the name of the file or the line
     number.
     """
 
-    def __init__(self, *args, **kwargs):
+    log: ItemLog
+    meta: dict[str, Any]
+
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.log = ItemLog()
         self.meta = {}
 
-    def clone(self):
+    def clone(self) -> Item:
         item = copy.deepcopy(self)
         item.log = self.log.clone()
         item.meta = copy.copy(self.meta)
         return item
 
-    def flatten(self):
-        item = Item(flatten(self))
+    def flatten(self) -> Item:
+        item = Item(_flatten(self))
         item.log = self.log.clone()
         item.meta = copy.copy(self.meta)
         return item
 
-    def to_json(self):
-        obj = {"data": dict(self), "logEntries": [], "meta": self.meta}
+    # introduce Encoders
+    def to_json(self) -> str:
+        log_entries = []
+
         for entry in self.log.entries:
-            obj["logEntries"].append(
+            log_entries.append(
                 {
                     "level": entry.level,
                     "message": entry.message,
                     "details": entry.details,
                 }
             )
-        return json.dumps(obj)
+
+        return json.dumps(
+            {
+                "data": dict(self),
+                "logEntries": log_entries,
+                "meta": self.meta,
+            }
+        )
 
 
-def from_json(j):
+def from_json(j: str | bytes) -> Item:
     obj = json.loads(j)
     item = Item(obj["data"])
     item.log = ItemLog()
     for entry in obj["logEntries"]:
         item.log.log(entry["level"], entry["message"], **entry["details"])
     item.meta = obj["meta"]
     return item
```

### Comparing `kojo-0.17.0/PKG-INFO` & `kojo-0.18.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 1.1
 Name: kojo
-Version: 0.17.0
+Version: 0.18.0
 Summary: A library to transform data through a pipeline
 Home-page: https://gitlab.com/filchos/kojo
 Author: Olaf Schneider
 Author-email: mail@olafschneider.com
 License: GNU GPLv3
-Download-URL: https://gitlab.com/filchos/kojo/-/archive/0.17.0/kojo-0.17.0.tar.gz
+Download-URL: https://gitlab.com/filchos/kojo/-/archive/0.18.0/kojo-0.18.0.tar.gz
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `kojo-0.17.0/setup.py` & `kojo-0.18.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
 setup(
     name="kojo",
     packages=["kojo"],
-    version="0.17.0",
+    version="0.18.0",
     license="GNU GPLv3",
     description="A library to transform data through a pipeline",
     author="Olaf Schneider",
     author_email="mail@olafschneider.com",
     url="https://gitlab.com/filchos/kojo",
-    download_url="https://gitlab.com/filchos/kojo/-/archive/0.17.0/kojo-0.17.0.tar.gz",
+    download_url="https://gitlab.com/filchos/kojo/-/archive/0.18.0/kojo-0.18.0.tar.gz",
     install_requires=["jsonschema"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3",
     ],
```

