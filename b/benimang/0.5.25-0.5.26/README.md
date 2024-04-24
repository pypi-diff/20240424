# Comparing `tmp/benimang-0.5.25.tar.gz` & `tmp/benimang-0.5.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benimang-0.5.25.tar", last modified: Tue Apr 23 08:29:15 2024, max compression
+gzip compressed data, was "benimang-0.5.26.tar", last modified: Wed Apr 24 03:20:45 2024, max compression
```

## Comparing `benimang-0.5.25.tar` & `benimang-0.5.26.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 08:29:15.883252 benimang-0.5.25/
--rw-rw-rw-   0        0        0       29 2024-01-16 03:49:18.000000 benimang-0.5.25/MANIFEST.in
--rw-rw-rw-   0        0        0      853 2024-04-23 08:29:15.882253 benimang-0.5.25/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-01-16 03:49:18.000000 benimang-0.5.25/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 08:29:15.867740 benimang-0.5.25/beni/
--rw-rw-rw-   0        0        0        0 2024-01-16 03:49:18.000000 benimang-0.5.25/beni/__init__.py
--rw-rw-rw-   0        0        0     6535 2024-01-16 03:49:31.000000 benimang-0.5.25/beni/bbyte.py
--rw-rw-rw-   0        0        0     1815 2024-01-16 03:49:31.000000 benimang-0.5.25/beni/bcache.py
--rw-rw-rw-   0        0        0     1812 2024-01-16 03:49:31.000000 benimang-0.5.25/beni/bcolor.py
--rw-rw-rw-   0        0        0     2796 2024-03-11 07:42:18.000000 benimang-0.5.25/beni/bcrypto.py
--rw-rw-rw-   0        0        0      436 2024-01-16 03:49:31.000000 benimang-0.5.25/beni/bdefine.py
--rw-rw-rw-   0        0        0     1594 2024-04-23 07:33:23.000000 benimang-0.5.25/beni/bexecute.py
--rw-rw-rw-   0        0        0     2697 2024-03-27 01:38:29.000000 benimang-0.5.25/beni/bfile.py
--rw-rw-rw-   0        0        0     6638 2024-04-23 03:25:59.000000 benimang-0.5.25/beni/bfunc.py
--rw-rw-rw-   0        0        0     5740 2024-03-19 08:01:51.000000 benimang-0.5.25/beni/bhttp.py
--rw-rw-rw-   0        0        0     2242 2024-01-16 03:49:31.000000 benimang-0.5.25/beni/binput.py
--rw-rw-rw-   0        0        0     1473 2024-04-23 06:13:33.000000 benimang-0.5.25/beni/bjwt.py
--rw-rw-rw-   0        0        0     4049 2024-04-23 08:22:52.000000 benimang-0.5.25/beni/block.py
--rw-rw-rw-   0        0        0     4147 2024-01-16 03:49:31.000000 benimang-0.5.25/beni/blog.py
--rw-rw-rw-   0        0        0     6115 2024-03-19 08:01:55.000000 benimang-0.5.25/beni/bmysql.py
--rw-rw-rw-   0        0        0     4023 2024-01-16 03:49:31.000000 benimang-0.5.25/beni/bpath.py
--rw-rw-rw-   0        0        0     1374 2024-01-16 03:49:31.000000 benimang-0.5.25/beni/bpathx.py
--rw-rw-rw-   0        0        0     2820 2024-01-17 09:05:37.000000 benimang-0.5.25/beni/bplaywright.py
--rw-rw-rw-   0        0        0     1055 2024-01-16 03:49:31.000000 benimang-0.5.25/beni/bprogress.py
--rw-rw-rw-   0        0        0     3949 2024-01-16 03:49:31.000000 benimang-0.5.25/beni/bqiniu.py
--rw-rw-rw-   0        0        0     3982 2024-01-16 03:49:31.000000 benimang-0.5.25/beni/bstore.py
--rw-rw-rw-   0        0        0     4514 2024-04-23 08:20:46.000000 benimang-0.5.25/beni/btask.py
--rw-rw-rw-   0        0        0     1559 2024-04-23 08:18:44.000000 benimang-0.5.25/beni/btime.py
--rw-rw-rw-   0        0        0      500 2024-02-08 08:49:32.000000 benimang-0.5.25/beni/btype.py
--rw-rw-rw-   0        0        0     2318 2024-01-16 03:49:31.000000 benimang-0.5.25/beni/bzip.py
-drwxrwxrwx   0        0        0        0 2024-04-23 08:29:15.882253 benimang-0.5.25/benimang.egg-info/
--rw-rw-rw-   0        0        0      853 2024-04-23 08:29:15.000000 benimang-0.5.25/benimang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      748 2024-04-23 08:29:15.000000 benimang-0.5.25/benimang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 08:29:15.000000 benimang-0.5.25/benimang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      222 2024-04-23 08:29:15.000000 benimang-0.5.25/benimang.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-23 08:29:15.000000 benimang-0.5.25/benimang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      816 2024-04-23 08:25:28.000000 benimang-0.5.25/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-23 08:29:15.884407 benimang-0.5.25/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-23 08:29:15.880252 benimang-0.5.25/test/
--rw-rw-rw-   0        0        0      398 2024-03-08 09:28:12.000000 benimang-0.5.25/test/test_bbyte.py
--rw-rw-rw-   0        0        0      420 2024-01-16 03:49:31.000000 benimang-0.5.25/test/test_bcache.py
--rw-rw-rw-   0        0        0      735 2024-02-19 03:32:56.000000 benimang-0.5.25/test/test_bcrypto.py
--rw-rw-rw-   0        0        0      406 2024-02-19 03:14:30.000000 benimang-0.5.25/test/test_bfile.py
--rw-rw-rw-   0        0        0      584 2024-04-23 03:29:36.000000 benimang-0.5.25/test/test_bfunc.py
--rw-rw-rw-   0        0        0      491 2024-03-11 06:44:11.000000 benimang-0.5.25/test/test_crypto.py
--rw-rw-rw-   0        0        0      485 2024-02-19 01:38:08.000000 benimang-0.5.25/test/test_mysql.py
--rw-rw-rw-   0        0        0      501 2024-04-23 08:20:46.000000 benimang-0.5.25/test/test_portLock.py
--rw-rw-rw-   0        0        0      447 2024-04-22 02:52:47.000000 benimang-0.5.25/test/test_rwlock.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:20:45.072678 benimang-0.5.26/
+-rw-rw-rw-   0        0        0       29 2024-01-16 03:49:18.000000 benimang-0.5.26/MANIFEST.in
+-rw-rw-rw-   0        0        0      853 2024-04-24 03:20:45.070665 benimang-0.5.26/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-01-16 03:49:18.000000 benimang-0.5.26/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 03:20:45.055633 benimang-0.5.26/beni/
+-rw-rw-rw-   0        0        0        0 2024-01-16 03:49:18.000000 benimang-0.5.26/beni/__init__.py
+-rw-rw-rw-   0        0        0     6535 2024-01-16 03:49:31.000000 benimang-0.5.26/beni/bbyte.py
+-rw-rw-rw-   0        0        0     1815 2024-01-16 03:49:31.000000 benimang-0.5.26/beni/bcache.py
+-rw-rw-rw-   0        0        0     1812 2024-01-16 03:49:31.000000 benimang-0.5.26/beni/bcolor.py
+-rw-rw-rw-   0        0        0     2796 2024-03-11 07:42:18.000000 benimang-0.5.26/beni/bcrypto.py
+-rw-rw-rw-   0        0        0      436 2024-01-16 03:49:31.000000 benimang-0.5.26/beni/bdefine.py
+-rw-rw-rw-   0        0        0     1594 2024-04-23 07:33:23.000000 benimang-0.5.26/beni/bexecute.py
+-rw-rw-rw-   0        0        0     2697 2024-03-27 01:38:29.000000 benimang-0.5.26/beni/bfile.py
+-rw-rw-rw-   0        0        0     6638 2024-04-23 03:25:59.000000 benimang-0.5.26/beni/bfunc.py
+-rw-rw-rw-   0        0        0     5740 2024-03-19 08:01:51.000000 benimang-0.5.26/beni/bhttp.py
+-rw-rw-rw-   0        0        0     2392 2024-04-24 03:19:21.000000 benimang-0.5.26/beni/binput.py
+-rw-rw-rw-   0        0        0     1473 2024-04-23 06:13:33.000000 benimang-0.5.26/beni/bjwt.py
+-rw-rw-rw-   0        0        0     4049 2024-04-23 08:22:52.000000 benimang-0.5.26/beni/block.py
+-rw-rw-rw-   0        0        0     4147 2024-01-16 03:49:31.000000 benimang-0.5.26/beni/blog.py
+-rw-rw-rw-   0        0        0     6115 2024-03-19 08:01:55.000000 benimang-0.5.26/beni/bmysql.py
+-rw-rw-rw-   0        0        0     4023 2024-01-16 03:49:31.000000 benimang-0.5.26/beni/bpath.py
+-rw-rw-rw-   0        0        0     1374 2024-01-16 03:49:31.000000 benimang-0.5.26/beni/bpathx.py
+-rw-rw-rw-   0        0        0     2820 2024-01-17 09:05:37.000000 benimang-0.5.26/beni/bplaywright.py
+-rw-rw-rw-   0        0        0     1055 2024-01-16 03:49:31.000000 benimang-0.5.26/beni/bprogress.py
+-rw-rw-rw-   0        0        0     3949 2024-01-16 03:49:31.000000 benimang-0.5.26/beni/bqiniu.py
+-rw-rw-rw-   0        0        0     3982 2024-01-16 03:49:31.000000 benimang-0.5.26/beni/bstore.py
+-rw-rw-rw-   0        0        0     4514 2024-04-23 08:20:46.000000 benimang-0.5.26/beni/btask.py
+-rw-rw-rw-   0        0        0     1559 2024-04-23 08:18:44.000000 benimang-0.5.26/beni/btime.py
+-rw-rw-rw-   0        0        0      500 2024-02-08 08:49:32.000000 benimang-0.5.26/beni/btype.py
+-rw-rw-rw-   0        0        0     2318 2024-01-16 03:49:31.000000 benimang-0.5.26/beni/bzip.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:20:45.069657 benimang-0.5.26/benimang.egg-info/
+-rw-rw-rw-   0        0        0      853 2024-04-24 03:20:45.000000 benimang-0.5.26/benimang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      748 2024-04-24 03:20:45.000000 benimang-0.5.26/benimang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 03:20:45.000000 benimang-0.5.26/benimang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      222 2024-04-24 03:20:45.000000 benimang-0.5.26/benimang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-24 03:20:45.000000 benimang-0.5.26/benimang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      816 2024-04-24 03:20:25.000000 benimang-0.5.26/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-24 03:20:45.072678 benimang-0.5.26/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 03:20:45.069150 benimang-0.5.26/test/
+-rw-rw-rw-   0        0        0      398 2024-03-08 09:28:12.000000 benimang-0.5.26/test/test_bbyte.py
+-rw-rw-rw-   0        0        0      420 2024-01-16 03:49:31.000000 benimang-0.5.26/test/test_bcache.py
+-rw-rw-rw-   0        0        0      735 2024-02-19 03:32:56.000000 benimang-0.5.26/test/test_bcrypto.py
+-rw-rw-rw-   0        0        0      406 2024-02-19 03:14:30.000000 benimang-0.5.26/test/test_bfile.py
+-rw-rw-rw-   0        0        0      584 2024-04-23 03:29:36.000000 benimang-0.5.26/test/test_bfunc.py
+-rw-rw-rw-   0        0        0      491 2024-03-11 06:44:11.000000 benimang-0.5.26/test/test_crypto.py
+-rw-rw-rw-   0        0        0      485 2024-02-19 01:38:08.000000 benimang-0.5.26/test/test_mysql.py
+-rw-rw-rw-   0        0        0      501 2024-04-23 08:20:46.000000 benimang-0.5.26/test/test_portLock.py
+-rw-rw-rw-   0        0        0      447 2024-04-22 02:52:47.000000 benimang-0.5.26/test/test_rwlock.py
```

### Comparing `benimang-0.5.25/PKG-INFO` & `benimang-0.5.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benimang
-Version: 0.5.25
+Version: 0.5.26
 Summary: Utils library for Beni
 Author-email: Beni Mang <benimang@126.com>
 Maintainer-email: Beni Mang <benimang@126.com>
 Keywords: benimang,beni
 Requires-Python: >=3.10
 Requires-Dist: aioconsole
 Requires-Dist: aiofiles
```

### Comparing `benimang-0.5.25/beni/bbyte.py` & `benimang-0.5.26/beni/bbyte.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.25/beni/bcache.py` & `benimang-0.5.26/beni/bcache.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.25/beni/bcolor.py` & `benimang-0.5.26/beni/bcolor.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.25/beni/bcrypto.py` & `benimang-0.5.26/beni/bcrypto.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.25/beni/bexecute.py` & `benimang-0.5.26/beni/bexecute.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.25/beni/bfile.py` & `benimang-0.5.26/beni/bfile.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.25/beni/bfunc.py` & `benimang-0.5.26/beni/bfunc.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.25/beni/bhttp.py` & `benimang-0.5.26/beni/bhttp.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.25/beni/binput.py` & `benimang-0.5.26/beni/binput.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 import getpass
 import random
+import string
 from typing import Any, Callable, Coroutine, cast
 
 import aioconsole
 
 from beni import bcolor
 
 
 async def hold(msg: str | None = None, isShowInput: bool = True, *exits: str):
     msg = msg or '测试暂停，输入exit可以退出'
     msg = f'{msg}: '
-    exits = exits or ('exit',)
+    exits = tuple([x.lower() for x in exits]) or ('exit', )
     while True:
         if isShowInput:
-
             result = cast(str, await aioconsole.ainput(msg))
         else:
             result = getpass.getpass(msg)
+        result = result.lower()
         if (result in exits) or ('*' in exits):
             return result
 
 
 async def confirm(msg: str = '确认', isShowInput: bool = False):
-    code = f'{random.randint(1, 999):03}'
-    await hold(f'{msg} [ {_getRemindMsg(code)} ]', not isShowInput, code)
+    codeAry = random.sample(string.ascii_uppercase, 3)
+    codeMsg = ' '.join(codeAry)
+    code = ''.join(codeAry)
+    await hold(f'{msg} [ {_getRemindMsg(codeMsg)} ]', not isShowInput, code)
 
 
 async def select(*data: tuple[str, str, str | Callable[[str], Any] | None, Callable[[str], Coroutine[Any, Any, Any]] | None]):
     '''
     value = binput.select(
         ('descA', 'confirmDescA', 'quanbuqueren', __handlerA),
         ('descB', 'confirmDescB', lambda x: ..., __handlerB),
```

### Comparing `benimang-0.5.25/beni/bjwt.py` & `benimang-0.5.26/beni/bjwt.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.25/beni/block.py` & `benimang-0.5.26/beni/block.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.25/beni/blog.py` & `benimang-0.5.26/beni/blog.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.25/beni/bmysql.py` & `benimang-0.5.26/beni/bmysql.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.25/beni/bpath.py` & `benimang-0.5.26/beni/bpath.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.25/beni/bpathx.py` & `benimang-0.5.26/beni/bpathx.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.25/beni/bplaywright.py` & `benimang-0.5.26/beni/bplaywright.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.25/beni/bprogress.py` & `benimang-0.5.26/beni/bprogress.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.25/beni/bqiniu.py` & `benimang-0.5.26/beni/bqiniu.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.25/beni/bstore.py` & `benimang-0.5.26/beni/bstore.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.25/beni/btask.py` & `benimang-0.5.26/beni/btask.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.25/beni/btime.py` & `benimang-0.5.26/beni/btime.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.25/beni/bzip.py` & `benimang-0.5.26/beni/bzip.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.25/benimang.egg-info/PKG-INFO` & `benimang-0.5.26/benimang.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benimang
-Version: 0.5.25
+Version: 0.5.26
 Summary: Utils library for Beni
 Author-email: Beni Mang <benimang@126.com>
 Maintainer-email: Beni Mang <benimang@126.com>
 Keywords: benimang,beni
 Requires-Python: >=3.10
 Requires-Dist: aioconsole
 Requires-Dist: aiofiles
```

### Comparing `benimang-0.5.25/benimang.egg-info/SOURCES.txt` & `benimang-0.5.26/benimang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `benimang-0.5.25/pyproject.toml` & `benimang-0.5.26/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # https://peps.python.org/pep-0621/#example
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata/#declaring-project-metadata
 
 [project]
 name = "benimang"
-version = "0.5.25"
+version = "0.5.26"
 description = "Utils library for Beni"
 requires-python = ">=3.10"
 keywords = ["benimang", "beni"]
 authors = [{ name = 'Beni Mang', email = 'benimang@126.com' }]
 maintainers = [{ name = 'Beni Mang', email = 'benimang@126.com' }]
 
 dependencies = [
```

### Comparing `benimang-0.5.25/test/test_bcrypto.py` & `benimang-0.5.26/test/test_bcrypto.py`

 * *Files identical despite different names*

### Comparing `benimang-0.5.25/test/test_bfunc.py` & `benimang-0.5.26/test/test_bfunc.py`

 * *Files identical despite different names*

