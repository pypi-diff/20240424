# Comparing `tmp/kv_sqlite_sync-0.1.6.tar.gz` & `tmp/kv_sqlite_sync-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv_sqlite_sync-0.1.6.tar", last modified: Sun Apr 21 18:04:02 2024, max compression
+gzip compressed data, was "kv_sqlite_sync-0.1.7.tar", last modified: Wed Apr 24 13:42:39 2024, max compression
```

## Comparing `kv_sqlite_sync-0.1.6.tar` & `kv_sqlite_sync-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,18 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:04:02.949883 kv_sqlite_sync-0.1.6/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      854 2024-04-21 18:04:02.949883 kv_sqlite_sync-0.1.6/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      401 2024-04-05 13:15:45.000000 kv_sqlite_sync-0.1.6/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      667 2024-04-21 18:04:00.000000 kv_sqlite_sync-0.1.6/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-21 18:04:02.949883 kv_sqlite_sync-0.1.6/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:04:02.949883 kv_sqlite_sync-0.1.6/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:04:02.949883 kv_sqlite_sync-0.1.6/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:04:02.949883 kv_sqlite_sync-0.1.6/src/kv/sqlite/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      146 2024-04-05 13:12:45.000000 kv_sqlite_sync-0.1.6/src/kv/sqlite/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:04:02.949883 kv_sqlite_sync-0.1.6/src/kv/sqlite/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       25 2024-04-05 13:12:45.000000 kv_sqlite_sync-0.1.6/src/kv/sqlite/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4060 2024-04-21 17:44:40.000000 kv_sqlite_sync-0.1.6/src/kv/sqlite/api/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:04:02.949883 kv_sqlite_sync-0.1.6/src/kv/sqlite/queries/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       92 2024-04-05 13:12:45.000000 kv_sqlite_sync-0.1.6/src/kv/sqlite/queries/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1487 2024-04-21 17:44:50.000000 kv_sqlite_sync-0.1.6/src/kv/sqlite/queries/queries.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-21 18:04:02.949883 kv_sqlite_sync-0.1.6/src/kv_sqlite_sync.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      854 2024-04-21 18:04:02.000000 kv_sqlite_sync-0.1.6/src/kv_sqlite_sync.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      381 2024-04-21 18:04:02.000000 kv_sqlite_sync-0.1.6/src/kv_sqlite_sync.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-21 18:04:02.000000 kv_sqlite_sync-0.1.6/src/kv_sqlite_sync.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-04-21 18:04:02.000000 kv_sqlite_sync-0.1.6/src/kv_sqlite_sync.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-21 18:04:02.000000 kv_sqlite_sync-0.1.6/src/kv_sqlite_sync.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 13:42:39.953952 kv_sqlite_sync-0.1.7/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      894 2024-04-24 13:42:39.953952 kv_sqlite_sync-0.1.7/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      401 2024-04-24 13:02:36.000000 kv_sqlite_sync-0.1.7/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      695 2024-04-24 13:42:37.000000 kv_sqlite_sync-0.1.7/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-24 13:42:39.953952 kv_sqlite_sync-0.1.7/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 13:42:39.953952 kv_sqlite_sync-0.1.7/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 13:42:39.953952 kv_sqlite_sync-0.1.7/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 13:42:39.953952 kv_sqlite_sync-0.1.7/src/kv/sqlite/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 13:32:50.000000 kv_sqlite_sync-0.1.7/src/kv/sqlite/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      203 2024-04-24 13:32:38.000000 kv_sqlite_sync-0.1.7/src/kv/sqlite/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3669 2024-04-24 13:41:44.000000 kv_sqlite_sync-0.1.7/src/kv/sqlite/api.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1631 2024-04-24 13:37:20.000000 kv_sqlite_sync-0.1.7/src/kv/sqlite/queries.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 13:42:39.953952 kv_sqlite_sync-0.1.7/src/kv_sqlite_sync.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      894 2024-04-24 13:42:39.000000 kv_sqlite_sync-0.1.7/src/kv_sqlite_sync.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      332 2024-04-24 13:42:39.000000 kv_sqlite_sync-0.1.7/src/kv_sqlite_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-24 13:42:39.000000 kv_sqlite_sync-0.1.7/src/kv_sqlite_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       30 2024-04-24 13:42:39.000000 kv_sqlite_sync-0.1.7/src/kv_sqlite_sync.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-24 13:42:39.000000 kv_sqlite_sync-0.1.7/src/kv_sqlite_sync.egg-info/top_level.txt
```

### Comparing `kv_sqlite_sync-0.1.6/PKG-INFO` & `kv_sqlite_sync-0.1.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: kv-sqlite-sync
-Version: 0.1.6
+Version: 0.1.7
 Summary: Key-Value interface over SQLite. Supports any datatype, including JSON and BLOB
 Author-email: Marcel Claramunt <marcel@moveread.com>
-Project-URL: repo, https://github.com/moveread/python-kv
-Project-URL: home, https://github.com/moveread/python-kv/tree/main/kv-sqlite-sync
+Project-URL: repo, https://github.com/moveread/python-storage
+Project-URL: home, https://github.com/moveread/python-storage/tree/main/kv/kv-sqlite-sync
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kv-api
 Requires-Dist: haskellian
+Requires-Dist: lazy-loader
 
 # Sqlite Kv (Sync)
 
 > Synchronous Key-Value interface over SQLite. Supports any datatype, including JSON and BLOB
 
 ## Usage
```

### Comparing `kv_sqlite_sync-0.1.6/pyproject.toml` & `kv_sqlite_sync-0.1.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kv-sqlite-sync"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Key-Value interface over SQLite. Supports any datatype, including JSON and BLOB"
 dependencies = [
-  "kv-api", "haskellian"
+  "kv-api", "haskellian", "lazy-loader"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
-repo = "https://github.com/moveread/python-kv"
-home = "https://github.com/moveread/python-kv/tree/main/kv-sqlite-sync"
+repo = "https://github.com/moveread/python-storage"
+home = "https://github.com/moveread/python-storage/tree/main/kv/kv-sqlite-sync"
 
 # [project.optional-dependencies]
 # test = [
 #   "pytest < 5.0.0",
 #   "pytest-cov[all]"
 # ]
```

### Comparing `kv_sqlite_sync-0.1.6/src/kv/sqlite/api/api.py` & `kv_sqlite_sync-0.1.7/src/kv/sqlite/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import AsyncIterable, TypeVar, Generic, Callable, Never, cast
+from typing import AsyncIterable, TypeVar, Generic, Callable, cast
 from dataclasses import dataclass
 from haskellian import either as E, promise as P, asyn_iter as AI
 from pydantic import RootModel
 from kv.api import KV
 from kv.api.errors import InexistentItem, DBError, InvalidData
 import sqlite3
 import os
-from .. import queries
+from . import queries
 
 T = TypeVar('T')
 M = TypeVar('M')
 
 @dataclass
 class SQLiteKV(KV[T], Generic[T]):
 
@@ -49,26 +49,25 @@
     try:
       cur = self.conn.execute(*query)
       self.conn.commit()
       return E.Right(cur)
     except sqlite3.Error as err:
       return E.Left(DBError(str(err)))
 
-  # @P.lift
-  # async def update(self, key: str, value: T) -> E.Either[DBError|InexistentItem, None]:
-  #   return self.execute(queries.update(key, self.dump(value), table=self.table)).bind(
-  #     lambda cur: E.Left(InexistentItem(key)) if cur.rowcount == 0 else E.Right(None)
-  #   )
-  
   @P.lift
-  async def insert(self, key: str, value: T, *, replace = False) -> E.Either[DBError, None]:
-    make_query = queries.upsert if replace else queries.insert
-    return self.execute(make_query(key, self.dump(value), table=self.table)) | (lambda _: None)
+  async def insert(self, key: str, value: T) -> E.Either[DBError, None]:
+    return self.execute(queries.upsert(key, self.dump(value), table=self.table)) | (lambda _: None)
   
   @P.lift
+  async def has(self, key: str) -> E.Either[DBError, bool]:
+    return self.execute(queries.read(key, table=self.table)).fmap(
+      lambda cur: cur.fetchone() is not None
+    )
+    
+  @P.lift
   async def read(self, key: str) -> E.Either[DBError | InvalidData | InexistentItem, T]:
     res = self.execute(queries.read(key, table=self.table)) \
       | sqlite3.Cursor.fetchone
     match res:
       case E.Right(None):
         return E.Left(InexistentItem(key))
       case E.Right([data]):
@@ -99,15 +98,8 @@
     match self.execute(queries.items(self.table)):
       case E.Right(cur):
         while (batch := cur.fetchmany(batch_size or 256)) != []:
           for k, v in batch:
             yield self.parse(v) | (lambda v: (k, v))
       case E.Left(err):
         yield E.Left(err)
-  
-  @P.lift
-  async def commit(self) -> E.Either[Never, None]:
-    return E.Right(self.conn.commit())
-  
-  @P.lift
-  async def rollback(self) -> E.Either[Never, None]:
-    return E.Right(self.conn.rollback())
+
```

### Comparing `kv_sqlite_sync-0.1.6/src/kv/sqlite/queries/queries.py` & `kv_sqlite_sync-0.1.7/src/kv/sqlite/queries.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import NamedTuple
+from typing import NamedTuple as _NamedTuple
 
-class Query(NamedTuple):
+class Query(_NamedTuple):
   """Query `q` to be run via `conn.execute(*q)`"""
   query: str
   params: list
 
 def quote(unsafe: str) -> str:
   """Safely quote user input"""
   unquoted = unsafe.replace('"', '')
@@ -28,14 +28,18 @@
   query = f'UPDATE {quote(table)} SET VALUE = ? WHERE KEY = ?'
   return Query(query, [value, key])
 
 def read(key: str, table: str) -> Query:
   query = f'SELECT VALUE FROM {quote(table)} WHERE KEY = ?'
   return Query(query, [key])
 
+def has(key: str, table: str) -> Query:
+  query = f'SELECT KEY FROM {quote(table)} WHERE KEY = ?'
+  return Query(query, [key])
+
 def keys(table: str) -> Query:
   query = f'SELECT KEY FROM {quote(table)}'
   return Query(query, [])
 
 def items(table: str) -> Query:
   query = f'SELECT KEY, VALUE FROM {quote(table)}'
   return Query(query, [])
```

### Comparing `kv_sqlite_sync-0.1.6/src/kv_sqlite_sync.egg-info/PKG-INFO` & `kv_sqlite_sync-0.1.7/src/kv_sqlite_sync.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: kv-sqlite-sync
-Version: 0.1.6
+Version: 0.1.7
 Summary: Key-Value interface over SQLite. Supports any datatype, including JSON and BLOB
 Author-email: Marcel Claramunt <marcel@moveread.com>
-Project-URL: repo, https://github.com/moveread/python-kv
-Project-URL: home, https://github.com/moveread/python-kv/tree/main/kv-sqlite-sync
+Project-URL: repo, https://github.com/moveread/python-storage
+Project-URL: home, https://github.com/moveread/python-storage/tree/main/kv/kv-sqlite-sync
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kv-api
 Requires-Dist: haskellian
+Requires-Dist: lazy-loader
 
 # Sqlite Kv (Sync)
 
 > Synchronous Key-Value interface over SQLite. Supports any datatype, including JSON and BLOB
 
 ## Usage
```

