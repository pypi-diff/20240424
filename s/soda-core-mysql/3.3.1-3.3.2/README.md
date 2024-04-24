# Comparing `tmp/soda-core-mysql-3.3.1.tar.gz` & `tmp/soda_core_mysql-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-mysql-3.3.1.tar", last modified: Sun Mar 24 04:29:20 2024, max compression
+gzip compressed data, was "soda_core_mysql-3.3.2.tar", last modified: Wed Apr 24 15:26:21 2024, max compression
```

## Comparing `soda-core-mysql-3.3.1.tar` & `soda_core_mysql-3.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:20.869290 soda-core-mysql-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-24 04:28:40.000000 soda-core-mysql-3.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-24 04:29:20.869290 soda-core-mysql-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 04:29:20.869290 soda-core-mysql-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-24 04:28:40.000000 soda-core-mysql-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:20.865290 soda-core-mysql-3.3.1/soda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:20.869290 soda-core-mysql-3.3.1/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-03-24 04:28:40.000000 soda-core-mysql-3.3.1/soda/data_sources/mysql_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:20.869290 soda-core-mysql-3.3.1/soda_core_mysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-24 04:29:20.000000 soda-core-mysql-3.3.1/soda_core_mysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-24 04:29:20.000000 soda-core-mysql-3.3.1/soda_core_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 04:29:20.000000 soda-core-mysql-3.3.1/soda_core_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-24 04:29:20.000000 soda-core-mysql-3.3.1/soda_core_mysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-24 04:29:20.000000 soda-core-mysql-3.3.1/soda_core_mysql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:20.869290 soda-core-mysql-3.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-24 04:28:40.000000 soda-core-mysql-3.3.1/tests/test_mysql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:21.143783 soda_core_mysql-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 15:25:40.000000 soda_core_mysql-3.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-24 15:26:21.143783 soda_core_mysql-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:26:21.143783 soda_core_mysql-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-24 15:25:40.000000 soda_core_mysql-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:21.139783 soda_core_mysql-3.3.2/soda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:21.139783 soda_core_mysql-3.3.2/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-24 15:25:40.000000 soda_core_mysql-3.3.2/soda/data_sources/mysql_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:21.143783 soda_core_mysql-3.3.2/soda_core_mysql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-24 15:26:21.000000 soda_core_mysql-3.3.2/soda_core_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-24 15:26:21.000000 soda_core_mysql-3.3.2/soda_core_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:26:21.000000 soda_core_mysql-3.3.2/soda_core_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-24 15:26:21.000000 soda_core_mysql-3.3.2/soda_core_mysql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 15:26:21.000000 soda_core_mysql-3.3.2/soda_core_mysql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:21.143783 soda_core_mysql-3.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 15:25:40.000000 soda_core_mysql-3.3.2/tests/test_mysql.py
```

### Comparing `soda-core-mysql-3.3.1/LICENSE` & `soda_core_mysql-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `soda-core-mysql-3.3.1/soda/data_sources/mysql_data_source.py` & `soda_core_mysql-3.3.2/soda/data_sources/mysql_data_source.py`

 * *Files identical despite different names*

