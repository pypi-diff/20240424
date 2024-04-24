# Comparing `tmp/rtorrent_rpc-0.3.0.tar.gz` & `tmp/rtorrent_rpc-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtorrent_rpc-0.3.0.tar", max compression
+gzip compressed data, was "rtorrent_rpc-0.3.1.tar", max compression
```

## Comparing `rtorrent_rpc-0.3.0.tar` & `rtorrent_rpc-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1084 2024-04-24 16:32:15.819316 rtorrent_rpc-0.3.0/LICENSE
--rw-r--r--   0        0        0     2467 2024-04-24 16:32:15.823316 rtorrent_rpc-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1077 2024-04-24 16:32:15.823316 rtorrent_rpc-0.3.0/readme.md
--rw-r--r--   0        0        0    28220 2024-04-24 16:32:15.823316 rtorrent_rpc-0.3.0/rtorrent_rpc/__init__.py
--rw-r--r--   0        0        0     2665 2024-04-24 16:32:15.823316 rtorrent_rpc-0.3.0/rtorrent_rpc/helper.py
--rw-r--r--   0        0        0        0 2024-04-24 16:32:15.823316 rtorrent_rpc-0.3.0/rtorrent_rpc/py.typed
--rw-r--r--   0        0        0     3889 2024-04-24 16:32:15.823316 rtorrent_rpc-0.3.0/rtorrent_rpc/scgi.py
--rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 rtorrent_rpc-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-04-24 16:50:29.866301 rtorrent_rpc-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2433 2024-04-24 16:50:29.866301 rtorrent_rpc-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1077 2024-04-24 16:50:29.866301 rtorrent_rpc-0.3.1/readme.md
+-rw-r--r--   0        0        0    28279 2024-04-24 16:50:29.870301 rtorrent_rpc-0.3.1/rtorrent_rpc/__init__.py
+-rw-r--r--   0        0        0     2701 2024-04-24 16:50:29.870301 rtorrent_rpc-0.3.1/rtorrent_rpc/helper.py
+-rw-r--r--   0        0        0        0 2024-04-24 16:50:29.870301 rtorrent_rpc-0.3.1/rtorrent_rpc/py.typed
+-rw-r--r--   0        0        0     3925 2024-04-24 16:50:29.870301 rtorrent_rpc-0.3.1/rtorrent_rpc/scgi.py
+-rw-r--r--   0        0        0     2004 1970-01-01 00:00:00.000000 rtorrent_rpc-0.3.1/PKG-INFO
```

### Comparing `rtorrent_rpc-0.3.0/LICENSE` & `rtorrent_rpc-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.3.0/pyproject.toml` & `rtorrent_rpc-0.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rtorrent-rpc"
-version = "0.3.0"
+version = "0.3.1"
 description = "Typed rtorrent rpc client"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'readme.md'
 repository = 'https://github.com/trim21/rtorrent-rpc'
 license = 'MIT'
 packages = [{ include = 'rtorrent_rpc' }]
 keywords = ['rtorrent', 'rpc']
 classifiers = [
     'Intended Audience :: Developers',
     'Development Status :: 4 - Beta',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3 :: Only',
-    'Programming Language :: Python :: 3.10',
-    'Programming Language :: Python :: 3.11',
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
 # dependencies
 typing-extensions = ">=4.7.1"
 bencode2 = ">=0.0.6,<1"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = { version = "^7.0.0", python = "^3.9" }
 furo = { version = "^2024.0.0", python = "^3.9" }
@@ -37,38 +35,38 @@
 pytest-github-actions-annotate-failures = "==0.2.0"
 coverage = "==7.4.4"
 
 # linter and formatter
 pre-commit = { version = "==3.7.0", markers = "implementation_name != 'pypy'", python = "^3.9" }
 #mypy = { version = "==1.4.1", markers = "implementation_name != 'pypy'", python = "^3.9" }
 ruff = "0.3.7"
-sphinx-autobuild = "2024.4.16"
-mypy = "1.9.0"
+sphinx-autobuild = { version = "2024.4.16", python = "^3.9" }
+mypy = { version = "1.9.0", python = "^3.9" }
 
 [tool.poetry-plugin-bump]
 commit_msg = 'bump: v{version}'
 
 [tool.pytest.ini_options]
 addopts = '-rav -Werror'
 
 [tool.mypy]
-python_version = "3.10"
+python_version = "3.8"
 disallow_untyped_defs = true
 ignore_missing_imports = true
 warn_return_any = false
 warn_unused_configs = true
 show_error_codes = true
 
 platform = 'unix'
 
 [tool.black]
-target-version = ['py310']
+target-version = ['py38']
 
 [tool.ruff]
-target-version = "py310"
+target-version = "py38"
 
 [tool.ruff.lint]
 select = [
     "B",
     "C",
     "E",
     "F",
```

### Comparing `rtorrent_rpc-0.3.0/readme.md` & `rtorrent_rpc-0.3.1/readme.md`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.3.0/rtorrent_rpc/__init__.py` & `rtorrent_rpc-0.3.1/rtorrent_rpc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,28 @@
+from __future__ import annotations
+
 import time
 import urllib.parse
 import xmlrpc.client
 from collections.abc import Iterable
-from typing import Any, Literal, Protocol, TypeAlias, TypedDict
+from typing import Any, Literal, Protocol
 from urllib.parse import quote
 
 import bencode2
-from typing_extensions import NotRequired
+from typing_extensions import NotRequired, TypeAlias, TypedDict
 
 from .scgi import SCGIServerProxy
 
-__all__ = ["RTorrent", "MultiCall"]
+__all__ = ["RTorrent", "MultiCall", "RutorrentCompatibilityDisabledError"]
 
 Unknown: TypeAlias = Any
 
 
 class RutorrentCompatibilityDisabledError(Exception):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__("you need enable ruTorrent compatibility to use this feature")
 
 
 class MultiCall(TypedDict):
     methodName: str
     params: NotRequired[Any]
 
@@ -29,19 +31,17 @@
     if not tags:
         return ""
 
     return ",".join(sorted(quote(t) for t in {x.strip() for x in tags} if t))
 
 
 class _DirectoryRpc(Protocol):
-    def __call__(self, info_hash: str, /) -> str:
-        ...
+    def __call__(self, info_hash: str, /) -> str: ...
 
-    def set(self, info_hash: str, value: str, /) -> None:
-        ...
+    def set(self, info_hash: str, value: str, /) -> None: ...
 
 
 class _CustomSet(Protocol):
     def __call__(self, info_hash: str, key: str, /) -> str:
         """get download's custom value"""
 
     def set(self, info_hash: str, key: str, value: str, /) -> int:
@@ -62,16 +62,15 @@
         """base directory"""
 
     @property
     def directory(self) -> _DirectoryRpc:
         """directory"""
 
     @property
-    def custom(self) -> _CustomSet:
-        ...
+    def custom(self) -> _CustomSet: ...
 
 
 class _SystemRpc(Protocol):
     """this is not a real class, it's a typing protocol for rpc typing"""
 
     def multicall(self, commands: list[MultiCall]) -> Any:
         """run multiple rpc calls"""
```

### Comparing `rtorrent_rpc-0.3.0/rtorrent_rpc/helper.py` & `rtorrent_rpc-0.3.1/rtorrent_rpc/helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import hashlib
 from pathlib import Path
 from typing import Any
 from urllib.parse import unquote
 
 import bencode2
```

### Comparing `rtorrent_rpc-0.3.0/rtorrent_rpc/scgi.py` & `rtorrent_rpc-0.3.1/rtorrent_rpc/scgi.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 # Python module for interacting with rtorrent's XML-RPC interface
 # directly over SCGI, instead of through an HTTP server intermediary.
 # Inspired by Glenn Washburn's xmlrpc2scgi.py [1], but subclasses the
 # built-in xmlrpclib classes so that it is compatible with features
 # such as MultiCall objects.
 #
 # [1] <http://libtorrent.rakshasa.no/wiki/UtilsXmlrpc2scgi>
+from __future__ import annotations
+
 import socket
 import urllib
 import urllib.parse
 import xmlrpc.client
 from typing import Any
 
 __all__ = ["SCGITransport", "SCGIServerProxy"]
```

### Comparing `rtorrent_rpc-0.3.0/PKG-INFO` & `rtorrent_rpc-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: rtorrent-rpc
-Version: 0.3.0
+Version: 0.3.1
 Summary: Typed rtorrent rpc client
 Home-page: https://github.com/trim21/rtorrent-rpc
 License: MIT
 Keywords: rtorrent,rpc
 Author: Trim21
 Author-email: i@trim21.me
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: bencode2 (>=0.0.6,<1)
 Requires-Dist: typing-extensions (>=4.7.1)
 Project-URL: Repository, https://github.com/trim21/rtorrent-rpc
```

