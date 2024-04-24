# Comparing `tmp/pih-ds-0.13.tar.gz` & `tmp/pih-ds-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-ds-0.13.tar", last modified: Wed Apr 10 01:29:49 2024, max compression
+gzip compressed data, was "pih-ds-0.14.tar", last modified: Wed Apr 24 06:43:15 2024, max compression
```

## Comparing `pih-ds-0.13.tar` & `pih-ds-0.14.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 01:29:49.203405 pih-ds-0.13/
-drwxrwxrwx   0        0        0        0 2024-04-10 01:29:48.412367 pih-ds-0.13/DataSourceService/
--rw-rw-rw-   0        0        0        0 2024-02-15 06:26:50.000000 pih-ds-0.13/DataSourceService/__init__.py
--rw-rw-rw-   0        0        0      144 2024-02-15 23:04:12.000000 pih-ds-0.13/DataSourceService/__main__.py
--rw-rw-rw-   0        0        0    15082 2024-02-15 07:48:06.000000 pih-ds-0.13/DataSourceService/anecdotica.py
--rw-rw-rw-   0        0        0    38013 2024-02-19 04:03:42.000000 pih-ds-0.13/DataSourceService/api.py
--rw-rw-rw-   0        0        0     3309 2024-04-09 23:56:15.000000 pih-ds-0.13/DataSourceService/const.py
--rw-rw-rw-   0        0        0     9780 2024-03-13 07:33:29.000000 pih-ds-0.13/DataSourceService/service.py
--rw-rw-rw-   0        0        0      100 2024-02-13 00:15:00.000000 pih-ds-0.13/DataSourceService/test.py
--rw-rw-rw-   0        0        0      380 2024-02-15 08:29:16.000000 pih-ds-0.13/DataSourceService/tools.py
--rw-rw-rw-   0        0        0      394 2024-04-10 01:29:49.187781 pih-ds-0.13/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 01:29:49.140907 pih-ds-0.13/pih_ds.egg-info/
--rw-rw-rw-   0        0        0      394 2024-04-10 01:29:47.000000 pih-ds-0.13/pih_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2024-04-10 01:29:47.000000 pih-ds-0.13/pih_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 01:29:47.000000 pih-ds-0.13/pih_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-10 01:29:47.000000 pih-ds-0.13/pih_ds.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2024-04-10 01:29:47.000000 pih-ds-0.13/pih_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-10 01:29:47.000000 pih-ds-0.13/pih_ds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 01:29:49.219033 pih-ds-0.13/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 06:43:15.763197 pih-ds-0.14/
+drwxrwxrwx   0        0        0        0 2024-04-24 06:43:15.126701 pih-ds-0.14/DataSourceService/
+-rw-rw-rw-   0        0        0        0 2024-02-15 06:26:50.000000 pih-ds-0.14/DataSourceService/__init__.py
+-rw-rw-rw-   0        0        0      144 2024-02-15 23:04:12.000000 pih-ds-0.14/DataSourceService/__main__.py
+-rw-rw-rw-   0        0        0    15082 2024-02-15 07:48:06.000000 pih-ds-0.14/DataSourceService/anecdotica.py
+-rw-rw-rw-   0        0        0    39146 2024-04-23 05:34:57.000000 pih-ds-0.14/DataSourceService/api.py
+-rw-rw-rw-   0        0        0     3309 2024-04-24 06:42:00.000000 pih-ds-0.14/DataSourceService/const.py
+-rw-rw-rw-   0        0        0     9779 2024-04-24 04:51:16.000000 pih-ds-0.14/DataSourceService/service.py
+-rw-rw-rw-   0        0        0      380 2024-02-15 08:29:16.000000 pih-ds-0.14/DataSourceService/tools.py
+-rw-rw-rw-   0        0        0      394 2024-04-24 06:43:15.700723 pih-ds-0.14/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 06:43:15.622547 pih-ds-0.14/pih_ds.egg-info/
+-rw-rw-rw-   0        0        0      394 2024-04-24 06:43:14.000000 pih-ds-0.14/pih_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2024-04-24 06:43:14.000000 pih-ds-0.14/pih_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 06:43:14.000000 pih-ds-0.14/pih_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-24 06:43:14.000000 pih-ds-0.14/pih_ds.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2024-04-24 06:43:14.000000 pih-ds-0.14/pih_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-24 06:43:14.000000 pih-ds-0.14/pih_ds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 06:43:15.763197 pih-ds-0.14/setup.cfg
```

### Comparing `pih-ds-0.13/DataSourceService/anecdotica.py` & `pih-ds-0.14/DataSourceService/anecdotica.py`

 * *Files identical despite different names*

### Comparing `pih-ds-0.13/DataSourceService/api.py` & `pih-ds-0.14/DataSourceService/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,27 +31,29 @@
 from mysql.connector import ProgrammingError
 from concurrent.futures import Future, as_completed
 from mysql.connector.pooling import PooledMySQLConnection
 
 executor: PIHThreadPoolExecutor = PIHThreadPoolExecutor(max_workers=1)
 executor_task_list: list[Future] = []
 
+
 class JsonLmdb(Lmdb):
     def _pre_key(self, value):
         return value.encode("utf-8")
 
     def _post_key(self, value):
         return value.decode("utf-8")
 
     def _pre_value(self, value):
         return json.dumps(value).encode("utf-8")
 
     def _post_value(self, value):
         return json.loads(value.decode("utf-8"))
 
+
 class DataStorageAndSourceApi:
     def __init__(self) -> None:
         self.connection_pool = pooling.MySQLConnectionPool(
             pool_name="pool",
             pool_size=DATABASE_POOL_SIZE,
             pool_reset_session=True,
             host=A.CT_H.BACKUP_WORKER.ALIAS,
@@ -251,72 +253,94 @@
                                     ),
                                     escaped_string=True,
                                 ),
                             )
                         )
                         for key, value in parameter_list
                     ]
-                timestamp: datetime | date | str | int | None = event.timestamp
-                if ne(timestamp):
-                    if isinstance(timestamp, str):
-                        timestamp_sign: str | None = None
-                        try:
-                            timestamp = A.D.datetime_or_date_from_string(timestamp)
-                        except ValueError as _:
-                            for sign in SIGN_COLLECTION:
-                                if timestamp.startswith(sign):
-                                    timestamp = A.D.datetime_or_date_from_string(
-                                        timestamp[len(sign) :].lstrip()
-                                    )
-                                    timestamp_sign = sign
-                                    break
-                        if n(timestamp_sign):
-                            if isinstance(timestamp, datetime):
-                                timestamp = j(("=", escs(timestamp)))
-                            elif isinstance(timestamp, date):
-                                timestamp = j(
-                                    (
-                                        KEYWORD_COLLECTION.LIKE,
-                                        escs(j((event.timestamp, ANY_SYMBOL))),
+                timestamp: (
+                    datetime | date | str | int | list[date | datetime | str] | None
+                ) = event.timestamp
+                if isinstance(timestamp, list):
+                    if len(timestamp) == 2:
+                        timestamp[0] = j((">=", timestamp[0]))
+                        timestamp[1] = j(("<=", timestamp[1]))
+                for timestamp_item in (
+                    timestamp if isinstance(timestamp, list) else [timestamp]
+                ):
+                    if ne(timestamp_item):
+                        if isinstance(timestamp_item, str):
+                            timestamp_sign: str | None = None
+                            try:
+                                timestamp_item = A.D.datetime_or_date_from_string(
+                                    timestamp_item
+                                )
+                            except ValueError as _:
+                                for sign in SIGN_COLLECTION:
+                                    if timestamp_item.startswith(sign):
+                                        timestamp_item = (
+                                            A.D.datetime_or_date_from_string(
+                                                timestamp_item[len(sign) :].lstrip()
+                                            )
+                                        )
+                                        timestamp_sign = sign
+                                        break
+                            if n(timestamp_sign):
+                                if isinstance(timestamp_item, datetime):
+                                    timestamp_item = j(("=", escs(timestamp_item)))
+                                elif isinstance(timestamp_item, date):
+                                    timestamp_item = js(
+                                        (
+                                            KEYWORD_COLLECTION.LIKE,
+                                            escs(j((event.timestamp, ANY_SYMBOL))),
+                                        )
                                     )
+                            else:
+                                timestamp_item = j(
+                                    (timestamp_sign, escs(timestamp_item))
                                 )
-                        else:
-                            timestamp = j((timestamp_sign, escs(timestamp)))
-                        condition_statement_list.append(j(("timestamp", timestamp)))
+                            condition_statement_list.append(
+                                js(("timestamp", timestamp_item))
+                            )
                 query_string = js(
                     (
                         if_else(
-                            value in [ACTIONS.SELECT, ACTIONS.COUNT], "select", "delete"
+                            value in [ACTIONS.SELECT, ACTIONS.COUNT],
+                            "select",
+                            "delete",
                         ),
                         if_else(
                             value == ACTIONS.SELECT,
                             A.D.list_to_string(self.get_events_table_field_list()),
                             if_else(value == ACTIONS.COUNT, "count(*)", ""),
                         ),
                         js(
                             (
                                 "from",
                                 EVENTS_TABLE,
                                 (
                                     ""
                                     if e(condition_statement_list)
                                     else js(
-                                        ("where", j(condition_statement_list, " and "))
+                                        (
+                                            "where",
+                                            j(condition_statement_list, " and "),
+                                        )
                                     )
                                 ),
                                 (
                                     js(
                                         (
                                             "order by timestamp",
-                                            "asc" if timestamp > 0 else "desc",
+                                            "asc" if timestamp_item > 0 else "desc",
                                             "limit",
-                                            abs(timestamp),
+                                            abs(timestamp_item),
                                         )
                                     )
-                                    if isinstance(timestamp, int)
+                                    if isinstance(timestamp_item, int)
                                     else None
                                 ),
                             )
                         ),
                     )
                 )
             if value == ACTIONS.INSERT:
```

### Comparing `pih-ds-0.13/DataSourceService/const.py` & `pih-ds-0.14/DataSourceService/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 DATABASE_NAME: str = "pih_db"
 DATABASE_PORT: int = 3306
 DATABASE_POOL_SIZE: int = 5
 
 HOST = Hosts.BACKUP_WORKER
 
-VERSION: str = "0.13"
+VERSION: str = "0.14"
 
 MODULES: tuple[str, ...] = ("mysql-connector-python", "lmdb==1.4.0", "lmdbm", "dadata")
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Data storage and source service",
     host=HOST.NAME,
```

### Comparing `pih-ds-0.13/DataSourceService/service.py` & `pih-ds-0.14/DataSourceService/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import ipih
 
 from pih import A
 from DataSourceService.const import SD, JOKE
 
 SC = A.CT_SC
 
-ISOLATED: bool = False
+ISOLATED: bool = True
 
 
 def start(as_standalone: bool = False) -> None:
 
     if A.U.for_service(SD, as_standalone=as_standalone):
 
         from pih.collections import (
@@ -25,16 +25,16 @@
             PolibasePersonVisitNotification,
             ChillerIndicationsValueContainer,
             PolibasePersonVisitNotificationDS,
             PolibasePersonNotificationConfirmation,
         )
         from pih.tools import ParameterList
         from pih.consts.errors import Error
-        from DataSourceService.api import DataStorageAndSourceApi as Api
         from DataSourceService.anecdotica import RandomItemApi
+        from DataSourceService.api import DataStorageAndSourceApi as Api
         
         import grpc
         from typing import Any
         from dadata import Dadata
     
 
         api: Api = Api()
```

