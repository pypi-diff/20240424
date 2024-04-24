# Comparing `tmp/soda-core-dremio-3.3.1.tar.gz` & `tmp/soda_core_dremio-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-dremio-3.3.1.tar", last modified: Sun Mar 24 04:29:14 2024, max compression
+gzip compressed data, was "soda_core_dremio-3.3.2.tar", last modified: Wed Apr 24 15:26:15 2024, max compression
```

## Comparing `soda-core-dremio-3.3.1.tar` & `soda_core_dremio-3.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:14.393255 soda-core-dremio-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-24 04:28:40.000000 soda-core-dremio-3.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-24 04:29:14.393255 soda-core-dremio-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 04:29:14.393255 soda-core-dremio-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-24 04:28:40.000000 soda-core-dremio-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:14.389255 soda-core-dremio-3.3.1/soda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:14.389255 soda-core-dremio-3.3.1/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-03-24 04:28:40.000000 soda-core-dremio-3.3.1/soda/data_sources/dremio_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:14.393255 soda-core-dremio-3.3.1/soda_core_dremio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-24 04:29:14.000000 soda-core-dremio-3.3.1/soda_core_dremio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-24 04:29:14.000000 soda-core-dremio-3.3.1/soda_core_dremio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 04:29:14.000000 soda-core-dremio-3.3.1/soda_core_dremio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-24 04:29:14.000000 soda-core-dremio-3.3.1/soda_core_dremio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-24 04:29:14.000000 soda-core-dremio-3.3.1/soda_core_dremio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:14.389255 soda-core-dremio-3.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-24 04:28:40.000000 soda-core-dremio-3.3.1/tests/test_dremio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:15.599760 soda_core_dremio-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 15:25:40.000000 soda_core_dremio-3.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-24 15:26:15.599760 soda_core_dremio-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:26:15.599760 soda_core_dremio-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-24 15:25:40.000000 soda_core_dremio-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:15.595760 soda_core_dremio-3.3.2/soda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:15.595760 soda_core_dremio-3.3.2/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-04-24 15:25:40.000000 soda_core_dremio-3.3.2/soda/data_sources/dremio_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:15.599760 soda_core_dremio-3.3.2/soda_core_dremio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-24 15:26:15.000000 soda_core_dremio-3.3.2/soda_core_dremio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-24 15:26:15.000000 soda_core_dremio-3.3.2/soda_core_dremio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:26:15.000000 soda_core_dremio-3.3.2/soda_core_dremio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-24 15:26:15.000000 soda_core_dremio-3.3.2/soda_core_dremio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 15:26:15.000000 soda_core_dremio-3.3.2/soda_core_dremio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:15.595760 soda_core_dremio-3.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-24 15:25:40.000000 soda_core_dremio-3.3.2/tests/test_dremio.py
```

### Comparing `soda-core-dremio-3.3.1/LICENSE` & `soda_core_dremio-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `soda-core-dremio-3.3.1/soda/data_sources/dremio_data_source.py` & `soda_core_dremio-3.3.2/soda/data_sources/dremio_data_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         self.port = data_source_properties.get("port", "32010")
         self.username = data_source_properties.get("username")
         self.password = data_source_properties.get("password")
         self.token = data_source_properties.get("token")
         self.schema = data_source_properties.get("schema")
         self.use_encryption = data_source_properties.get("use_encryption", "false")
         self.routing_queue = data_source_properties.get("routing_queue", "")
+        self.disable_certificate_verification = data_source_properties.get("disable_certificate_verification", "false")
 
     def connect(self):
         try:
             token_string = ""
             if self.token:
                 token_string = f";TOKEN={self.token}"
 
@@ -89,15 +90,17 @@
                 + self.username
                 + ";PWD="
                 + self.password
                 + token_string
                 + ";useEncryption="
                 + self.use_encryption
                 + ";routing_queue="
-                + self.routing_queue,
+                + self.routing_queue
+                + ";disableCertificateVerification="
+                + self.disable_certificate_verification,
                 autocommit=True,
             )
         except Exception as e:
             raise DataSourceConnectionError(self.TYPE, e)
 
     def regex_replace_flags(self) -> str:
         return ""
```

