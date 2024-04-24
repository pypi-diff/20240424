# Comparing `tmp/firebolt_sqlalchemy-1.0.1.tar.gz` & `tmp/firebolt_sqlalchemy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/firebolt-sqlalchemy/firebolt-sqlalchemy/dist/.tmp-5_tkm26m/firebolt_sqlalchemy-1.0.1.tar", last modified: Tue Feb  6 16:27:28 2024, max compression
+gzip compressed data, was "/home/runner/work/firebolt-sqlalchemy/firebolt-sqlalchemy/dist/.tmp-713uyl76/firebolt_sqlalchemy-1.0.2.tar", last modified: Wed Apr 24 17:07:20 2024, max compression
```

## Comparing `firebolt_sqlalchemy-1.0.1.tar` & `firebolt_sqlalchemy-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:27:28.000000 firebolt_sqlalchemy-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-02-06 16:27:10.000000 firebolt_sqlalchemy-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-02-06 16:27:28.000000 firebolt_sqlalchemy-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-02-06 16:27:10.000000 firebolt_sqlalchemy-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-02-06 16:27:10.000000 firebolt_sqlalchemy-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-02-06 16:27:28.000000 firebolt_sqlalchemy-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:27:28.000000 firebolt_sqlalchemy-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:27:28.000000 firebolt_sqlalchemy-1.0.1/src/firebolt_db/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-06 16:27:20.000000 firebolt_sqlalchemy-1.0.1/src/firebolt_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-02-06 16:27:10.000000 firebolt_sqlalchemy-1.0.1/src/firebolt_db/firebolt_async_dialect.py
--rw-r--r--   0 runner    (1001) docker     (127)    10912 2024-02-06 16:27:10.000000 firebolt_sqlalchemy-1.0.1/src/firebolt_db/firebolt_dialect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 16:27:28.000000 firebolt_sqlalchemy-1.0.1/src/firebolt_sqlalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-02-06 16:27:28.000000 firebolt_sqlalchemy-1.0.1/src/firebolt_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-02-06 16:27:28.000000 firebolt_sqlalchemy-1.0.1/src/firebolt_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 16:27:28.000000 firebolt_sqlalchemy-1.0.1/src/firebolt_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-06 16:27:28.000000 firebolt_sqlalchemy-1.0.1/src/firebolt_sqlalchemy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-06 16:27:28.000000 firebolt_sqlalchemy-1.0.1/src/firebolt_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-06 16:27:28.000000 firebolt_sqlalchemy-1.0.1/src/firebolt_sqlalchemy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:07:20.000000 firebolt_sqlalchemy-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-04-24 17:07:02.000000 firebolt_sqlalchemy-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-24 17:07:20.000000 firebolt_sqlalchemy-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-24 17:07:02.000000 firebolt_sqlalchemy-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-24 17:07:02.000000 firebolt_sqlalchemy-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-24 17:07:20.000000 firebolt_sqlalchemy-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:07:20.000000 firebolt_sqlalchemy-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:07:20.000000 firebolt_sqlalchemy-1.0.2/src/firebolt_db/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 17:07:15.000000 firebolt_sqlalchemy-1.0.2/src/firebolt_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-24 17:07:02.000000 firebolt_sqlalchemy-1.0.2/src/firebolt_db/firebolt_async_dialect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11191 2024-04-24 17:07:02.000000 firebolt_sqlalchemy-1.0.2/src/firebolt_db/firebolt_dialect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:07:20.000000 firebolt_sqlalchemy-1.0.2/src/firebolt_sqlalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-24 17:07:20.000000 firebolt_sqlalchemy-1.0.2/src/firebolt_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-24 17:07:20.000000 firebolt_sqlalchemy-1.0.2/src/firebolt_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 17:07:20.000000 firebolt_sqlalchemy-1.0.2/src/firebolt_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-24 17:07:20.000000 firebolt_sqlalchemy-1.0.2/src/firebolt_sqlalchemy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-24 17:07:20.000000 firebolt_sqlalchemy-1.0.2/src/firebolt_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 17:07:20.000000 firebolt_sqlalchemy-1.0.2/src/firebolt_sqlalchemy.egg-info/top_level.txt
```

### Comparing `firebolt_sqlalchemy-1.0.1/LICENSE` & `firebolt_sqlalchemy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `firebolt_sqlalchemy-1.0.1/PKG-INFO` & `firebolt_sqlalchemy-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebolt_sqlalchemy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Sqlalchemy adapter for Firebolt
 Home-page: https://github.com/firebolt-db/firebolt-sqlalchemy
 Download-URL: https://github.com/firebolt-db/firebolt-sqlalchemy/archive/refs/tags/0.0.9.tar.gz
 Author: Firebolt
 Author-email: pypi@firebolt.io
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/firebolt-db/firebolt-sqlalchemy
```

### Comparing `firebolt_sqlalchemy-1.0.1/README.md` & `firebolt_sqlalchemy-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `firebolt_sqlalchemy-1.0.1/setup.cfg` & `firebolt_sqlalchemy-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `firebolt_sqlalchemy-1.0.1/src/firebolt_db/firebolt_async_dialect.py` & `firebolt_sqlalchemy-1.0.2/src/firebolt_db/firebolt_async_dialect.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 from asyncio import Lock
 from functools import partial
 from types import ModuleType
 from typing import Any, Dict, Iterator, List, Optional, Tuple
 
 import firebolt.async_db as async_dbapi
 from firebolt.async_db import Connection
+from sqlalchemy.engine import AdaptedConnection  # type: ignore[attr-defined]
 
 # Ignoring type since sqlalchemy-stubs doesn't cover AdaptedConnection
 # and util.concurrency
-from sqlalchemy.engine import AdaptedConnection  # type: ignore[attr-defined]
+from sqlalchemy.pool import AsyncAdaptedQueuePool  # type: ignore[attr-defined]
 from sqlalchemy.util.concurrency import await_only  # type: ignore[import]
 from trio import run
 
 from firebolt_db.firebolt_dialect import FireboltDialect
 
 
 class AsyncCursorWrapper:
@@ -163,14 +164,15 @@
 
 
 class AsyncFireboltDialect(FireboltDialect):
     driver = "firebolt_aio"
     supports_statement_cache: bool = False
     supports_server_side_cursors: bool = False
     is_async: bool = True
+    poolclass = AsyncAdaptedQueuePool
 
     @classmethod
     def dbapi(cls) -> AsyncAPIWrapper:
         return AsyncAPIWrapper(async_dbapi)
 
 
 dialect = AsyncFireboltDialect
```

### Comparing `firebolt_sqlalchemy-1.0.1/src/firebolt_db/firebolt_dialect.py` & `firebolt_sqlalchemy-1.0.2/src/firebolt_db/firebolt_dialect.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,27 +115,34 @@
     type_compiler = FireboltTypeCompiler
     supports_alter = False
     supports_pk_autoincrement = False
     supports_default_values = False
     supports_empty_insert = False
     supports_unicode_statements = True
     supports_unicode_binds = True
+    supports_statement_cache = False
+    # supports_statement_cache Set to False to disable warning
+    # https://sqlalche.me/e/20/cprf
     returns_unicode_strings = True
     description_encoding = None
     supports_native_boolean = True
     _set_parameters: Dict[str, Any] = dict()
 
     def __init__(
         self, context: Optional[ExecutionContext] = None, *args: Any, **kwargs: Any
     ):
         super(FireboltDialect, self).__init__(*args, **kwargs)
         self.context: Union[ExecutionContext, Dict] = context or {}
 
     @classmethod
-    def dbapi(cls) -> ModuleType:
+    def import_dbapi(cls) -> ModuleType:  # For sqlalchemy >= 2.0.0
+        return dbapi
+
+    @classmethod
+    def dbapi(cls) -> ModuleType:  # Kept for backwards compatibility
         return dbapi
 
     def create_connect_args(self, url: URL) -> Tuple[List, Dict]:
         """
         Build firebolt-sdk compatible connection arguments.
         URL format : firebolt://id:secret@host:port/db_name
         """
```

### Comparing `firebolt_sqlalchemy-1.0.1/src/firebolt_sqlalchemy.egg-info/PKG-INFO` & `firebolt_sqlalchemy-1.0.2/src/firebolt_sqlalchemy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebolt-sqlalchemy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Sqlalchemy adapter for Firebolt
 Home-page: https://github.com/firebolt-db/firebolt-sqlalchemy
 Download-URL: https://github.com/firebolt-db/firebolt-sqlalchemy/archive/refs/tags/0.0.9.tar.gz
 Author: Firebolt
 Author-email: pypi@firebolt.io
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/firebolt-db/firebolt-sqlalchemy
```

