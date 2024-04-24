# Comparing `tmp/vvm_lib-1.0.1.tar.gz` & `tmp/vvm_lib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vvm_lib-1.0.1.tar", last modified: Tue Apr 23 05:45:39 2024, max compression
+gzip compressed data, was "vvm_lib-1.0.2.tar", last modified: Wed Apr 24 07:14:21 2024, max compression
```

## Comparing `vvm_lib-1.0.1.tar` & `vvm_lib-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 05:45:39.277611 vvm_lib-1.0.1/
--rw-rw-rw-   0        0        0      454 2024-04-23 05:45:39.277611 vvm_lib-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4707 2024-04-23 05:44:57.000000 vvm_lib-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 05:45:39.283541 vvm_lib-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      747 2024-04-23 05:28:25.000000 vvm_lib-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 05:45:39.253531 vvm_lib-1.0.1/vvm_lib/
-drwxrwxrwx   0        0        0        0 2024-04-23 05:45:39.276582 vvm_lib-1.0.1/vvm_lib/DB/
--rw-rw-rw-   0        0        0       30 2024-04-22 09:33:28.000000 vvm_lib-1.0.1/vvm_lib/DB/__init__.py
--rw-rw-rw-   0        0        0     6564 2024-04-23 05:43:08.000000 vvm_lib-1.0.1/vvm_lib/DB/db.py
--rw-rw-rw-   0        0        0      229 2024-04-20 07:29:21.000000 vvm_lib-1.0.1/vvm_lib/__init__.py
--rw-rw-rw-   0        0        0     2747 2024-04-20 07:29:21.000000 vvm_lib-1.0.1/vvm_lib/google_book.py
--rw-rw-rw-   0        0        0     3545 2024-04-20 07:29:21.000000 vvm_lib-1.0.1/vvm_lib/greenplum.py
--rw-rw-rw-   0        0        0      654 2024-04-20 07:29:21.000000 vvm_lib-1.0.1/vvm_lib/mssql.py
--rw-rw-rw-   0        0        0      855 2024-04-20 07:29:21.000000 vvm_lib-1.0.1/vvm_lib/vault.py
-drwxrwxrwx   0        0        0        0 2024-04-23 05:45:39.277611 vvm_lib-1.0.1/vvm_lib.egg-info/
--rw-rw-rw-   0        0        0      454 2024-04-23 05:45:39.000000 vvm_lib-1.0.1/vvm_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2024-04-23 05:45:39.000000 vvm_lib-1.0.1/vvm_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 05:45:39.000000 vvm_lib-1.0.1/vvm_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-22 08:57:19.000000 vvm_lib-1.0.1/vvm_lib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       94 2024-04-23 05:45:39.000000 vvm_lib-1.0.1/vvm_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-23 05:45:39.000000 vvm_lib-1.0.1/vvm_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 07:14:21.760422 vvm_lib-1.0.2/
+-rw-rw-rw-   0        0        0      513 2024-04-24 07:14:21.759424 vvm_lib-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4707 2024-04-23 05:44:57.000000 vvm_lib-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 07:14:21.766421 vvm_lib-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      800 2024-04-24 07:10:50.000000 vvm_lib-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 07:14:21.714396 vvm_lib-1.0.2/vvm_lib/
+drwxrwxrwx   0        0        0        0 2024-04-24 07:14:21.756424 vvm_lib-1.0.2/vvm_lib/DB/
+-rw-rw-rw-   0        0        0       30 2024-04-22 09:33:28.000000 vvm_lib-1.0.2/vvm_lib/DB/__init__.py
+-rw-rw-rw-   0        0        0     6351 2024-04-24 07:13:44.000000 vvm_lib-1.0.2/vvm_lib/DB/db.py
+-rw-rw-rw-   0        0        0      229 2024-04-20 07:29:21.000000 vvm_lib-1.0.2/vvm_lib/__init__.py
+-rw-rw-rw-   0        0        0     2747 2024-04-20 07:29:21.000000 vvm_lib-1.0.2/vvm_lib/google_book.py
+-rw-rw-rw-   0        0        0     3545 2024-04-20 07:29:21.000000 vvm_lib-1.0.2/vvm_lib/greenplum.py
+-rw-rw-rw-   0        0        0      654 2024-04-20 07:29:21.000000 vvm_lib-1.0.2/vvm_lib/mssql.py
+-rw-rw-rw-   0        0        0      855 2024-04-20 07:29:21.000000 vvm_lib-1.0.2/vvm_lib/vault.py
+drwxrwxrwx   0        0        0        0 2024-04-24 07:14:21.758423 vvm_lib-1.0.2/vvm_lib.egg-info/
+-rw-rw-rw-   0        0        0      513 2024-04-24 07:14:21.000000 vvm_lib-1.0.2/vvm_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2024-04-24 07:14:21.000000 vvm_lib-1.0.2/vvm_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 07:14:21.000000 vvm_lib-1.0.2/vvm_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-22 08:57:19.000000 vvm_lib-1.0.2/vvm_lib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      121 2024-04-24 07:14:21.000000 vvm_lib-1.0.2/vvm_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-24 07:14:21.000000 vvm_lib-1.0.2/vvm_lib.egg-info/top_level.txt
```

### Comparing `vvm_lib-1.0.1/README.md` & `vvm_lib-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `vvm_lib-1.0.1/vvm_lib/DB/db.py` & `vvm_lib-1.0.2/vvm_lib/DB/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,21 +4,15 @@
 import pymssql
 from clickhouse_connect import get_client, driver
 
 
 class DB:
     """
     Класс для работы с базами данных postgresql и mssql для моего личного пользования
-    Конструктор:
-        :param dbname: Название БД
-        :param user: пользователь
-        :param password: пароль
-        :param port: порт
-        :param host: хост
-        :param what_db: 'postgresql' , 'mssql', 'clickhouse'
+    для  'mssql', 'clickhouse' доступен только select
     """
 
     def __init__(self, dbname, user, password, port, host, what_db='postgresql') -> None:
         """
         :param dbname: Название БД
         :param user: пользователь
         :param password: пароль
```

### Comparing `vvm_lib-1.0.1/vvm_lib/google_book.py` & `vvm_lib-1.0.2/vvm_lib/google_book.py`

 * *Files identical despite different names*

### Comparing `vvm_lib-1.0.1/vvm_lib/greenplum.py` & `vvm_lib-1.0.2/vvm_lib/greenplum.py`

 * *Files identical despite different names*

### Comparing `vvm_lib-1.0.1/vvm_lib/mssql.py` & `vvm_lib-1.0.2/vvm_lib/mssql.py`

 * *Files identical despite different names*

### Comparing `vvm_lib-1.0.1/vvm_lib/vault.py` & `vvm_lib-1.0.2/vvm_lib/vault.py`

 * *Files identical despite different names*

