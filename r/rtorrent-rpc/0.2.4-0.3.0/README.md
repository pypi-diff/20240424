# Comparing `tmp/rtorrent_rpc-0.2.4.tar.gz` & `tmp/rtorrent_rpc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtorrent_rpc-0.2.4.tar", max compression
+gzip compressed data, was "rtorrent_rpc-0.3.0.tar", max compression
```

## Comparing `rtorrent_rpc-0.2.4.tar` & `rtorrent_rpc-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1084 2024-04-14 19:12:32.080026 rtorrent_rpc-0.2.4/LICENSE
--rw-r--r--   0        0        0     2467 2024-04-14 19:12:32.084026 rtorrent_rpc-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1077 2024-04-14 19:12:32.084026 rtorrent_rpc-0.2.4/readme.md
--rw-r--r--   0        0        0    27945 2024-04-14 19:12:32.084026 rtorrent_rpc-0.2.4/rtorrent_rpc/__init__.py
--rw-r--r--   0        0        0     2665 2024-04-14 19:12:32.084026 rtorrent_rpc-0.2.4/rtorrent_rpc/helper.py
--rw-r--r--   0        0        0        0 2024-04-14 19:12:32.084026 rtorrent_rpc-0.2.4/rtorrent_rpc/py.typed
--rw-r--r--   0        0        0     3889 2024-04-14 19:12:32.084026 rtorrent_rpc-0.2.4/rtorrent_rpc/scgi.py
--rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 rtorrent_rpc-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-04-24 16:32:15.819316 rtorrent_rpc-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2467 2024-04-24 16:32:15.823316 rtorrent_rpc-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1077 2024-04-24 16:32:15.823316 rtorrent_rpc-0.3.0/readme.md
+-rw-r--r--   0        0        0    28220 2024-04-24 16:32:15.823316 rtorrent_rpc-0.3.0/rtorrent_rpc/__init__.py
+-rw-r--r--   0        0        0     2665 2024-04-24 16:32:15.823316 rtorrent_rpc-0.3.0/rtorrent_rpc/helper.py
+-rw-r--r--   0        0        0        0 2024-04-24 16:32:15.823316 rtorrent_rpc-0.3.0/rtorrent_rpc/py.typed
+-rw-r--r--   0        0        0     3889 2024-04-24 16:32:15.823316 rtorrent_rpc-0.3.0/rtorrent_rpc/scgi.py
+-rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 rtorrent_rpc-0.3.0/PKG-INFO
```

### Comparing `rtorrent_rpc-0.2.4/LICENSE` & `rtorrent_rpc-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.2.4/pyproject.toml` & `rtorrent_rpc-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rtorrent-rpc"
-version = "0.2.4"
+version = "0.3.0"
 description = "Typed rtorrent rpc client"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'readme.md'
 repository = 'https://github.com/trim21/rtorrent-rpc'
 license = 'MIT'
 packages = [{ include = 'rtorrent_rpc' }]
 keywords = ['rtorrent', 'rpc']
@@ -37,15 +37,15 @@
 pytest-github-actions-annotate-failures = "==0.2.0"
 coverage = "==7.4.4"
 
 # linter and formatter
 pre-commit = { version = "==3.7.0", markers = "implementation_name != 'pypy'", python = "^3.9" }
 #mypy = { version = "==1.4.1", markers = "implementation_name != 'pypy'", python = "^3.9" }
 ruff = "0.3.7"
-sphinx-autobuild = "2024.4.13"
+sphinx-autobuild = "2024.4.16"
 mypy = "1.9.0"
 
 [tool.poetry-plugin-bump]
 commit_msg = 'bump: v{version}'
 
 [tool.pytest.ini_options]
 addopts = '-rav -Werror'
```

### Comparing `rtorrent_rpc-0.2.4/readme.md` & `rtorrent_rpc-0.3.0/readme.md`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.2.4/rtorrent_rpc/__init__.py` & `rtorrent_rpc-0.3.0/rtorrent_rpc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 from .scgi import SCGIServerProxy
 
 __all__ = ["RTorrent", "MultiCall"]
 
 Unknown: TypeAlias = Any
 
 
+class RutorrentCompatibilityDisabledError(Exception):
+    def __init__(self):
+        super().__init__("you need enable ruTorrent compatibility to use this feature")
+
+
 class MultiCall(TypedDict):
     methodName: str
     params: NotRequired[Any]
 
 
 def _encode_tags(tags: Iterable[str] | None) -> str:
     if not tags:
@@ -152,14 +157,16 @@
             'd.tied_to_file.set=""',
             f'd.directory_base.set="{directory}"',
             # custom.addtime is used by ruTorrent and flood.
             f"d.custom.set=addtime,{int(time.time())}",
         ]
 
         if tags:
+            if not self.rutorrent_compatibility:
+                raise RutorrentCompatibilityDisabledError
             params.append(f'd.custom1.set="{_encode_tags(tags)}"')
 
         if self.rutorrent_compatibility:
             t = bencode2.bdecode(content)
             if "comment" in t:
                 params.append(
                     f'd.custom2.set="VRS24mrker{quote(t[b"comment"].decode().strip())}"'
```

### Comparing `rtorrent_rpc-0.2.4/rtorrent_rpc/helper.py` & `rtorrent_rpc-0.3.0/rtorrent_rpc/helper.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.2.4/rtorrent_rpc/scgi.py` & `rtorrent_rpc-0.3.0/rtorrent_rpc/scgi.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.2.4/PKG-INFO` & `rtorrent_rpc-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtorrent-rpc
-Version: 0.2.4
+Version: 0.3.0
 Summary: Typed rtorrent rpc client
 Home-page: https://github.com/trim21/rtorrent-rpc
 License: MIT
 Keywords: rtorrent,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.10,<4.0
```

