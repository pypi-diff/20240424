# Comparing `tmp/soda-core-spark-3.3.1.tar.gz` & `tmp/soda_core_spark-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-spark-3.3.1.tar", last modified: Sun Mar 24 04:29:38 2024, max compression
+gzip compressed data, was "soda_core_spark-3.3.2.tar", last modified: Wed Apr 24 15:26:39 2024, max compression
```

## Comparing `soda-core-spark-3.3.1.tar` & `soda_core_spark-3.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:38.749386 soda-core-spark-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-24 04:28:40.000000 soda-core-spark-3.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-24 04:29:38.749386 soda-core-spark-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 04:29:38.749386 soda-core-spark-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-24 04:28:40.000000 soda-core-spark-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:38.749386 soda-core-spark-3.3.1/soda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:38.749386 soda-core-spark-3.3.1/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)    17426 2024-03-24 04:28:40.000000 soda-core-spark-3.3.1/soda/data_sources/spark_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:38.749386 soda-core-spark-3.3.1/soda_core_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-24 04:29:38.000000 soda-core-spark-3.3.1/soda_core_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-24 04:29:38.000000 soda-core-spark-3.3.1/soda_core_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 04:29:38.000000 soda-core-spark-3.3.1/soda_core_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-24 04:29:38.000000 soda-core-spark-3.3.1/soda_core_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-24 04:29:38.000000 soda-core-spark-3.3.1/soda_core_spark.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:38.749386 soda-core-spark-3.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-24 04:28:40.000000 soda-core-spark-3.3.1/tests/test_table_name_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:39.107855 soda_core_spark-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 15:25:40.000000 soda_core_spark-3.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-24 15:26:39.107855 soda_core_spark-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:26:39.107855 soda_core_spark-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-24 15:25:40.000000 soda_core_spark-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:39.107855 soda_core_spark-3.3.2/soda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:39.107855 soda_core_spark-3.3.2/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)    17426 2024-04-24 15:25:40.000000 soda_core_spark-3.3.2/soda/data_sources/spark_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:39.107855 soda_core_spark-3.3.2/soda_core_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-24 15:26:39.000000 soda_core_spark-3.3.2/soda_core_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-24 15:26:39.000000 soda_core_spark-3.3.2/soda_core_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:26:39.000000 soda_core_spark-3.3.2/soda_core_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-24 15:26:39.000000 soda_core_spark-3.3.2/soda_core_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 15:26:39.000000 soda_core_spark-3.3.2/soda_core_spark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:39.107855 soda_core_spark-3.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-24 15:25:40.000000 soda_core_spark-3.3.2/tests/test_table_name_filtering.py
```

### Comparing `soda-core-spark-3.3.1/LICENSE` & `soda_core_spark-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `soda-core-spark-3.3.1/setup.py` & `soda_core_spark-3.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import find_namespace_packages, setup
 
 package_name = "soda-core-spark"
-package_version = "3.3.1"
+package_version = "3.3.2"
 description = "Soda Core Spark Package"
 
 requires = [f"soda-core=={package_version}"]
 
 extras = {
     "hive": [
         "PyHive[hive]",
```

### Comparing `soda-core-spark-3.3.1/soda/data_sources/spark_data_source.py` & `soda_core_spark-3.3.2/soda/data_sources/spark_data_source.py`

 * *Files identical despite different names*

### Comparing `soda-core-spark-3.3.1/tests/test_table_name_filtering.py` & `soda_core_spark-3.3.2/tests/test_table_name_filtering.py`

 * *Files identical despite different names*

