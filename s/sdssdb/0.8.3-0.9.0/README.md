# Comparing `tmp/sdssdb-0.8.3.tar.gz` & `tmp/sdssdb-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdssdb-0.8.3.tar", last modified: Mon Dec 11 14:39:14 2023, max compression
+gzip compressed data, was "sdssdb-0.9.0.tar", last modified: Fri Mar  8 22:14:30 2024, max compression
```

## Comparing `sdssdb-0.8.3.tar` & `sdssdb-0.9.0.tar`

### file list

```diff
@@ -1,82 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 14:39:14.769296 sdssdb-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2023-12-11 14:38:54.000000 sdssdb-0.8.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2023-12-11 14:39:14.769296 sdssdb-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2023-12-11 14:38:54.000000 sdssdb-0.8.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 14:39:14.757296 sdssdb-0.8.3/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 14:39:14.757296 sdssdb-0.8.3/python/sdssdb/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22907 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 14:39:14.761296 sdssdb-0.8.3/python/sdssdb/etc/
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/etc/sdssdb.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 14:39:14.761296 sdssdb-0.8.3/python/sdssdb/peewee/
--rw-r--r--   0 runner    (1001) docker     (127)    13557 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/peewee/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 14:39:14.761296 sdssdb-0.8.3/python/sdssdb/peewee/lvmdb/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/peewee/lvmdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9497 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/peewee/lvmdb/lvmopsdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 14:39:14.761296 sdssdb-0.8.3/python/sdssdb/peewee/operationsdb/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/peewee/operationsdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10312 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/peewee/operationsdb/apogeeqldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6387 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/peewee/operationsdb/mangadb.py
--rw-r--r--   0 runner    (1001) docker     (127)    28649 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/peewee/operationsdb/platedb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 14:39:14.761296 sdssdb-0.8.3/python/sdssdb/peewee/sdss5db/
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/peewee/sdss5db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/peewee/sdss5db/apogee_drpdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    11946 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/peewee/sdss5db/boss_drp.py
--rw-r--r--   0 runner    (1001) docker     (127)    63834 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/peewee/sdss5db/catalogdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/peewee/sdss5db/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    10470 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/peewee/sdss5db/opsdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    11763 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/peewee/sdss5db/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    17707 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/peewee/sdss5db/targetdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/peewee/sdss5db/vizdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 14:39:14.761296 sdssdb-0.8.3/python/sdssdb/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 14:39:14.761296 sdssdb-0.8.3/python/sdssdb/sqlalchemy/archive/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6609 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/archive/sas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 14:39:14.765296 sdssdb-0.8.3/python/sdssdb/sqlalchemy/mangadb/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/mangadb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/mangadb/auxdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    10958 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/mangadb/dapdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    22440 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/mangadb/datadb.py
--rw-r--r--   0 runner    (1001) docker     (127)    10213 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/mangadb/sampledb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 14:39:14.765296 sdssdb-0.8.3/python/sdssdb/sqlalchemy/operationsdb/
--rw-r--r--   0 runner    (1001) docker     (127)      724 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/operationsdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/operationsdb/apogeeqldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/operationsdb/mangadb.py
--rw-r--r--   0 runner    (1001) docker     (127)    40377 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/operationsdb/platedb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 14:39:14.765296 sdssdb-0.8.3/python/sdssdb/sqlalchemy/operationsdb/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/operationsdb/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/operationsdb/tools/astrodatetime.py
--rw-r--r--   0 runner    (1001) docker     (127)    33824 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/operationsdb/tools/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/operationsdb/tools/dateObs2HA.py
--rw-r--r--   0 runner    (1001) docker     (127)    21382 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/operationsdb/tools/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/operationsdb/tools/moon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/operationsdb/tools/sun.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 14:39:14.765296 sdssdb-0.8.3/python/sdssdb/sqlalchemy/sdss5db/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/sdss5db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21543 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/sdss5db/apogee_drpdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    10385 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/sdss5db/boss_drp.py
--rw-r--r--   0 runner    (1001) docker     (127)   358255 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/sdss5db/catalogdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     8453 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/sdss5db/opsdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    13164 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/sdss5db/targetdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/sqlalchemy/sdss5db/vizdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 14:39:14.769296 sdssdb-0.8.3/python/sdssdb/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/utils/adaptors.py
--rw-r--r--   0 runner    (1001) docker     (127)    18463 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/utils/ingest.py
--rw-r--r--   0 runner    (1001) docker     (127)    11140 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/utils/internals.py
--rw-r--r--   0 runner    (1001) docker     (127)     6005 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    11512 2023-12-11 14:38:54.000000 sdssdb-0.8.3/python/sdssdb/utils/schemadisplay.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 14:39:14.769296 sdssdb-0.8.3/python/sdssdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2023-12-11 14:39:14.000000 sdssdb-0.8.3/python/sdssdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2023-12-11 14:39:14.000000 sdssdb-0.8.3/python/sdssdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 14:39:14.000000 sdssdb-0.8.3/python/sdssdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 14:39:07.000000 sdssdb-0.8.3/python/sdssdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      486 2023-12-11 14:39:14.000000 sdssdb-0.8.3/python/sdssdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-11 14:39:14.000000 sdssdb-0.8.3/python/sdssdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2023-12-11 14:39:14.773296 sdssdb-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-12-11 14:38:54.000000 sdssdb-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 14:39:14.769296 sdssdb-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2023-12-11 14:38:54.000000 sdssdb-0.8.3/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2023-12-11 14:38:54.000000 sdssdb-0.8.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:14:30.957357 sdssdb-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-08 22:14:22.000000 sdssdb-0.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-03-08 22:14:30.957357 sdssdb-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-08 22:14:22.000000 sdssdb-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:14:30.941357 sdssdb-0.9.0/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:14:30.945356 sdssdb-0.9.0/python/sdssdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22907 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:14:30.945356 sdssdb-0.9.0/python/sdssdb/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/etc/sdssdb.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:14:30.945356 sdssdb-0.9.0/python/sdssdb/peewee/
+-rw-r--r--   0 runner    (1001) docker     (127)    13557 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/peewee/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:14:30.945356 sdssdb-0.9.0/python/sdssdb/peewee/lvmdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/peewee/lvmdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/peewee/lvmdb/lvmopsdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:14:30.949357 sdssdb-0.9.0/python/sdssdb/peewee/operationsdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/peewee/operationsdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10312 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/peewee/operationsdb/apogeeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/peewee/operationsdb/mangadb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28649 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/peewee/operationsdb/platedb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:14:30.949357 sdssdb-0.9.0/python/sdssdb/peewee/sdss5db/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/peewee/sdss5db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/peewee/sdss5db/apogee_drpdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96847 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/peewee/sdss5db/astradb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11946 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/peewee/sdss5db/boss_drp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65719 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/peewee/sdss5db/catalogdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/peewee/sdss5db/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10470 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/peewee/sdss5db/opsdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/peewee/sdss5db/sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17707 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/peewee/sdss5db/targetdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/peewee/sdss5db/vizdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:14:30.949357 sdssdb-0.9.0/python/sdssdb/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:14:30.949357 sdssdb-0.9.0/python/sdssdb/sqlalchemy/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/archive/sas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:14:30.949357 sdssdb-0.9.0/python/sdssdb/sqlalchemy/mangadb/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/mangadb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/mangadb/auxdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/mangadb/dapdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22440 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/mangadb/datadb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10213 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/mangadb/sampledb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:14:30.953357 sdssdb-0.9.0/python/sdssdb/sqlalchemy/operationsdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/operationsdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/operationsdb/apogeeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/operationsdb/mangadb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40377 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/operationsdb/platedb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:14:30.953357 sdssdb-0.9.0/python/sdssdb/sqlalchemy/operationsdb/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/operationsdb/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/operationsdb/tools/astrodatetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33824 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/operationsdb/tools/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/operationsdb/tools/dateObs2HA.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21382 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/operationsdb/tools/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/operationsdb/tools/moon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/operationsdb/tools/sun.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:14:30.953357 sdssdb-0.9.0/python/sdssdb/sqlalchemy/sdss5db/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/sdss5db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21543 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/sdss5db/apogee_drpdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94873 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/sdss5db/astradb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10385 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/sdss5db/boss_drp.py
+-rw-r--r--   0 runner    (1001) docker     (127)   358255 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/sdss5db/catalogdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/sdss5db/opsdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13164 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/sdss5db/targetdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/sqlalchemy/sdss5db/vizdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:14:30.957357 sdssdb-0.9.0/python/sdssdb/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/utils/adaptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18463 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/utils/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11140 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/utils/internals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11512 2024-03-08 22:14:22.000000 sdssdb-0.9.0/python/sdssdb/utils/schemadisplay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:14:30.957357 sdssdb-0.9.0/python/sdssdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-03-08 22:14:30.000000 sdssdb-0.9.0/python/sdssdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-03-08 22:14:30.000000 sdssdb-0.9.0/python/sdssdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 22:14:30.000000 sdssdb-0.9.0/python/sdssdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 22:14:27.000000 sdssdb-0.9.0/python/sdssdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-08 22:14:30.000000 sdssdb-0.9.0/python/sdssdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-08 22:14:30.000000 sdssdb-0.9.0/python/sdssdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-03-08 22:14:30.957357 sdssdb-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-08 22:14:22.000000 sdssdb-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 22:14:30.957357 sdssdb-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-08 22:14:22.000000 sdssdb-0.9.0/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-03-08 22:14:22.000000 sdssdb-0.9.0/tests/test_utils.py
```

### Comparing `sdssdb-0.8.3/LICENSE.md` & `sdssdb-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/PKG-INFO` & `sdssdb-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdssdb
-Version: 0.8.3
+Version: 0.9.0
 Summary: SDSS product for database management
 Home-page: https://github.com/sdss/sdssdb
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/sdssdb
 Project-URL: Documentation, https://sdssdb.readthedocs.org
```

### Comparing `sdssdb-0.8.3/README.rst` & `sdssdb-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/__init__.py` & `sdssdb-0.9.0/python/sdssdb/__init__.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/connection.py` & `sdssdb-0.9.0/python/sdssdb/connection.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/etc/sdssdb.yml` & `sdssdb-0.9.0/python/sdssdb/etc/sdssdb.yml`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/exceptions.py` & `sdssdb-0.9.0/python/sdssdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/peewee/__init__.py` & `sdssdb-0.9.0/python/sdssdb/peewee/__init__.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/peewee/lvmdb/__init__.py` & `sdssdb-0.9.0/python/sdssdb/peewee/lvmdb/__init__.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/peewee/lvmdb/lvmopsdb.py` & `sdssdb-0.9.0/python/sdssdb/peewee/lvmdb/lvmopsdb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/peewee/operationsdb/__init__.py` & `sdssdb-0.9.0/python/sdssdb/peewee/operationsdb/__init__.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/peewee/operationsdb/apogeeqldb.py` & `sdssdb-0.9.0/python/sdssdb/peewee/operationsdb/apogeeqldb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/peewee/operationsdb/mangadb.py` & `sdssdb-0.9.0/python/sdssdb/peewee/operationsdb/mangadb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/peewee/operationsdb/platedb.py` & `sdssdb-0.9.0/python/sdssdb/peewee/operationsdb/platedb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/peewee/sdss5db/__init__.py` & `sdssdb-0.9.0/python/sdssdb/peewee/sdss5db/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         on the fly and are only available after a successful connection.
 
         """
 
         modules = ['sdssdb.peewee.sdss5db.catalogdb',
                    'sdssdb.peewee.sdss5db.targetdb',
                    'sdssdb.peewee.sdss5db.opsdb',
+                   'sdssdb.peewee.sdss5db.astradb',
                    'sdssdb.peewee.sdss5db.apogee_drpdb',
                    'sdssdb.peewee.sdss5db.boss_drp',
                    'sdssdb.peewee.sdss5db.vizdb']
 
         for module in modules:
             if module in sys.modules:
                 importlib.reload(sys.modules[module])
```

### Comparing `sdssdb-0.8.3/python/sdssdb/peewee/sdss5db/apogee_drpdb.py` & `sdssdb-0.9.0/python/sdssdb/peewee/sdss5db/apogee_drpdb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/peewee/sdss5db/boss_drp.py` & `sdssdb-0.9.0/python/sdssdb/peewee/sdss5db/boss_drp.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/peewee/sdss5db/catalogdb.py` & `sdssdb-0.9.0/python/sdssdb/peewee/sdss5db/catalogdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,22 @@
 
     id = BigIntegerField(primary_key=True)
 
     class Meta:
         table_name = 'catalog_ver25_to_ver31_full_all'
 
 
+class Target_non_carton(CatalogdbModel):
+
+    pk = BigIntegerField(primary_key=True)
+
+    class Meta:
+        table_name = 'target_non_carton'
+
+
 class AllWise(CatalogdbModel):
 
     cntr = BigIntegerField(primary_key=True)
     designation = TextField()
     tmass_key = BigIntegerField()
 
     class Meta:
@@ -732,14 +740,94 @@
         object_id_name='source_id',
         backref='+')
 
     class Meta:
         table_name = 'sagitta_edr3'
 
 
+class Mangadapall(CatalogdbModel):
+
+    pk = BigIntegerField(primary_key=True)
+
+    class Meta:
+        table_name = 'mangadapall'
+
+
+class Mangadrpall(CatalogdbModel):
+
+    plateifu = CharField(primary_key=True)
+
+    class Meta:
+        table_name = 'mangadrpall'
+
+
+class Mangatarget(CatalogdbModel):
+
+    mangaid = CharField(primary_key=True)
+
+    class Meta:
+        table_name = 'mangatarget'
+
+
+class Mastar_goodstars(CatalogdbModel):
+
+    mangaid = CharField(primary_key=True)
+
+    class Meta:
+        table_name = 'mastar_goodstars'
+
+
+class Mastar_goodvisits(CatalogdbModel):
+
+    pk = BigIntegerField(primary_key=True)
+
+    class Meta:
+        table_name = 'mastar_goodvisits'
+
+
+class Marvels_dr11_star(CatalogdbModel):
+
+    starname = CharField(primary_key=True)
+
+    class Meta:
+        table_name = 'marvels_dr11_star'
+
+
+class Marvels_dr11_velocitycurve_ccf(CatalogdbModel):
+
+    pk = BigIntegerField(primary_key=True)
+
+    class Meta:
+        table_name = 'marvels_dr11_velocitycurve_ccf'
+
+
+class Marvels_dr11_velocitycurve_dfdi(CatalogdbModel):
+
+    pk = BigIntegerField(primary_key=True)
+
+    class Meta:
+        table_name = 'marvels_dr11_velocitycurve_dfdi'
+
+
+class Marvels_dr12_star(CatalogdbModel):
+
+    pk = BigIntegerField(primary_key=True)
+
+    class Meta:
+        table_name = 'marvels_dr12_star'
+
+
+class Marvels_dr12_velocitycurve_uf1d(CatalogdbModel):
+
+    pk = BigIntegerField(primary_key=True)
+
+    class Meta:
+        table_name = 'marvels_dr12_velocitycurve_uf1d'
+
+
 class SDSSV_Plateholes_Meta(CatalogdbModel):
 
     yanny_uid = BigIntegerField(primary_key=True)
 
     class Meta:
         table_name = 'sdssv_plateholes_meta'
 
@@ -2032,14 +2120,23 @@
                                        object_id_name='bestobjid',
                                        backref='+')
 
     class Meta:
         table_name = 'sdss_dr16_specobj'
 
 
+class SDSS_DR17_SpecObj(CatalogdbModel):
+    # The column specobjid has data type varchar since
+    # it has values which do not fit in bigint.
+    specobjid = CharField(primary_key=True)
+
+    class Meta:
+        table_name = 'sdss_dr17_specobj'
+
+
 class Gaia_DR2_TwoMass_Best_Neighbour(CatalogdbModel):
 
     source_id = BigIntegerField(primary_key=True)
 
     gaia = ForeignKeyField(Gaia_DR2,
                            field='source_id',
                            column_name='source_id',
```

### Comparing `sdssdb-0.8.3/python/sdssdb/peewee/sdss5db/deprecated.py` & `sdssdb-0.9.0/python/sdssdb/peewee/sdss5db/deprecated.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/peewee/sdss5db/opsdb.py` & `sdssdb-0.9.0/python/sdssdb/peewee/sdss5db/opsdb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/peewee/sdss5db/sandbox.py` & `sdssdb-0.9.0/python/sdssdb/peewee/sdss5db/sandbox.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/peewee/sdss5db/targetdb.py` & `sdssdb-0.9.0/python/sdssdb/peewee/sdss5db/targetdb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/peewee/sdss5db/vizdb.py` & `sdssdb-0.9.0/python/sdssdb/peewee/sdss5db/vizdb.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 # Code generated by:
 # python -m pwiz -e postgresql sdss5db -s vizdb -i -o -H localhost -p 6000 -u u0857802
 # Date: October 18, 2023 03:26PM
 # Database: sdss5db
 # Peewee version: 3.13.2
 
 from peewee import (AutoField, BigIntegerField, BooleanField,
-                    DoubleField, SmallIntegerField, TextField)
+                    DoubleField, IntegerField, SmallIntegerField, TextField)
+from playhouse.postgres_ext import ArrayField
 
 from .. import BaseModel
 from . import database  # noqa
 
 
 class VizBase(BaseModel):
 
@@ -75,7 +76,31 @@
     description = TextField(null=True)
     unit = TextField(null=True)
     sql_type = TextField(null=True)
 
     class Meta:
         table_name = 'db_metadata'
         print_fields = ['schema', 'table_name', 'column_name', 'display_name']
+
+
+class Releases(VizBase):
+
+    pk = AutoField()
+    release = TextField(null=True)
+    run2d = ArrayField(TextField, null=True)
+    run1d = ArrayField(TextField, null=True)
+    apred_vers = ArrayField(TextField, null=True)
+    v_astra = TextField(null=True)
+    v_speccomp = TextField(null=True)
+    v_targ = TextField(null=True)
+    drpver = TextField(null=True)
+    dapver = TextField(null=True)
+    apstar_vers = TextField(null=True)
+    aspcap_vers = TextField(null=True)
+    results_vers = TextField(null=True)
+    public = BooleanField(null=False)
+    mjd_cutoff_apo = IntegerField(null=False)
+    mjd_cutoff_lco = IntegerField(null=False)
+
+    class Meta:
+        table_name = 'releases'
+        print_fields = ['release']
```

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/__init__.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/archive/__init__.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/archive/sas.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/archive/sas.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/mangadb/__init__.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/mangadb/__init__.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/mangadb/auxdb.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/mangadb/auxdb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/mangadb/dapdb.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/mangadb/dapdb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/mangadb/datadb.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/mangadb/datadb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/mangadb/sampledb.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/mangadb/sampledb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/operationsdb/__init__.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/operationsdb/__init__.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/operationsdb/apogeeqldb.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/operationsdb/apogeeqldb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/operationsdb/mangadb.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/operationsdb/mangadb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/operationsdb/platedb.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/operationsdb/platedb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/operationsdb/tools/astrodatetime.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/operationsdb/tools/astrodatetime.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/operationsdb/tools/convert.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/operationsdb/tools/convert.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/operationsdb/tools/dateObs2HA.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/operationsdb/tools/dateObs2HA.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/operationsdb/tools/geometry.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/operationsdb/tools/geometry.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/operationsdb/tools/moon.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/operationsdb/tools/moon.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/operationsdb/tools/sun.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/operationsdb/tools/sun.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/sdss5db/apogee_drpdb.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/sdss5db/apogee_drpdb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/sdss5db/boss_drp.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/sdss5db/boss_drp.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/sdss5db/catalogdb.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/sdss5db/catalogdb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/sdss5db/opsdb.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/sdss5db/opsdb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/sdss5db/targetdb.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/sdss5db/targetdb.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/sqlalchemy/sdss5db/vizdb.py` & `sdssdb-0.9.0/python/sdssdb/sqlalchemy/sdss5db/vizdb.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 #
 
 # this file was autogenerated with sqlacodegen and then adapted for sdssdb
 # flake8: noqa=E501,E741
 
 
 from sqlalchemy.ext.declarative import AbstractConcreteBase, declared_attr
-from sqlalchemy import BigInteger, Boolean, Column, Float, Integer, SmallInteger, Text, text
+from sqlalchemy import (ARRAY, BigInteger, Boolean, Column, Float, Integer,
+                        SmallInteger, Text, text)
 
 from sdssdb.sqlalchemy.sdss5db import SDSS5dbBase, database
 
 
 SCHEMA = 'vizdb'
 
 
@@ -73,14 +74,36 @@
     pk = Column('pk', BigInteger, primary_key=True)
     sdss_id = Column('sdss_id', BigInteger)
     in_boss = Column('in_boss', Boolean)
     in_apogee = Column('in_apogee', Boolean)
     in_astra = Column('in_astra', Boolean)
 
 
+class Releases(Base):
+    __tablename__ = 'releases'
+    print_fields = ['release']
+
+    pk = Column('pk', BigInteger, primary_key=True)
+    release = Column(Text)
+    run2d = Column(ARRAY(Text()))
+    run1d = Column(ARRAY(Text()))
+    apred_vers = Column(ARRAY(Text()))
+    v_astra = Column(Text)
+    v_speccomp = Column(Text)
+    v_targ = Column(Text)
+    drpver = Column(Text)
+    dapver = Column(Text)
+    apstar_vers = Column(Text)
+    aspcap_vers = Column(Text)
+    results_vers = Column(Text)
+    public = Column(Boolean)
+    mjd_cutoff_apo = Column(Integer)
+    mjd_cutoff_lco = Column(Integer)
+
+
 def define_relations():
     """ leaving this empty as relations were autogenerated """
     pass
 
 
 # prepare the base
 database.add_base(Base)
```

### Comparing `sdssdb-0.8.3/python/sdssdb/utils/adaptors.py` & `sdssdb-0.9.0/python/sdssdb/utils/adaptors.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/utils/ingest.py` & `sdssdb-0.9.0/python/sdssdb/utils/ingest.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/utils/internals.py` & `sdssdb-0.9.0/python/sdssdb/utils/internals.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/utils/registry.py` & `sdssdb-0.9.0/python/sdssdb/utils/registry.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb/utils/schemadisplay.py` & `sdssdb-0.9.0/python/sdssdb/utils/schemadisplay.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/python/sdssdb.egg-info/PKG-INFO` & `sdssdb-0.9.0/python/sdssdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdssdb
-Version: 0.8.3
+Version: 0.9.0
 Summary: SDSS product for database management
 Home-page: https://github.com/sdss/sdssdb
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/sdssdb
 Project-URL: Documentation, https://sdssdb.readthedocs.org
```

### Comparing `sdssdb-0.8.3/python/sdssdb.egg-info/SOURCES.txt` & `sdssdb-0.9.0/python/sdssdb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 python/sdssdb/peewee/lvmdb/lvmopsdb.py
 python/sdssdb/peewee/operationsdb/__init__.py
 python/sdssdb/peewee/operationsdb/apogeeqldb.py
 python/sdssdb/peewee/operationsdb/mangadb.py
 python/sdssdb/peewee/operationsdb/platedb.py
 python/sdssdb/peewee/sdss5db/__init__.py
 python/sdssdb/peewee/sdss5db/apogee_drpdb.py
+python/sdssdb/peewee/sdss5db/astradb.py
 python/sdssdb/peewee/sdss5db/boss_drp.py
 python/sdssdb/peewee/sdss5db/catalogdb.py
 python/sdssdb/peewee/sdss5db/deprecated.py
 python/sdssdb/peewee/sdss5db/opsdb.py
 python/sdssdb/peewee/sdss5db/sandbox.py
 python/sdssdb/peewee/sdss5db/targetdb.py
 python/sdssdb/peewee/sdss5db/vizdb.py
@@ -45,14 +46,15 @@
 python/sdssdb/sqlalchemy/operationsdb/tools/convert.py
 python/sdssdb/sqlalchemy/operationsdb/tools/dateObs2HA.py
 python/sdssdb/sqlalchemy/operationsdb/tools/geometry.py
 python/sdssdb/sqlalchemy/operationsdb/tools/moon.py
 python/sdssdb/sqlalchemy/operationsdb/tools/sun.py
 python/sdssdb/sqlalchemy/sdss5db/__init__.py
 python/sdssdb/sqlalchemy/sdss5db/apogee_drpdb.py
+python/sdssdb/sqlalchemy/sdss5db/astradb.py
 python/sdssdb/sqlalchemy/sdss5db/boss_drp.py
 python/sdssdb/sqlalchemy/sdss5db/catalogdb.py
 python/sdssdb/sqlalchemy/sdss5db/opsdb.py
 python/sdssdb/sqlalchemy/sdss5db/targetdb.py
 python/sdssdb/sqlalchemy/sdss5db/vizdb.py
 python/sdssdb/utils/__init__.py
 python/sdssdb/utils/adaptors.py
```

### Comparing `sdssdb-0.8.3/setup.cfg` & `sdssdb-0.9.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sdssdb
-version = 0.8.3
+version = 0.9.0
 author = José Sánchez-Gallego
 author_email = gallegoj@uw.edu
 description = SDSS product for database management
 url = https://github.com/sdss/sdssdb
 project_urls = 
 	Repository = https://github.com/sdss/sdssdb
 	Documentation = https://sdssdb.readthedocs.org
```

### Comparing `sdssdb-0.8.3/tests/test_connection.py` & `sdssdb-0.9.0/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `sdssdb-0.8.3/tests/test_utils.py` & `sdssdb-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

