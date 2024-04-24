# Comparing `tmp/soda-core-db2-3.3.1.tar.gz` & `tmp/soda_core_db2-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-db2-3.3.1.tar", last modified: Sun Mar 24 04:29:04 2024, max compression
+gzip compressed data, was "soda_core_db2-3.3.2.tar", last modified: Wed Apr 24 15:26:05 2024, max compression
```

## Comparing `soda-core-db2-3.3.1.tar` & `soda_core_db2-3.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:04.345199 soda-core-db2-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-24 04:28:40.000000 soda-core-db2-3.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-24 04:29:04.345199 soda-core-db2-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 04:29:04.345199 soda-core-db2-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-24 04:28:40.000000 soda-core-db2-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:04.345199 soda-core-db2-3.3.1/soda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:04.345199 soda-core-db2-3.3.1/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-03-24 04:28:40.000000 soda-core-db2-3.3.1/soda/data_sources/db2_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:04.345199 soda-core-db2-3.3.1/soda_core_db2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-24 04:29:04.000000 soda-core-db2-3.3.1/soda_core_db2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-24 04:29:04.000000 soda-core-db2-3.3.1/soda_core_db2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 04:29:04.000000 soda-core-db2-3.3.1/soda_core_db2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-24 04:29:04.000000 soda-core-db2-3.3.1/soda_core_db2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-24 04:29:04.000000 soda-core-db2-3.3.1/soda_core_db2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:05.923721 soda_core_db2-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 15:25:40.000000 soda_core_db2-3.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 15:26:05.923721 soda_core_db2-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:26:05.923721 soda_core_db2-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-24 15:25:40.000000 soda_core_db2-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:05.923721 soda_core_db2-3.3.2/soda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:05.923721 soda_core_db2-3.3.2/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-04-24 15:25:40.000000 soda_core_db2-3.3.2/soda/data_sources/db2_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:05.923721 soda_core_db2-3.3.2/soda_core_db2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 15:26:05.000000 soda_core_db2-3.3.2/soda_core_db2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-24 15:26:05.000000 soda_core_db2-3.3.2/soda_core_db2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:26:05.000000 soda_core_db2-3.3.2/soda_core_db2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-24 15:26:05.000000 soda_core_db2-3.3.2/soda_core_db2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 15:26:05.000000 soda_core_db2-3.3.2/soda_core_db2.egg-info/top_level.txt
```

### Comparing `soda-core-db2-3.3.1/LICENSE` & `soda_core_db2-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `soda-core-db2-3.3.1/soda/data_sources/db2_data_source.py` & `soda_core_db2-3.3.2/soda/data_sources/db2_data_source.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,20 +61,23 @@
         super().__init__(logs, data_source_name, data_source_properties)
         self.host = data_source_properties.get("host")
         self.port = data_source_properties.get("port")
         self.password = data_source_properties.get("password")
         self.username = data_source_properties.get("username")
         self.database = data_source_properties.get("database")
         self.schema = data_source_properties.get("schema")
+        self.security = data_source_properties.get("security")
         self.update_schema(self.schema)
 
     def connect(self):
         conn_str = (
             f"DATABASE={self.database};HOSTNAME={self.host};PORT={self.port};UID={self.username};PWD={self.password}"
         )
+        if self.security is not None:
+            conn_str += f";SECURITY={self.security}"
         self.connection = ibm_db_dbi.connect(conn_str)
         return self.connection
 
     def validate_configuration(self, logs: Logs) -> None:
         pass
 
     def sql_information_schema_tables(self) -> str:
```

