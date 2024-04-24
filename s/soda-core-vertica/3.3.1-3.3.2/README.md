# Comparing `tmp/soda-core-vertica-3.3.1.tar.gz` & `tmp/soda_core_vertica-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-vertica-3.3.1.tar", last modified: Sun Mar 24 04:29:53 2024, max compression
+gzip compressed data, was "soda_core_vertica-3.3.2.tar", last modified: Wed Apr 24 15:26:55 2024, max compression
```

## Comparing `soda-core-vertica-3.3.1.tar` & `soda_core_vertica-3.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:53.245460 soda-core-vertica-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-24 04:28:40.000000 soda-core-vertica-3.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-24 04:29:53.245460 soda-core-vertica-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 04:29:53.245460 soda-core-vertica-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-24 04:28:40.000000 soda-core-vertica-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:53.241460 soda-core-vertica-3.3.1/soda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:53.245460 soda-core-vertica-3.3.1/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-03-24 04:28:40.000000 soda-core-vertica-3.3.1/soda/data_sources/vertica_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:53.245460 soda-core-vertica-3.3.1/soda_core_vertica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-24 04:29:53.000000 soda-core-vertica-3.3.1/soda_core_vertica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-24 04:29:53.000000 soda-core-vertica-3.3.1/soda_core_vertica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 04:29:53.000000 soda-core-vertica-3.3.1/soda_core_vertica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-24 04:29:53.000000 soda-core-vertica-3.3.1/soda_core_vertica.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-24 04:29:53.000000 soda-core-vertica-3.3.1/soda_core_vertica.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:53.245460 soda-core-vertica-3.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-24 04:28:40.000000 soda-core-vertica-3.3.1/tests/test_vertica.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:55.623923 soda_core_vertica-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 15:25:40.000000 soda_core_vertica-3.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-24 15:26:55.623923 soda_core_vertica-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:26:55.623923 soda_core_vertica-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-24 15:25:40.000000 soda_core_vertica-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:55.623923 soda_core_vertica-3.3.2/soda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:55.623923 soda_core_vertica-3.3.2/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-04-24 15:25:40.000000 soda_core_vertica-3.3.2/soda/data_sources/vertica_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:55.623923 soda_core_vertica-3.3.2/soda_core_vertica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-24 15:26:55.000000 soda_core_vertica-3.3.2/soda_core_vertica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-24 15:26:55.000000 soda_core_vertica-3.3.2/soda_core_vertica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:26:55.000000 soda_core_vertica-3.3.2/soda_core_vertica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 15:26:55.000000 soda_core_vertica-3.3.2/soda_core_vertica.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 15:26:55.000000 soda_core_vertica-3.3.2/soda_core_vertica.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:55.623923 soda_core_vertica-3.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-24 15:25:40.000000 soda_core_vertica-3.3.2/tests/test_vertica.py
```

### Comparing `soda-core-vertica-3.3.1/LICENSE` & `soda_core_vertica-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `soda-core-vertica-3.3.1/soda/data_sources/vertica_data_source.py` & `soda_core_vertica-3.3.2/soda/data_sources/vertica_data_source.py`

 * *Files identical despite different names*

