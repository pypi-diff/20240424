# Comparing `tmp/soda-core-contracts-3.3.1.tar.gz` & `tmp/soda_core_contracts-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-contracts-3.3.1.tar", last modified: Sun Mar 24 04:28:53 2024, max compression
+gzip compressed data, was "soda_core_contracts-3.3.2.tar", last modified: Wed Apr 24 15:25:53 2024, max compression
```

## Comparing `soda-core-contracts-3.3.1.tar` & `soda_core_contracts-3.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:28:53.829140 soda-core-contracts-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-24 04:28:53.829140 soda-core-contracts-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-24 04:28:40.000000 soda-core-contracts-3.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 04:28:53.829140 soda-core-contracts-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-24 04:28:40.000000 soda-core-contracts-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:28:53.825140 soda-core-contracts-3.3.1/soda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:28:53.825140 soda-core-contracts-3.3.1/soda/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-03-24 04:28:40.000000 soda-core-contracts-3.3.1/soda/contracts/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    34107 2024-03-24 04:28:40.000000 soda-core-contracts-3.3.1/soda/contracts/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:28:53.825140 soda-core-contracts-3.3.1/soda/contracts/impl/
--rw-r--r--   0 runner    (1001) docker     (127)    32025 2024-03-24 04:28:40.000000 soda-core-contracts-3.3.1/soda/contracts/impl/contract_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-24 04:28:40.000000 soda-core-contracts-3.3.1/soda/contracts/impl/json_schema_verifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-03-24 04:28:40.000000 soda-core-contracts-3.3.1/soda/contracts/impl/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-24 04:28:40.000000 soda-core-contracts-3.3.1/soda/contracts/impl/variable_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    13414 2024-03-24 04:28:40.000000 soda-core-contracts-3.3.1/soda/contracts/impl/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-03-24 04:28:40.000000 soda-core-contracts-3.3.1/soda/contracts/soda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    12339 2024-03-24 04:28:40.000000 soda-core-contracts-3.3.1/soda/contracts/soda_data_contract_json_schema_1_0_0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:28:53.829140 soda-core-contracts-3.3.1/soda_core_contracts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-24 04:28:53.000000 soda-core-contracts-3.3.1/soda_core_contracts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-24 04:28:53.000000 soda-core-contracts-3.3.1/soda_core_contracts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 04:28:53.000000 soda-core-contracts-3.3.1/soda_core_contracts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-24 04:28:53.000000 soda-core-contracts-3.3.1/soda_core_contracts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-24 04:28:53.000000 soda-core-contracts-3.3.1/soda_core_contracts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:53.827670 soda_core_contracts-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-24 15:25:53.827670 soda_core_contracts-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-24 15:25:40.000000 soda_core_contracts-3.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:25:53.827670 soda_core_contracts-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-24 15:25:40.000000 soda_core_contracts-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:53.823670 soda_core_contracts-3.3.2/soda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:53.823670 soda_core_contracts-3.3.2/soda/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-04-24 15:25:40.000000 soda_core_contracts-3.3.2/soda/contracts/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34107 2024-04-24 15:25:40.000000 soda_core_contracts-3.3.2/soda/contracts/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:53.827670 soda_core_contracts-3.3.2/soda/contracts/impl/
+-rw-r--r--   0 runner    (1001) docker     (127)    32025 2024-04-24 15:25:40.000000 soda_core_contracts-3.3.2/soda/contracts/impl/contract_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-24 15:25:40.000000 soda_core_contracts-3.3.2/soda/contracts/impl/json_schema_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-24 15:25:40.000000 soda_core_contracts-3.3.2/soda/contracts/impl/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-24 15:25:40.000000 soda_core_contracts-3.3.2/soda/contracts/impl/variable_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13414 2024-04-24 15:25:40.000000 soda_core_contracts-3.3.2/soda/contracts/impl/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-24 15:25:40.000000 soda_core_contracts-3.3.2/soda/contracts/soda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12339 2024-04-24 15:25:40.000000 soda_core_contracts-3.3.2/soda/contracts/soda_data_contract_json_schema_1_0_0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:53.827670 soda_core_contracts-3.3.2/soda_core_contracts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-24 15:25:53.000000 soda_core_contracts-3.3.2/soda_core_contracts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-24 15:25:53.000000 soda_core_contracts-3.3.2/soda_core_contracts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:25:53.000000 soda_core_contracts-3.3.2/soda_core_contracts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-24 15:25:53.000000 soda_core_contracts-3.3.2/soda_core_contracts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 15:25:53.000000 soda_core_contracts-3.3.2/soda_core_contracts.egg-info/top_level.txt
```

### Comparing `soda-core-contracts-3.3.1/soda/contracts/connection.py` & `soda_core_contracts-3.3.2/soda/contracts/connection.py`

 * *Files identical despite different names*

### Comparing `soda-core-contracts-3.3.1/soda/contracts/contract.py` & `soda_core_contracts-3.3.2/soda/contracts/contract.py`

 * *Files identical despite different names*

### Comparing `soda-core-contracts-3.3.1/soda/contracts/impl/contract_parser.py` & `soda_core_contracts-3.3.2/soda/contracts/impl/contract_parser.py`

 * *Files identical despite different names*

### Comparing `soda-core-contracts-3.3.1/soda/contracts/impl/json_schema_verifier.py` & `soda_core_contracts-3.3.2/soda/contracts/impl/json_schema_verifier.py`

 * *Files identical despite different names*

### Comparing `soda-core-contracts-3.3.1/soda/contracts/impl/logs.py` & `soda_core_contracts-3.3.2/soda/contracts/impl/logs.py`

 * *Files identical despite different names*

### Comparing `soda-core-contracts-3.3.1/soda/contracts/impl/variable_resolver.py` & `soda_core_contracts-3.3.2/soda/contracts/impl/variable_resolver.py`

 * *Files identical despite different names*

### Comparing `soda-core-contracts-3.3.1/soda/contracts/impl/yaml.py` & `soda_core_contracts-3.3.2/soda/contracts/impl/yaml.py`

 * *Files identical despite different names*

### Comparing `soda-core-contracts-3.3.1/soda/contracts/soda_cloud.py` & `soda_core_contracts-3.3.2/soda/contracts/soda_cloud.py`

 * *Files identical despite different names*

### Comparing `soda-core-contracts-3.3.1/soda/contracts/soda_data_contract_json_schema_1_0_0.json` & `soda_core_contracts-3.3.2/soda/contracts/soda_data_contract_json_schema_1_0_0.json`

 * *Files identical despite different names*

### Comparing `soda-core-contracts-3.3.1/soda_core_contracts.egg-info/SOURCES.txt` & `soda_core_contracts-3.3.2/soda_core_contracts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

