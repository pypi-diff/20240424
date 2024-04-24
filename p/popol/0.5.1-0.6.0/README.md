# Comparing `tmp/popol-0.5.1.tar.gz` & `tmp/popol-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popol-0.5.1.tar", max compression
+gzip compressed data, was "popol-0.6.0.tar", max compression
```

## Comparing `popol-0.5.1.tar` & `popol-0.6.0.tar`

### file list

```diff
@@ -1,58 +1,55 @@
--rw-r--r--   0        0        0     1072 2022-12-24 20:29:44.870854 popol-0.5.1/LICENSE
--rw-r--r--   0        0        0     1159 2022-12-24 20:29:44.870854 popol-0.5.1/README.md
--rw-r--r--   0        0        0      677 2022-12-24 20:29:44.874854 popol-0.5.1/popol/__init__.py
--rw-r--r--   0        0        0     1826 2022-12-24 20:29:44.874854 popol-0.5.1/popol/__main__.py
--rw-r--r--   0        0        0     2645 2022-12-24 20:29:44.874854 popol-0.5.1/popol/cache/__init__.py
--rw-r--r--   0        0        0       83 2022-12-24 20:29:44.874854 popol-0.5.1/popol/cache/backends/__init__.py
--rw-r--r--   0        0        0     1253 2022-12-24 20:29:44.874854 popol-0.5.1/popol/cache/backends/base.py
--rw-r--r--   0        0        0      508 2022-12-24 20:29:44.874854 popol-0.5.1/popol/cache/backends/dummy.py
--rw-r--r--   0        0        0     5884 2022-12-24 20:29:44.874854 popol-0.5.1/popol/cache/backends/redis.py
--rw-r--r--   0        0        0     3322 2022-12-24 20:29:44.874854 popol-0.5.1/popol/cache/decorators.py
--rw-r--r--   0        0        0      283 2022-12-24 20:29:44.874854 popol-0.5.1/popol/cache/globals.py
--rw-r--r--   0        0        0      681 2022-12-24 20:29:44.874854 popol-0.5.1/popol/cache/helpers.py
--rw-r--r--   0        0        0      830 2022-12-24 20:29:44.874854 popol-0.5.1/popol/cache/key.py
--rw-r--r--   0        0        0      127 2022-12-24 20:29:44.874854 popol-0.5.1/popol/cache/serializers/__init__.py
--rw-r--r--   0        0        0      520 2022-12-24 20:29:44.874854 popol-0.5.1/popol/cache/serializers/base.py
--rw-r--r--   0        0        0     1203 2022-12-24 20:29:44.874854 popol-0.5.1/popol/cache/serializers/json.py
--rw-r--r--   0        0        0      788 2022-12-24 20:29:44.874854 popol-0.5.1/popol/cache/serializers/pickle.py
--rw-r--r--   0        0        0      156 2022-12-24 20:29:44.874854 popol-0.5.1/popol/context/__init__.py
--rw-r--r--   0        0        0      245 2022-12-24 20:29:44.874854 popol-0.5.1/popol/context/globals.py
--rw-r--r--   0        0        0    12006 2022-12-24 20:29:44.874854 popol-0.5.1/popol/context/proxy.py
--rw-r--r--   0        0        0       70 2022-12-24 20:29:44.874854 popol-0.5.1/popol/context/vars.py
--rw-r--r--   0        0        0        0 2022-12-24 20:29:44.874854 popol-0.5.1/popol/db/__init__.py
--rw-r--r--   0        0        0     2253 2022-12-24 20:29:44.874854 popol-0.5.1/popol/db/sqlmodel/__init__.py
--rw-r--r--   0        0        0      152 2022-12-24 20:29:44.874854 popol-0.5.1/popol/db/sqlmodel/globals.py
--rw-r--r--   0        0        0      979 2022-12-24 20:29:44.874854 popol-0.5.1/popol/db/sqlmodel/models.py
--rw-r--r--   0        0        0     1354 2022-12-24 20:29:44.874854 popol-0.5.1/popol/email/__init__.py
--rw-r--r--   0        0        0     3191 2022-12-24 20:29:44.874854 popol-0.5.1/popol/email/backend.py
--rw-r--r--   0        0        0      173 2022-12-24 20:29:44.874854 popol-0.5.1/popol/email/globals.py
--rw-r--r--   0        0        0     2780 2022-12-24 20:29:44.874854 popol-0.5.1/popol/email/message.py
--rw-r--r--   0        0        0        0 2022-12-24 20:29:44.874854 popol-0.5.1/popol/jobs/__init__.py
--rw-r--r--   0        0        0      798 2022-12-24 20:29:44.874854 popol-0.5.1/popol/jobs/saq/__init__.py
--rw-r--r--   0        0        0     1799 2022-12-24 20:29:44.874854 popol-0.5.1/popol/jobs/saq/cli.py
--rw-r--r--   0        0        0      955 2022-12-24 20:29:44.874854 popol-0.5.1/popol/jobs/saq/config.py
--rw-r--r--   0        0        0      258 2022-12-24 20:29:44.874854 popol-0.5.1/popol/jobs/saq/globals.py
--rw-r--r--   0        0        0     1509 2022-12-24 20:29:44.874854 popol-0.5.1/popol/jobs/saq/queue.py
--rw-r--r--   0        0        0      864 2022-12-24 20:29:44.874854 popol-0.5.1/popol/json.py
--rw-r--r--   0        0        0     2634 2022-12-24 20:29:44.874854 popol-0.5.1/popol/pagination.py
--rw-r--r--   0        0        0      425 2022-12-24 20:29:44.874854 popol-0.5.1/popol/schema.py
--rw-r--r--   0        0        0      885 2022-12-24 20:29:44.874854 popol-0.5.1/popol/templates/.pre-commit-config.yaml
--rw-r--r--   0        0        0      438 2022-12-24 20:29:44.874854 popol-0.5.1/popol/templates/README.md
--rw-r--r--   0        0        0        0 2022-12-24 20:29:44.874854 popol-0.5.1/popol/templates/app/__init__.py
--rw-r--r--   0        0        0      108 2022-12-24 20:29:44.874854 popol-0.5.1/popol/templates/app/extensions/__init__.py
--rw-r--r--   0        0        0      287 2022-12-24 20:29:44.874854 popol-0.5.1/popol/templates/app/main.py
--rw-r--r--   0        0        0      108 2022-12-24 20:29:44.874854 popol-0.5.1/popol/templates/app/middleware/__init__.py
--rw-r--r--   0        0        0      102 2022-12-24 20:29:44.874854 popol-0.5.1/popol/templates/app/routers/__init__.py
--rw-r--r--   0        0        0      541 2022-12-24 20:29:44.874854 popol-0.5.1/popol/templates/app/settings/__init__.py
--rw-r--r--   0        0        0      171 2022-12-24 20:29:44.874854 popol-0.5.1/popol/templates/app/settings/development.py
--rw-r--r--   0        0        0      165 2022-12-24 20:29:44.874854 popol-0.5.1/popol/templates/app/settings/local.py
--rw-r--r--   0        0        0      170 2022-12-24 20:29:44.874854 popol-0.5.1/popol/templates/app/settings/production.py
--rw-r--r--   0        0        0       31 2022-12-24 20:29:44.874854 popol-0.5.1/popol/templates/pyproject.toml
--rw-r--r--   0        0        0       62 2022-12-24 20:29:44.874854 popol-0.5.1/popol/templates/requirements-dev.txt
--rw-r--r--   0        0        0       13 2022-12-24 20:29:44.874854 popol-0.5.1/popol/templates/requirements.txt
--rw-r--r--   0        0        0        0 2022-12-24 20:29:44.874854 popol-0.5.1/popol/templates/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-12-24 20:29:44.874854 popol-0.5.1/popol/templates/tests/conftest.py
--rw-r--r--   0        0        0     3364 2022-12-24 20:29:44.874854 popol-0.5.1/popol/utils.py
--rw-r--r--   0        0        0     2575 2022-12-24 20:29:44.874854 popol-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     3092 1970-01-01 00:00:00.000000 popol-0.5.1/setup.py
--rw-r--r--   0        0        0     3669 1970-01-01 00:00:00.000000 popol-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-24 21:32:52.965544 popol-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1128 2024-04-24 21:32:52.965544 popol-0.6.0/README.md
+-rw-r--r--   0        0        0      677 2024-04-24 21:32:52.969544 popol-0.6.0/popol/__init__.py
+-rw-r--r--   0        0        0     1858 2024-04-24 21:32:52.969544 popol-0.6.0/popol/__main__.py
+-rw-r--r--   0        0        0     2645 2024-04-24 21:32:52.969544 popol-0.6.0/popol/cache/__init__.py
+-rw-r--r--   0        0        0       83 2024-04-24 21:32:52.969544 popol-0.6.0/popol/cache/backends/__init__.py
+-rw-r--r--   0        0        0     1253 2024-04-24 21:32:52.969544 popol-0.6.0/popol/cache/backends/base.py
+-rw-r--r--   0        0        0      508 2024-04-24 21:32:52.969544 popol-0.6.0/popol/cache/backends/dummy.py
+-rw-r--r--   0        0        0     5884 2024-04-24 21:32:52.969544 popol-0.6.0/popol/cache/backends/redis.py
+-rw-r--r--   0        0        0     3322 2024-04-24 21:32:52.969544 popol-0.6.0/popol/cache/decorators.py
+-rw-r--r--   0        0        0      283 2024-04-24 21:32:52.969544 popol-0.6.0/popol/cache/globals.py
+-rw-r--r--   0        0        0      681 2024-04-24 21:32:52.969544 popol-0.6.0/popol/cache/helpers.py
+-rw-r--r--   0        0        0      830 2024-04-24 21:32:52.969544 popol-0.6.0/popol/cache/key.py
+-rw-r--r--   0        0        0      127 2024-04-24 21:32:52.969544 popol-0.6.0/popol/cache/serializers/__init__.py
+-rw-r--r--   0        0        0      520 2024-04-24 21:32:52.969544 popol-0.6.0/popol/cache/serializers/base.py
+-rw-r--r--   0        0        0     1203 2024-04-24 21:32:52.969544 popol-0.6.0/popol/cache/serializers/json.py
+-rw-r--r--   0        0        0      788 2024-04-24 21:32:52.969544 popol-0.6.0/popol/cache/serializers/pickle.py
+-rw-r--r--   0        0        0      156 2024-04-24 21:32:52.969544 popol-0.6.0/popol/context/__init__.py
+-rw-r--r--   0        0        0      245 2024-04-24 21:32:52.969544 popol-0.6.0/popol/context/globals.py
+-rw-r--r--   0        0        0    12006 2024-04-24 21:32:52.969544 popol-0.6.0/popol/context/proxy.py
+-rw-r--r--   0        0        0       70 2024-04-24 21:32:52.969544 popol-0.6.0/popol/context/vars.py
+-rw-r--r--   0        0        0      250 2024-04-24 21:32:52.969544 popol-0.6.0/popol/dantic.py
+-rw-r--r--   0        0        0        0 2024-04-24 21:32:52.969544 popol-0.6.0/popol/db/__init__.py
+-rw-r--r--   0        0        0     2215 2024-04-24 21:32:52.969544 popol-0.6.0/popol/db/sqlmodel/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-24 21:32:52.969544 popol-0.6.0/popol/db/sqlmodel/globals.py
+-rw-r--r--   0        0        0      958 2024-04-24 21:32:52.969544 popol-0.6.0/popol/db/sqlmodel/models.py
+-rw-r--r--   0        0        0     1335 2024-04-24 21:32:52.969544 popol-0.6.0/popol/email/__init__.py
+-rw-r--r--   0        0        0     3192 2024-04-24 21:32:52.969544 popol-0.6.0/popol/email/backend.py
+-rw-r--r--   0        0        0      173 2024-04-24 21:32:52.969544 popol-0.6.0/popol/email/globals.py
+-rw-r--r--   0        0        0     2780 2024-04-24 21:32:52.969544 popol-0.6.0/popol/email/message.py
+-rw-r--r--   0        0        0        0 2024-04-24 21:32:52.969544 popol-0.6.0/popol/jobs/__init__.py
+-rw-r--r--   0        0        0      798 2024-04-24 21:32:52.969544 popol-0.6.0/popol/jobs/saq/__init__.py
+-rw-r--r--   0        0        0     1799 2024-04-24 21:32:52.969544 popol-0.6.0/popol/jobs/saq/cli.py
+-rw-r--r--   0        0        0      955 2024-04-24 21:32:52.969544 popol-0.6.0/popol/jobs/saq/config.py
+-rw-r--r--   0        0        0      258 2024-04-24 21:32:52.969544 popol-0.6.0/popol/jobs/saq/globals.py
+-rw-r--r--   0        0        0     1509 2024-04-24 21:32:52.969544 popol-0.6.0/popol/jobs/saq/queue.py
+-rw-r--r--   0        0        0      895 2024-04-24 21:32:52.969544 popol-0.6.0/popol/json.py
+-rw-r--r--   0        0        0     2634 2024-04-24 21:32:52.969544 popol-0.6.0/popol/pagination.py
+-rw-r--r--   0        0        0      561 2024-04-24 21:32:52.969544 popol-0.6.0/popol/schema.py
+-rw-r--r--   0        0        0      885 2024-04-24 21:32:52.973544 popol-0.6.0/popol/templates/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      438 2024-04-24 21:32:52.973544 popol-0.6.0/popol/templates/README.md
+-rw-r--r--   0        0        0        0 2024-04-24 21:32:52.973544 popol-0.6.0/popol/templates/app/__init__.py
+-rw-r--r--   0        0        0      108 2024-04-24 21:32:52.973544 popol-0.6.0/popol/templates/app/extensions/__init__.py
+-rw-r--r--   0        0        0      287 2024-04-24 21:32:52.973544 popol-0.6.0/popol/templates/app/main.py
+-rw-r--r--   0        0        0      108 2024-04-24 21:32:52.973544 popol-0.6.0/popol/templates/app/middleware/__init__.py
+-rw-r--r--   0        0        0      102 2024-04-24 21:32:52.973544 popol-0.6.0/popol/templates/app/routers/__init__.py
+-rw-r--r--   0        0        0      663 2024-04-24 21:32:52.973544 popol-0.6.0/popol/templates/app/settings.py
+-rw-r--r--   0        0        0       31 2024-04-24 21:32:52.973544 popol-0.6.0/popol/templates/pyproject.toml
+-rw-r--r--   0        0        0       62 2024-04-24 21:32:52.973544 popol-0.6.0/popol/templates/requirements-dev.txt
+-rw-r--r--   0        0        0       13 2024-04-24 21:32:52.973544 popol-0.6.0/popol/templates/requirements.txt
+-rw-r--r--   0        0        0        0 2024-04-24 21:32:52.973544 popol-0.6.0/popol/templates/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 21:32:52.973544 popol-0.6.0/popol/templates/tests/conftest.py
+-rw-r--r--   0        0        0     3364 2024-04-24 21:32:52.973544 popol-0.6.0/popol/utils.py
+-rw-r--r--   0        0        0     2746 2024-04-24 21:32:52.973544 popol-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3744 1970-01-01 00:00:00.000000 popol-0.6.0/PKG-INFO
```

### Comparing `popol-0.5.1/LICENSE` & `popol-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `popol-0.5.1/README.md` & `popol-0.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,42 +9,41 @@
 ## Features 🌟
 
 - [x] Project Layout
 - [x] Command Line Interface (like `flask` command)
 - [x] Pagination
 - Cache Framework
 
-    - Backends
+  - Backends
 
-        - [x] Redis (Sync/Async)
-        - [ ] Memcached
+    - [x] Redis (Sync/Async)
+    - [ ] Memcached
 
-    - Serializers
+  - Serializers
 
-        - [x] JSON
-        - [x] Pickle
-        - [ ] MsgPack
+    - [x] JSON
+    - [x] Pickle
+    - [ ] MsgPack
 
 - ORM Integration
 
-    - [x] SQLModel (Async/Sync)
-    - [ ] Tortoise ORM
+  - [x] SQLModel (Async/Sync)
+  - [ ] Tortoise ORM
 
 - ODM Integration
 
-    - [ ] MongoEngine
+  - [ ] MongoEngine
 
 - [x] SMTP client (using aiosmtplib) to send emails.
 - Background Jobs:
 
-    - [x] SAQ queue support for task scheduling
-
+  - [x] SAQ queue support for task scheduling
 
 ## Installation 📚
 
-```
+```sh
 pip install popol>=0.4.0
 ```
 
 ## Documentation 📖
 
 Not available at this time, please learn from the [examples](https://github.com/aprilahijriyan/popol/tree/main/examples).
```

### Comparing `popol-0.5.1/popol/__init__.py` & `popol-0.6.0/popol/__init__.py`

 * *Files identical despite different names*

### Comparing `popol-0.5.1/popol/__main__.py` & `popol-0.6.0/popol/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,21 +18,20 @@
     for ep in iter_entry_points("popol.commands"):
         try:
             cmd = ep.load()
             if isinstance(cmd, Typer):
                 popol.add_typer(cmd)
             else:
                 popol.command(ep.name, cmd)
-        except Exception:
-            # TODO: log error
-            pass
+        except Exception as e:
+            echo(f"Failed to load command {ep.name}: {e}", err=True)
 
 
 @popol.callback()
-def init(
+def _calbback(
     ctx: Context,
     version: Optional[bool] = Option(
         None, "-v", "--version", is_eager=True, help="Show version number and exit"
     ),
 ):
     if ctx.resilient_parsing:  # pragma: no cover
         return
```

### Comparing `popol-0.5.1/popol/cache/__init__.py` & `popol-0.6.0/popol/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `popol-0.5.1/popol/cache/backends/base.py` & `popol-0.6.0/popol/cache/backends/base.py`

 * *Files identical despite different names*

### Comparing `popol-0.5.1/popol/cache/backends/redis.py` & `popol-0.6.0/popol/cache/backends/redis.py`

 * *Files identical despite different names*

### Comparing `popol-0.5.1/popol/cache/decorators.py` & `popol-0.6.0/popol/cache/decorators.py`

 * *Files identical despite different names*

### Comparing `popol-0.5.1/popol/cache/helpers.py` & `popol-0.6.0/popol/cache/helpers.py`

 * *Files identical despite different names*

### Comparing `popol-0.5.1/popol/cache/key.py` & `popol-0.6.0/popol/cache/key.py`

 * *Files identical despite different names*

### Comparing `popol-0.5.1/popol/cache/serializers/base.py` & `popol-0.6.0/popol/cache/serializers/base.py`

 * *Files identical despite different names*

### Comparing `popol-0.5.1/popol/cache/serializers/json.py` & `popol-0.6.0/popol/cache/serializers/json.py`

 * *Files identical despite different names*

### Comparing `popol-0.5.1/popol/cache/serializers/pickle.py` & `popol-0.6.0/popol/cache/serializers/pickle.py`

 * *Files identical despite different names*

### Comparing `popol-0.5.1/popol/context/proxy.py` & `popol-0.6.0/popol/context/proxy.py`

 * *Files identical despite different names*

### Comparing `popol-0.5.1/popol/db/sqlmodel/__init__.py` & `popol-0.6.0/popol/db/sqlmodel/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from typing import Union
+from typing import Any, Union
 
 from fastapi import FastAPI
-from pydantic import BaseSettings
 
 from ...utils import get_settings
 
 try:
     from sqlalchemy.engine import Engine
     from sqlalchemy.ext.asyncio import AsyncEngine, create_async_engine
     from sqlmodel import Session, SQLModel, create_engine
@@ -29,15 +28,15 @@
     def open(self) -> Union[Session, AsyncSession]:
         if self.is_async:
             return AsyncSession(self.engine)
         else:
             return Session(self.engine)
 
 
-def setup(app: FastAPI, settings: BaseSettings = None) -> Database:
+def setup(app: FastAPI, settings: Any = None) -> Database:
     """
     Install the sqlmodel plugin to the app.
     This will attach 1 attribute to `app.state` i.e:
 
     * `db` - `popol.sqlmodel.Database` instance object to open db connection.
 
     Args:
```

### Comparing `popol-0.5.1/popol/email/__init__.py` & `popol-0.6.0/popol/email/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from typing import Any
+
 from fastapi import FastAPI
-from pydantic import BaseSettings
 
 from ..utils import get_settings, import_attr
 from .backend import EmailBackend
 
 
-def setup(app: FastAPI, settings: BaseSettings = None) -> EmailBackend:
+def setup(app: FastAPI, settings: Any = None) -> EmailBackend:
     """
     Install the email plugin to the app.
     This will attach 1 attribute to `app.state` i.e:
 
     * `email` - `popol.email.backend.EmailBackend` instance object for sending email.
 
     Args:
```

### Comparing `popol-0.5.1/popol/email/backend.py` & `popol-0.6.0/popol/email/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Awaitable, Iterable, Optional, Sequence, Union
 
 try:
     from aiosmtplib import SMTP
-    from aiosmtplib.connection import DEFAULT_TIMEOUT
+    from aiosmtplib.smtp import DEFAULT_TIMEOUT
 except ImportError:
     raise RuntimeError(
-        "aiosmtplib is not installed. Please install it with `pip install aiosmtplib`"
+        "aiosmtplib is not installed. Please install it with `pip install aiosmtplib>=3.0.1`"
     )
 
 from ..utils import run_sync
 from .message import Message
 
 
 class EmailBackend:
```

### Comparing `popol-0.5.1/popol/email/message.py` & `popol-0.6.0/popol/email/message.py`

 * *Files identical despite different names*

### Comparing `popol-0.5.1/popol/jobs/saq/__init__.py` & `popol-0.6.0/popol/jobs/saq/__init__.py`

 * *Files identical despite different names*

### Comparing `popol-0.5.1/popol/jobs/saq/cli.py` & `popol-0.6.0/popol/jobs/saq/cli.py`

 * *Files identical despite different names*

### Comparing `popol-0.5.1/popol/jobs/saq/config.py` & `popol-0.6.0/popol/jobs/saq/config.py`

 * *Files identical despite different names*

### Comparing `popol-0.5.1/popol/jobs/saq/queue.py` & `popol-0.6.0/popol/jobs/saq/queue.py`

 * *Files identical despite different names*

### Comparing `popol-0.5.1/popol/json.py` & `popol-0.6.0/popol/json.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 Taken from: https://github.com/aprilahijriyan/falca/blob/main/falca/compat.py
 """
 
 from functools import partial
 
 from pydantic import BaseModel
 
+from . import dantic
+
 
 def _json_default(o: object):
     if isinstance(o, BaseModel):
-        return o.dict()
+        return dantic.to_dict(o)
     raise ValueError(f"unknown object {o!r}")
 
 
 try:
     import orjson as json
 
     _dumps = json.dumps
```

### Comparing `popol-0.5.1/popol/pagination.py` & `popol-0.6.0/popol/pagination.py`

 * *Files identical despite different names*

### Comparing `popol-0.5.1/popol/templates/.pre-commit-config.yaml` & `popol-0.6.0/popol/templates/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `popol-0.5.1/popol/utils.py` & `popol-0.6.0/popol/utils.py`

 * *Files identical despite different names*

### Comparing `popol-0.5.1/pyproject.toml` & `popol-0.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "popol"
-version = "0.5.1"
+version = "0.6.0"
 description = "Adding new power to your FastAPI application ⛅"
 authors = ["aprilahijriyan <hijriyan23@gmail.com>"]
 license = "MIT"
 maintainers = ["aprilahijriyan <hijriyan23@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/aprilahijriyan/popol"
 repository = "https://github.com/aprilahijriyan/popol"
@@ -26,40 +26,42 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-fastapi = {version = "^0.88.0", optional = true}
-uvicorn = {extras = ["standard"], version = "^0.20.0", optional = true}
-pydantic = {extras = ["email"], version = "^1.10.2", optional = true}
-asyncer = "^0.0.1"
-typer = "^0.7.0"
+fastapi = {version = "^0.110.2", optional = true}
+uvicorn = {extras = ["standard"], version = "^0.29.0", optional = true}
+pydantic = {extras = ["email"], version = "^2.7.0", optional = true}
+asyncer = "^0.0.5"
+typer = {version = "^0.12.3"}
 redis = {version = "^4.3.4", optional = true}
-saq = {version = "^0.8.0", optional = true}
-sqlmodel = {version = "^0.0.6", optional = true}
-pyhumps = {version = "^3.7.2", optional = true}
-aiosmtplib = {version = "^1.1.6", optional = true}
+saq = {version = "^0.12.5", optional = true}
+sqlmodel = {version = "^0.0.16", optional = true}
+pyhumps = {version = "^3.8.0", optional = true}
+aiosmtplib = {version = "^3.0.1", optional = true}
+pydantic-settings = {version = "^2.2.1", optional = true}
 
 [tool.poetry.extras]
 
 # units
 sqlmodel = ["sqlmodel", "pyhumps"]
 redis = ["redis"]
 saq = ["saq"]
 aiosmtplib = ["aiosmtplib"]
 
 # bundles
 cache = ["redis"]
 background_jobs = ["saq"]
 orm = ["sqlmodel", "pyhumps"]
+fastapi = ["fastapi", "uvicorn", "pydantic", "pydantic-settings"]
 
 # all
-all = ["fastapi", "pydantic", "sqlmodel", "pyhumps", "redis", "saq", "aiosmtplib"]
+all = ["fastapi", "uvicorn", "pydantic", "pydantic-settings", "sqlmodel", "pyhumps", "redis", "saq", "aiosmtplib"]
 
 [tool.poetry.dev-dependencies]
 ipython = "^8.1.1"
 pre-commit = "^2.17.0"
 black = "^22.1.0"
 pytest = "^7.0.1"
 mkdocs-material = "^8.2.5"
```

### Comparing `popol-0.5.1/PKG-INFO` & `popol-0.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popol
-Version: 0.5.1
+Version: 0.6.0
 Summary: Adding new power to your FastAPI application ⛅
 Home-page: https://github.com/aprilahijriyan/popol
 License: MIT
 Author: aprilahijriyan
 Author-email: hijriyan23@gmail.com
 Maintainer: aprilahijriyan
 Maintainer-email: hijriyan23@gmail.com
@@ -18,41 +18,41 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: aiosmtplib
 Provides-Extra: all
 Provides-Extra: background-jobs
 Provides-Extra: cache
+Provides-Extra: fastapi
 Provides-Extra: orm
 Provides-Extra: redis
 Provides-Extra: saq
 Provides-Extra: sqlmodel
-Requires-Dist: aiosmtplib (>=1.1.6,<2.0.0) ; extra == "aiosmtplib" or extra == "all"
-Requires-Dist: asyncer (>=0.0.1,<0.0.2)
-Requires-Dist: fastapi (>=0.88.0,<0.89.0) ; extra == "all"
-Requires-Dist: pydantic[email] (>=1.10.2,<2.0.0) ; extra == "all"
-Requires-Dist: pyhumps (>=3.7.2,<4.0.0) ; extra == "sqlmodel" or extra == "orm" or extra == "all"
+Requires-Dist: aiosmtplib (>=3.0.1,<4.0.0) ; extra == "aiosmtplib" or extra == "all"
+Requires-Dist: asyncer (>=0.0.5,<0.0.6)
+Requires-Dist: fastapi (>=0.110.2,<0.111.0) ; extra == "fastapi" or extra == "all"
+Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0) ; extra == "fastapi" or extra == "all"
+Requires-Dist: pydantic[email] (>=2.7.0,<3.0.0) ; extra == "fastapi" or extra == "all"
+Requires-Dist: pyhumps (>=3.8.0,<4.0.0) ; extra == "sqlmodel" or extra == "orm" or extra == "all"
 Requires-Dist: redis (>=4.3.4,<5.0.0) ; extra == "redis" or extra == "cache" or extra == "all"
-Requires-Dist: saq (>=0.8.0,<0.9.0) ; extra == "saq" or extra == "background-jobs" or extra == "all"
-Requires-Dist: sqlmodel (>=0.0.6,<0.0.7) ; extra == "sqlmodel" or extra == "orm" or extra == "all"
-Requires-Dist: typer (>=0.7.0,<0.8.0)
-Requires-Dist: uvicorn[standard] (>=0.20.0,<0.21.0)
+Requires-Dist: saq (>=0.12.5,<0.13.0) ; extra == "saq" or extra == "background-jobs" or extra == "all"
+Requires-Dist: sqlmodel (>=0.0.16,<0.0.17) ; extra == "sqlmodel" or extra == "orm" or extra == "all"
+Requires-Dist: typer (>=0.12.3,<0.13.0)
+Requires-Dist: uvicorn[standard] (>=0.29.0,<0.30.0) ; extra == "fastapi" or extra == "all"
 Project-URL: Bug Tracker, https://github.com/aprilahijriyan/popol/issues
 Project-URL: Repository, https://github.com/aprilahijriyan/popol
 Description-Content-Type: text/markdown
 
 # Popol ⛅
 
 > Adding new power to your FastAPI application ⛅
@@ -64,43 +64,42 @@
 ## Features 🌟
 
 - [x] Project Layout
 - [x] Command Line Interface (like `flask` command)
 - [x] Pagination
 - Cache Framework
 
-    - Backends
+  - Backends
 
-        - [x] Redis (Sync/Async)
-        - [ ] Memcached
+    - [x] Redis (Sync/Async)
+    - [ ] Memcached
 
-    - Serializers
+  - Serializers
 
-        - [x] JSON
-        - [x] Pickle
-        - [ ] MsgPack
+    - [x] JSON
+    - [x] Pickle
+    - [ ] MsgPack
 
 - ORM Integration
 
-    - [x] SQLModel (Async/Sync)
-    - [ ] Tortoise ORM
+  - [x] SQLModel (Async/Sync)
+  - [ ] Tortoise ORM
 
 - ODM Integration
 
-    - [ ] MongoEngine
+  - [ ] MongoEngine
 
 - [x] SMTP client (using aiosmtplib) to send emails.
 - Background Jobs:
 
-    - [x] SAQ queue support for task scheduling
-
+  - [x] SAQ queue support for task scheduling
 
 ## Installation 📚
 
-```
+```sh
 pip install popol>=0.4.0
 ```
 
 ## Documentation 📖
 
 Not available at this time, please learn from the [examples](https://github.com/aprilahijriyan/popol/tree/main/examples).
```

