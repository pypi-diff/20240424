# Comparing `tmp/soda-core-dbt-3.3.1.tar.gz` & `tmp/soda_core_dbt-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-dbt-3.3.1.tar", last modified: Sun Mar 24 04:29:07 2024, max compression
+gzip compressed data, was "soda_core_dbt-3.3.2.tar", last modified: Wed Apr 24 15:26:10 2024, max compression
```

## Comparing `soda-core-dbt-3.3.1.tar` & `soda_core_dbt-3.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:07.533217 soda-core-dbt-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-24 04:28:40.000000 soda-core-dbt-3.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-24 04:29:07.533217 soda-core-dbt-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 04:29:07.533217 soda-core-dbt-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-24 04:28:40.000000 soda-core-dbt-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:07.529217 soda-core-dbt-3.3.1/soda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:07.529217 soda-core-dbt-3.3.1/soda/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)    17144 2024-03-24 04:28:40.000000 soda-core-dbt-3.3.1/soda/cloud/dbt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:07.529217 soda-core-dbt-3.3.1/soda/execution/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:07.529217 soda-core-dbt-3.3.1/soda/execution/check/
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-03-24 04:28:40.000000 soda-core-dbt-3.3.1/soda/execution/check/dbt_check.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:07.529217 soda-core-dbt-3.3.1/soda/sodacl/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-24 04:28:40.000000 soda-core-dbt-3.3.1/soda/sodacl/dbt_check_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:07.529217 soda-core-dbt-3.3.1/soda_core_dbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-24 04:29:07.000000 soda-core-dbt-3.3.1/soda_core_dbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-24 04:29:07.000000 soda-core-dbt-3.3.1/soda_core_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 04:29:07.000000 soda-core-dbt-3.3.1/soda_core_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-24 04:29:07.000000 soda-core-dbt-3.3.1/soda_core_dbt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-24 04:29:07.000000 soda-core-dbt-3.3.1/soda_core_dbt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:07.529217 soda-core-dbt-3.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-24 04:28:40.000000 soda-core-dbt-3.3.1/tests/test_dbt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:10.235738 soda_core_dbt-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 15:25:40.000000 soda_core_dbt-3.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 15:26:10.235738 soda_core_dbt-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:26:10.235738 soda_core_dbt-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-24 15:25:40.000000 soda_core_dbt-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:10.231738 soda_core_dbt-3.3.2/soda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:10.231738 soda_core_dbt-3.3.2/soda/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)    17144 2024-04-24 15:25:40.000000 soda_core_dbt-3.3.2/soda/cloud/dbt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:10.231738 soda_core_dbt-3.3.2/soda/execution/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:10.231738 soda_core_dbt-3.3.2/soda/execution/check/
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-24 15:25:40.000000 soda_core_dbt-3.3.2/soda/execution/check/dbt_check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:10.231738 soda_core_dbt-3.3.2/soda/sodacl/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-24 15:25:40.000000 soda_core_dbt-3.3.2/soda/sodacl/dbt_check_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:10.235738 soda_core_dbt-3.3.2/soda_core_dbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 15:26:10.000000 soda_core_dbt-3.3.2/soda_core_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-24 15:26:10.000000 soda_core_dbt-3.3.2/soda_core_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:26:10.000000 soda_core_dbt-3.3.2/soda_core_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-24 15:26:10.000000 soda_core_dbt-3.3.2/soda_core_dbt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 15:26:10.000000 soda_core_dbt-3.3.2/soda_core_dbt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:10.235738 soda_core_dbt-3.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-24 15:25:40.000000 soda_core_dbt-3.3.2/tests/test_dbt.py
```

### Comparing `soda-core-dbt-3.3.1/LICENSE` & `soda_core_dbt-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `soda-core-dbt-3.3.1/soda/cloud/dbt.py` & `soda_core_dbt-3.3.2/soda/cloud/dbt.py`

 * *Files identical despite different names*

### Comparing `soda-core-dbt-3.3.1/soda/execution/check/dbt_check.py` & `soda_core_dbt-3.3.2/soda/execution/check/dbt_check.py`

 * *Files identical despite different names*

### Comparing `soda-core-dbt-3.3.1/tests/test_dbt.py` & `soda_core_dbt-3.3.2/tests/test_dbt.py`

 * *Files identical despite different names*

