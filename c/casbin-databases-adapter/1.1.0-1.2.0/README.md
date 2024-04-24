# Comparing `tmp/casbin_databases_adapter-1.1.0.tar.gz` & `tmp/casbin_databases_adapter-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casbin_databases_adapter-1.1.0.tar", last modified: Sat Mar 23 05:40:12 2024, max compression
+gzip compressed data, was "casbin_databases_adapter-1.2.0.tar", last modified: Wed Apr 24 12:56:58 2024, max compression
```

## Comparing `casbin_databases_adapter-1.1.0.tar` & `casbin_databases_adapter-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 05:40:12.499318 casbin_databases_adapter-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-23 05:39:38.000000 casbin_databases_adapter-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-03-23 05:40:12.499318 casbin_databases_adapter-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-23 05:39:38.000000 casbin_databases_adapter-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 05:40:12.499318 casbin_databases_adapter-1.1.0/casbin_databases_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 05:39:38.000000 casbin_databases_adapter-1.1.0/casbin_databases_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-03-23 05:39:38.000000 casbin_databases_adapter-1.1.0/casbin_databases_adapter/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 05:40:12.499318 casbin_databases_adapter-1.1.0/casbin_databases_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-03-23 05:40:12.000000 casbin_databases_adapter-1.1.0/casbin_databases_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-23 05:40:12.000000 casbin_databases_adapter-1.1.0/casbin_databases_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 05:40:12.000000 casbin_databases_adapter-1.1.0/casbin_databases_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-23 05:40:12.000000 casbin_databases_adapter-1.1.0/casbin_databases_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-23 05:40:12.000000 casbin_databases_adapter-1.1.0/casbin_databases_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-23 05:40:12.503317 casbin_databases_adapter-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-23 05:39:38.000000 casbin_databases_adapter-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 05:40:12.499318 casbin_databases_adapter-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-03-23 05:39:38.000000 casbin_databases_adapter-1.1.0/tests/test_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:58.570085 casbin_databases_adapter-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 12:56:26.000000 casbin_databases_adapter-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-24 12:56:58.570085 casbin_databases_adapter-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-24 12:56:26.000000 casbin_databases_adapter-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:58.566085 casbin_databases_adapter-1.2.0/casbin_databases_adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 12:56:26.000000 casbin_databases_adapter-1.2.0/casbin_databases_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-24 12:56:26.000000 casbin_databases_adapter-1.2.0/casbin_databases_adapter/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:58.570085 casbin_databases_adapter-1.2.0/casbin_databases_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-24 12:56:58.000000 casbin_databases_adapter-1.2.0/casbin_databases_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-24 12:56:58.000000 casbin_databases_adapter-1.2.0/casbin_databases_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:56:58.000000 casbin_databases_adapter-1.2.0/casbin_databases_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-24 12:56:58.000000 casbin_databases_adapter-1.2.0/casbin_databases_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 12:56:58.000000 casbin_databases_adapter-1.2.0/casbin_databases_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-24 12:56:58.570085 casbin_databases_adapter-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-24 12:56:26.000000 casbin_databases_adapter-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:58.570085 casbin_databases_adapter-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-04-24 12:56:26.000000 casbin_databases_adapter-1.2.0/tests/test_adapter.py
```

### Comparing `casbin_databases_adapter-1.1.0/LICENSE` & `casbin_databases_adapter-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `casbin_databases_adapter-1.1.0/PKG-INFO` & `casbin_databases_adapter-1.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: casbin_databases_adapter
-Version: 1.1.0
-Summary: This is an Adapter for PyCasbin that implemented using Databases connection to achieve async process
-Home-page: https://github.com/pycasbin/casbin-databases-adapter
-Author: Isa Setiawan Abdurrazaq
-Author-email: isasetiawan@protonmail.com
-License: Apache 2.0
-Keywords: casbin,asynccasbin,async,databases,casbin-adapter,rbac,access control,abac,acl,permission
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: asynccasbin==1.1.7
-Requires-Dist: databases==0.7.0
-Requires-Dist: SQLAlchemy==1.4.42
-
 # Databases Casbin Adapter
 
 [![GitHub Actions](https://github.com/pycasbin/casbin-databases-adapter/workflows/build/badge.svg?branch=master)](https://github.com/pycasbin/casbin-databases-adapter/actions)
 [![Coverage Status](https://coveralls.io/repos/github/pycasbin/casbin-databases-adapter/badge.svg?branch=master)](https://coveralls.io/github/pycasbin/casbin-databases-adapter?branch=master)
 [![Version](https://img.shields.io/pypi/v/casbin_databases_adapter.svg)](https://pypi.org/project/casbin_databases_adapter/)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/casbin_databases_adapter.svg)](https://pypi.org/project/casbin_databases_adapter/)
 [![Pyversions](https://img.shields.io/pypi/pyversions/casbin_databases_adapter.svg)](https://pypi.org/project/casbin_databases_adapter/)
@@ -34,14 +12,68 @@
 
 ## Installation
 
 ```
 pip install casbin_databases_adapter
 ```
 
+## Simple Example
+
+```python
+import casbin_databases_adapter
+import casbin
+from databases import Database
+import sqlalchemy
+from sqlalchemy import Table, Column, String, Integer
+from sqlalchemy.sql.ddl import CreateTable
+import asyncio
+
+DATABASE_URL = "sqlite+aiosqlite:///example.db"
+
+async def create_casbin_rule_table(db: Database):
+    metadata = sqlalchemy.MetaData()
+    table = Table(
+        "casbin_rules",
+        metadata,
+        Column("id", Integer, primary_key=True),
+        Column("ptype", String(255)),
+        Column("v0", String(255)),
+        Column("v1", String(255)),
+        Column("v2", String(255)),
+        Column("v3", String(255)),
+        Column("v4", String(255)),
+        Column("v5", String(255)),
+    )
+    q = CreateTable(table)
+    await db.execute(query=str(q))
+    return table
+
+async def main():
+    database = Database(DATABASE_URL)
+    await database.connect()
+    casbin_rule_table = await create_casbin_rule_table(database)
+    adapter = casbin_databases_adapter.DatabasesAdapter(db=database, table=casbin_rule_table)
+    
+    e = casbin.Enforcer('path/to/model.conf', adapter)
+    
+    sub = "alice"  # the user that wants to access a resource.
+    obj = "data1"  # the resource that is going to be accessed.
+    act = "read"  # the operation that the user performs on the resource.
+    
+    if e.enforce(sub, obj, act):
+        # permit alice to read data1
+        pass
+    else:
+        # deny the request, show an error
+        pass
+
+# run the main function
+asyncio.run(main())
+```
+
 ### Getting Help
 
 - [PyCasbin](https://github.com/casbin/pycasbin)
 
 ### License
 
-This project is licensed under the [Apache 2.0 license](LICENSE).
+This project is licensed under the [Apache 2.0 license](LICENSE).
```

### Comparing `casbin_databases_adapter-1.1.0/casbin_databases_adapter/adapter.py` & `casbin_databases_adapter-1.2.0/casbin_databases_adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `casbin_databases_adapter-1.1.0/setup.py` & `casbin_databases_adapter-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `casbin_databases_adapter-1.1.0/tests/test_adapter.py` & `casbin_databases_adapter-1.2.0/tests/test_adapter.py`

 * *Files identical despite different names*

