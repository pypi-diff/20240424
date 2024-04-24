# Comparing `tmp/soda-core-denodo-3.3.1.tar.gz` & `tmp/soda_core_denodo-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-denodo-3.3.1.tar", last modified: Sun Mar 24 04:29:10 2024, max compression
+gzip compressed data, was "soda_core_denodo-3.3.2.tar", last modified: Wed Apr 24 15:26:12 2024, max compression
```

## Comparing `soda-core-denodo-3.3.1.tar` & `soda_core_denodo-3.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:10.845236 soda-core-denodo-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-24 04:28:40.000000 soda-core-denodo-3.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-24 04:29:10.845236 soda-core-denodo-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 04:29:10.845236 soda-core-denodo-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-24 04:28:40.000000 soda-core-denodo-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:10.845236 soda-core-denodo-3.3.1/soda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:10.845236 soda-core-denodo-3.3.1/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-03-24 04:28:40.000000 soda-core-denodo-3.3.1/soda/data_sources/denodo_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:10.845236 soda-core-denodo-3.3.1/soda_core_denodo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-24 04:29:10.000000 soda-core-denodo-3.3.1/soda_core_denodo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-24 04:29:10.000000 soda-core-denodo-3.3.1/soda_core_denodo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 04:29:10.000000 soda-core-denodo-3.3.1/soda_core_denodo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-24 04:29:10.000000 soda-core-denodo-3.3.1/soda_core_denodo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-24 04:29:10.000000 soda-core-denodo-3.3.1/soda_core_denodo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:12.859749 soda_core_denodo-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 15:25:40.000000 soda_core_denodo-3.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-24 15:26:12.859749 soda_core_denodo-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:26:12.859749 soda_core_denodo-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-24 15:25:40.000000 soda_core_denodo-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:12.855749 soda_core_denodo-3.3.2/soda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:12.859749 soda_core_denodo-3.3.2/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-24 15:25:40.000000 soda_core_denodo-3.3.2/soda/data_sources/denodo_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:12.859749 soda_core_denodo-3.3.2/soda_core_denodo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-24 15:26:12.000000 soda_core_denodo-3.3.2/soda_core_denodo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-24 15:26:12.000000 soda_core_denodo-3.3.2/soda_core_denodo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:26:12.000000 soda_core_denodo-3.3.2/soda_core_denodo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-24 15:26:12.000000 soda_core_denodo-3.3.2/soda_core_denodo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 15:26:12.000000 soda_core_denodo-3.3.2/soda_core_denodo.egg-info/top_level.txt
```

### Comparing `soda-core-denodo-3.3.1/LICENSE` & `soda_core_denodo-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `soda-core-denodo-3.3.1/soda/data_sources/denodo_data_source.py` & `soda_core_denodo-3.3.2/soda/data_sources/denodo_data_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
     def __init__(self, logs: Logs, data_source_name: str, data_source_properties: dict):
         super().__init__(logs, data_source_name, data_source_properties)
         self.host = data_source_properties.get("host")
         self.port = data_source_properties.get("port")
         self.password = data_source_properties.get("password")
         self.username = data_source_properties.get("username")
+        self.connection_timeout = data_source_properties.get("connection_timeout")
 
     def connect(self):
         import psycopg2
 
         self.connection = psycopg2.connect(
             user=self.username,
             password=self.password,
```

