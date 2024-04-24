# Comparing `tmp/rtorrent_rpc-0.3.1.tar.gz` & `tmp/rtorrent_rpc-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtorrent_rpc-0.3.1.tar", max compression
+gzip compressed data, was "rtorrent_rpc-0.4.0.tar", max compression
```

## Comparing `rtorrent_rpc-0.3.1.tar` & `rtorrent_rpc-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1084 2024-04-24 16:50:29.866301 rtorrent_rpc-0.3.1/LICENSE
--rw-r--r--   0        0        0     2433 2024-04-24 16:50:29.866301 rtorrent_rpc-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1077 2024-04-24 16:50:29.866301 rtorrent_rpc-0.3.1/readme.md
--rw-r--r--   0        0        0    28279 2024-04-24 16:50:29.870301 rtorrent_rpc-0.3.1/rtorrent_rpc/__init__.py
--rw-r--r--   0        0        0     2701 2024-04-24 16:50:29.870301 rtorrent_rpc-0.3.1/rtorrent_rpc/helper.py
--rw-r--r--   0        0        0        0 2024-04-24 16:50:29.870301 rtorrent_rpc-0.3.1/rtorrent_rpc/py.typed
--rw-r--r--   0        0        0     3925 2024-04-24 16:50:29.870301 rtorrent_rpc-0.3.1/rtorrent_rpc/scgi.py
--rw-r--r--   0        0        0     2004 1970-01-01 00:00:00.000000 rtorrent_rpc-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-04-24 16:59:40.890687 rtorrent_rpc-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2433 2024-04-24 16:59:40.890687 rtorrent_rpc-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1077 2024-04-24 16:59:40.890687 rtorrent_rpc-0.4.0/readme.md
+-rw-r--r--   0        0        0    28294 2024-04-24 16:59:40.890687 rtorrent_rpc-0.4.0/rtorrent_rpc/__init__.py
+-rw-r--r--   0        0        0     2934 2024-04-24 16:59:40.890687 rtorrent_rpc-0.4.0/rtorrent_rpc/helper.py
+-rw-r--r--   0        0        0        0 2024-04-24 16:59:40.890687 rtorrent_rpc-0.4.0/rtorrent_rpc/py.typed
+-rw-r--r--   0        0        0     3925 2024-04-24 16:59:40.890687 rtorrent_rpc-0.4.0/rtorrent_rpc/scgi.py
+-rw-r--r--   0        0        0     2004 1970-01-01 00:00:00.000000 rtorrent_rpc-0.4.0/PKG-INFO
```

### Comparing `rtorrent_rpc-0.3.1/LICENSE` & `rtorrent_rpc-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.3.1/pyproject.toml` & `rtorrent_rpc-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rtorrent-rpc"
-version = "0.3.1"
+version = "0.4.0"
 description = "Typed rtorrent rpc client"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'readme.md'
 repository = 'https://github.com/trim21/rtorrent-rpc'
 license = 'MIT'
 packages = [{ include = 'rtorrent_rpc' }]
 keywords = ['rtorrent', 'rpc']
```

### Comparing `rtorrent_rpc-0.3.1/readme.md` & `rtorrent_rpc-0.4.0/readme.md`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.3.1/rtorrent_rpc/__init__.py` & `rtorrent_rpc-0.4.0/rtorrent_rpc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,31 +134,31 @@
     def get_session_path(self) -> str:
         """get current rtorrent session path"""
         return self.rpc.session.path()  # type: ignore
 
     def add_torrent_by_file(
         self,
         content: bytes,
-        directory: str,
+        directory_base: str,
         tags: list[str] | None = None,
     ) -> None:
         """
         Add a torrent to the client by providing the torrent file content as bytes.
 
         Args:
             content: The content of the torrent file as bytes.
-            directory: The base directory where the downloaded files will be saved.
+            directory_base: The base directory where the downloaded files will be saved.
             tags: A list of tags associated with the torrent. Defaults to None.
                 This argument is compatible with ruTorrent and flood.
         """
         params: list[str | bytes] = [
             "",
             content,
             'd.tied_to_file.set=""',
-            f'd.directory_base.set="{directory}"',
+            f'd.directory_base.set="{directory_base}"',
             # custom.addtime is used by ruTorrent and flood.
             f"d.custom.set=addtime,{int(time.time())}",
         ]
 
         if tags:
             if not self.rutorrent_compatibility:
                 raise RutorrentCompatibilityDisabledError
```

### Comparing `rtorrent_rpc-0.3.1/rtorrent_rpc/helper.py` & `rtorrent_rpc-0.4.0/rtorrent_rpc/helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import hashlib
+import sys
 from pathlib import Path
 from typing import Any
 from urllib.parse import unquote
 
 import bencode2
 
 __all__ = [
@@ -21,18 +22,29 @@
     for t in s.split(","):
         tt = t.strip()
         if tt:
             tags.add(tt)
     return tags
 
 
+if sys.version_info >= (3, 9):
+
+    def __remove_prefix(s: str, prefix: str) -> str:
+        return s.removeprefix(prefix)
+
+else:
+
+    def __remove_prefix(s: str, prefix: str) -> str:
+        return s[len(prefix) :]
+
+
 def parse_comment(s: str) -> str:
     """ruTorrent compatibility method to parse ``d.custom2`` as torrent comment"""
     if s.startswith("VRS24mrker"):
-        return unquote(s.removeprefix("VRS24mrker"))
+        return unquote(__remove_prefix(s, "VRS24mrker"))
     return s
 
 
 def get_torrent_info_hash(content: bytes) -> str:
     """get torrent info_hash in low case string"""
     data = bencode2.bdecode(content)
     return hashlib.sha1(bencode2.bencode(data[b"info"])).hexdigest()
```

### Comparing `rtorrent_rpc-0.3.1/rtorrent_rpc/scgi.py` & `rtorrent_rpc-0.4.0/rtorrent_rpc/scgi.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.3.1/PKG-INFO` & `rtorrent_rpc-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtorrent-rpc
-Version: 0.3.1
+Version: 0.4.0
 Summary: Typed rtorrent rpc client
 Home-page: https://github.com/trim21/rtorrent-rpc
 License: MIT
 Keywords: rtorrent,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.8,<4.0
```

