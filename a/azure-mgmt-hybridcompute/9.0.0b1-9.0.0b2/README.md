# Comparing `tmp/azure-mgmt-hybridcompute-9.0.0b1.tar.gz` & `tmp/azure-mgmt-hybridcompute-9.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-mgmt-hybridcompute-9.0.0b1.tar", last modified: Tue Nov 21 05:50:00 2023, max compression
+gzip compressed data, was "azure-mgmt-hybridcompute-9.0.0b2.tar", last modified: Wed Apr 24 04:41:19 2024, max compression
```

## Comparing `azure-mgmt-hybridcompute-9.0.0b1.tar` & `azure-mgmt-hybridcompute-9.0.0b2.tar`

### file list

```diff
@@ -1,76 +1,70 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-21 05:50:00.002434 azure-mgmt-hybridcompute-9.0.0b1/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13772 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      219 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/MANIFEST.in
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    16900 2023-11-21 05:50:00.002434 azure-mgmt-hybridcompute-9.0.0b1/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2045 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/README.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      634 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/_meta.json
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-21 05:49:59.994434 azure-mgmt-hybridcompute-9.0.0b1/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-21 05:49:59.994434 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-21 05:49:59.994434 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      928 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3529 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7880 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/_hybrid_compute_management_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    79289 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/_serialization.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1347 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/_vendor.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      488 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-21 05:49:59.994434 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      875 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3577 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8075 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/_hybrid_compute_management_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1087 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/_vendor.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-21 05:49:59.994434 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2062 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7070 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_agent_version_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9793 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_extension_metadata_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12889 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_hybrid_compute_management_client_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9818 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_hybrid_identity_metadata_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    41334 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_license_profiles_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    48566 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_licenses_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    40177 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_machine_extensions_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    34096 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_machines_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4891 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_network_profile_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5840 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    28547 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_private_endpoint_connections_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9830 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_private_link_resources_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    39425 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_private_link_scopes_operations.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-21 05:49:59.998434 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9565 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7270 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/models/_hybrid_compute_management_client_enums.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   162730 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/models/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-21 05:49:59.998434 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2062 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8994 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/_agent_version_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12517 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/_extension_metadata_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    14378 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/_hybrid_compute_management_client_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12744 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/_hybrid_identity_metadata_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    49129 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/_license_profiles_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    57202 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/_licenses_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    47927 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/_machine_extensions_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    41881 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/_machines_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6334 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/_network_profile_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6523 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    34636 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/_private_endpoint_connections_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12551 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/_private_link_resources_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    49901 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/_private_link_scopes_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-21 05:49:59.998434 azure-mgmt-hybridcompute-9.0.0b1/azure_mgmt_hybridcompute.egg-info/
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    16900 2023-11-21 05:49:59.000000 azure-mgmt-hybridcompute-9.0.0b1/azure_mgmt_hybridcompute.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3284 2023-11-21 05:49:59.000000 azure-mgmt-hybridcompute-9.0.0b1/azure_mgmt_hybridcompute.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-11-21 05:49:59.000000 azure-mgmt-hybridcompute-9.0.0b1/azure_mgmt_hybridcompute.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-11-21 05:49:59.000000 azure-mgmt-hybridcompute-9.0.0b1/azure_mgmt_hybridcompute.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      124 2023-11-21 05:49:59.000000 azure-mgmt-hybridcompute-9.0.0b1/azure_mgmt_hybridcompute.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2023-11-21 05:49:59.000000 azure-mgmt-hybridcompute-9.0.0b1/azure_mgmt_hybridcompute.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2023-11-21 05:50:00.002434 azure-mgmt-hybridcompute-9.0.0b1/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2853 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-11-21 05:49:59.998434 azure-mgmt-hybridcompute-9.0.0b1/tests/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2616 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/tests/conftest.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1711 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/tests/disable_test_hybridcompute.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      977 2023-11-21 05:49:16.000000 azure-mgmt-hybridcompute-9.0.0b1/tests/test_mgmt_hybridcompute.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:41:19.085571 azure-mgmt-hybridcompute-9.0.0b2/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15626 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      219 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/MANIFEST.in
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18574 2024-04-24 04:41:19.085571 azure-mgmt-hybridcompute-9.0.0b2/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2045 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/README.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      636 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/_meta.json
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:41:19.077571 azure-mgmt-hybridcompute-9.0.0b2/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:41:19.077571 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:41:19.077571 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      928 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3461 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8017 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/_hybrid_compute_management_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/_serialization.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1347 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/_vendor.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      488 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:41:19.077571 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      875 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3509 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8229 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/_hybrid_compute_management_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1087 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/_vendor.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:41:19.081571 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1778 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9159 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_extension_metadata_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10447 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_hybrid_compute_management_client_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33666 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_machine_extensions_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    24342 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_machine_run_commands_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    29433 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_machines_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4617 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_network_profile_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5639 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    24188 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_private_endpoint_connections_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9146 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_private_link_resources_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    35542 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_private_link_scopes_operations.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:41:19.081571 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11969 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10220 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/models/_hybrid_compute_management_client_enums.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   215695 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/models/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:41:19.085571 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1778 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11883 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_extension_metadata_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11974 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_hybrid_compute_management_client_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    41526 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_machine_extensions_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    30384 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_machine_run_commands_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    37220 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_machines_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6068 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_network_profile_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6322 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    30433 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_private_endpoint_connections_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11925 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_private_link_resources_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    46177 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_private_link_scopes_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:41:19.085571 azure-mgmt-hybridcompute-9.0.0b2/azure_mgmt_hybridcompute.egg-info/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18574 2024-04-24 04:41:19.000000 azure-mgmt-hybridcompute-9.0.0b2/azure_mgmt_hybridcompute.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2878 2024-04-24 04:41:19.000000 azure-mgmt-hybridcompute-9.0.0b2/azure_mgmt_hybridcompute.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-24 04:41:19.000000 azure-mgmt-hybridcompute-9.0.0b2/azure_mgmt_hybridcompute.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-24 04:41:18.000000 azure-mgmt-hybridcompute-9.0.0b2/azure_mgmt_hybridcompute.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       56 2024-04-24 04:41:19.000000 azure-mgmt-hybridcompute-9.0.0b2/azure_mgmt_hybridcompute.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-04-24 04:41:19.000000 azure-mgmt-hybridcompute-9.0.0b2/azure_mgmt_hybridcompute.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-04-24 04:41:19.089571 azure-mgmt-hybridcompute-9.0.0b2/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2780 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:41:19.085571 azure-mgmt-hybridcompute-9.0.0b2/tests/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2616 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/tests/conftest.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1711 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/tests/disable_test_hybridcompute.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      977 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/tests/test_mgmt_hybridcompute.py
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/CHANGELOG.md` & `azure-mgmt-hybridcompute-9.0.0b2/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,43 @@
 # Release History
 
+## 9.0.0b2 (2024-04-22)
+
+### Features Added
+
+  - Added operation group MachineRunCommandsOperations
+  - Model LicenseProfile has a new parameter billing_start_date
+  - Model LicenseProfile has a new parameter disenrollment_date
+  - Model LicenseProfile has a new parameter enrollment_date
+  - Model LicenseProfile has a new parameter product_features
+  - Model LicenseProfile has a new parameter product_type
+  - Model LicenseProfile has a new parameter software_assurance_customer
+  - Model LicenseProfile has a new parameter subscription_status
+  - Model LicenseProfileMachineInstanceView has a new parameter billing_start_date
+  - Model LicenseProfileMachineInstanceView has a new parameter disenrollment_date
+  - Model LicenseProfileMachineInstanceView has a new parameter enrollment_date
+  - Model LicenseProfileMachineInstanceView has a new parameter license_channel
+  - Model LicenseProfileMachineInstanceView has a new parameter license_status
+  - Model LicenseProfileMachineInstanceView has a new parameter product_features
+  - Model LicenseProfileMachineInstanceView has a new parameter product_type
+  - Model LicenseProfileMachineInstanceView has a new parameter software_assurance_customer
+  - Model LicenseProfileMachineInstanceView has a new parameter subscription_status
+  - Model LicenseProfileUpdate has a new parameter product_features
+  - Model LicenseProfileUpdate has a new parameter product_type
+  - Model LicenseProfileUpdate has a new parameter software_assurance_customer
+  - Model LicenseProfileUpdate has a new parameter subscription_status
+  - Model Machine has a new parameter os_edition
+
+### Breaking Changes
+
+  - Removed operation group AgentVersionOperations
+  - Removed operation group HybridIdentityMetadataOperations
+  - Removed operation group LicenseProfilesOperations
+  - Removed operation group LicensesOperations
+
 ## 9.0.0b1 (2023-11-20)
 
 ### Features Added
 
   - Added operation MachinesOperations.begin_assess_patches
   - Added operation MachinesOperations.begin_install_patches
   - Added operation group AgentVersionOperations
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/LICENSE` & `azure-mgmt-hybridcompute-9.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/PKG-INFO` & `azure-mgmt-hybridcompute-9.0.0b2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-hybridcompute
-Version: 9.0.0b1
+Version: 9.0.0b2
 Summary: Microsoft Azure Hybrid Compute Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: isodate<1.0.0,>=0.6.1
-Requires-Dist: azure-common~=1.1
-Requires-Dist: azure-mgmt-core<2.0.0,>=1.3.2
-Requires-Dist: typing-extensions>=4.3.0; python_version < "3.8.0"
 
 # Microsoft Azure SDK for Python
 
 This is the Microsoft Azure Hybrid Compute Management Client Library.
-This package has been tested with Python 3.7+.
+This package has been tested with Python 3.8+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
 ## Getting started
 
 ### Prerequisites
 
-- Python 3.7+ is required to use this package.
+- Python 3.8+ is required to use this package.
 - [Azure subscription](https://azure.microsoft.com/free/)
 
 ### Install the package
 
 ```bash
 pip install azure-mgmt-hybridcompute
 pip install azure-identity
@@ -86,14 +82,48 @@
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 # Release History
 
+## 9.0.0b2 (2024-04-22)
+
+### Features Added
+
+  - Added operation group MachineRunCommandsOperations
+  - Model LicenseProfile has a new parameter billing_start_date
+  - Model LicenseProfile has a new parameter disenrollment_date
+  - Model LicenseProfile has a new parameter enrollment_date
+  - Model LicenseProfile has a new parameter product_features
+  - Model LicenseProfile has a new parameter product_type
+  - Model LicenseProfile has a new parameter software_assurance_customer
+  - Model LicenseProfile has a new parameter subscription_status
+  - Model LicenseProfileMachineInstanceView has a new parameter billing_start_date
+  - Model LicenseProfileMachineInstanceView has a new parameter disenrollment_date
+  - Model LicenseProfileMachineInstanceView has a new parameter enrollment_date
+  - Model LicenseProfileMachineInstanceView has a new parameter license_channel
+  - Model LicenseProfileMachineInstanceView has a new parameter license_status
+  - Model LicenseProfileMachineInstanceView has a new parameter product_features
+  - Model LicenseProfileMachineInstanceView has a new parameter product_type
+  - Model LicenseProfileMachineInstanceView has a new parameter software_assurance_customer
+  - Model LicenseProfileMachineInstanceView has a new parameter subscription_status
+  - Model LicenseProfileUpdate has a new parameter product_features
+  - Model LicenseProfileUpdate has a new parameter product_type
+  - Model LicenseProfileUpdate has a new parameter software_assurance_customer
+  - Model LicenseProfileUpdate has a new parameter subscription_status
+  - Model Machine has a new parameter os_edition
+
+### Breaking Changes
+
+  - Removed operation group AgentVersionOperations
+  - Removed operation group HybridIdentityMetadataOperations
+  - Removed operation group LicenseProfilesOperations
+  - Removed operation group LicensesOperations
+
 ## 9.0.0b1 (2023-11-20)
 
 ### Features Added
 
   - Added operation MachinesOperations.begin_assess_patches
   - Added operation MachinesOperations.begin_install_patches
   - Added operation group AgentVersionOperations
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/README.md` & `azure-mgmt-hybridcompute-9.0.0b2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Microsoft Azure SDK for Python
 
 This is the Microsoft Azure Hybrid Compute Management Client Library.
-This package has been tested with Python 3.7+.
+This package has been tested with Python 3.8+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
 ## Getting started
 
 ### Prerequisites
 
-- Python 3.7+ is required to use this package.
+- Python 3.8+ is required to use this package.
 - [Azure subscription](https://azure.microsoft.com/free/)
 
 ### Install the package
 
 ```bash
 pip install azure-mgmt-hybridcompute
 pip install azure-identity
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/_meta.json` & `azure-mgmt-hybridcompute-9.0.0b2/_meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'autorest_command'": "'autorest specification/hybridcompute/resource-manager/readme.md "*

 * *                       '--generate-sample=True --include-x-ms-examples-original-file=True --python '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk '*

 * *                       '--use=@autorest/python@6.13.7 --use=@autorest/modelerfour@4.27.0 '*

 * *                       "--version=3.9.7 --version-tolerant=False'",*

 * * "'commit'": "'71a0c7adf2a6e169ab9a33c7cf36bb93db083e86'",*

 * * "'use'": "[ […]*

```diff
@@ -1,11 +1,11 @@
 {
     "autorest": "3.9.7",
-    "autorest_command": "autorest specification/hybridcompute/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.7.1 --use=@autorest/modelerfour@4.26.2 --version=3.9.7 --version-tolerant=False",
-    "commit": "11bbc2b1df2e915a2227a6a1a48a27b9e67c3311",
+    "autorest_command": "autorest specification/hybridcompute/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.13.7 --use=@autorest/modelerfour@4.27.0 --version=3.9.7 --version-tolerant=False",
+    "commit": "71a0c7adf2a6e169ab9a33c7cf36bb93db083e86",
     "readme": "specification/hybridcompute/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
-        "@autorest/python@6.7.1",
-        "@autorest/modelerfour@4.26.2"
+        "@autorest/python@6.13.7",
+        "@autorest/modelerfour@4.27.0"
     ]
 }
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/__init__.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/_configuration.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/_configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,63 +4,62 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any, TYPE_CHECKING
 
-from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
 
 from ._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 
-class HybridComputeManagementClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+class HybridComputeManagementClientConfiguration:  # pylint: disable=too-many-instance-attributes,name-too-long
     """Configuration for HybridComputeManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2023-06-20-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-10-03-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        super(HybridComputeManagementClientConfiguration, self).__init__(**kwargs)
-        api_version: str = kwargs.pop("api_version", "2023-06-20-preview")
+        api_version: str = kwargs.pop("api_version", "2023-10-03-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
         self.subscription_id = subscription_id
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["https://management.azure.com/.default"])
         kwargs.setdefault("sdk_moniker", "mgmt-hybridcompute/{}".format(VERSION))
+        self.polling_interval = kwargs.get("polling_interval", 30)
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
         self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
             self.authentication_policy = ARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/_patch.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/_serialization.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/_serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,16 @@
     from urllib import quote  # type: ignore
 except ImportError:
     from urllib.parse import quote
 import xml.etree.ElementTree as ET
 
 import isodate  # type: ignore
 
-from azure.core.exceptions import DeserializationError, SerializationError, raise_with_traceback
-from azure.core.serialization import NULL as AzureCoreNull
+from azure.core.exceptions import DeserializationError, SerializationError
+from azure.core.serialization import NULL as CoreNull
 
 _BOM = codecs.BOM_UTF8.decode(encoding="utf-8")
 
 ModelType = TypeVar("ModelType", bound="Model")
 JSON = MutableMapping[str, Any]
 
 
@@ -120,15 +120,15 @@
                     if isinstance(data, unicode):  # type: ignore
                         # If I'm Python 2.7 and unicode XML will scream if I try a "fromstring" on unicode string
                         data_as_str = data_as_str.encode(encoding="utf-8")  # type: ignore
                 except NameError:
                     pass
 
                 return ET.fromstring(data_as_str)  # nosec
-            except ET.ParseError:
+            except ET.ParseError as err:
                 # It might be because the server has an issue, and returned JSON with
                 # content-type XML....
                 # So let's try a JSON load, and if it's still broken
                 # let's flow the initial exception
                 def _json_attemp(data):
                     try:
                         return True, json.loads(data)
@@ -139,15 +139,15 @@
                 if success:
                     return json_result
                 # If i'm here, it's not JSON, it's not XML, let's scream
                 # and raise the last context in this block (the XML exception)
                 # The function hack is because Py2.7 messes up with exception
                 # context otherwise.
                 _LOGGER.critical("Wasn't XML not JSON, failing")
-                raise_with_traceback(DeserializationError, "XML is invalid")
+                raise DeserializationError("XML is invalid") from err
         raise DeserializationError("Cannot deserialize content-type: {}".format(content_type))
 
     @classmethod
     def deserialize_from_http_generics(cls, body_bytes: Optional[Union[AnyStr, IO]], headers: Mapping) -> Any:
         """Deserialize from HTTP response.
 
         Use bytes and headers to NOT use any requests/aiohttp or whatever
@@ -166,21 +166,14 @@
             content_type = "application/json"
 
         if body_bytes:
             return cls.deserialize_from_text(body_bytes, content_type)
         return None
 
 
-try:
-    basestring  # type: ignore
-    unicode_str = unicode  # type: ignore
-except NameError:
-    basestring = str
-    unicode_str = str
-
 _LOGGER = logging.getLogger(__name__)
 
 try:
     _long_type = long  # type: ignore
 except NameError:
     _long_type = int
 
@@ -291,15 +284,15 @@
     """
 
     _subtype_map: Dict[str, Dict[str, Any]] = {}
     _attribute_map: Dict[str, Dict[str, Any]] = {}
     _validation: Dict[str, Dict[str, Any]] = {}
 
     def __init__(self, **kwargs: Any) -> None:
-        self.additional_properties: Dict[str, Any] = {}
+        self.additional_properties: Optional[Dict[str, Any]] = {}
         for k in kwargs:
             if k not in self._attribute_map:
                 _LOGGER.warning("%s is not a known attribute of class %s and will be ignored", k, self.__class__)
             elif k in self._validation and self._validation[k].get("readonly", False):
                 _LOGGER.warning("Readonly attribute %s will be ignored in class %s", k, self.__class__)
             else:
                 setattr(self, k, kwargs[k])
@@ -336,26 +329,26 @@
             xml_map = cls._xml_map  # type: ignore
         except AttributeError:
             xml_map = {}
 
         return _create_xml_node(xml_map.get("name", cls.__name__), xml_map.get("prefix", None), xml_map.get("ns", None))
 
     def serialize(self, keep_readonly: bool = False, **kwargs: Any) -> JSON:
-        """Return the JSON that would be sent to azure from this model.
+        """Return the JSON that would be sent to server from this model.
 
         This is an alias to `as_dict(full_restapi_key_transformer, keep_readonly=False)`.
 
         If you want XML serialization, you can pass the kwargs is_xml=True.
 
         :param bool keep_readonly: If you want to serialize the readonly attributes
         :returns: A dict JSON compatible object
         :rtype: dict
         """
         serializer = Serializer(self._infer_class_models())
-        return serializer._serialize(self, keep_readonly=keep_readonly, **kwargs)
+        return serializer._serialize(self, keep_readonly=keep_readonly, **kwargs)  # type: ignore
 
     def as_dict(
         self,
         keep_readonly: bool = True,
         key_transformer: Callable[[str, Dict[str, Any], Any], Any] = attribute_transformer,
         **kwargs: Any
     ) -> JSON:
@@ -386,15 +379,15 @@
         If you want XML serialization, you can pass the kwargs is_xml=True.
 
         :param function key_transformer: A key transformer function.
         :returns: A dict JSON compatible object
         :rtype: dict
         """
         serializer = Serializer(self._infer_class_models())
-        return serializer._serialize(self, key_transformer=key_transformer, keep_readonly=keep_readonly, **kwargs)
+        return serializer._serialize(self, key_transformer=key_transformer, keep_readonly=keep_readonly, **kwargs)  # type: ignore
 
     @classmethod
     def _infer_class_models(cls):
         try:
             str_models = cls.__module__.rsplit(".", 1)[0]
             models = sys.modules[str_models]
             client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
@@ -411,15 +404,15 @@
 
         :param str data: A str using RestAPI structure. JSON by default.
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
-        return deserializer(cls.__name__, data, content_type=content_type)
+        return deserializer(cls.__name__, data, content_type=content_type)  # type: ignore
 
     @classmethod
     def from_dict(
         cls: Type[ModelType],
         data: Any,
         key_extractors: Optional[Callable[[str, Dict[str, Any], Any], Any]] = None,
         content_type: Optional[str] = None,
@@ -441,15 +434,15 @@
                 attribute_key_case_insensitive_extractor,
                 rest_key_case_insensitive_extractor,
                 last_rest_key_case_insensitive_extractor,
             ]
             if key_extractors is None
             else key_extractors
         )
-        return deserializer(cls.__name__, data, content_type=content_type)
+        return deserializer(cls.__name__, data, content_type=content_type)  # type: ignore
 
     @classmethod
     def _flatten_subtype(cls, key, objects):
         if "_subtype_map" not in cls.__dict__:
             return {}
         result = dict(cls._subtype_map[key])
         for valuetype in cls._subtype_map[key].values():
@@ -541,15 +534,15 @@
         "min_items": lambda x, y: len(x) < y,
         "max_items": lambda x, y: len(x) > y,
         "pattern": lambda x, y: not re.match(y, x, re.UNICODE),
         "unique": lambda x, y: len(x) != len(set(x)),
         "multiple": lambda x, y: x % y != 0,
     }
 
-    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
+    def __init__(self, classes: Optional[Mapping[str, type]] = None):
         self.serialize_type = {
             "iso-8601": Serializer.serialize_iso,
             "rfc-1123": Serializer.serialize_rfc,
             "unix-time": Serializer.serialize_unix,
             "duration": Serializer.serialize_duration,
             "date": Serializer.serialize_date,
             "time": Serializer.serialize_time,
@@ -557,15 +550,15 @@
             "long": Serializer.serialize_long,
             "bytearray": Serializer.serialize_bytearray,
             "base64": Serializer.serialize_base64,
             "object": self.serialize_object,
             "[]": self.serialize_iter,
             "{}": self.serialize_dict,
         }
-        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
+        self.dependencies: Dict[str, type] = dict(classes) if classes else {}
         self.key_transformer = full_restapi_key_transformer
         self.client_side_validation = True
 
     def _serialize(self, target_obj, data_type=None, **kwargs):
         """Serialize data into a string according to type.
 
         :param target_obj: The data to be serialized.
@@ -645,15 +638,15 @@
                                     new_attr.tag = "}".join([splitted_tag[0], xml_name])
                                 else:
                                     new_attr.tag = xml_name
                             serialized.append(new_attr)  # type: ignore
                         else:  # That's a basic type
                             # Integrate namespace if necessary
                             local_node = _create_xml_node(xml_name, xml_prefix, xml_ns)
-                            local_node.text = unicode_str(new_attr)
+                            local_node.text = str(new_attr)
                             serialized.append(local_node)  # type: ignore
                     else:  # JSON
                         for k in reversed(keys):  # type: ignore
                             new_attr = {k: new_attr}
 
                         _new_attr = new_attr
                         _serialized = serialized
@@ -664,15 +657,15 @@
                             _serialized = _serialized[k]
                 except ValueError as err:
                     if isinstance(err, SerializationError):
                         raise
 
         except (AttributeError, KeyError, TypeError) as err:
             msg = "Attribute {} in object {} cannot be serialized.\n{}".format(attr_name, class_name, str(target_obj))
-            raise_with_traceback(SerializationError, msg, err)
+            raise SerializationError(msg) from err
         else:
             return serialized
 
     def body(self, data, data_type, **kwargs):
         """Serialize data intended for a request body.
 
         :param data: The data to be serialized.
@@ -706,15 +699,15 @@
                     deserializer.key_extractors = [
                         rest_key_case_insensitive_extractor,
                         attribute_key_case_insensitive_extractor,
                         last_rest_key_case_insensitive_extractor,
                     ]
                 data = deserializer._deserialize(data_type, data)
             except DeserializationError as err:
-                raise_with_traceback(SerializationError, "Unable to build a model: " + str(err), err)
+                raise SerializationError("Unable to build a model: " + str(err)) from err
 
         return self._serialize(data, data_type, **kwargs)
 
     def url(self, name, data, data_type, **kwargs):
         """Serialize data intended for a URL path.
 
         :param data: The data to be serialized.
@@ -726,38 +719,39 @@
         try:
             output = self.serialize_data(data, data_type, **kwargs)
             if data_type == "bool":
                 output = json.dumps(output)
 
             if kwargs.get("skip_quote") is True:
                 output = str(output)
+                output = output.replace("{", quote("{")).replace("}", quote("}"))
             else:
                 output = quote(str(output), safe="")
         except SerializationError:
             raise TypeError("{} must be type {}.".format(name, data_type))
         else:
             return output
 
     def query(self, name, data, data_type, **kwargs):
         """Serialize data intended for a URL query.
 
         :param data: The data to be serialized.
         :param str data_type: The type to be serialized from.
         :keyword bool skip_quote: Whether to skip quote the serialized result.
         Defaults to False.
-        :rtype: str
+        :rtype: str, list
         :raises: TypeError if serialization fails.
         :raises: ValueError if data is None
         """
         try:
             # Treat the list aside, since we don't want to encode the div separator
             if data_type.startswith("["):
                 internal_data_type = data_type[1:-1]
                 do_quote = not kwargs.get("skip_quote", False)
-                return str(self.serialize_iter(data, internal_data_type, do_quote=do_quote, **kwargs))
+                return self.serialize_iter(data, internal_data_type, do_quote=do_quote, **kwargs)
 
             # Not a list, regular serialization
             output = self.serialize_data(data, data_type, **kwargs)
             if data_type == "bool":
                 output = json.dumps(output)
             if kwargs.get("skip_quote") is True:
                 output = str(output)
@@ -800,15 +794,15 @@
         :raises: ValueError if data is None
         :raises: SerializationError if serialization fails.
         """
         if data is None:
             raise ValueError("No value for given attribute")
 
         try:
-            if data is AzureCoreNull:
+            if data is CoreNull:
                 return None
             if data_type in self.basic_types.values():
                 return self.serialize_basic(data, data_type, **kwargs)
 
             elif data_type in self.serialize_type:
                 return self.serialize_type[data_type](data, **kwargs)
 
@@ -820,15 +814,15 @@
 
             iter_type = data_type[0] + data_type[-1]
             if iter_type in self.serialize_type:
                 return self.serialize_type[iter_type](data, data_type[1:-1], **kwargs)
 
         except (ValueError, TypeError) as err:
             msg = "Unable to serialize value: {!r} as type: {!r}."
-            raise_with_traceback(SerializationError, msg.format(data, data_type), err)
+            raise SerializationError(msg.format(data, data_type)) from err
         else:
             return self._serialize(data, **kwargs)
 
     @classmethod
     def _get_custom_serializers(cls, data_type, **kwargs):
         custom_serializer = kwargs.get("basic_types_serializers", {}).get(data_type)
         if custom_serializer:
@@ -989,15 +983,15 @@
         if isinstance(attr, ET.Element):
             return attr
         obj_type = type(attr)
         if obj_type in self.basic_types:
             return self.serialize_basic(attr, self.basic_types[obj_type], **kwargs)
         if obj_type is _long_type:
             return self.serialize_long(attr)
-        if obj_type is unicode_str:
+        if obj_type is str:
             return self.serialize_unicode(attr)
         if obj_type is datetime.datetime:
             return self.serialize_iso(attr)
         if obj_type is datetime.date:
             return self.serialize_date(attr)
         if obj_type is datetime.time:
             return self.serialize_time(attr)
@@ -1166,18 +1160,18 @@
                 microseconds = "." + microseconds
             date = "{:04}-{:02}-{:02}T{:02}:{:02}:{:02}".format(
                 utc.tm_year, utc.tm_mon, utc.tm_mday, utc.tm_hour, utc.tm_min, utc.tm_sec
             )
             return date + microseconds + "Z"
         except (ValueError, OverflowError) as err:
             msg = "Unable to serialize datetime object."
-            raise_with_traceback(SerializationError, msg, err)
+            raise SerializationError(msg) from err
         except AttributeError as err:
             msg = "ISO-8601 object must be valid Datetime object."
-            raise_with_traceback(TypeError, msg, err)
+            raise TypeError(msg) from err
 
     @staticmethod
     def serialize_unix(attr, **kwargs):
         """Serialize Datetime object into IntTime format.
         This is represented as seconds.
 
         :param Datetime attr: Object to be serialized.
@@ -1205,15 +1199,14 @@
             key = _decode_attribute_map_key(dict_keys[0])
             break
         working_key = _decode_attribute_map_key(dict_keys[0])
         working_data = working_data.get(working_key, data)
         if working_data is None:
             # If at any point while following flatten JSON path see None, it means
             # that all properties under are None as well
-            # https://github.com/Azure/msrest-for-python/issues/197
             return None
         key = ".".join(dict_keys[1:])
 
     return working_data.get(key)
 
 
 def rest_key_case_insensitive_extractor(attr, attr_desc, data):
@@ -1226,15 +1219,14 @@
             key = _decode_attribute_map_key(dict_keys[0])
             break
         working_key = _decode_attribute_map_key(dict_keys[0])
         working_data = attribute_key_case_insensitive_extractor(working_key, None, working_data)
         if working_data is None:
             # If at any point while following flatten JSON path see None, it means
             # that all properties under are None as well
-            # https://github.com/Azure/msrest-for-python/issues/197
             return None
         key = ".".join(dict_keys[1:])
 
     if working_data:
         return attribute_key_case_insensitive_extractor(key, None, working_data)
 
 
@@ -1367,15 +1359,15 @@
     :ivar list key_extractors: Ordered list of extractors to be used by this deserializer.
     """
 
     basic_types = {str: "str", int: "int", bool: "bool", float: "float"}
 
     valid_date = re.compile(r"\d{4}[-]\d{2}[-]\d{2}T\d{2}:\d{2}:\d{2}" r"\.?\d*Z?[-+]?[\d{2}]?:?[\d{2}]?")
 
-    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
+    def __init__(self, classes: Optional[Mapping[str, type]] = None):
         self.deserialize_type = {
             "iso-8601": Deserializer.deserialize_iso,
             "rfc-1123": Deserializer.deserialize_rfc,
             "unix-time": Deserializer.deserialize_unix,
             "duration": Deserializer.deserialize_duration,
             "date": Deserializer.deserialize_date,
             "time": Deserializer.deserialize_time,
@@ -1387,15 +1379,15 @@
             "[]": self.deserialize_iter,
             "{}": self.deserialize_dict,
         }
         self.deserialize_expected_types = {
             "duration": (isodate.Duration, datetime.timedelta),
             "iso-8601": (datetime.datetime),
         }
-        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
+        self.dependencies: Dict[str, type] = dict(classes) if classes else {}
         self.key_extractors = [rest_key_extractor, xml_key_extractor]
         # Additional properties only works if the "rest_key_extractor" is used to
         # extract the keys. Making it to work whatever the key extractor is too much
         # complicated, with no real scenario for now.
         # So adding a flag to disable additional properties detection. This flag should be
         # used if your expect the deserialization to NOT come from a JSON REST syntax.
         # Otherwise, result are unexpected
@@ -1440,15 +1432,15 @@
                     setattr(data, attr, self._deserialize(local_type, value))
                 return data
             except AttributeError:
                 return
 
         response, class_name = self._classify_target(target_obj, data)
 
-        if isinstance(response, basestring):
+        if isinstance(response, str):
             return self.deserialize_data(data, response)
         elif isinstance(response, type) and issubclass(response, Enum):
             return self.deserialize_enum(data, response)
 
         if data is None:
             return data
         try:
@@ -1477,15 +1469,15 @@
                             continue
                         raw_value = found_value
 
                 value = self.deserialize_data(raw_value, attr_desc["type"])
                 d_attrs[attr] = value
         except (AttributeError, TypeError, KeyError) as err:
             msg = "Unable to deserialize to object: " + class_name  # type: ignore
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             additional_properties = self._build_additional_properties(attributes, data)
             return self._instantiate_model(response, d_attrs, additional_properties)
 
     def _build_additional_properties(self, attribute_map, data):
         if not self.additional_properties_detection:
             return None
@@ -1511,22 +1503,22 @@
 
         :param str target: The target object type to deserialize to.
         :param str/dict data: The response data to deserialize.
         """
         if target is None:
             return None, None
 
-        if isinstance(target, basestring):
+        if isinstance(target, str):
             try:
                 target = self.dependencies[target]
             except KeyError:
                 return target, target
 
         try:
-            target = target._classify(data, self.dependencies)
+            target = target._classify(data, self.dependencies)  # type: ignore
         except AttributeError:
             pass  # Target is not a Model, no classify
         return target, target.__class__.__name__  # type: ignore
 
     def failsafe_deserialize(self, target_obj, data, content_type=None):
         """Ignores any errors encountered in deserialization,
         and falls back to not deserializing the object. Recommended
@@ -1574,15 +1566,15 @@
         if hasattr(raw_data, "body"):
             return RawDeserializer.deserialize_from_http_generics(raw_data.text(), raw_data.headers)
 
         # Assume this enough to recognize requests.Response without importing it.
         if hasattr(raw_data, "_content_consumed"):
             return RawDeserializer.deserialize_from_http_generics(raw_data.text, raw_data.headers)
 
-        if isinstance(raw_data, (basestring, bytes)) or hasattr(raw_data, "read"):
+        if isinstance(raw_data, (str, bytes)) or hasattr(raw_data, "read"):
             return RawDeserializer.deserialize_from_text(raw_data, content_type)  # type: ignore
         return raw_data
 
     def _instantiate_model(self, response, attrs, additional_properties=None):
         """Instantiate a response model passing in deserialized args.
 
         :param response: The response model class.
@@ -1648,15 +1640,15 @@
                 if isinstance(data, ET.Element):
                     data = data.text
                 return self.deserialize_enum(data, obj_type)
 
         except (ValueError, TypeError, AttributeError) as err:
             msg = "Unable to deserialize response data."
             msg += " Data: {}, {}".format(data, data_type)
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return self._deserialize(obj_type, data)
 
     def deserialize_iter(self, attr, iter_type):
         """Deserialize an iterable.
 
         :param list attr: Iterable to be deserialized.
@@ -1696,15 +1688,15 @@
         :raises: TypeError if non-builtin datatype encountered.
         """
         if attr is None:
             return None
         if isinstance(attr, ET.Element):
             # Do no recurse on XML, just return the tree as-is
             return attr
-        if isinstance(attr, basestring):
+        if isinstance(attr, str):
             return self.deserialize_basic(attr, "str")
         obj_type = type(attr)
         if obj_type in self.basic_types:
             return self.deserialize_basic(attr, self.basic_types[obj_type])
         if obj_type is _long_type:
             return self.deserialize_long(attr)
 
@@ -1753,15 +1745,15 @@
                     # None or '', node <a/> with a strong type is None.
                     # Don't try to model "empty bool" or "empty int"
                     return None
 
         if data_type == "bool":
             if attr in [True, False, 1, 0]:
                 return bool(attr)
-            elif isinstance(attr, basestring):
+            elif isinstance(attr, str):
                 if attr.lower() in ["true", "1"]:
                     return True
                 elif attr.lower() in ["false", "0"]:
                     return False
             raise TypeError("Invalid boolean value: {}".format(attr))
 
         if data_type == "str":
@@ -1804,15 +1796,14 @@
         """
         if isinstance(data, enum_obj) or data is None:
             return data
         if isinstance(data, Enum):
             data = data.value
         if isinstance(data, int):
             # Workaround. We might consider remove it in the future.
-            # https://github.com/Azure/azure-rest-api-specs/issues/141
             try:
                 return list(enum_obj.__members__.values())[data]
             except IndexError:
                 error = "{!r} is not a valid index for enum {!r}"
                 raise DeserializationError(error.format(data, enum_obj))
         try:
             return enum_obj(str(data))
@@ -1858,18 +1849,18 @@
         :param str attr: response string to be deserialized.
         :rtype: Decimal
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
-            return decimal.Decimal(attr)  # type: ignore
+            return decimal.Decimal(str(attr))  # type: ignore
         except decimal.DecimalException as err:
             msg = "Invalid decimal {}".format(attr)
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
 
     @staticmethod
     def deserialize_long(attr):
         """Deserialize string into long (Py2) or int (Py3).
 
         :param str attr: response string to be deserialized.
         :rtype: long or int
@@ -1889,15 +1880,15 @@
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
             duration = isodate.parse_duration(attr)
         except (ValueError, OverflowError, AttributeError) as err:
             msg = "Cannot deserialize duration object."
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return duration
 
     @staticmethod
     def deserialize_date(attr):
         """Deserialize ISO-8601 formatted string into Date object.
 
@@ -1906,15 +1897,15 @@
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         if re.search(r"[^\W\d_]", attr, re.I + re.U):  # type: ignore
             raise DeserializationError("Date must have only digits and -. Received: %s" % attr)
         # This must NOT use defaultmonth/defaultday. Using None ensure this raises an exception.
-        return isodate.parse_date(attr, defaultmonth=None, defaultday=None)
+        return isodate.parse_date(attr, defaultmonth=0, defaultday=0)
 
     @staticmethod
     def deserialize_time(attr):
         """Deserialize ISO-8601 formatted string into time object.
 
         :param str attr: response string to be deserialized.
         :rtype: datetime.time
@@ -1941,15 +1932,15 @@
             date_obj = datetime.datetime(
                 *parsed_date[:6], tzinfo=_FixedOffset(datetime.timedelta(minutes=(parsed_date[9] or 0) / 60))
             )
             if not date_obj.tzinfo:
                 date_obj = date_obj.astimezone(tz=TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to rfc datetime object."
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return date_obj
 
     @staticmethod
     def deserialize_iso(attr):
         """Deserialize ISO-8601 formatted string into Datetime object.
 
@@ -1978,15 +1969,15 @@
 
             date_obj = isodate.parse_datetime(attr)
             test_utc = date_obj.utctimetuple()
             if test_utc.tm_year > 9999 or test_utc.tm_year < 1:
                 raise OverflowError("Hit max or min date")
         except (ValueError, OverflowError, AttributeError) as err:
             msg = "Cannot deserialize datetime object."
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return date_obj
 
     @staticmethod
     def deserialize_unix(attr):
         """Serialize Datetime object into IntTime format.
         This is represented as seconds.
@@ -1994,13 +1985,14 @@
         :param int attr: Object to be serialized.
         :rtype: Datetime
         :raises: DeserializationError if format invalid
         """
         if isinstance(attr, ET.Element):
             attr = int(attr.text)  # type: ignore
         try:
+            attr = int(attr)
             date_obj = datetime.datetime.fromtimestamp(attr, TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to unix datetime object."
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return date_obj
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/_vendor.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/__init__.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/_configuration.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/_configuration.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,63 +4,62 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any, TYPE_CHECKING
 
-from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
 
 from .._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
-class HybridComputeManagementClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+class HybridComputeManagementClientConfiguration:  # pylint: disable=too-many-instance-attributes,name-too-long
     """Configuration for HybridComputeManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2023-06-20-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-10-03-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        super(HybridComputeManagementClientConfiguration, self).__init__(**kwargs)
-        api_version: str = kwargs.pop("api_version", "2023-06-20-preview")
+        api_version: str = kwargs.pop("api_version", "2023-10-03-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
         self.subscription_id = subscription_id
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["https://management.azure.com/.default"])
         kwargs.setdefault("sdk_moniker", "mgmt-hybridcompute/{}".format(VERSION))
+        self.polling_interval = kwargs.get("polling_interval", 30)
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
         self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
             self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/_patch.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/_vendor.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/__init__.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,42 +2,36 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._licenses_operations import LicensesOperations
 from ._machines_operations import MachinesOperations
-from ._license_profiles_operations import LicenseProfilesOperations
 from ._machine_extensions_operations import MachineExtensionsOperations
 from ._hybrid_compute_management_client_operations import HybridComputeManagementClientOperationsMixin
 from ._extension_metadata_operations import ExtensionMetadataOperations
 from ._operations import Operations
 from ._network_profile_operations import NetworkProfileOperations
-from ._hybrid_identity_metadata_operations import HybridIdentityMetadataOperations
-from ._agent_version_operations import AgentVersionOperations
+from ._machine_run_commands_operations import MachineRunCommandsOperations
 from ._private_link_scopes_operations import PrivateLinkScopesOperations
 from ._private_link_resources_operations import PrivateLinkResourcesOperations
 from ._private_endpoint_connections_operations import PrivateEndpointConnectionsOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
-    "LicensesOperations",
     "MachinesOperations",
-    "LicenseProfilesOperations",
     "MachineExtensionsOperations",
     "HybridComputeManagementClientOperationsMixin",
     "ExtensionMetadataOperations",
     "Operations",
     "NetworkProfileOperations",
-    "HybridIdentityMetadataOperations",
-    "AgentVersionOperations",
+    "MachineRunCommandsOperations",
     "PrivateLinkScopesOperations",
     "PrivateLinkResourcesOperations",
     "PrivateEndpointConnectionsOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_agent_version_operations.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_operations.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,168 +1,151 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, Callable, Dict, Optional, TypeVar
+from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
+import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
+from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse
+from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
-from azure.core.tracing.decorator_async import distributed_trace_async
+from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
-from ... import models as _models
-from ..._vendor import _convert_request
-from ...operations._agent_version_operations import build_get_request, build_list_request
-from .._vendor import HybridComputeManagementClientMixinABC
+from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import HybridComputeManagementClientMixinABC, _convert_request
 
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
 
-class AgentVersionOperations:
+
+def build_list_request(**kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop("template_url", "/providers/Microsoft.HybridCompute/operations")
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+class Operations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.hybridcompute.aio.HybridComputeManagementClient`'s
-        :attr:`agent_version` attribute.
+        :class:`~azure.mgmt.hybridcompute.HybridComputeManagementClient`'s
+        :attr:`operations` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    @distributed_trace_async
-    async def list(self, os_type: str, **kwargs: Any) -> _models.AgentVersionsList:
-        """Gets all Agent Versions along with the download link currently present.
-
-        :param os_type: Defines the os type. Required.
-        :type os_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: AgentVersionsList or the result of cls(response)
-        :rtype: ~azure.mgmt.hybridcompute.models.AgentVersionsList
+    @distributed_trace
+    def list(self, **kwargs: Any) -> Iterable["_models.OperationValue"]:
+        """Gets a list of hybrid compute operations.
+
+        :return: An iterator like instance of either OperationValue or the result of cls(response)
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.hybridcompute.models.OperationValue]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.AgentVersionsList] = kwargs.pop("cls", None)
+        cls: ClsType[_models.OperationListResult] = kwargs.pop("cls", None)
 
-        request = build_list_request(
-            os_type=os_type,
-            api_version=api_version,
-            template_url=self.list.metadata["url"],
-            headers=_headers,
-            params=_params,
-        )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
-
-        _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.ErrorResponseAutoGenerated, pipeline_response)
-            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-        deserialized = self._deserialize("AgentVersionsList", pipeline_response)
-
-        if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
-
-    list.metadata = {"url": "/providers/Microsoft.HybridCompute/osType/{osType}/agentVersions"}
-
-    @distributed_trace_async
-    async def get(self, os_type: str, version: str, **kwargs: Any) -> _models.AgentVersion:
-        """Gets an Agent Version along with the download link currently present.
-
-        :param os_type: Defines the os type. Required.
-        :type os_type: str
-        :param version: Defines the agent version. To get latest, use latest or else a specific agent
-         version. Required.
-        :type version: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: AgentVersion or the result of cls(response)
-        :rtype: ~azure.mgmt.hybridcompute.models.AgentVersion
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.AgentVersion] = kwargs.pop("cls", None)
-
-        request = build_get_request(
-            os_type=os_type,
-            version=version,
-            api_version=api_version,
-            template_url=self.get.metadata["url"],
-            headers=_headers,
-            params=_params,
-        )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
-
-        _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.ErrorResponseAutoGenerated, pipeline_response)
-            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-        deserialized = self._deserialize("AgentVersion", pipeline_response)
+        def prepare_request(next_link=None):
+            if not next_link:
 
-        if cls:
-            return cls(pipeline_response, deserialized, {})
+                _request = build_list_request(
+                    api_version=api_version,
+                    headers=_headers,
+                    params=_params,
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+
+            else:
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                _request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
+
+        def extract_data(pipeline_response):
+            deserialized = self._deserialize("OperationListResult", pipeline_response)
+            list_of_elem = deserialized.value
+            if cls:
+                list_of_elem = cls(list_of_elem)  # type: ignore
+            return None, iter(list_of_elem)
+
+        def get_next(next_link=None):
+            _request = prepare_request(next_link)
+
+            _stream = False
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+            response = pipeline_response.http_response
+
+            if response.status_code not in [200]:
+                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        return deserialized
+            return pipeline_response
 
-    get.metadata = {"url": "/providers/Microsoft.HybridCompute/osType/{osType}/agentVersions/{version}"}
+        return ItemPaged(get_next, extract_data)
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_extension_metadata_operations.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_extension_metadata_operations.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -64,15 +64,14 @@
         :type location: str
         :param publisher: The publisher of the Extension being received. Required.
         :type publisher: str
         :param extension_type: The extensionType of the Extension being received. Required.
         :type extension_type: str
         :param version: The version of the Extension being received. Required.
         :type version: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ExtensionValue or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.ExtensionValue
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -83,64 +82,58 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ExtensionValue] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             location=location,
             publisher=publisher,
             extension_type=extension_type,
             version=version,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ExtensionValue", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.HybridCompute/locations/{location}/publishers/{publisher}/extensionTypes/{extensionType}/versions/{version}"
-    }
+        return deserialized  # type: ignore
 
     @distributed_trace
     def list(
         self, location: str, publisher: str, extension_type: str, **kwargs: Any
     ) -> AsyncIterable["_models.ExtensionValue"]:
         """Gets all Extension versions based on location, publisher, extensionType.
 
         :param location: The location of the Extension being received. Required.
         :type location: str
         :param publisher: The publisher of the Extension being received. Required.
         :type publisher: str
         :param extension_type: The extensionType of the Extension being received. Required.
         :type extension_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ExtensionValue or the result of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.hybridcompute.models.ExtensionValue]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -155,66 +148,61 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     location=location,
                     publisher=publisher,
                     extension_type=extension_type,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ExtensionValueListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
-
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.HybridCompute/locations/{location}/publishers/{publisher}/extensionTypes/{extensionType}/versions"
-    }
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_hybrid_compute_management_client_operations.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_hybrid_compute_management_client_operations.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -31,20 +31,22 @@
 from ...operations._hybrid_compute_management_client_operations import build_upgrade_extensions_request
 from .._vendor import HybridComputeManagementClientMixinABC
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class HybridComputeManagementClientOperationsMixin(HybridComputeManagementClientMixinABC):
+class HybridComputeManagementClientOperationsMixin(  # pylint: disable=name-too-long
+    HybridComputeManagementClientMixinABC
+):
     async def _upgrade_extensions_initial(  # pylint: disable=inconsistent-return-statements
         self,
         resource_group_name: str,
         machine_name: str,
-        extension_upgrade_parameters: Union[_models.MachineExtensionUpgrade, IO],
+        extension_upgrade_parameters: Union[_models.MachineExtensionUpgrade, IO[bytes]],
         **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -62,32 +64,31 @@
         _json = None
         _content = None
         if isinstance(extension_upgrade_parameters, (IOBase, bytes)):
             _content = extension_upgrade_parameters
         else:
             _json = self._serialize.body(extension_upgrade_parameters, "MachineExtensionUpgrade")
 
-        request = build_upgrade_extensions_request(
+        _request = build_upgrade_extensions_request(
             resource_group_name=resource_group_name,
             machine_name=machine_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._upgrade_extensions_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -98,19 +99,15 @@
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _upgrade_extensions_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/upgradeExtensions"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @overload
     async def begin_upgrade_extensions(
         self,
         resource_group_name: str,
         machine_name: str,
         extension_upgrade_parameters: _models.MachineExtensionUpgrade,
@@ -127,93 +124,66 @@
         :type machine_name: str
         :param extension_upgrade_parameters: Parameters supplied to the Upgrade Extensions operation.
          Required.
         :type extension_upgrade_parameters: ~azure.mgmt.hybridcompute.models.MachineExtensionUpgrade
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_upgrade_extensions(
         self,
         resource_group_name: str,
         machine_name: str,
-        extension_upgrade_parameters: IO,
+        extension_upgrade_parameters: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """The operation to Upgrade Machine Extensions.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param machine_name: The name of the hybrid machine. Required.
         :type machine_name: str
         :param extension_upgrade_parameters: Parameters supplied to the Upgrade Extensions operation.
          Required.
-        :type extension_upgrade_parameters: IO
+        :type extension_upgrade_parameters: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_upgrade_extensions(
         self,
         resource_group_name: str,
         machine_name: str,
-        extension_upgrade_parameters: Union[_models.MachineExtensionUpgrade, IO],
+        extension_upgrade_parameters: Union[_models.MachineExtensionUpgrade, IO[bytes]],
         **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """The operation to Upgrade Machine Extensions.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param machine_name: The name of the hybrid machine. Required.
         :type machine_name: str
         :param extension_upgrade_parameters: Parameters supplied to the Upgrade Extensions operation.
-         Is either a MachineExtensionUpgrade type or a IO type. Required.
+         Is either a MachineExtensionUpgrade type or a IO[bytes] type. Required.
         :type extension_upgrade_parameters: ~azure.mgmt.hybridcompute.models.MachineExtensionUpgrade or
-         IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+         IO[bytes]
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -235,27 +205,23 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_upgrade_extensions.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/upgradeExtensions"
-    }
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_hybrid_identity_metadata_operations.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_hybrid_compute_management_client_operations.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,221 +1,267 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
-import urllib.parse
+from io import IOBase
+from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 
-from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse
+from azure.core.pipeline.transport import HttpResponse
+from azure.core.polling import LROPoller, NoPolling, PollingMethod
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
-from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
+from azure.mgmt.core.polling.arm_polling import ARMPolling
 
-from ... import models as _models
-from ..._vendor import _convert_request
-from ...operations._hybrid_identity_metadata_operations import build_get_request, build_list_by_machines_request
-from .._vendor import HybridComputeManagementClientMixinABC
+from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import HybridComputeManagementClientMixinABC, _convert_request
 
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
 
-class HybridIdentityMetadataOperations:
-    """
-    .. warning::
-        **DO NOT** instantiate this class directly.
-
-        Instead, you should access the following operations through
-        :class:`~azure.mgmt.hybridcompute.aio.HybridComputeManagementClient`'s
-        :attr:`hybrid_identity_metadata` attribute.
-    """
-
-    models = _models
-
-    def __init__(self, *args, **kwargs) -> None:
-        input_args = list(args)
-        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
-        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
-        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
-        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
-
-    @distributed_trace_async
-    async def get(
-        self, resource_group_name: str, machine_name: str, metadata_name: str, **kwargs: Any
-    ) -> _models.HybridIdentityMetadata:
-        """Gets HybridIdentityMetadata.
 
-        Implements HybridIdentityMetadata GET method.
+def build_upgrade_extensions_request(
+    resource_group_name: str, machine_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/upgradeExtensions",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "machineName": _SERIALIZER.url(
+            "machine_name", machine_name, "str", max_length=54, min_length=1, pattern=r"^[a-zA-Z0-9-_\.]{1,54}$"
+        ),
+    }
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param machine_name: The name of the hybrid machine. Required.
-        :type machine_name: str
-        :param metadata_name: Name of the HybridIdentityMetadata. Required.
-        :type metadata_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: HybridIdentityMetadata or the result of cls(response)
-        :rtype: ~azure.mgmt.hybridcompute.models.HybridIdentityMetadata
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+class HybridComputeManagementClientOperationsMixin(  # pylint: disable=name-too-long
+    HybridComputeManagementClientMixinABC
+):
+    def _upgrade_extensions_initial(  # pylint: disable=inconsistent-return-statements
+        self,
+        resource_group_name: str,
+        machine_name: str,
+        extension_upgrade_parameters: Union[_models.MachineExtensionUpgrade, IO[bytes]],
+        **kwargs: Any
+    ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        _headers = kwargs.pop("headers", {}) or {}
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.HybridIdentityMetadata] = kwargs.pop("cls", None)
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(extension_upgrade_parameters, (IOBase, bytes)):
+            _content = extension_upgrade_parameters
+        else:
+            _json = self._serialize.body(extension_upgrade_parameters, "MachineExtensionUpgrade")
 
-        request = build_get_request(
+        _request = build_upgrade_extensions_request(
             resource_group_name=resource_group_name,
             machine_name=machine_name,
-            metadata_name=metadata_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
+            content_type=content_type,
+            json=_json,
+            content=_content,
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200]:
+        if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("HybridIdentityMetadata", pipeline_response)
+        response_headers = {}
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
-        return deserialized
+    @overload
+    def begin_upgrade_extensions(
+        self,
+        resource_group_name: str,
+        machine_name: str,
+        extension_upgrade_parameters: _models.MachineExtensionUpgrade,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> LROPoller[None]:
+        """The operation to Upgrade Machine Extensions.
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/hybridIdentityMetadata/{metadataName}"
-    }
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param machine_name: The name of the hybrid machine. Required.
+        :type machine_name: str
+        :param extension_upgrade_parameters: Parameters supplied to the Upgrade Extensions operation.
+         Required.
+        :type extension_upgrade_parameters: ~azure.mgmt.hybridcompute.models.MachineExtensionUpgrade
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: An instance of LROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[None]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
 
-    @distributed_trace
-    def list_by_machines(
-        self, resource_group_name: str, machine_name: str, **kwargs: Any
-    ) -> AsyncIterable["_models.HybridIdentityMetadata"]:
-        """Implements GET HybridIdentityMetadata in a machine.
+    @overload
+    def begin_upgrade_extensions(
+        self,
+        resource_group_name: str,
+        machine_name: str,
+        extension_upgrade_parameters: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> LROPoller[None]:
+        """The operation to Upgrade Machine Extensions.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param machine_name: The name of the hybrid machine. Required.
+        :type machine_name: str
+        :param extension_upgrade_parameters: Parameters supplied to the Upgrade Extensions operation.
+         Required.
+        :type extension_upgrade_parameters: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: An instance of LROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[None]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
 
-        Returns the list of HybridIdentityMetadata of the given machine.
+    @distributed_trace
+    def begin_upgrade_extensions(
+        self,
+        resource_group_name: str,
+        machine_name: str,
+        extension_upgrade_parameters: Union[_models.MachineExtensionUpgrade, IO[bytes]],
+        **kwargs: Any
+    ) -> LROPoller[None]:
+        """The operation to Upgrade Machine Extensions.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param machine_name: The name of the hybrid machine. Required.
         :type machine_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either HybridIdentityMetadata or the result of
-         cls(response)
-        :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.hybridcompute.models.HybridIdentityMetadata]
+        :param extension_upgrade_parameters: Parameters supplied to the Upgrade Extensions operation.
+         Is either a MachineExtensionUpgrade type or a IO[bytes] type. Required.
+        :type extension_upgrade_parameters: ~azure.mgmt.hybridcompute.models.MachineExtensionUpgrade or
+         IO[bytes]
+        :return: An instance of LROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        _headers = kwargs.pop("headers", {}) or {}
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.HybridIdentityMetadataList] = kwargs.pop("cls", None)
-
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        def prepare_request(next_link=None):
-            if not next_link:
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = self._upgrade_extensions_initial(  # type: ignore
+                resource_group_name=resource_group_name,
+                machine_name=machine_name,
+                extension_upgrade_parameters=extension_upgrade_parameters,
+                api_version=api_version,
+                content_type=content_type,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
 
-                request = build_list_by_machines_request(
-                    resource_group_name=resource_group_name,
-                    machine_name=machine_name,
-                    subscription_id=self._config.subscription_id,
-                    api_version=api_version,
-                    template_url=self.list_by_machines.metadata["url"],
-                    headers=_headers,
-                    params=_params,
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-
-            else:
-                # make call to next link with the client's api-version
-                _parsed_next_link = urllib.parse.urlparse(next_link)
-                _next_request_params = case_insensitive_dict(
-                    {
-                        key: [urllib.parse.quote(v) for v in value]
-                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
-                    }
-                )
-                _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
-                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
-
-        async def extract_data(pipeline_response):
-            deserialized = self._deserialize("HybridIdentityMetadataList", pipeline_response)
-            list_of_elem = deserialized.value
+        def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, AsyncList(list_of_elem)
+                return cls(pipeline_response, None, {})  # type: ignore
 
-        async def get_next(next_link=None):
-            request = prepare_request(next_link)
-
-            _stream = False
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+        if polling is True:
+            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
+        elif polling is False:
+            polling_method = cast(PollingMethod, NoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return LROPoller[None].from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
             )
-            response = pipeline_response.http_response
-
-            if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-            return pipeline_response
-
-        return AsyncItemPaged(get_next, extract_data)
-
-    list_by_machines.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/hybridIdentityMetadata"
-    }
+        return LROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_license_profiles_operations.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_machines_operations.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-import sys
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -28,813 +27,634 @@
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._license_profiles_operations import (
-    build_create_or_update_request,
+from ...operations._machines_operations import (
+    build_assess_patches_request,
     build_delete_request,
     build_get_request,
-    build_list_request,
-    build_update_request,
+    build_install_patches_request,
+    build_list_by_resource_group_request,
+    build_list_by_subscription_request,
 )
 from .._vendor import HybridComputeManagementClientMixinABC
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class LicenseProfilesOperations:
+class MachinesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.hybridcompute.aio.HybridComputeManagementClient`'s
-        :attr:`license_profiles` attribute.
+        :attr:`machines` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    async def _create_or_update_initial(
-        self, resource_group_name: str, machine_name: str, parameters: Union[_models.LicenseProfile, IO], **kwargs: Any
-    ) -> _models.LicenseProfile:
+    @distributed_trace_async
+    async def delete(  # pylint: disable=inconsistent-return-statements
+        self, resource_group_name: str, machine_name: str, **kwargs: Any
+    ) -> None:
+        """The operation to delete a hybrid machine.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param machine_name: The name of the hybrid machine. Required.
+        :type machine_name: str
+        :return: None or the result of cls(response)
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        license_profile_name: Literal["default"] = kwargs.pop("license_profile_name", "default")
-        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.LicenseProfile] = kwargs.pop("cls", None)
-
-        content_type = content_type or "application/json"
-        _json = None
-        _content = None
-        if isinstance(parameters, (IOBase, bytes)):
-            _content = parameters
-        else:
-            _json = self._serialize.body(parameters, "LicenseProfile")
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_create_or_update_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             machine_name=machine_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            license_profile_name=license_profile_name,
-            content_type=content_type,
-            json=_json,
-            content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 201]:
+        if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        response_headers = {}
-        if response.status_code == 200:
-            deserialized = self._deserialize("LicenseProfile", pipeline_response)
-
-        if response.status_code == 201:
-            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["Azure-AsyncOperation"] = self._deserialize(
-                "str", response.headers.get("Azure-AsyncOperation")
-            )
-
-            deserialized = self._deserialize("LicenseProfile", pipeline_response)
-
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
+            return cls(pipeline_response, None, {})  # type: ignore
 
-        return deserialized  # type: ignore
-
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/licenseProfiles/{licenseProfileName}"
-    }
-
-    @overload
-    async def begin_create_or_update(
-        self,
-        resource_group_name: str,
-        machine_name: str,
-        parameters: _models.LicenseProfile,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> AsyncLROPoller[_models.LicenseProfile]:
-        """The operation to create or update a license profile.
+    @distributed_trace_async
+    async def get(
+        self, resource_group_name: str, machine_name: str, expand: Optional[str] = None, **kwargs: Any
+    ) -> _models.Machine:
+        """Retrieves information about the model view or the instance view of a hybrid machine.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param machine_name: The name of the hybrid machine. Required.
         :type machine_name: str
-        :param parameters: Parameters supplied to the Create license profile operation. Required.
-        :type parameters: ~azure.mgmt.hybridcompute.models.LicenseProfile
-        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :keyword license_profile_name: The name of the license profile. Default value is "default".
-         Note that overriding this default value may result in unsupported behavior.
-        :paramtype license_profile_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either LicenseProfile or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.LicenseProfile]
+        :param expand: The expand expression to apply on the operation. Default value is None.
+        :type expand: str
+        :return: Machine or the result of cls(response)
+        :rtype: ~azure.mgmt.hybridcompute.models.Machine
         :raises ~azure.core.exceptions.HttpResponseError:
         """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
 
-    @overload
-    async def begin_create_or_update(
-        self,
-        resource_group_name: str,
-        machine_name: str,
-        parameters: IO,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> AsyncLROPoller[_models.LicenseProfile]:
-        """The operation to create or update a license profile.
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param machine_name: The name of the hybrid machine. Required.
-        :type machine_name: str
-        :param parameters: Parameters supplied to the Create license profile operation. Required.
-        :type parameters: IO
-        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :keyword license_profile_name: The name of the license profile. Default value is "default".
-         Note that overriding this default value may result in unsupported behavior.
-        :paramtype license_profile_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either LicenseProfile or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.LicenseProfile]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.Machine] = kwargs.pop("cls", None)
+
+        _request = build_get_request(
+            resource_group_name=resource_group_name,
+            machine_name=machine_name,
+            subscription_id=self._config.subscription_id,
+            expand=expand,
+            api_version=api_version,
+            headers=_headers,
+            params=_params,
+        )
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = self._deserialize("Machine", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+    async def _assess_patches_initial(
+        self, resource_group_name: str, name: str, **kwargs: Any
+    ) -> Optional[_models.MachineAssessPatchesResult]:
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[Optional[_models.MachineAssessPatchesResult]] = kwargs.pop("cls", None)
+
+        _request = build_assess_patches_request(
+            resource_group_name=resource_group_name,
+            name=name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            headers=_headers,
+            params=_params,
+        )
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = None
+        response_headers = {}
+        if response.status_code == 200:
+            deserialized = self._deserialize("MachineAssessPatchesResult", pipeline_response)
+
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
+        if cls:
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
+
+        return deserialized  # type: ignore
 
     @distributed_trace_async
-    async def begin_create_or_update(
-        self, resource_group_name: str, machine_name: str, parameters: Union[_models.LicenseProfile, IO], **kwargs: Any
-    ) -> AsyncLROPoller[_models.LicenseProfile]:
-        """The operation to create or update a license profile.
+    async def begin_assess_patches(
+        self, resource_group_name: str, name: str, **kwargs: Any
+    ) -> AsyncLROPoller[_models.MachineAssessPatchesResult]:
+        """The operation to assess patches on a hybrid machine identity in Azure.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
-        :param machine_name: The name of the hybrid machine. Required.
-        :type machine_name: str
-        :param parameters: Parameters supplied to the Create license profile operation. Is either a
-         LicenseProfile type or a IO type. Required.
-        :type parameters: ~azure.mgmt.hybridcompute.models.LicenseProfile or IO
-        :keyword license_profile_name: The name of the license profile. Default value is "default".
-         Note that overriding this default value may result in unsupported behavior.
-        :paramtype license_profile_name: str
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either LicenseProfile or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.LicenseProfile]
+        :param name: The name of the hybrid machine. Required.
+        :type name: str
+        :return: An instance of AsyncLROPoller that returns either MachineAssessPatchesResult or the
+         result of cls(response)
+        :rtype:
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.MachineAssessPatchesResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        license_profile_name: Literal["default"] = kwargs.pop("license_profile_name", "default")
-        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.LicenseProfile] = kwargs.pop("cls", None)
+        cls: ClsType[_models.MachineAssessPatchesResult] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._create_or_update_initial(
+            raw_result = await self._assess_patches_initial(
                 resource_group_name=resource_group_name,
-                machine_name=machine_name,
-                parameters=parameters,
+                name=name,
                 api_version=api_version,
-                license_profile_name=license_profile_name,
-                content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("LicenseProfile", pipeline_response)
+            deserialized = self._deserialize("MachineAssessPatchesResult", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.MachineAssessPatchesResult].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/licenseProfiles/{licenseProfileName}"
-    }
+        return AsyncLROPoller[_models.MachineAssessPatchesResult](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
-    async def _update_initial(
+    async def _install_patches_initial(
         self,
         resource_group_name: str,
-        machine_name: str,
-        parameters: Union[_models.LicenseProfileUpdate, IO],
+        name: str,
+        install_patches_input: Union[_models.MachineInstallPatchesParameters, IO[bytes]],
         **kwargs: Any
-    ) -> Optional[_models.LicenseProfile]:
+    ) -> Optional[_models.MachineInstallPatchesResult]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        license_profile_name: Literal["default"] = kwargs.pop("license_profile_name", "default")
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[Optional[_models.LicenseProfile]] = kwargs.pop("cls", None)
+        cls: ClsType[Optional[_models.MachineInstallPatchesResult]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
-            _content = parameters
+        if isinstance(install_patches_input, (IOBase, bytes)):
+            _content = install_patches_input
         else:
-            _json = self._serialize.body(parameters, "LicenseProfileUpdate")
+            _json = self._serialize.body(install_patches_input, "MachineInstallPatchesParameters")
 
-        request = build_update_request(
+        _request = build_install_patches_request(
             resource_group_name=resource_group_name,
-            machine_name=machine_name,
+            name=name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            license_profile_name=license_profile_name,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
-            deserialized = self._deserialize("LicenseProfile", pipeline_response)
+            deserialized = self._deserialize("MachineInstallPatchesResult", pipeline_response)
 
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["Azure-AsyncOperation"] = self._deserialize(
-                "str", response.headers.get("Azure-AsyncOperation")
-            )
 
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)
-
-        return deserialized
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
-    _update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/licenseProfiles/{licenseProfileName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
-    async def begin_update(
+    async def begin_install_patches(
         self,
         resource_group_name: str,
-        machine_name: str,
-        parameters: _models.LicenseProfileUpdate,
+        name: str,
+        install_patches_input: _models.MachineInstallPatchesParameters,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.LicenseProfile]:
-        """The operation to update a license profile.
+    ) -> AsyncLROPoller[_models.MachineInstallPatchesResult]:
+        """The operation to install patches on a hybrid machine identity in Azure.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
-        :param machine_name: The name of the hybrid machine. Required.
-        :type machine_name: str
-        :param parameters: Parameters supplied to the Update license profile operation. Required.
-        :type parameters: ~azure.mgmt.hybridcompute.models.LicenseProfileUpdate
+        :param name: The name of the hybrid machine. Required.
+        :type name: str
+        :param install_patches_input: Input for InstallPatches as directly received by the API.
+         Required.
+        :type install_patches_input: ~azure.mgmt.hybridcompute.models.MachineInstallPatchesParameters
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword license_profile_name: The name of the license profile. Default value is "default".
-         Note that overriding this default value may result in unsupported behavior.
-        :paramtype license_profile_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either LicenseProfile or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.LicenseProfile]
+        :return: An instance of AsyncLROPoller that returns either MachineInstallPatchesResult or the
+         result of cls(response)
+        :rtype:
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.MachineInstallPatchesResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    async def begin_update(
+    async def begin_install_patches(
         self,
         resource_group_name: str,
-        machine_name: str,
-        parameters: IO,
+        name: str,
+        install_patches_input: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.LicenseProfile]:
-        """The operation to update a license profile.
+    ) -> AsyncLROPoller[_models.MachineInstallPatchesResult]:
+        """The operation to install patches on a hybrid machine identity in Azure.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
-        :param machine_name: The name of the hybrid machine. Required.
-        :type machine_name: str
-        :param parameters: Parameters supplied to the Update license profile operation. Required.
-        :type parameters: IO
+        :param name: The name of the hybrid machine. Required.
+        :type name: str
+        :param install_patches_input: Input for InstallPatches as directly received by the API.
+         Required.
+        :type install_patches_input: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword license_profile_name: The name of the license profile. Default value is "default".
-         Note that overriding this default value may result in unsupported behavior.
-        :paramtype license_profile_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either LicenseProfile or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.LicenseProfile]
+        :return: An instance of AsyncLROPoller that returns either MachineInstallPatchesResult or the
+         result of cls(response)
+        :rtype:
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.MachineInstallPatchesResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
-    async def begin_update(
+    async def begin_install_patches(
         self,
         resource_group_name: str,
-        machine_name: str,
-        parameters: Union[_models.LicenseProfileUpdate, IO],
+        name: str,
+        install_patches_input: Union[_models.MachineInstallPatchesParameters, IO[bytes]],
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.LicenseProfile]:
-        """The operation to update a license profile.
+    ) -> AsyncLROPoller[_models.MachineInstallPatchesResult]:
+        """The operation to install patches on a hybrid machine identity in Azure.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
-        :param machine_name: The name of the hybrid machine. Required.
-        :type machine_name: str
-        :param parameters: Parameters supplied to the Update license profile operation. Is either a
-         LicenseProfileUpdate type or a IO type. Required.
-        :type parameters: ~azure.mgmt.hybridcompute.models.LicenseProfileUpdate or IO
-        :keyword license_profile_name: The name of the license profile. Default value is "default".
-         Note that overriding this default value may result in unsupported behavior.
-        :paramtype license_profile_name: str
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either LicenseProfile or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.LicenseProfile]
+        :param name: The name of the hybrid machine. Required.
+        :type name: str
+        :param install_patches_input: Input for InstallPatches as directly received by the API. Is
+         either a MachineInstallPatchesParameters type or a IO[bytes] type. Required.
+        :type install_patches_input: ~azure.mgmt.hybridcompute.models.MachineInstallPatchesParameters
+         or IO[bytes]
+        :return: An instance of AsyncLROPoller that returns either MachineInstallPatchesResult or the
+         result of cls(response)
+        :rtype:
+         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.MachineInstallPatchesResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        license_profile_name: Literal["default"] = kwargs.pop("license_profile_name", "default")
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.LicenseProfile] = kwargs.pop("cls", None)
+        cls: ClsType[_models.MachineInstallPatchesResult] = kwargs.pop("cls", None)
         polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._update_initial(
+            raw_result = await self._install_patches_initial(
                 resource_group_name=resource_group_name,
-                machine_name=machine_name,
-                parameters=parameters,
+                name=name,
+                install_patches_input=install_patches_input,
                 api_version=api_version,
-                license_profile_name=license_profile_name,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("LicenseProfile", pipeline_response)
+            deserialized = self._deserialize("MachineInstallPatchesResult", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.MachineInstallPatchesResult].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/licenseProfiles/{licenseProfileName}"
-    }
+        return AsyncLROPoller[_models.MachineInstallPatchesResult](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
-    @distributed_trace_async
-    async def get(self, resource_group_name: str, machine_name: str, **kwargs: Any) -> _models.LicenseProfile:
-        """Retrieves information about the view of a license profile.
+    @distributed_trace
+    def list_by_resource_group(
+        self, resource_group_name: str, expand: Optional[str] = None, **kwargs: Any
+    ) -> AsyncIterable["_models.Machine"]:
+        """Lists all the hybrid machines in the specified resource group. Use the nextLink property in the
+        response to get the next page of hybrid machines.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param machine_name: The name of the hybrid machine. Required.
-        :type machine_name: str
-        :keyword license_profile_name: The name of the license profile. Default value is "default".
-         Note that overriding this default value may result in unsupported behavior.
-        :paramtype license_profile_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: LicenseProfile or the result of cls(response)
-        :rtype: ~azure.mgmt.hybridcompute.models.LicenseProfile
+        :param expand: Expands referenced resources. Default value is None.
+        :type expand: str
+        :return: An iterator like instance of either Machine or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.hybridcompute.models.Machine]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        license_profile_name: Literal["default"] = kwargs.pop("license_profile_name", "default")
-        cls: ClsType[_models.LicenseProfile] = kwargs.pop("cls", None)
-
-        request = build_get_request(
-            resource_group_name=resource_group_name,
-            machine_name=machine_name,
-            subscription_id=self._config.subscription_id,
-            api_version=api_version,
-            license_profile_name=license_profile_name,
-            template_url=self.get.metadata["url"],
-            headers=_headers,
-            params=_params,
-        )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
-
-        _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-        deserialized = self._deserialize("LicenseProfile", pipeline_response)
-
-        if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+        cls: ClsType[_models.MachineListResult] = kwargs.pop("cls", None)
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/licenseProfiles/{licenseProfileName}"
-    }
-
-    async def _delete_initial(  # pylint: disable=inconsistent-return-statements
-        self, resource_group_name: str, machine_name: str, **kwargs: Any
-    ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        license_profile_name: Literal["default"] = kwargs.pop("license_profile_name", "default")
-        cls: ClsType[None] = kwargs.pop("cls", None)
-
-        request = build_delete_request(
-            resource_group_name=resource_group_name,
-            machine_name=machine_name,
-            subscription_id=self._config.subscription_id,
-            api_version=api_version,
-            license_profile_name=license_profile_name,
-            template_url=self._delete_initial.metadata["url"],
-            headers=_headers,
-            params=_params,
-        )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
-
-        _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [202, 204]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-        response_headers = {}
-        if response.status_code == 202:
-            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["Azure-AsyncOperation"] = self._deserialize(
-                "str", response.headers.get("Azure-AsyncOperation")
-            )
+        def prepare_request(next_link=None):
+            if not next_link:
 
-        if cls:
-            return cls(pipeline_response, None, response_headers)
+                _request = build_list_by_resource_group_request(
+                    resource_group_name=resource_group_name,
+                    subscription_id=self._config.subscription_id,
+                    expand=expand,
+                    api_version=api_version,
+                    headers=_headers,
+                    params=_params,
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/licenseProfiles/{licenseProfileName}"
-    }
+            else:
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                _request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
-    @distributed_trace_async
-    async def begin_delete(self, resource_group_name: str, machine_name: str, **kwargs: Any) -> AsyncLROPoller[None]:
-        """The operation to delete a license profile.
+        async def extract_data(pipeline_response):
+            deserialized = self._deserialize("MachineListResult", pipeline_response)
+            list_of_elem = deserialized.value
+            if cls:
+                list_of_elem = cls(list_of_elem)  # type: ignore
+            return deserialized.next_link or None, AsyncList(list_of_elem)
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param machine_name: The name of the hybrid machine. Required.
-        :type machine_name: str
-        :keyword license_profile_name: The name of the license profile. Default value is "default".
-         Note that overriding this default value may result in unsupported behavior.
-        :paramtype license_profile_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[None]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+        async def get_next(next_link=None):
+            _request = prepare_request(next_link)
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        license_profile_name: Literal["default"] = kwargs.pop("license_profile_name", "default")
-        cls: ClsType[None] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
-        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
-        if cont_token is None:
-            raw_result = await self._delete_initial(  # type: ignore
-                resource_group_name=resource_group_name,
-                machine_name=machine_name,
-                api_version=api_version,
-                license_profile_name=license_profile_name,
-                cls=lambda x, y, z: x,
-                headers=_headers,
-                params=_params,
-                **kwargs
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
             )
-        kwargs.pop("error_map", None)
+            response = pipeline_response.http_response
 
-        def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
-            if cls:
-                return cls(pipeline_response, None, {})
+            if response.status_code not in [200]:
+                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        if polling is True:
-            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
-        elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
-        else:
-            polling_method = polling
-        if cont_token:
-            return AsyncLROPoller.from_continuation_token(
-                polling_method=polling_method,
-                continuation_token=cont_token,
-                client=self._client,
-                deserialization_callback=get_long_running_output,
-            )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+            return pipeline_response
 
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/licenseProfiles/{licenseProfileName}"
-    }
+        return AsyncItemPaged(get_next, extract_data)
 
     @distributed_trace
-    def list(
-        self, resource_group_name: str, machine_name: str, **kwargs: Any
-    ) -> AsyncIterable["_models.LicenseProfile"]:
-        """The operation to get all license profiles of a non-Azure machine.
+    def list_by_subscription(self, **kwargs: Any) -> AsyncIterable["_models.Machine"]:
+        """Lists all the hybrid machines in the specified subscription. Use the nextLink property in the
+        response to get the next page of hybrid machines.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param machine_name: The name of the machine. Required.
-        :type machine_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either LicenseProfile or the result of cls(response)
-        :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.hybridcompute.models.LicenseProfile]
+        :return: An iterator like instance of either Machine or the result of cls(response)
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.hybridcompute.models.Machine]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.LicenseProfilesListResult] = kwargs.pop("cls", None)
+        cls: ClsType[_models.MachineListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
-                    resource_group_name=resource_group_name,
-                    machine_name=machine_name,
+                _request = build_list_by_subscription_request(
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize("LicenseProfilesListResult", pipeline_response)
+            deserialized = self._deserialize("MachineListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
-
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/licenseProfiles"
-    }
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_machine_extensions_operations.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_machines_operations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,844 +1,849 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
-from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
+from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse
-from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
+from azure.core.pipeline.transport import HttpResponse
+from azure.core.polling import LROPoller, NoPolling, PollingMethod
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
-from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
-from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
+from azure.mgmt.core.polling.arm_polling import ARMPolling
 
-from ... import models as _models
-from ..._vendor import _convert_request
-from ...operations._machine_extensions_operations import (
-    build_create_or_update_request,
-    build_delete_request,
-    build_get_request,
-    build_list_request,
-    build_update_request,
-)
-from .._vendor import HybridComputeManagementClientMixinABC
+from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import HybridComputeManagementClientMixinABC, _convert_request
 
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
+
+
+def build_delete_request(
+    resource_group_name: str, machine_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "machineName": _SERIALIZER.url(
+            "machine_name", machine_name, "str", max_length=54, min_length=1, pattern=r"^[a-zA-Z0-9-_\.]{1,54}$"
+        ),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_get_request(
+    resource_group_name: str, machine_name: str, subscription_id: str, *, expand: Optional[str] = None, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "machineName": _SERIALIZER.url(
+            "machine_name", machine_name, "str", max_length=54, min_length=1, pattern=r"^[a-zA-Z0-9-_\.]{1,54}$"
+        ),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+    if expand is not None:
+        _params["$expand"] = _SERIALIZER.query("expand", expand, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_assess_patches_request(
+    resource_group_name: str, name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{name}/assessPatches",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "name": _SERIALIZER.url("name", name, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_install_patches_request(
+    resource_group_name: str, name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{name}/installPatches",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+        "name": _SERIALIZER.url("name", name, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_list_by_resource_group_request(
+    resource_group_name: str, subscription_id: str, *, expand: Optional[str] = None, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+    if expand is not None:
+        _params["$expand"] = _SERIALIZER.query("expand", expand, "str")
 
-class MachineExtensionsOperations:
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_list_by_subscription_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.HybridCompute/machines")
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+class MachinesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.hybridcompute.aio.HybridComputeManagementClient`'s
-        :attr:`machine_extensions` attribute.
+        :class:`~azure.mgmt.hybridcompute.HybridComputeManagementClient`'s
+        :attr:`machines` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    async def _create_or_update_initial(
-        self,
-        resource_group_name: str,
-        machine_name: str,
-        extension_name: str,
-        extension_parameters: Union[_models.MachineExtension, IO],
-        **kwargs: Any
-    ) -> Optional[_models.MachineExtension]:
+    @distributed_trace
+    def delete(  # pylint: disable=inconsistent-return-statements
+        self, resource_group_name: str, machine_name: str, **kwargs: Any
+    ) -> None:
+        """The operation to delete a hybrid machine.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param machine_name: The name of the hybrid machine. Required.
+        :type machine_name: str
+        :return: None or the result of cls(response)
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[Optional[_models.MachineExtension]] = kwargs.pop("cls", None)
-
-        content_type = content_type or "application/json"
-        _json = None
-        _content = None
-        if isinstance(extension_parameters, (IOBase, bytes)):
-            _content = extension_parameters
-        else:
-            _json = self._serialize.body(extension_parameters, "MachineExtension")
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_create_or_update_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             machine_name=machine_name,
-            extension_name=extension_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            content_type=content_type,
-            json=_json,
-            content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 202]:
+        if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = None
-        if response.status_code == 200:
-            deserialized = self._deserialize("MachineExtension", pipeline_response)
-
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, None, {})  # type: ignore
 
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/extensions/{extensionName}"
-    }
-
-    @overload
-    async def begin_create_or_update(
-        self,
-        resource_group_name: str,
-        machine_name: str,
-        extension_name: str,
-        extension_parameters: _models.MachineExtension,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> AsyncLROPoller[_models.MachineExtension]:
-        """The operation to create or update the extension.
+    @distributed_trace
+    def get(
+        self, resource_group_name: str, machine_name: str, expand: Optional[str] = None, **kwargs: Any
+    ) -> _models.Machine:
+        """Retrieves information about the model view or the instance view of a hybrid machine.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param machine_name: The name of the machine where the extension should be created or updated.
-         Required.
+        :param machine_name: The name of the hybrid machine. Required.
         :type machine_name: str
-        :param extension_name: The name of the machine extension. Required.
-        :type extension_name: str
-        :param extension_parameters: Parameters supplied to the Create Machine Extension operation.
-         Required.
-        :type extension_parameters: ~azure.mgmt.hybridcompute.models.MachineExtension
-        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either MachineExtension or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.MachineExtension]
+        :param expand: The expand expression to apply on the operation. Default value is None.
+        :type expand: str
+        :return: Machine or the result of cls(response)
+        :rtype: ~azure.mgmt.hybridcompute.models.Machine
         :raises ~azure.core.exceptions.HttpResponseError:
         """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
 
-    @overload
-    async def begin_create_or_update(
-        self,
-        resource_group_name: str,
-        machine_name: str,
-        extension_name: str,
-        extension_parameters: IO,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> AsyncLROPoller[_models.MachineExtension]:
-        """The operation to create or update the extension.
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param machine_name: The name of the machine where the extension should be created or updated.
-         Required.
-        :type machine_name: str
-        :param extension_name: The name of the machine extension. Required.
-        :type extension_name: str
-        :param extension_parameters: Parameters supplied to the Create Machine Extension operation.
-         Required.
-        :type extension_parameters: IO
-        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either MachineExtension or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.MachineExtension]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.Machine] = kwargs.pop("cls", None)
 
-    @distributed_trace_async
-    async def begin_create_or_update(
-        self,
-        resource_group_name: str,
-        machine_name: str,
-        extension_name: str,
-        extension_parameters: Union[_models.MachineExtension, IO],
-        **kwargs: Any
-    ) -> AsyncLROPoller[_models.MachineExtension]:
-        """The operation to create or update the extension.
+        _request = build_get_request(
+            resource_group_name=resource_group_name,
+            machine_name=machine_name,
+            subscription_id=self._config.subscription_id,
+            expand=expand,
+            api_version=api_version,
+            headers=_headers,
+            params=_params,
+        )
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = self._deserialize("Machine", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
+
+    def _assess_patches_initial(
+        self, resource_group_name: str, name: str, **kwargs: Any
+    ) -> Optional[_models.MachineAssessPatchesResult]:
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[Optional[_models.MachineAssessPatchesResult]] = kwargs.pop("cls", None)
+
+        _request = build_assess_patches_request(
+            resource_group_name=resource_group_name,
+            name=name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            headers=_headers,
+            params=_params,
+        )
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = None
+        response_headers = {}
+        if response.status_code == 200:
+            deserialized = self._deserialize("MachineAssessPatchesResult", pipeline_response)
+
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+
+        if cls:
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @distributed_trace
+    def begin_assess_patches(
+        self, resource_group_name: str, name: str, **kwargs: Any
+    ) -> LROPoller[_models.MachineAssessPatchesResult]:
+        """The operation to assess patches on a hybrid machine identity in Azure.
+
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
-        :param machine_name: The name of the machine where the extension should be created or updated.
-         Required.
-        :type machine_name: str
-        :param extension_name: The name of the machine extension. Required.
-        :type extension_name: str
-        :param extension_parameters: Parameters supplied to the Create Machine Extension operation. Is
-         either a MachineExtension type or a IO type. Required.
-        :type extension_parameters: ~azure.mgmt.hybridcompute.models.MachineExtension or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either MachineExtension or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.MachineExtension]
+        :param name: The name of the hybrid machine. Required.
+        :type name: str
+        :return: An instance of LROPoller that returns either MachineAssessPatchesResult or the result
+         of cls(response)
+        :rtype:
+         ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.MachineAssessPatchesResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.MachineExtension] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        cls: ClsType[_models.MachineAssessPatchesResult] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._create_or_update_initial(
+            raw_result = self._assess_patches_initial(
                 resource_group_name=resource_group_name,
-                machine_name=machine_name,
-                extension_name=extension_name,
-                extension_parameters=extension_parameters,
+                name=name,
                 api_version=api_version,
-                content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("MachineExtension", pipeline_response)
+            deserialized = self._deserialize("MachineAssessPatchesResult", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+            polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return LROPoller[_models.MachineAssessPatchesResult].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/extensions/{extensionName}"
-    }
+        return LROPoller[_models.MachineAssessPatchesResult](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
-    async def _update_initial(
+    def _install_patches_initial(
         self,
         resource_group_name: str,
-        machine_name: str,
-        extension_name: str,
-        extension_parameters: Union[_models.MachineExtensionUpdate, IO],
+        name: str,
+        install_patches_input: Union[_models.MachineInstallPatchesParameters, IO[bytes]],
         **kwargs: Any
-    ) -> Optional[_models.MachineExtension]:
+    ) -> Optional[_models.MachineInstallPatchesResult]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[Optional[_models.MachineExtension]] = kwargs.pop("cls", None)
+        cls: ClsType[Optional[_models.MachineInstallPatchesResult]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(extension_parameters, (IOBase, bytes)):
-            _content = extension_parameters
+        if isinstance(install_patches_input, (IOBase, bytes)):
+            _content = install_patches_input
         else:
-            _json = self._serialize.body(extension_parameters, "MachineExtensionUpdate")
+            _json = self._serialize.body(install_patches_input, "MachineInstallPatchesParameters")
 
-        request = build_update_request(
+        _request = build_install_patches_request(
             resource_group_name=resource_group_name,
-            machine_name=machine_name,
-            extension_name=extension_name,
+            name=name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
-            deserialized = self._deserialize("MachineExtension", pipeline_response)
+            deserialized = self._deserialize("MachineInstallPatchesResult", pipeline_response)
 
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["Azure-AsyncOperation"] = self._deserialize(
-                "str", response.headers.get("Azure-AsyncOperation")
-            )
 
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)
-
-        return deserialized
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
-    _update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/extensions/{extensionName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
-    async def begin_update(
+    def begin_install_patches(
         self,
         resource_group_name: str,
-        machine_name: str,
-        extension_name: str,
-        extension_parameters: _models.MachineExtensionUpdate,
+        name: str,
+        install_patches_input: _models.MachineInstallPatchesParameters,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.MachineExtension]:
-        """The operation to create or update the extension.
+    ) -> LROPoller[_models.MachineInstallPatchesResult]:
+        """The operation to install patches on a hybrid machine identity in Azure.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
-        :param machine_name: The name of the machine where the extension should be created or updated.
+        :param name: The name of the hybrid machine. Required.
+        :type name: str
+        :param install_patches_input: Input for InstallPatches as directly received by the API.
          Required.
-        :type machine_name: str
-        :param extension_name: The name of the machine extension. Required.
-        :type extension_name: str
-        :param extension_parameters: Parameters supplied to the Create Machine Extension operation.
-         Required.
-        :type extension_parameters: ~azure.mgmt.hybridcompute.models.MachineExtensionUpdate
+        :type install_patches_input: ~azure.mgmt.hybridcompute.models.MachineInstallPatchesParameters
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either MachineExtension or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.MachineExtension]
+        :return: An instance of LROPoller that returns either MachineInstallPatchesResult or the result
+         of cls(response)
+        :rtype:
+         ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.MachineInstallPatchesResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    async def begin_update(
+    def begin_install_patches(
         self,
         resource_group_name: str,
-        machine_name: str,
-        extension_name: str,
-        extension_parameters: IO,
+        name: str,
+        install_patches_input: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.MachineExtension]:
-        """The operation to create or update the extension.
+    ) -> LROPoller[_models.MachineInstallPatchesResult]:
+        """The operation to install patches on a hybrid machine identity in Azure.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
-        :param machine_name: The name of the machine where the extension should be created or updated.
+        :param name: The name of the hybrid machine. Required.
+        :type name: str
+        :param install_patches_input: Input for InstallPatches as directly received by the API.
          Required.
-        :type machine_name: str
-        :param extension_name: The name of the machine extension. Required.
-        :type extension_name: str
-        :param extension_parameters: Parameters supplied to the Create Machine Extension operation.
-         Required.
-        :type extension_parameters: IO
+        :type install_patches_input: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either MachineExtension or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.MachineExtension]
+        :return: An instance of LROPoller that returns either MachineInstallPatchesResult or the result
+         of cls(response)
+        :rtype:
+         ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.MachineInstallPatchesResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
-    @distributed_trace_async
-    async def begin_update(
+    @distributed_trace
+    def begin_install_patches(
         self,
         resource_group_name: str,
-        machine_name: str,
-        extension_name: str,
-        extension_parameters: Union[_models.MachineExtensionUpdate, IO],
+        name: str,
+        install_patches_input: Union[_models.MachineInstallPatchesParameters, IO[bytes]],
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.MachineExtension]:
-        """The operation to create or update the extension.
+    ) -> LROPoller[_models.MachineInstallPatchesResult]:
+        """The operation to install patches on a hybrid machine identity in Azure.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
+        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
-        :param machine_name: The name of the machine where the extension should be created or updated.
-         Required.
-        :type machine_name: str
-        :param extension_name: The name of the machine extension. Required.
-        :type extension_name: str
-        :param extension_parameters: Parameters supplied to the Create Machine Extension operation. Is
-         either a MachineExtensionUpdate type or a IO type. Required.
-        :type extension_parameters: ~azure.mgmt.hybridcompute.models.MachineExtensionUpdate or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either MachineExtension or the result of
-         cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.MachineExtension]
+        :param name: The name of the hybrid machine. Required.
+        :type name: str
+        :param install_patches_input: Input for InstallPatches as directly received by the API. Is
+         either a MachineInstallPatchesParameters type or a IO[bytes] type. Required.
+        :type install_patches_input: ~azure.mgmt.hybridcompute.models.MachineInstallPatchesParameters
+         or IO[bytes]
+        :return: An instance of LROPoller that returns either MachineInstallPatchesResult or the result
+         of cls(response)
+        :rtype:
+         ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.MachineInstallPatchesResult]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.MachineExtension] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        cls: ClsType[_models.MachineInstallPatchesResult] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._update_initial(
+            raw_result = self._install_patches_initial(
                 resource_group_name=resource_group_name,
-                machine_name=machine_name,
-                extension_name=extension_name,
-                extension_parameters=extension_parameters,
+                name=name,
+                install_patches_input=install_patches_input,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("MachineExtension", pipeline_response)
+            deserialized = self._deserialize("MachineInstallPatchesResult", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            )
         elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+            polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return LROPoller[_models.MachineInstallPatchesResult].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/extensions/{extensionName}"
-    }
-
-    async def _delete_initial(  # pylint: disable=inconsistent-return-statements
-        self, resource_group_name: str, machine_name: str, extension_name: str, **kwargs: Any
-    ) -> None:
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[None] = kwargs.pop("cls", None)
-
-        request = build_delete_request(
-            resource_group_name=resource_group_name,
-            machine_name=machine_name,
-            extension_name=extension_name,
-            subscription_id=self._config.subscription_id,
-            api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
-            headers=_headers,
-            params=_params,
-        )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
-
-        _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        return LROPoller[_models.MachineInstallPatchesResult](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
         )
 
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200, 202, 204]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-        response_headers = {}
-        if response.status_code == 202:
-            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["Azure-AsyncOperation"] = self._deserialize(
-                "str", response.headers.get("Azure-AsyncOperation")
-            )
-
-        if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/extensions/{extensionName}"
-    }
-
-    @distributed_trace_async
-    async def begin_delete(
-        self, resource_group_name: str, machine_name: str, extension_name: str, **kwargs: Any
-    ) -> AsyncLROPoller[None]:
-        """The operation to delete the extension.
+    @distributed_trace
+    def list_by_resource_group(
+        self, resource_group_name: str, expand: Optional[str] = None, **kwargs: Any
+    ) -> Iterable["_models.Machine"]:
+        """Lists all the hybrid machines in the specified resource group. Use the nextLink property in the
+        response to get the next page of hybrid machines.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param machine_name: The name of the machine where the extension should be deleted. Required.
-        :type machine_name: str
-        :param extension_name: The name of the machine extension. Required.
-        :type extension_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[None]
+        :param expand: Expands referenced resources. Default value is None.
+        :type expand: str
+        :return: An iterator like instance of either Machine or the result of cls(response)
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.hybridcompute.models.Machine]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[None] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
-        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
-        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
-        if cont_token is None:
-            raw_result = await self._delete_initial(  # type: ignore
-                resource_group_name=resource_group_name,
-                machine_name=machine_name,
-                extension_name=extension_name,
-                api_version=api_version,
-                cls=lambda x, y, z: x,
-                headers=_headers,
-                params=_params,
-                **kwargs
-            )
-        kwargs.pop("error_map", None)
-
-        def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
-            if cls:
-                return cls(pipeline_response, None, {})
-
-        if polling is True:
-            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
-        elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
-        else:
-            polling_method = polling
-        if cont_token:
-            return AsyncLROPoller.from_continuation_token(
-                polling_method=polling_method,
-                continuation_token=cont_token,
-                client=self._client,
-                deserialization_callback=get_long_running_output,
-            )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/extensions/{extensionName}"
-    }
+        cls: ClsType[_models.MachineListResult] = kwargs.pop("cls", None)
 
-    @distributed_trace_async
-    async def get(
-        self, resource_group_name: str, machine_name: str, extension_name: str, **kwargs: Any
-    ) -> _models.MachineExtension:
-        """The operation to get the extension.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param machine_name: The name of the machine containing the extension. Required.
-        :type machine_name: str
-        :param extension_name: The name of the machine extension. Required.
-        :type extension_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: MachineExtension or the result of cls(response)
-        :rtype: ~azure.mgmt.hybridcompute.models.MachineExtension
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.MachineExtension] = kwargs.pop("cls", None)
+        def prepare_request(next_link=None):
+            if not next_link:
 
-        request = build_get_request(
-            resource_group_name=resource_group_name,
-            machine_name=machine_name,
-            extension_name=extension_name,
-            subscription_id=self._config.subscription_id,
-            api_version=api_version,
-            template_url=self.get.metadata["url"],
-            headers=_headers,
-            params=_params,
-        )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+                _request = build_list_by_resource_group_request(
+                    resource_group_name=resource_group_name,
+                    subscription_id=self._config.subscription_id,
+                    expand=expand,
+                    api_version=api_version,
+                    headers=_headers,
+                    params=_params,
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
-        _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
-        )
+            else:
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                _request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
-        response = pipeline_response.http_response
+        def extract_data(pipeline_response):
+            deserialized = self._deserialize("MachineListResult", pipeline_response)
+            list_of_elem = deserialized.value
+            if cls:
+                list_of_elem = cls(list_of_elem)  # type: ignore
+            return deserialized.next_link or None, iter(list_of_elem)
 
-        if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+        def get_next(next_link=None):
+            _request = prepare_request(next_link)
 
-        deserialized = self._deserialize("MachineExtension", pipeline_response)
+            _stream = False
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+            response = pipeline_response.http_response
 
-        if cls:
-            return cls(pipeline_response, deserialized, {})
+            if response.status_code not in [200]:
+                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        return deserialized
+            return pipeline_response
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/extensions/{extensionName}"
-    }
+        return ItemPaged(get_next, extract_data)
 
     @distributed_trace
-    def list(
-        self, resource_group_name: str, machine_name: str, expand: Optional[str] = None, **kwargs: Any
-    ) -> AsyncIterable["_models.MachineExtension"]:
-        """The operation to get all extensions of a non-Azure machine.
+    def list_by_subscription(self, **kwargs: Any) -> Iterable["_models.Machine"]:
+        """Lists all the hybrid machines in the specified subscription. Use the nextLink property in the
+        response to get the next page of hybrid machines.
 
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param machine_name: The name of the machine containing the extension. Required.
-        :type machine_name: str
-        :param expand: The expand expression to apply on the operation. Default value is None.
-        :type expand: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either MachineExtension or the result of cls(response)
-        :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.hybridcompute.models.MachineExtension]
+        :return: An iterator like instance of either Machine or the result of cls(response)
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.hybridcompute.models.Machine]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.MachineExtensionsListResult] = kwargs.pop("cls", None)
+        cls: ClsType[_models.MachineListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
-                    resource_group_name=resource_group_name,
-                    machine_name=machine_name,
+                _request = build_list_by_subscription_request(
                     subscription_id=self._config.subscription_id,
-                    expand=expand,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
-        async def extract_data(pipeline_response):
-            deserialized = self._deserialize("MachineExtensionsListResult", pipeline_response)
+        def extract_data(pipeline_response):
+            deserialized = self._deserialize("MachineListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, AsyncList(list_of_elem)
+            return deserialized.next_link or None, iter(list_of_elem)
 
-        async def get_next(next_link=None):
-            request = prepare_request(next_link)
+        def get_next(next_link=None):
+            _request = prepare_request(next_link)
 
             _stream = False
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return AsyncItemPaged(get_next, extract_data)
-
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/extensions"
-    }
+        return ItemPaged(get_next, extract_data)
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_machines_operations.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_machine_run_commands_operations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,738 +1,674 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
-from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
+from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse
-from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
+from azure.core.pipeline.transport import HttpResponse
+from azure.core.polling import LROPoller, NoPolling, PollingMethod
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
-from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
-from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
+from azure.mgmt.core.polling.arm_polling import ARMPolling
 
-from ... import models as _models
-from ..._vendor import _convert_request
-from ...operations._machines_operations import (
-    build_assess_patches_request,
-    build_delete_request,
-    build_get_request,
-    build_install_patches_request,
-    build_list_by_resource_group_request,
-    build_list_by_subscription_request,
-)
-from .._vendor import HybridComputeManagementClientMixinABC
+from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import HybridComputeManagementClientMixinABC, _convert_request
 
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
+
+
+def build_create_or_update_request(
+    resource_group_name: str, machine_name: str, run_command_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/runCommands/{runCommandName}",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "machineName": _SERIALIZER.url("machine_name", machine_name, "str", pattern=r"[a-zA-Z0-9-_\.]+"),
+        "runCommandName": _SERIALIZER.url("run_command_name", run_command_name, "str", pattern=r"[a-zA-Z0-9-_\.]+"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_delete_request(
+    resource_group_name: str, machine_name: str, run_command_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/runCommands/{runCommandName}",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "machineName": _SERIALIZER.url("machine_name", machine_name, "str", pattern=r"[a-zA-Z0-9-_\.]+"),
+        "runCommandName": _SERIALIZER.url("run_command_name", run_command_name, "str", pattern=r"[a-zA-Z0-9-_\.]+"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_get_request(
+    resource_group_name: str, machine_name: str, run_command_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/runCommands/{runCommandName}",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "machineName": _SERIALIZER.url("machine_name", machine_name, "str", pattern=r"[a-zA-Z0-9-_\.]+"),
+        "runCommandName": _SERIALIZER.url("run_command_name", run_command_name, "str", pattern=r"[a-zA-Z0-9-_\.]+"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_list_request(
+    resource_group_name: str, machine_name: str, subscription_id: str, *, expand: Optional[str] = None, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/runCommands",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "machineName": _SERIALIZER.url("machine_name", machine_name, "str", pattern=r"[a-zA-Z0-9-_\.]+"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
+    # Construct parameters
+    if expand is not None:
+        _params["$expand"] = _SERIALIZER.query("expand", expand, "str")
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
-class MachinesOperations:
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+class MachineRunCommandsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.hybridcompute.aio.HybridComputeManagementClient`'s
-        :attr:`machines` attribute.
+        :class:`~azure.mgmt.hybridcompute.HybridComputeManagementClient`'s
+        :attr:`machine_run_commands` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    @distributed_trace_async
-    async def delete(  # pylint: disable=inconsistent-return-statements
-        self, resource_group_name: str, machine_name: str, **kwargs: Any
-    ) -> None:
-        """The operation to delete a hybrid machine.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param machine_name: The name of the hybrid machine. Required.
-        :type machine_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: None or the result of cls(response)
-        :rtype: None
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
+    def _create_or_update_initial(
+        self,
+        resource_group_name: str,
+        machine_name: str,
+        run_command_name: str,
+        run_command_properties: Union[_models.MachineRunCommand, IO[bytes]],
+        **kwargs: Any
+    ) -> _models.MachineRunCommand:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        _headers = kwargs.pop("headers", {}) or {}
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[None] = kwargs.pop("cls", None)
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.MachineRunCommand] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(run_command_properties, (IOBase, bytes)):
+            _content = run_command_properties
+        else:
+            _json = self._serialize.body(run_command_properties, "MachineRunCommand")
 
-        request = build_delete_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             machine_name=machine_name,
+            run_command_name=run_command_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.delete.metadata["url"],
+            content_type=content_type,
+            json=_json,
+            content=_content,
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 204]:
+        if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
+        response_headers = {}
+        if response.status_code == 200:
+            deserialized = self._deserialize("MachineRunCommand", pipeline_response)
+
+        if response.status_code == 201:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
+            deserialized = self._deserialize("MachineRunCommand", pipeline_response)
+
         if cls:
-            return cls(pipeline_response, None, {})
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
-    delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}"
-    }
+        return deserialized  # type: ignore
 
-    @distributed_trace_async
-    async def get(
+    @overload
+    def begin_create_or_update(
         self,
         resource_group_name: str,
         machine_name: str,
-        expand: Optional[Union[str, _models.InstanceViewTypes]] = None,
+        run_command_name: str,
+        run_command_properties: _models.MachineRunCommand,
+        *,
+        content_type: str = "application/json",
         **kwargs: Any
-    ) -> _models.Machine:
-        """Retrieves information about the model view or the instance view of a hybrid machine.
+    ) -> LROPoller[_models.MachineRunCommand]:
+        """The operation to create or update a run command.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param machine_name: The name of the hybrid machine. Required.
         :type machine_name: str
-        :param expand: The expand expression to apply on the operation. "instanceView" Default value is
-         None.
-        :type expand: str or ~azure.mgmt.hybridcompute.models.InstanceViewTypes
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: Machine or the result of cls(response)
-        :rtype: ~azure.mgmt.hybridcompute.models.Machine
+        :param run_command_name: The name of the run command. Required.
+        :type run_command_name: str
+        :param run_command_properties: Parameters supplied to the Create Run Command. Required.
+        :type run_command_properties: ~azure.mgmt.hybridcompute.models.MachineRunCommand
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: An instance of LROPoller that returns either MachineRunCommand or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.MachineRunCommand]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
 
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.Machine] = kwargs.pop("cls", None)
-
-        request = build_get_request(
-            resource_group_name=resource_group_name,
-            machine_name=machine_name,
-            subscription_id=self._config.subscription_id,
-            expand=expand,
-            api_version=api_version,
-            template_url=self.get.metadata["url"],
-            headers=_headers,
-            params=_params,
-        )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
-
-        _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-        deserialized = self._deserialize("Machine", pipeline_response)
-
-        if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
-
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}"
-    }
-
-    async def _assess_patches_initial(
-        self, resource_group_name: str, name: str, **kwargs: Any
-    ) -> Optional[_models.MachineAssessPatchesResult]:
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[Optional[_models.MachineAssessPatchesResult]] = kwargs.pop("cls", None)
-
-        request = build_assess_patches_request(
-            resource_group_name=resource_group_name,
-            name=name,
-            subscription_id=self._config.subscription_id,
-            api_version=api_version,
-            template_url=self._assess_patches_initial.metadata["url"],
-            headers=_headers,
-            params=_params,
-        )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
-
-        _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200, 202]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-        deserialized = None
-        response_headers = {}
-        if response.status_code == 200:
-            deserialized = self._deserialize("MachineAssessPatchesResult", pipeline_response)
-
-        if response.status_code == 202:
-            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
-
-        if cls:
-            return cls(pipeline_response, deserialized, response_headers)
-
-        return deserialized
+    @overload
+    def begin_create_or_update(
+        self,
+        resource_group_name: str,
+        machine_name: str,
+        run_command_name: str,
+        run_command_properties: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> LROPoller[_models.MachineRunCommand]:
+        """The operation to create or update a run command.
 
-    _assess_patches_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{name}/assessPatches"
-    }
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param machine_name: The name of the hybrid machine. Required.
+        :type machine_name: str
+        :param run_command_name: The name of the run command. Required.
+        :type run_command_name: str
+        :param run_command_properties: Parameters supplied to the Create Run Command. Required.
+        :type run_command_properties: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: An instance of LROPoller that returns either MachineRunCommand or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.MachineRunCommand]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
 
-    @distributed_trace_async
-    async def begin_assess_patches(
-        self, resource_group_name: str, name: str, **kwargs: Any
-    ) -> AsyncLROPoller[_models.MachineAssessPatchesResult]:
-        """The operation to assess patches on a hybrid machine identity in Azure.
+    @distributed_trace
+    def begin_create_or_update(
+        self,
+        resource_group_name: str,
+        machine_name: str,
+        run_command_name: str,
+        run_command_properties: Union[_models.MachineRunCommand, IO[bytes]],
+        **kwargs: Any
+    ) -> LROPoller[_models.MachineRunCommand]:
+        """The operation to create or update a run command.
 
-        :param resource_group_name: The name of the resource group. Required.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
         :type resource_group_name: str
-        :param name: The name of the hybrid machine. Required.
-        :type name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either MachineAssessPatchesResult or the
-         result of cls(response)
-        :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.MachineAssessPatchesResult]
+        :param machine_name: The name of the hybrid machine. Required.
+        :type machine_name: str
+        :param run_command_name: The name of the run command. Required.
+        :type run_command_name: str
+        :param run_command_properties: Parameters supplied to the Create Run Command. Is either a
+         MachineRunCommand type or a IO[bytes] type. Required.
+        :type run_command_properties: ~azure.mgmt.hybridcompute.models.MachineRunCommand or IO[bytes]
+        :return: An instance of LROPoller that returns either MachineRunCommand or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.MachineRunCommand]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        _headers = kwargs.pop("headers", {}) or {}
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.MachineAssessPatchesResult] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.MachineRunCommand] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._assess_patches_initial(
+            raw_result = self._create_or_update_initial(
                 resource_group_name=resource_group_name,
-                name=name,
+                machine_name=machine_name,
+                run_command_name=run_command_name,
+                run_command_properties=run_command_properties,
                 api_version=api_version,
+                content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("MachineAssessPatchesResult", pipeline_response)
+            deserialized = self._deserialize("MachineRunCommand", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(
-                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
             )
         elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+            polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return LROPoller[_models.MachineRunCommand].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_assess_patches.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{name}/assessPatches"
-    }
+        return LROPoller[_models.MachineRunCommand](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
-    async def _install_patches_initial(
-        self,
-        resource_group_name: str,
-        name: str,
-        install_patches_input: Union[_models.MachineInstallPatchesParameters, IO],
-        **kwargs: Any
-    ) -> Optional[_models.MachineInstallPatchesResult]:
+    def _delete_initial(  # pylint: disable=inconsistent-return-statements
+        self, resource_group_name: str, machine_name: str, run_command_name: str, **kwargs: Any
+    ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[Optional[_models.MachineInstallPatchesResult]] = kwargs.pop("cls", None)
-
-        content_type = content_type or "application/json"
-        _json = None
-        _content = None
-        if isinstance(install_patches_input, (IOBase, bytes)):
-            _content = install_patches_input
-        else:
-            _json = self._serialize.body(install_patches_input, "MachineInstallPatchesParameters")
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_install_patches_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
-            name=name,
+            machine_name=machine_name,
+            run_command_name=run_command_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            content_type=content_type,
-            json=_json,
-            content=_content,
-            template_url=self._install_patches_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 202]:
+        if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = None
         response_headers = {}
-        if response.status_code == 200:
-            deserialized = self._deserialize("MachineInstallPatchesResult", pipeline_response)
-
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
 
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)
-
-        return deserialized
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
-    _install_patches_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{name}/installPatches"
-    }
-
-    @overload
-    async def begin_install_patches(
-        self,
-        resource_group_name: str,
-        name: str,
-        install_patches_input: _models.MachineInstallPatchesParameters,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> AsyncLROPoller[_models.MachineInstallPatchesResult]:
-        """The operation to install patches on a hybrid machine identity in Azure.
-
-        :param resource_group_name: The name of the resource group. Required.
-        :type resource_group_name: str
-        :param name: The name of the hybrid machine. Required.
-        :type name: str
-        :param install_patches_input: Input for InstallPatches as directly received by the API.
-         Required.
-        :type install_patches_input: ~azure.mgmt.hybridcompute.models.MachineInstallPatchesParameters
-        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either MachineInstallPatchesResult or the
-         result of cls(response)
-        :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.MachineInstallPatchesResult]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-
-    @overload
-    async def begin_install_patches(
-        self,
-        resource_group_name: str,
-        name: str,
-        install_patches_input: IO,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> AsyncLROPoller[_models.MachineInstallPatchesResult]:
-        """The operation to install patches on a hybrid machine identity in Azure.
+    @distributed_trace
+    def begin_delete(
+        self, resource_group_name: str, machine_name: str, run_command_name: str, **kwargs: Any
+    ) -> LROPoller[None]:
+        """The operation to delete a run command.
 
-        :param resource_group_name: The name of the resource group. Required.
-        :type resource_group_name: str
-        :param name: The name of the hybrid machine. Required.
-        :type name: str
-        :param install_patches_input: Input for InstallPatches as directly received by the API.
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
-        :type install_patches_input: IO
-        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either MachineInstallPatchesResult or the
-         result of cls(response)
-        :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.MachineInstallPatchesResult]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-
-    @distributed_trace_async
-    async def begin_install_patches(
-        self,
-        resource_group_name: str,
-        name: str,
-        install_patches_input: Union[_models.MachineInstallPatchesParameters, IO],
-        **kwargs: Any
-    ) -> AsyncLROPoller[_models.MachineInstallPatchesResult]:
-        """The operation to install patches on a hybrid machine identity in Azure.
-
-        :param resource_group_name: The name of the resource group. Required.
         :type resource_group_name: str
-        :param name: The name of the hybrid machine. Required.
-        :type name: str
-        :param install_patches_input: Input for InstallPatches as directly received by the API. Is
-         either a MachineInstallPatchesParameters type or a IO type. Required.
-        :type install_patches_input: ~azure.mgmt.hybridcompute.models.MachineInstallPatchesParameters
-         or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of AsyncLROPoller that returns either MachineInstallPatchesResult or the
-         result of cls(response)
-        :rtype:
-         ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.MachineInstallPatchesResult]
+        :param machine_name: The name of the hybrid machine. Required.
+        :type machine_name: str
+        :param run_command_name: The name of the run command. Required.
+        :type run_command_name: str
+        :return: An instance of LROPoller that returns either None or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.MachineInstallPatchesResult] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        cls: ClsType[None] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._install_patches_initial(
+            raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
-                name=name,
-                install_patches_input=install_patches_input,
+                machine_name=machine_name,
+                run_command_name=run_command_name,
                 api_version=api_version,
-                content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
-        def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("MachineInstallPatchesResult", pipeline_response)
+        def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, deserialized, {})
-            return deserialized
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(
-                AsyncPollingMethod, AsyncARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
+            polling_method: PollingMethod = cast(
+                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "location"}, **kwargs)
             )
         elif polling is False:
-            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+            polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return LROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_install_patches.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{name}/installPatches"
-    }
+        return LROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     @distributed_trace
-    def list_by_resource_group(
-        self, resource_group_name: str, expand: Optional[str] = None, **kwargs: Any
-    ) -> AsyncIterable["_models.Machine"]:
-        """Lists all the hybrid machines in the specified resource group. Use the nextLink property in the
-        response to get the next page of hybrid machines.
+    def get(
+        self, resource_group_name: str, machine_name: str, run_command_name: str, **kwargs: Any
+    ) -> _models.MachineRunCommand:
+        """The operation to get a run command.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param expand: Expands referenced resources. Default value is None.
-        :type expand: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either Machine or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.hybridcompute.models.Machine]
+        :param machine_name: The name of the hybrid machine. Required.
+        :type machine_name: str
+        :param run_command_name: The name of the run command. Required.
+        :type run_command_name: str
+        :return: MachineRunCommand or the result of cls(response)
+        :rtype: ~azure.mgmt.hybridcompute.models.MachineRunCommand
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.MachineListResult] = kwargs.pop("cls", None)
-
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        def prepare_request(next_link=None):
-            if not next_link:
-
-                request = build_list_by_resource_group_request(
-                    resource_group_name=resource_group_name,
-                    subscription_id=self._config.subscription_id,
-                    expand=expand,
-                    api_version=api_version,
-                    template_url=self.list_by_resource_group.metadata["url"],
-                    headers=_headers,
-                    params=_params,
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-            else:
-                # make call to next link with the client's api-version
-                _parsed_next_link = urllib.parse.urlparse(next_link)
-                _next_request_params = case_insensitive_dict(
-                    {
-                        key: [urllib.parse.quote(v) for v in value]
-                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
-                    }
-                )
-                _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
-                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
-                )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.MachineRunCommand] = kwargs.pop("cls", None)
 
-        async def extract_data(pipeline_response):
-            deserialized = self._deserialize("MachineListResult", pipeline_response)
-            list_of_elem = deserialized.value
-            if cls:
-                list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, AsyncList(list_of_elem)
+        _request = build_get_request(
+            resource_group_name=resource_group_name,
+            machine_name=machine_name,
+            run_command_name=run_command_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            headers=_headers,
+            params=_params,
+        )
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
-        async def get_next(next_link=None):
-            request = prepare_request(next_link)
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
 
-            _stream = False
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
-            )
-            response = pipeline_response.http_response
+        response = pipeline_response.http_response
 
-            if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
-                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-            return pipeline_response
+        deserialized = self._deserialize("MachineRunCommand", pipeline_response)
 
-        return AsyncItemPaged(get_next, extract_data)
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    list_by_resource_group.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines"
-    }
+        return deserialized  # type: ignore
 
     @distributed_trace
-    def list_by_subscription(self, **kwargs: Any) -> AsyncIterable["_models.Machine"]:
-        """Lists all the hybrid machines in the specified subscription. Use the nextLink property in the
-        response to get the next page of hybrid machines.
-
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either Machine or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.hybridcompute.models.Machine]
+    def list(
+        self, resource_group_name: str, machine_name: str, expand: Optional[str] = None, **kwargs: Any
+    ) -> Iterable["_models.MachineRunCommand"]:
+        """The operation to get all the run commands of a non-Azure machine.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param machine_name: The name of the hybrid machine. Required.
+        :type machine_name: str
+        :param expand: The expand expression to apply on the operation. Default value is None.
+        :type expand: str
+        :return: An iterator like instance of either MachineRunCommand or the result of cls(response)
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.hybridcompute.models.MachineRunCommand]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.MachineListResult] = kwargs.pop("cls", None)
+        cls: ClsType[_models.MachineRunCommandsListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_subscription_request(
+                _request = build_list_request(
+                    resource_group_name=resource_group_name,
+                    machine_name=machine_name,
                     subscription_id=self._config.subscription_id,
+                    expand=expand,
                     api_version=api_version,
-                    template_url=self.list_by_subscription.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
-        async def extract_data(pipeline_response):
-            deserialized = self._deserialize("MachineListResult", pipeline_response)
+        def extract_data(pipeline_response):
+            deserialized = self._deserialize("MachineRunCommandsListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
-            return deserialized.next_link or None, AsyncList(list_of_elem)
+            return deserialized.next_link or None, iter(list_of_elem)
 
-        async def get_next(next_link=None):
-            request = prepare_request(next_link)
+        def get_next(next_link=None):
+            _request = prepare_request(next_link)
 
             _stream = False
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return AsyncItemPaged(get_next, extract_data)
-
-    list_by_subscription.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.HybridCompute/machines"
-    }
+        return ItemPaged(get_next, extract_data)
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_network_profile_operations.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_network_profile_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -56,15 +56,14 @@
         """The operation to get network information of hybrid machine.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param machine_name: The name of the hybrid machine. Required.
         :type machine_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: NetworkProfile or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.NetworkProfile
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -75,41 +74,36 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.NetworkProfile] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             machine_name=machine_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("NetworkProfile", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/networkProfile"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_operations.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -53,15 +53,14 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, **kwargs: Any) -> AsyncIterable["_models.OperationValue"]:
         """Gets a list of hybrid compute operations.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either OperationValue or the result of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.hybridcompute.models.OperationValue]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -76,60 +75,57 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("OperationListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
-
-    list.metadata = {"url": "/providers/Microsoft.HybridCompute/operations"}
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_patch.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_private_endpoint_connections_operations.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_private_endpoint_connections_operations.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -71,15 +71,14 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
         :type private_endpoint_connection_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateEndpointConnection or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.PrivateEndpointConnection
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -90,56 +89,51 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateEndpointConnection] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             scope_name=scope_name,
             private_endpoint_connection_name=private_endpoint_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+        return deserialized  # type: ignore
 
     async def _create_or_update_initial(
         self,
         resource_group_name: str,
         scope_name: str,
         private_endpoint_connection_name: str,
-        parameters: Union[_models.PrivateEndpointConnection, IO],
+        parameters: Union[_models.PrivateEndpointConnection, IO[bytes]],
         **kwargs: Any
     ) -> Optional[_models.PrivateEndpointConnection]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -157,54 +151,49 @@
         _json = None
         _content = None
         if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "PrivateEndpointConnection")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             scope_name=scope_name,
             private_endpoint_connection_name=private_endpoint_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
         if response.status_code == 200:
             deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         scope_name: str,
         private_endpoint_connection_name: str,
@@ -223,100 +212,73 @@
         :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
         :type private_endpoint_connection_name: str
         :param parameters: Required.
         :type parameters: ~azure.mgmt.hybridcompute.models.PrivateEndpointConnection
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either PrivateEndpointConnection or the
          result of cls(response)
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.PrivateEndpointConnection]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         scope_name: str,
         private_endpoint_connection_name: str,
-        parameters: IO,
+        parameters: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.PrivateEndpointConnection]:
         """Approve or reject a private endpoint connection with a given name.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
         :type private_endpoint_connection_name: str
         :param parameters: Required.
-        :type parameters: IO
+        :type parameters: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either PrivateEndpointConnection or the
          result of cls(response)
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.PrivateEndpointConnection]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         scope_name: str,
         private_endpoint_connection_name: str,
-        parameters: Union[_models.PrivateEndpointConnection, IO],
+        parameters: Union[_models.PrivateEndpointConnection, IO[bytes]],
         **kwargs: Any
     ) -> AsyncLROPoller[_models.PrivateEndpointConnection]:
         """Approve or reject a private endpoint connection with a given name.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
         :type private_endpoint_connection_name: str
-        :param parameters: Is either a PrivateEndpointConnection type or a IO type. Required.
-        :type parameters: ~azure.mgmt.hybridcompute.models.PrivateEndpointConnection or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+        :param parameters: Is either a PrivateEndpointConnection type or a IO[bytes] type. Required.
+        :type parameters: ~azure.mgmt.hybridcompute.models.PrivateEndpointConnection or IO[bytes]
         :return: An instance of AsyncLROPoller that returns either PrivateEndpointConnection or the
          result of cls(response)
         :rtype:
          ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.PrivateEndpointConnection]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
@@ -342,35 +304,33 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.PrivateEndpointConnection].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+        return AsyncLROPoller[_models.PrivateEndpointConnection](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, scope_name: str, private_endpoint_connection_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -381,30 +341,29 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             scope_name=scope_name,
             private_endpoint_connection_name=private_endpoint_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -415,41 +374,29 @@
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(
         self, resource_group_name: str, scope_name: str, private_endpoint_connection_name: str, **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Deletes a private endpoint connection with a given name.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
         :type private_endpoint_connection_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -469,47 +416,42 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     @distributed_trace
     def list_by_private_link_scope(
         self, resource_group_name: str, scope_name: str, **kwargs: Any
     ) -> AsyncIterable["_models.PrivateEndpointConnection"]:
         """Gets all private endpoint connections on a private link scope.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PrivateEndpointConnection or the result of
          cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.hybridcompute.models.PrivateEndpointConnection]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
@@ -525,65 +467,60 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_private_link_scope_request(
+                _request = build_list_by_private_link_scope_request(
                     resource_group_name=resource_group_name,
                     scope_name=scope_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_private_link_scope.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("PrivateEndpointConnectionListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
-
-    list_by_private_link_scope.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateEndpointConnections"
-    }
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_private_link_resources_operations.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_private_link_resources_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -61,15 +61,14 @@
         """Gets the private link resources that need to be created for a Azure Monitor PrivateLinkScope.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PrivateLinkResource or the result of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.hybridcompute.models.PrivateLinkResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -84,87 +83,81 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_private_link_scope_request(
+                _request = build_list_by_private_link_scope_request(
                     resource_group_name=resource_group_name,
                     scope_name=scope_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_private_link_scope.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("PrivateLinkResourceListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_private_link_scope.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateLinkResources"
-    }
-
     @distributed_trace_async
     async def get(
         self, resource_group_name: str, scope_name: str, group_name: str, **kwargs: Any
     ) -> _models.PrivateLinkResource:
         """Gets the private link resources that need to be created for a Azure Monitor PrivateLinkScope.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
         :param group_name: The name of the private link resource. Required.
         :type group_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateLinkResource or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.PrivateLinkResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -175,42 +168,37 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateLinkResource] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             scope_name=scope_name,
             group_name=group_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("PrivateLinkResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateLinkResources/{groupName}"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/aio/operations/_private_link_scopes_operations.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_private_link_scopes_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -66,15 +66,14 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, **kwargs: Any) -> AsyncIterable["_models.HybridComputePrivateLinkScope"]:
         """Gets a list of all Azure Arc PrivateLinkScopes within a subscription.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either HybridComputePrivateLinkScope or the result of
          cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
@@ -90,79 +89,75 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("HybridComputePrivateLinkScopeListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.HybridCompute/privateLinkScopes"}
-
     @distributed_trace
     def list_by_resource_group(
         self, resource_group_name: str, **kwargs: Any
     ) -> AsyncIterable["_models.HybridComputePrivateLinkScope"]:
         """Gets a list of Azure Arc PrivateLinkScopes within a resource group.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either HybridComputePrivateLinkScope or the result of
          cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
@@ -178,72 +173,67 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_resource_group_request(
+                _request = build_list_by_resource_group_request(
                     resource_group_name=resource_group_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_resource_group.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("HybridComputePrivateLinkScopeListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_by_resource_group.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes"
-    }
-
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, scope_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -253,29 +243,28 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             scope_name=scope_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -286,37 +275,25 @@
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def begin_delete(self, resource_group_name: str, scope_name: str, **kwargs: Any) -> AsyncLROPoller[None]:
         """Deletes a Azure Arc PrivateLinkScope.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be AsyncARMPolling. Pass in False for
-         this operation to not poll, or pass in your own initialized polling object for a personal
-         polling strategy.
-        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -335,47 +312,42 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}"
-    }
+        return AsyncLROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     @distributed_trace_async
     async def get(
         self, resource_group_name: str, scope_name: str, **kwargs: Any
     ) -> _models.HybridComputePrivateLinkScope:
         """Returns a Azure Arc PrivateLinkScope.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: HybridComputePrivateLinkScope or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -386,48 +358,43 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.HybridComputePrivateLinkScope] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             scope_name=scope_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("HybridComputePrivateLinkScope", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     async def create_or_update(
         self,
         resource_group_name: str,
         scope_name: str,
         parameters: _models.HybridComputePrivateLinkScope,
@@ -445,74 +412,68 @@
         :type scope_name: str
         :param parameters: Properties that need to be specified to create or update a Azure Arc for
          Servers and Clusters PrivateLinkScope. Required.
         :type parameters: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: HybridComputePrivateLinkScope or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def create_or_update(
         self,
         resource_group_name: str,
         scope_name: str,
-        parameters: IO,
+        parameters: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.HybridComputePrivateLinkScope:
         """Creates (or updates) a Azure Arc PrivateLinkScope. Note: You cannot specify a different value
         for InstrumentationKey nor AppId in the Put operation.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
         :param parameters: Properties that need to be specified to create or update a Azure Arc for
          Servers and Clusters PrivateLinkScope. Required.
-        :type parameters: IO
+        :type parameters: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: HybridComputePrivateLinkScope or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def create_or_update(
         self,
         resource_group_name: str,
         scope_name: str,
-        parameters: Union[_models.HybridComputePrivateLinkScope, IO],
+        parameters: Union[_models.HybridComputePrivateLinkScope, IO[bytes]],
         **kwargs: Any
     ) -> _models.HybridComputePrivateLinkScope:
         """Creates (or updates) a Azure Arc PrivateLinkScope. Note: You cannot specify a different value
         for InstrumentationKey nor AppId in the Put operation.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
         :param parameters: Properties that need to be specified to create or update a Azure Arc for
-         Servers and Clusters PrivateLinkScope. Is either a HybridComputePrivateLinkScope type or a IO
-         type. Required.
-        :type parameters: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         Servers and Clusters PrivateLinkScope. Is either a HybridComputePrivateLinkScope type or a
+         IO[bytes] type. Required.
+        :type parameters: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope or IO[bytes]
         :return: HybridComputePrivateLinkScope or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -532,32 +493,31 @@
         _json = None
         _content = None
         if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "HybridComputePrivateLinkScope")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             scope_name=scope_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -570,18 +530,14 @@
             deserialized = self._deserialize("HybridComputePrivateLinkScope", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}"
-    }
-
     @overload
     async def update_tags(
         self,
         resource_group_name: str,
         scope_name: str,
         private_link_scope_tags: _models.TagsResource,
         *,
@@ -598,73 +554,67 @@
         :type scope_name: str
         :param private_link_scope_tags: Updated tag information to set into the PrivateLinkScope
          instance. Required.
         :type private_link_scope_tags: ~azure.mgmt.hybridcompute.models.TagsResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: HybridComputePrivateLinkScope or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def update_tags(
         self,
         resource_group_name: str,
         scope_name: str,
-        private_link_scope_tags: IO,
+        private_link_scope_tags: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.HybridComputePrivateLinkScope:
         """Updates an existing PrivateLinkScope's tags. To update other fields use the CreateOrUpdate
         method.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
         :param private_link_scope_tags: Updated tag information to set into the PrivateLinkScope
          instance. Required.
-        :type private_link_scope_tags: IO
+        :type private_link_scope_tags: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: HybridComputePrivateLinkScope or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def update_tags(
         self,
         resource_group_name: str,
         scope_name: str,
-        private_link_scope_tags: Union[_models.TagsResource, IO],
+        private_link_scope_tags: Union[_models.TagsResource, IO[bytes]],
         **kwargs: Any
     ) -> _models.HybridComputePrivateLinkScope:
         """Updates an existing PrivateLinkScope's tags. To update other fields use the CreateOrUpdate
         method.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
         :param private_link_scope_tags: Updated tag information to set into the PrivateLinkScope
-         instance. Is either a TagsResource type or a IO type. Required.
-        :type private_link_scope_tags: ~azure.mgmt.hybridcompute.models.TagsResource or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         instance. Is either a TagsResource type or a IO[bytes] type. Required.
+        :type private_link_scope_tags: ~azure.mgmt.hybridcompute.models.TagsResource or IO[bytes]
         :return: HybridComputePrivateLinkScope or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -684,64 +634,58 @@
         _json = None
         _content = None
         if isinstance(private_link_scope_tags, (IOBase, bytes)):
             _content = private_link_scope_tags
         else:
             _json = self._serialize.body(private_link_scope_tags, "TagsResource")
 
-        request = build_update_tags_request(
+        _request = build_update_tags_request(
             resource_group_name=resource_group_name,
             scope_name=scope_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.update_tags.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("HybridComputePrivateLinkScope", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    update_tags.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}"
-    }
+        return deserialized  # type: ignore
 
     @distributed_trace_async
     async def get_validation_details(
         self, location: str, private_link_scope_id: str, **kwargs: Any
     ) -> _models.PrivateLinkScopeValidationDetails:
         """Returns a Azure Arc PrivateLinkScope's validation details.
 
         :param location: The location of the target resource. Required.
         :type location: str
         :param private_link_scope_id: The id (Guid) of the Azure Arc PrivateLinkScope resource.
          Required.
         :type private_link_scope_id: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateLinkScopeValidationDetails or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.PrivateLinkScopeValidationDetails
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -752,62 +696,56 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateLinkScopeValidationDetails] = kwargs.pop("cls", None)
 
-        request = build_get_validation_details_request(
+        _request = build_get_validation_details_request(
             location=location,
             private_link_scope_id=private_link_scope_id,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get_validation_details.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("PrivateLinkScopeValidationDetails", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get_validation_details.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.HybridCompute/locations/{location}/privateLinkScopes/{privateLinkScopeId}"
-    }
+        return deserialized  # type: ignore
 
     @distributed_trace_async
     async def get_validation_details_for_machine(
         self, resource_group_name: str, machine_name: str, **kwargs: Any
     ) -> _models.PrivateLinkScopeValidationDetails:
         """Returns a Azure Arc PrivateLinkScope's validation details for a given machine.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param machine_name: The name of the target machine to get the private link scope validation
          details for. Required.
         :type machine_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateLinkScopeValidationDetails or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.PrivateLinkScopeValidationDetails
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -818,41 +756,36 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateLinkScopeValidationDetails] = kwargs.pop("cls", None)
 
-        request = build_get_validation_details_for_machine_request(
+        _request = build_get_validation_details_for_machine_request(
             resource_group_name=resource_group_name,
             machine_name=machine_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get_validation_details_for_machine.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("PrivateLinkScopeValidationDetails", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get_validation_details_for_machine.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/privateLinkScopes/current"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/models/__init__.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/models/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,38 +2,40 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+from ._models_py3 import AccessRule
 from ._models_py3 import AgentConfiguration
 from ._models_py3 import AgentUpgrade
 from ._models_py3 import AgentVersion
 from ._models_py3 import AgentVersionsList
 from ._models_py3 import AvailablePatchCountByClassification
 from ._models_py3 import CloudMetadata
 from ._models_py3 import ConfigurationExtension
 from ._models_py3 import ConnectionDetail
 from ._models_py3 import ErrorAdditionalInfo
 from ._models_py3 import ErrorDetail
-from ._models_py3 import ErrorDetailAutoGenerated
 from ._models_py3 import ErrorResponse
-from ._models_py3 import ErrorResponseAutoGenerated
 from ._models_py3 import EsuKey
 from ._models_py3 import ExtensionTargetProperties
 from ._models_py3 import ExtensionValue
 from ._models_py3 import ExtensionValueListResult
+from ._models_py3 import ExtensionsResourceStatus
 from ._models_py3 import HybridComputePrivateLinkScope
 from ._models_py3 import HybridComputePrivateLinkScopeListResult
 from ._models_py3 import HybridComputePrivateLinkScopeProperties
 from ._models_py3 import HybridIdentityMetadata
 from ._models_py3 import HybridIdentityMetadataList
 from ._models_py3 import Identity
 from ._models_py3 import IpAddress
+from ._models_py3 import KeyDetails
+from ._models_py3 import KeyProperties
 from ._models_py3 import License
 from ._models_py3 import LicenseDetails
 from ._models_py3 import LicenseProfile
 from ._models_py3 import LicenseProfileArmEsuProperties
 from ._models_py3 import LicenseProfileArmEsuPropertiesWithoutAssignedLicense
 from ._models_py3 import LicenseProfileMachineInstanceView
 from ._models_py3 import LicenseProfileMachineInstanceViewEsuProperties
@@ -52,17 +54,27 @@
 from ._models_py3 import MachineExtensionProperties
 from ._models_py3 import MachineExtensionUpdate
 from ._models_py3 import MachineExtensionUpgrade
 from ._models_py3 import MachineExtensionsListResult
 from ._models_py3 import MachineInstallPatchesParameters
 from ._models_py3 import MachineInstallPatchesResult
 from ._models_py3 import MachineListResult
+from ._models_py3 import MachineRunCommand
+from ._models_py3 import MachineRunCommandInstanceView
+from ._models_py3 import MachineRunCommandScriptSource
+from ._models_py3 import MachineRunCommandUpdate
+from ._models_py3 import MachineRunCommandsListResult
 from ._models_py3 import MachineUpdate
+from ._models_py3 import NetworkConfiguration
 from ._models_py3 import NetworkInterface
 from ._models_py3 import NetworkProfile
+from ._models_py3 import NetworkSecurityPerimeter
+from ._models_py3 import NetworkSecurityPerimeterConfiguration
+from ._models_py3 import NetworkSecurityPerimeterConfigurationListResult
+from ._models_py3 import NetworkSecurityPerimeterProfile
 from ._models_py3 import OSProfile
 from ._models_py3 import OSProfileLinuxConfiguration
 from ._models_py3 import OSProfileWindowsConfiguration
 from ._models_py3 import OperationListResult
 from ._models_py3 import OperationValue
 from ._models_py3 import OperationValueDisplay
 from ._models_py3 import PrivateEndpointConnection
@@ -72,82 +84,99 @@
 from ._models_py3 import PrivateEndpointProperty
 from ._models_py3 import PrivateLinkResource
 from ._models_py3 import PrivateLinkResourceListResult
 from ._models_py3 import PrivateLinkResourceProperties
 from ._models_py3 import PrivateLinkScopeValidationDetails
 from ._models_py3 import PrivateLinkScopesResource
 from ._models_py3 import PrivateLinkServiceConnectionStateProperty
+from ._models_py3 import ProductFeature
+from ._models_py3 import ProductFeatureUpdate
+from ._models_py3 import ProvisioningIssue
 from ._models_py3 import ProxyResource
 from ._models_py3 import Resource
+from ._models_py3 import ResourceAssociation
 from ._models_py3 import ResourceUpdate
+from ._models_py3 import RunCommandInputParameter
+from ._models_py3 import RunCommandManagedIdentity
 from ._models_py3 import ServiceStatus
 from ._models_py3 import ServiceStatuses
 from ._models_py3 import Subnet
 from ._models_py3 import SystemData
 from ._models_py3 import TagsResource
 from ._models_py3 import TrackedResource
 from ._models_py3 import WindowsParameters
 
+from ._hybrid_compute_management_client_enums import AccessMode
+from ._hybrid_compute_management_client_enums import AccessRuleDirection
 from ._hybrid_compute_management_client_enums import AgentConfigurationMode
 from ._hybrid_compute_management_client_enums import ArcKindEnum
 from ._hybrid_compute_management_client_enums import AssessmentModeTypes
 from ._hybrid_compute_management_client_enums import CreatedByType
 from ._hybrid_compute_management_client_enums import EsuEligibility
 from ._hybrid_compute_management_client_enums import EsuKeyState
 from ._hybrid_compute_management_client_enums import EsuServerType
-from ._hybrid_compute_management_client_enums import InstanceViewTypes
+from ._hybrid_compute_management_client_enums import ExecutionState
+from ._hybrid_compute_management_client_enums import ExtensionsStatusLevelTypes
 from ._hybrid_compute_management_client_enums import LastAttemptStatusEnum
 from ._hybrid_compute_management_client_enums import LicenseAssignmentState
 from ._hybrid_compute_management_client_enums import LicenseCoreType
 from ._hybrid_compute_management_client_enums import LicenseEdition
+from ._hybrid_compute_management_client_enums import LicenseProfileProductType
+from ._hybrid_compute_management_client_enums import LicenseProfileSubscriptionStatus
+from ._hybrid_compute_management_client_enums import LicenseProfileSubscriptionStatusUpdate
 from ._hybrid_compute_management_client_enums import LicenseState
+from ._hybrid_compute_management_client_enums import LicenseStatus
 from ._hybrid_compute_management_client_enums import LicenseTarget
 from ._hybrid_compute_management_client_enums import LicenseType
 from ._hybrid_compute_management_client_enums import OsType
 from ._hybrid_compute_management_client_enums import PatchModeTypes
 from ._hybrid_compute_management_client_enums import PatchOperationStartedBy
 from ._hybrid_compute_management_client_enums import PatchOperationStatus
 from ._hybrid_compute_management_client_enums import PatchServiceUsed
+from ._hybrid_compute_management_client_enums import ProvisioningIssueSeverity
+from ._hybrid_compute_management_client_enums import ProvisioningIssueType
 from ._hybrid_compute_management_client_enums import ProvisioningState
 from ._hybrid_compute_management_client_enums import PublicNetworkAccessType
 from ._hybrid_compute_management_client_enums import StatusLevelTypes
 from ._hybrid_compute_management_client_enums import StatusTypes
 from ._hybrid_compute_management_client_enums import VMGuestPatchClassificationLinux
 from ._hybrid_compute_management_client_enums import VMGuestPatchClassificationWindows
 from ._hybrid_compute_management_client_enums import VMGuestPatchRebootSetting
 from ._hybrid_compute_management_client_enums import VMGuestPatchRebootStatus
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
+    "AccessRule",
     "AgentConfiguration",
     "AgentUpgrade",
     "AgentVersion",
     "AgentVersionsList",
     "AvailablePatchCountByClassification",
     "CloudMetadata",
     "ConfigurationExtension",
     "ConnectionDetail",
     "ErrorAdditionalInfo",
     "ErrorDetail",
-    "ErrorDetailAutoGenerated",
     "ErrorResponse",
-    "ErrorResponseAutoGenerated",
     "EsuKey",
     "ExtensionTargetProperties",
     "ExtensionValue",
     "ExtensionValueListResult",
+    "ExtensionsResourceStatus",
     "HybridComputePrivateLinkScope",
     "HybridComputePrivateLinkScopeListResult",
     "HybridComputePrivateLinkScopeProperties",
     "HybridIdentityMetadata",
     "HybridIdentityMetadataList",
     "Identity",
     "IpAddress",
+    "KeyDetails",
+    "KeyProperties",
     "License",
     "LicenseDetails",
     "LicenseProfile",
     "LicenseProfileArmEsuProperties",
     "LicenseProfileArmEsuPropertiesWithoutAssignedLicense",
     "LicenseProfileMachineInstanceView",
     "LicenseProfileMachineInstanceViewEsuProperties",
@@ -166,17 +195,27 @@
     "MachineExtensionProperties",
     "MachineExtensionUpdate",
     "MachineExtensionUpgrade",
     "MachineExtensionsListResult",
     "MachineInstallPatchesParameters",
     "MachineInstallPatchesResult",
     "MachineListResult",
+    "MachineRunCommand",
+    "MachineRunCommandInstanceView",
+    "MachineRunCommandScriptSource",
+    "MachineRunCommandUpdate",
+    "MachineRunCommandsListResult",
     "MachineUpdate",
+    "NetworkConfiguration",
     "NetworkInterface",
     "NetworkProfile",
+    "NetworkSecurityPerimeter",
+    "NetworkSecurityPerimeterConfiguration",
+    "NetworkSecurityPerimeterConfigurationListResult",
+    "NetworkSecurityPerimeterProfile",
     "OSProfile",
     "OSProfileLinuxConfiguration",
     "OSProfileWindowsConfiguration",
     "OperationListResult",
     "OperationValue",
     "OperationValueDisplay",
     "PrivateEndpointConnection",
@@ -186,44 +225,59 @@
     "PrivateEndpointProperty",
     "PrivateLinkResource",
     "PrivateLinkResourceListResult",
     "PrivateLinkResourceProperties",
     "PrivateLinkScopeValidationDetails",
     "PrivateLinkScopesResource",
     "PrivateLinkServiceConnectionStateProperty",
+    "ProductFeature",
+    "ProductFeatureUpdate",
+    "ProvisioningIssue",
     "ProxyResource",
     "Resource",
+    "ResourceAssociation",
     "ResourceUpdate",
+    "RunCommandInputParameter",
+    "RunCommandManagedIdentity",
     "ServiceStatus",
     "ServiceStatuses",
     "Subnet",
     "SystemData",
     "TagsResource",
     "TrackedResource",
     "WindowsParameters",
+    "AccessMode",
+    "AccessRuleDirection",
     "AgentConfigurationMode",
     "ArcKindEnum",
     "AssessmentModeTypes",
     "CreatedByType",
     "EsuEligibility",
     "EsuKeyState",
     "EsuServerType",
-    "InstanceViewTypes",
+    "ExecutionState",
+    "ExtensionsStatusLevelTypes",
     "LastAttemptStatusEnum",
     "LicenseAssignmentState",
     "LicenseCoreType",
     "LicenseEdition",
+    "LicenseProfileProductType",
+    "LicenseProfileSubscriptionStatus",
+    "LicenseProfileSubscriptionStatusUpdate",
     "LicenseState",
+    "LicenseStatus",
     "LicenseTarget",
     "LicenseType",
     "OsType",
     "PatchModeTypes",
     "PatchOperationStartedBy",
     "PatchOperationStatus",
     "PatchServiceUsed",
+    "ProvisioningIssueSeverity",
+    "ProvisioningIssueType",
     "ProvisioningState",
     "PublicNetworkAccessType",
     "StatusLevelTypes",
     "StatusTypes",
     "VMGuestPatchClassificationLinux",
     "VMGuestPatchClassificationWindows",
     "VMGuestPatchRebootSetting",
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/models/_hybrid_compute_management_client_enums.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/models/_hybrid_compute_management_client_enums.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,36 @@
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from enum import Enum
 from azure.core import CaseInsensitiveEnumMeta
 
 
+class AccessMode(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Property that impacts a resource's logging behavior and its connectivity with other resources
+    and public networks.
+    """
+
+    ENFORCED = "enforced"
+    """Indicates that resource access is controlled by the NSP definition."""
+    AUDIT = "audit"
+    """Dry run mode, where traffic is evaluated against NSP Rules, logged but not enforced."""
+    LEARNING = "learning"
+    """Enables traffic evaluation to fall back to resource-specific firewall configurations."""
+
+
+class AccessRuleDirection(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Indicates direction of an access rule."""
+
+    INBOUND = "Inbound"
+    """Traffic originates outside of network."""
+    OUTBOUND = "Outbound"
+    """Traffic originates inside the network"""
+
+
 class AgentConfigurationMode(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Name of configuration mode to use. Modes are pre-defined configurations of security controls,
     extension allowlists and guest configuration, maintained by Microsoft.
     """
 
     FULL = "full"
     MONITOR = "monitor"
@@ -65,18 +87,32 @@
 class EsuServerType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The server types for Esu."""
 
     STANDARD = "Standard"
     DATACENTER = "Datacenter"
 
 
-class InstanceViewTypes(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """InstanceViewTypes."""
+class ExecutionState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Script execution status."""
+
+    UNKNOWN = "Unknown"
+    PENDING = "Pending"
+    RUNNING = "Running"
+    FAILED = "Failed"
+    SUCCEEDED = "Succeeded"
+    TIMED_OUT = "TimedOut"
+    CANCELED = "Canceled"
+
+
+class ExtensionsStatusLevelTypes(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The level code."""
 
-    INSTANCE_VIEW = "instanceView"
+    INFO = "Info"
+    WARNING = "Warning"
+    ERROR = "Error"
 
 
 class LastAttemptStatusEnum(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Specifies the status of Agent Upgrade."""
 
     SUCCESS = "Success"
     FAILED = "Failed"
@@ -99,21 +135,56 @@
 class LicenseEdition(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Describes the edition of the license. The values are either Standard or Datacenter."""
 
     STANDARD = "Standard"
     DATACENTER = "Datacenter"
 
 
+class LicenseProfileProductType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The product type of the license."""
+
+    WINDOWS_SERVER = "WindowsServer"
+    WINDOWS_IO_T_ENTERPRISE = "WindowsIoTEnterprise"
+
+
+class LicenseProfileSubscriptionStatus(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Subscription status of the OS or Product feature."""
+
+    UNKNOWN = "Unknown"
+    ENABLING = "Enabling"
+    ENABLED = "Enabled"
+    DISABLED = "Disabled"
+
+
+class LicenseProfileSubscriptionStatusUpdate(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Indicates the new subscription status of the OS or Product Features."""
+
+    ENABLE = "Enable"
+    DISABLE = "Disable"
+
+
 class LicenseState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Describes the state of the license."""
 
     ACTIVATED = "Activated"
     DEACTIVATED = "Deactivated"
 
 
+class LicenseStatus(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The license status."""
+
+    UNLICENSED = "Unlicensed"
+    LICENSED = "Licensed"
+    OOB_GRACE = "OOBGrace"
+    OOT_GRACE = "OOTGrace"
+    NON_GENUINE_GRACE = "NonGenuineGrace"
+    NOTIFICATION = "Notification"
+    EXTENDED_GRACE = "ExtendedGrace"
+
+
 class LicenseTarget(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Describes the license target server."""
 
     WINDOWS_SERVER2012 = "Windows Server 2012"
     WINDOWS_SERVER2012_R2 = "Windows Server 2012 R2"
 
 
@@ -166,14 +237,36 @@
     WU = "WU"
     WU_WSUS = "WU_WSUS"
     YUM = "YUM"
     APT = "APT"
     ZYPPER = "Zypper"
 
 
+class ProvisioningIssueSeverity(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Severity of the provisioning issue."""
+
+    WARNING = "Warning"
+    """Warnings can cause connectivity issues after provisioning succeeds."""
+    ERROR = "Error"
+    """Errors will cause association provisioning to fail."""
+
+
+class ProvisioningIssueType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Type of provisioning issue."""
+
+    MISSING_PERIMETER_CONFIGURATION = "MissingPerimeterConfiguration"
+    """Perimeter configuration is missing."""
+    MISSING_IDENTITY_CONFIGURATION = "MissingIdentityConfiguration"
+    """Identity configuration is missing."""
+    CONFIGURATION_PROPAGATION_FAILURE = "ConfigurationPropagationFailure"
+    """Configuration failed to propagate."""
+    OTHER = "Other"
+    """Other failure."""
+
+
 class ProvisioningState(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The provisioning state, which only appears in the response."""
 
     CREATING = "Creating"
     UPDATING = "Updating"
     DELETING = "Deleting"
     SUCCEEDED = "Succeeded"
@@ -186,18 +279,18 @@
 class PublicNetworkAccessType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The network access policy to determine if Azure Arc agents can use public Azure Arc service
     endpoints. Defaults to disabled (access to Azure Arc services only via private link).
     """
 
     ENABLED = "Enabled"
     """Allows Azure Arc agents to communicate with Azure Arc services over both public (internet) and
-    #: private endpoints."""
+    private endpoints."""
     DISABLED = "Disabled"
     """Does not allow Azure Arc agents to communicate with Azure Arc services over public (internet)
-    #: endpoints. The agents must use the private link."""
+    endpoints. The agents must use the private link."""
 
 
 class StatusLevelTypes(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The level code."""
 
     INFO = "Info"
     WARNING = "Warning"
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/models/_models_py3.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/models/_models_py3.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,29 +4,56 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 import datetime
-import sys
-from typing import Any, Dict, List, Optional, TYPE_CHECKING, Union
+from typing import Any, Dict, List, Literal, Optional, TYPE_CHECKING, Union
 
 from .. import _serialization
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
-
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from .. import models as _models
 
 
+class AccessRule(_serialization.Model):
+    """Access rule.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar name: Name of the access rule.
+    :vartype name: str
+    :ivar direction: Direction of the access rule. Known values are: "Inbound" and "Outbound".
+    :vartype direction: str or ~azure.mgmt.hybridcompute.models.AccessRuleDirection
+    :ivar address_prefixes: Address prefixes that are allowed access.
+    :vartype address_prefixes: list[str]
+    """
+
+    _validation = {
+        "name": {"readonly": True},
+        "direction": {"readonly": True},
+        "address_prefixes": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "name": {"key": "name", "type": "str"},
+        "direction": {"key": "properties.direction", "type": "str"},
+        "address_prefixes": {"key": "properties.addressPrefixes", "type": "[str]"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.name = None
+        self.direction = None
+        self.address_prefixes = None
+
+
 class AgentConfiguration(_serialization.Model):
     """Configurable properties that the user can set locally via the azcmagent config command, or
     remotely via ARM.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar proxy_url: Specifies the URL of the proxy to be used.
@@ -97,15 +124,15 @@
     :ivar correlation_id: The correlation ID passed in from RSM per upgrade.
     :vartype correlation_id: str
     :ivar enable_automatic_upgrade: Specifies if RSM should try to upgrade this machine.
     :vartype enable_automatic_upgrade: bool
     :ivar last_attempt_desired_version: Specifies the version of the last attempt.
     :vartype last_attempt_desired_version: str
     :ivar last_attempt_timestamp: Timestamp of last upgrade attempt.
-    :vartype last_attempt_timestamp: str
+    :vartype last_attempt_timestamp: ~datetime.datetime
     :ivar last_attempt_status: Specifies the status of Agent Upgrade. Known values are: "Success"
      and "Failed".
     :vartype last_attempt_status: str or ~azure.mgmt.hybridcompute.models.LastAttemptStatusEnum
     :ivar last_attempt_message: Failure message of last upgrade attempt if any.
     :vartype last_attempt_message: str
     """
 
@@ -117,15 +144,15 @@
     }
 
     _attribute_map = {
         "desired_version": {"key": "desiredVersion", "type": "str"},
         "correlation_id": {"key": "correlationId", "type": "str"},
         "enable_automatic_upgrade": {"key": "enableAutomaticUpgrade", "type": "bool"},
         "last_attempt_desired_version": {"key": "lastAttemptDesiredVersion", "type": "str"},
-        "last_attempt_timestamp": {"key": "lastAttemptTimestamp", "type": "str"},
+        "last_attempt_timestamp": {"key": "lastAttemptTimestamp", "type": "iso-8601"},
         "last_attempt_status": {"key": "lastAttemptStatus", "type": "str"},
         "last_attempt_message": {"key": "lastAttemptMessage", "type": "str"},
     }
 
     def __init__(
         self,
         *,
@@ -443,57 +470,14 @@
         self.code = None
         self.message = None
         self.target = None
         self.details = None
         self.additional_info = None
 
 
-class ErrorDetailAutoGenerated(_serialization.Model):
-    """The error detail.
-
-    Variables are only populated by the server, and will be ignored when sending a request.
-
-    :ivar code: The error code.
-    :vartype code: str
-    :ivar message: The error message.
-    :vartype message: str
-    :ivar target: The error target.
-    :vartype target: str
-    :ivar details: The error details.
-    :vartype details: list[~azure.mgmt.hybridcompute.models.ErrorDetailAutoGenerated]
-    :ivar additional_info: The error additional info.
-    :vartype additional_info: list[~azure.mgmt.hybridcompute.models.ErrorAdditionalInfo]
-    """
-
-    _validation = {
-        "code": {"readonly": True},
-        "message": {"readonly": True},
-        "target": {"readonly": True},
-        "details": {"readonly": True},
-        "additional_info": {"readonly": True},
-    }
-
-    _attribute_map = {
-        "code": {"key": "code", "type": "str"},
-        "message": {"key": "message", "type": "str"},
-        "target": {"key": "target", "type": "str"},
-        "details": {"key": "details", "type": "[ErrorDetailAutoGenerated]"},
-        "additional_info": {"key": "additionalInfo", "type": "[ErrorAdditionalInfo]"},
-    }
-
-    def __init__(self, **kwargs: Any) -> None:
-        """ """
-        super().__init__(**kwargs)
-        self.code = None
-        self.message = None
-        self.target = None
-        self.details = None
-        self.additional_info = None
-
-
 class ErrorResponse(_serialization.Model):
     """Common error response for all Azure Resource Manager APIs to return error details for failed
     operations. (This also follows the OData error response format.).
 
     :ivar error: The error object.
     :vartype error: ~azure.mgmt.hybridcompute.models.ErrorDetail
     """
@@ -507,35 +491,14 @@
         :keyword error: The error object.
         :paramtype error: ~azure.mgmt.hybridcompute.models.ErrorDetail
         """
         super().__init__(**kwargs)
         self.error = error
 
 
-class ErrorResponseAutoGenerated(_serialization.Model):
-    """Common error response for all Azure Resource Manager APIs to return error details for failed
-    operations. (This also follows the OData error response format.).
-
-    :ivar error: The error object.
-    :vartype error: ~azure.mgmt.hybridcompute.models.ErrorDetailAutoGenerated
-    """
-
-    _attribute_map = {
-        "error": {"key": "error", "type": "ErrorDetailAutoGenerated"},
-    }
-
-    def __init__(self, *, error: Optional["_models.ErrorDetailAutoGenerated"] = None, **kwargs: Any) -> None:
-        """
-        :keyword error: The error object.
-        :paramtype error: ~azure.mgmt.hybridcompute.models.ErrorDetailAutoGenerated
-        """
-        super().__init__(**kwargs)
-        self.error = error
-
-
 class EsuKey(_serialization.Model):
     """ESU key.
 
     :ivar sku: SKU number.
     :vartype sku: str
     :ivar license_status: The current status of the license profile key.
     :vartype license_status: str
@@ -554,14 +517,67 @@
         :paramtype license_status: str
         """
         super().__init__(**kwargs)
         self.sku = sku
         self.license_status = license_status
 
 
+class ExtensionsResourceStatus(_serialization.Model):
+    """Instance view status.
+
+    :ivar code: The status code.
+    :vartype code: str
+    :ivar level: The level code. Known values are: "Info", "Warning", and "Error".
+    :vartype level: str or ~azure.mgmt.hybridcompute.models.ExtensionsStatusLevelTypes
+    :ivar display_status: The short localizable label for the status.
+    :vartype display_status: str
+    :ivar message: The detailed status message, including for alerts and error messages.
+    :vartype message: str
+    :ivar time: The time of the status.
+    :vartype time: ~datetime.datetime
+    """
+
+    _attribute_map = {
+        "code": {"key": "code", "type": "str"},
+        "level": {"key": "level", "type": "str"},
+        "display_status": {"key": "displayStatus", "type": "str"},
+        "message": {"key": "message", "type": "str"},
+        "time": {"key": "time", "type": "iso-8601"},
+    }
+
+    def __init__(
+        self,
+        *,
+        code: Optional[str] = None,
+        level: Optional[Union[str, "_models.ExtensionsStatusLevelTypes"]] = None,
+        display_status: Optional[str] = None,
+        message: Optional[str] = None,
+        time: Optional[datetime.datetime] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword code: The status code.
+        :paramtype code: str
+        :keyword level: The level code. Known values are: "Info", "Warning", and "Error".
+        :paramtype level: str or ~azure.mgmt.hybridcompute.models.ExtensionsStatusLevelTypes
+        :keyword display_status: The short localizable label for the status.
+        :paramtype display_status: str
+        :keyword message: The detailed status message, including for alerts and error messages.
+        :paramtype message: str
+        :keyword time: The time of the status.
+        :paramtype time: ~datetime.datetime
+        """
+        super().__init__(**kwargs)
+        self.code = code
+        self.level = level
+        self.display_status = display_status
+        self.message = message
+        self.time = time
+
+
 class ExtensionTargetProperties(_serialization.Model):
     """Describes the Machine Extension Target Version Properties.
 
     :ivar target_version: Properties for the specified Extension to Upgrade.
     :vartype target_version: str
     """
 
@@ -580,15 +596,15 @@
 
 class Resource(_serialization.Model):
     """Common fields that are returned in the response for all Azure Resource Manager resources.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -622,52 +638,34 @@
 class ProxyResource(Resource):
     """The resource model definition for a Azure Resource Manager proxy resource. It will not have
     tags and a location.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
     :vartype system_data: ~azure.mgmt.hybridcompute.models.SystemData
     """
 
-    _validation = {
-        "id": {"readonly": True},
-        "name": {"readonly": True},
-        "type": {"readonly": True},
-        "system_data": {"readonly": True},
-    }
-
-    _attribute_map = {
-        "id": {"key": "id", "type": "str"},
-        "name": {"key": "name", "type": "str"},
-        "type": {"key": "type", "type": "str"},
-        "system_data": {"key": "systemData", "type": "SystemData"},
-    }
-
-    def __init__(self, **kwargs: Any) -> None:
-        """ """
-        super().__init__(**kwargs)
-
 
 class ExtensionValue(ProxyResource):
     """Describes a Extension Metadata.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -733,15 +731,15 @@
 
 
 class PrivateLinkScopesResource(_serialization.Model):
     """An azure resource object.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar id: Azure resource Id.
     :vartype id: str
     :ivar name: Azure resource name.
     :vartype name: str
     :ivar type: Azure resource type.
     :vartype type: str
@@ -782,15 +780,15 @@
 
 
 class HybridComputePrivateLinkScope(PrivateLinkScopesResource):
     """An Azure Arc PrivateLinkScope definition.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar id: Azure resource Id.
     :vartype id: str
     :ivar name: Azure resource name.
     :vartype name: str
     :ivar type: Azure resource type.
     :vartype type: str
@@ -842,15 +840,15 @@
         self.properties = properties
         self.system_data = None
 
 
 class HybridComputePrivateLinkScopeListResult(_serialization.Model):
     """Describes the list of Azure Arc PrivateLinkScope resources.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar value: List of Azure Arc PrivateLinkScope definitions. Required.
     :vartype value: list[~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope]
     :ivar next_link: The URI to get the next set of Azure Arc PrivateLinkScope definitions if too
      many PrivateLinkScopes where returned in the result set.
     :vartype next_link: str
     """
@@ -933,15 +931,15 @@
 
 class HybridIdentityMetadata(ProxyResource):
     """Defines the HybridIdentityMetadata.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -985,15 +983,15 @@
         self.public_key = public_key
         self.identity = None
 
 
 class HybridIdentityMetadataList(_serialization.Model):
     """List of HybridIdentityMetadata.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar next_link: Url to follow for getting next page of HybridIdentityMetadata.
     :vartype next_link: str
     :ivar value: Array of HybridIdentityMetadata. Required.
     :vartype value: list[~azure.mgmt.hybridcompute.models.HybridIdentityMetadata]
     """
 
@@ -1089,24 +1087,85 @@
         """
         super().__init__(**kwargs)
         self.address = address
         self.ip_address_version = ip_address_version
         self.subnet = None
 
 
+class KeyDetails(_serialization.Model):
+    """Public key details.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar public_key: Public key.
+    :vartype public_key: str
+    :ivar not_after: Key expiration date.
+    :vartype not_after: ~datetime.datetime
+    :ivar renew_after: Recommended key renewal date.
+    :vartype renew_after: ~datetime.datetime
+    """
+
+    _validation = {
+        "public_key": {"readonly": True},
+        "not_after": {"readonly": True},
+        "renew_after": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "public_key": {"key": "publicKey", "type": "str"},
+        "not_after": {"key": "notAfter", "type": "iso-8601"},
+        "renew_after": {"key": "renewAfter", "type": "iso-8601"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.public_key = None
+        self.not_after = None
+        self.renew_after = None
+
+
+class KeyProperties(_serialization.Model):
+    """Public key information for client authentication.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar client_public_key: Current public key details.
+    :vartype client_public_key: ~azure.mgmt.hybridcompute.models.KeyDetails
+    :ivar candidate_public_key: Candidate public key details.
+    :vartype candidate_public_key: ~azure.mgmt.hybridcompute.models.KeyDetails
+    """
+
+    _validation = {
+        "client_public_key": {"readonly": True},
+        "candidate_public_key": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "client_public_key": {"key": "clientPublicKey", "type": "KeyDetails"},
+        "candidate_public_key": {"key": "candidatePublicKey", "type": "KeyDetails"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.client_public_key = None
+        self.candidate_public_key = None
+
+
 class TrackedResource(Resource):
     """The resource model definition for an Azure Resource Manager tracked top level resource which
     has 'tags' and a 'location'.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -1148,18 +1207,18 @@
 
 
 class License(TrackedResource):
     """Describes a license in a hybrid machine.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -1309,18 +1368,18 @@
 
 
 class LicenseProfile(TrackedResource):  # pylint: disable=too-many-instance-attributes
     """Describes a license profile in a hybrid machine.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -1330,37 +1389,58 @@
     :vartype tags: dict[str, str]
     :ivar location: The geo-location where the resource lives. Required.
     :vartype location: str
     :ivar provisioning_state: The provisioning state, which only appears in the response. Known
      values are: "Creating", "Updating", "Deleting", "Succeeded", "Failed", "Accepted", "Canceled",
      and "Deleted".
     :vartype provisioning_state: str or ~azure.mgmt.hybridcompute.models.ProvisioningState
+    :ivar subscription_status: Indicates the subscription status of the product. Known values are:
+     "Unknown", "Enabling", "Enabled", and "Disabled".
+    :vartype subscription_status: str or
+     ~azure.mgmt.hybridcompute.models.LicenseProfileSubscriptionStatus
+    :ivar product_type: Indicates the product type of the license. Known values are:
+     "WindowsServer" and "WindowsIoTEnterprise".
+    :vartype product_type: str or ~azure.mgmt.hybridcompute.models.LicenseProfileProductType
+    :ivar billing_start_date: The timestamp in UTC when the billing starts.
+    :vartype billing_start_date: ~datetime.datetime
+    :ivar enrollment_date: The timestamp in UTC when the user enrolls the feature.
+    :vartype enrollment_date: ~datetime.datetime
+    :ivar disenrollment_date: The timestamp in UTC when the user disenrolled the feature.
+    :vartype disenrollment_date: ~datetime.datetime
+    :ivar product_features: The list of product features.
+    :vartype product_features: list[~azure.mgmt.hybridcompute.models.ProductFeature]
     :ivar assigned_license_immutable_id: The guid id of the license.
     :vartype assigned_license_immutable_id: str
     :ivar esu_keys: The list of ESU keys.
     :vartype esu_keys: list[~azure.mgmt.hybridcompute.models.EsuKey]
     :ivar server_type: The type of the Esu servers. Known values are: "Standard" and "Datacenter".
     :vartype server_type: str or ~azure.mgmt.hybridcompute.models.EsuServerType
     :ivar esu_eligibility: Indicates the eligibility state of Esu. Known values are: "Eligible",
      "Ineligible", and "Unknown".
     :vartype esu_eligibility: str or ~azure.mgmt.hybridcompute.models.EsuEligibility
     :ivar esu_key_state: Indicates whether there is an ESU Key currently active for the machine.
      Known values are: "Inactive" and "Active".
     :vartype esu_key_state: str or ~azure.mgmt.hybridcompute.models.EsuKeyState
     :ivar assigned_license: The resource id of the license.
     :vartype assigned_license: str
+    :ivar software_assurance_customer: Specifies if this machine is licensed as part of a Software
+     Assurance agreement.
+    :vartype software_assurance_customer: bool
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "system_data": {"readonly": True},
         "location": {"required": True},
         "provisioning_state": {"readonly": True},
+        "billing_start_date": {"readonly": True},
+        "enrollment_date": {"readonly": True},
+        "disenrollment_date": {"readonly": True},
         "assigned_license_immutable_id": {"readonly": True},
         "esu_keys": {"readonly": True},
         "server_type": {"readonly": True},
         "esu_eligibility": {"readonly": True},
         "esu_key_state": {"readonly": True},
     }
 
@@ -1368,46 +1448,79 @@
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "system_data": {"key": "systemData", "type": "SystemData"},
         "tags": {"key": "tags", "type": "{str}"},
         "location": {"key": "location", "type": "str"},
         "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
+        "subscription_status": {"key": "properties.productProfile.subscriptionStatus", "type": "str"},
+        "product_type": {"key": "properties.productProfile.productType", "type": "str"},
+        "billing_start_date": {"key": "properties.productProfile.billingStartDate", "type": "iso-8601"},
+        "enrollment_date": {"key": "properties.productProfile.enrollmentDate", "type": "iso-8601"},
+        "disenrollment_date": {"key": "properties.productProfile.disenrollmentDate", "type": "iso-8601"},
+        "product_features": {"key": "properties.productProfile.productFeatures", "type": "[ProductFeature]"},
         "assigned_license_immutable_id": {"key": "properties.esuProfile.assignedLicenseImmutableId", "type": "str"},
         "esu_keys": {"key": "properties.esuProfile.esuKeys", "type": "[EsuKey]"},
         "server_type": {"key": "properties.esuProfile.serverType", "type": "str"},
         "esu_eligibility": {"key": "properties.esuProfile.esuEligibility", "type": "str"},
         "esu_key_state": {"key": "properties.esuProfile.esuKeyState", "type": "str"},
         "assigned_license": {"key": "properties.esuProfile.assignedLicense", "type": "str"},
+        "software_assurance_customer": {
+            "key": "properties.softwareAssurance.softwareAssuranceCustomer",
+            "type": "bool",
+        },
     }
 
     def __init__(
         self,
         *,
         location: str,
         tags: Optional[Dict[str, str]] = None,
+        subscription_status: Optional[Union[str, "_models.LicenseProfileSubscriptionStatus"]] = None,
+        product_type: Optional[Union[str, "_models.LicenseProfileProductType"]] = None,
+        product_features: Optional[List["_models.ProductFeature"]] = None,
         assigned_license: Optional[str] = None,
+        software_assurance_customer: Optional[bool] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         :keyword location: The geo-location where the resource lives. Required.
         :paramtype location: str
+        :keyword subscription_status: Indicates the subscription status of the product. Known values
+         are: "Unknown", "Enabling", "Enabled", and "Disabled".
+        :paramtype subscription_status: str or
+         ~azure.mgmt.hybridcompute.models.LicenseProfileSubscriptionStatus
+        :keyword product_type: Indicates the product type of the license. Known values are:
+         "WindowsServer" and "WindowsIoTEnterprise".
+        :paramtype product_type: str or ~azure.mgmt.hybridcompute.models.LicenseProfileProductType
+        :keyword product_features: The list of product features.
+        :paramtype product_features: list[~azure.mgmt.hybridcompute.models.ProductFeature]
         :keyword assigned_license: The resource id of the license.
         :paramtype assigned_license: str
+        :keyword software_assurance_customer: Specifies if this machine is licensed as part of a
+         Software Assurance agreement.
+        :paramtype software_assurance_customer: bool
         """
         super().__init__(tags=tags, location=location, **kwargs)
         self.provisioning_state = None
+        self.subscription_status = subscription_status
+        self.product_type = product_type
+        self.billing_start_date = None
+        self.enrollment_date = None
+        self.disenrollment_date = None
+        self.product_features = product_features
         self.assigned_license_immutable_id = None
         self.esu_keys = None
         self.server_type = None
         self.esu_eligibility = None
         self.esu_key_state = None
         self.assigned_license = assigned_license
+        self.software_assurance_customer = software_assurance_customer
 
 
 class LicenseProfileStorageModelEsuProperties(_serialization.Model):
     """License profile storage model for ESU properties.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
@@ -1430,15 +1543,17 @@
     def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.assigned_license_immutable_id = None
         self.esu_keys = None
 
 
-class LicenseProfileArmEsuPropertiesWithoutAssignedLicense(LicenseProfileStorageModelEsuProperties):
+class LicenseProfileArmEsuPropertiesWithoutAssignedLicense(
+    LicenseProfileStorageModelEsuProperties
+):  # pylint: disable=name-too-long
     """Describes the properties of a License Profile ARM model.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar assigned_license_immutable_id: The guid id of the license.
     :vartype assigned_license_immutable_id: str
     :ivar esu_keys: The list of ESU keys.
@@ -1523,36 +1638,108 @@
         super().__init__(**kwargs)
         self.assigned_license = assigned_license
 
 
 class LicenseProfileMachineInstanceView(_serialization.Model):
     """License Profile Instance View in Machine Properties.
 
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar license_status: Indicates the license status of the OS. Known values are: "Unlicensed",
+     "Licensed", "OOBGrace", "OOTGrace", "NonGenuineGrace", "Notification", and "ExtendedGrace".
+    :vartype license_status: str or ~azure.mgmt.hybridcompute.models.LicenseStatus
+    :ivar license_channel: Indicates the license channel.
+    :vartype license_channel: str
     :ivar esu_profile: Properties for the Machine ESU profile.
     :vartype esu_profile:
      ~azure.mgmt.hybridcompute.models.LicenseProfileMachineInstanceViewEsuProperties
+    :ivar subscription_status: Indicates the subscription status of the product. Known values are:
+     "Unknown", "Enabling", "Enabled", and "Disabled".
+    :vartype subscription_status: str or
+     ~azure.mgmt.hybridcompute.models.LicenseProfileSubscriptionStatus
+    :ivar product_type: Indicates the product type of the license. Known values are:
+     "WindowsServer" and "WindowsIoTEnterprise".
+    :vartype product_type: str or ~azure.mgmt.hybridcompute.models.LicenseProfileProductType
+    :ivar billing_start_date: The timestamp in UTC when the billing starts.
+    :vartype billing_start_date: ~datetime.datetime
+    :ivar enrollment_date: The timestamp in UTC when the user enrolls the feature.
+    :vartype enrollment_date: ~datetime.datetime
+    :ivar disenrollment_date: The timestamp in UTC when the user disenrolled the feature.
+    :vartype disenrollment_date: ~datetime.datetime
+    :ivar product_features: The list of product features.
+    :vartype product_features: list[~azure.mgmt.hybridcompute.models.ProductFeature]
+    :ivar software_assurance_customer: Specifies if this machine is licensed as part of a Software
+     Assurance agreement.
+    :vartype software_assurance_customer: bool
     """
 
+    _validation = {
+        "license_status": {"readonly": True},
+        "license_channel": {"readonly": True},
+        "billing_start_date": {"readonly": True},
+        "enrollment_date": {"readonly": True},
+        "disenrollment_date": {"readonly": True},
+    }
+
     _attribute_map = {
+        "license_status": {"key": "licenseStatus", "type": "str"},
+        "license_channel": {"key": "licenseChannel", "type": "str"},
         "esu_profile": {"key": "esuProfile", "type": "LicenseProfileMachineInstanceViewEsuProperties"},
+        "subscription_status": {"key": "productProfile.subscriptionStatus", "type": "str"},
+        "product_type": {"key": "productProfile.productType", "type": "str"},
+        "billing_start_date": {"key": "productProfile.billingStartDate", "type": "iso-8601"},
+        "enrollment_date": {"key": "productProfile.enrollmentDate", "type": "iso-8601"},
+        "disenrollment_date": {"key": "productProfile.disenrollmentDate", "type": "iso-8601"},
+        "product_features": {"key": "productProfile.productFeatures", "type": "[ProductFeature]"},
+        "software_assurance_customer": {"key": "softwareAssurance.softwareAssuranceCustomer", "type": "bool"},
     }
 
     def __init__(
-        self, *, esu_profile: Optional["_models.LicenseProfileMachineInstanceViewEsuProperties"] = None, **kwargs: Any
+        self,
+        *,
+        esu_profile: Optional["_models.LicenseProfileMachineInstanceViewEsuProperties"] = None,
+        subscription_status: Optional[Union[str, "_models.LicenseProfileSubscriptionStatus"]] = None,
+        product_type: Optional[Union[str, "_models.LicenseProfileProductType"]] = None,
+        product_features: Optional[List["_models.ProductFeature"]] = None,
+        software_assurance_customer: Optional[bool] = None,
+        **kwargs: Any
     ) -> None:
         """
         :keyword esu_profile: Properties for the Machine ESU profile.
         :paramtype esu_profile:
          ~azure.mgmt.hybridcompute.models.LicenseProfileMachineInstanceViewEsuProperties
+        :keyword subscription_status: Indicates the subscription status of the product. Known values
+         are: "Unknown", "Enabling", "Enabled", and "Disabled".
+        :paramtype subscription_status: str or
+         ~azure.mgmt.hybridcompute.models.LicenseProfileSubscriptionStatus
+        :keyword product_type: Indicates the product type of the license. Known values are:
+         "WindowsServer" and "WindowsIoTEnterprise".
+        :paramtype product_type: str or ~azure.mgmt.hybridcompute.models.LicenseProfileProductType
+        :keyword product_features: The list of product features.
+        :paramtype product_features: list[~azure.mgmt.hybridcompute.models.ProductFeature]
+        :keyword software_assurance_customer: Specifies if this machine is licensed as part of a
+         Software Assurance agreement.
+        :paramtype software_assurance_customer: bool
         """
         super().__init__(**kwargs)
+        self.license_status = None
+        self.license_channel = None
         self.esu_profile = esu_profile
+        self.subscription_status = subscription_status
+        self.product_type = product_type
+        self.billing_start_date = None
+        self.enrollment_date = None
+        self.disenrollment_date = None
+        self.product_features = product_features
+        self.software_assurance_customer = software_assurance_customer
 
 
-class LicenseProfileMachineInstanceViewEsuProperties(LicenseProfileArmEsuPropertiesWithoutAssignedLicense):
+class LicenseProfileMachineInstanceViewEsuProperties(
+    LicenseProfileArmEsuPropertiesWithoutAssignedLicense
+):  # pylint: disable=name-too-long
     """Properties for the Machine ESU profile.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar assigned_license_immutable_id: The guid id of the license.
     :vartype assigned_license_immutable_id: str
     :ivar esu_keys: The list of ESU keys.
@@ -1610,15 +1797,15 @@
         self.assigned_license = assigned_license
         self.license_assignment_state = license_assignment_state
 
 
 class LicenseProfilesListResult(_serialization.Model):
     """The List hybrid machine license profile operation response.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar value: The list of license profiles. Required.
     :vartype value: list[~azure.mgmt.hybridcompute.models.LicenseProfile]
     :ivar next_link: The URI to fetch the next page of Machines. Call ListNext() with this URI to
      fetch the next page of license profile.
     :vartype next_link: str
     """
@@ -1668,40 +1855,83 @@
 
 
 class LicenseProfileUpdate(ResourceUpdate):
     """Describes a License Profile Update.
 
     :ivar tags: Resource tags.
     :vartype tags: dict[str, str]
+    :ivar subscription_status: Indicates the subscription status of the product. Known values are:
+     "Enable" and "Disable".
+    :vartype subscription_status: str or
+     ~azure.mgmt.hybridcompute.models.LicenseProfileSubscriptionStatusUpdate
+    :ivar product_type: Indicates the product type of the license. Known values are:
+     "WindowsServer" and "WindowsIoTEnterprise".
+    :vartype product_type: str or ~azure.mgmt.hybridcompute.models.LicenseProfileProductType
+    :ivar product_features: The list of product feature updates.
+    :vartype product_features: list[~azure.mgmt.hybridcompute.models.ProductFeatureUpdate]
     :ivar assigned_license: The resource id of the license.
     :vartype assigned_license: str
+    :ivar software_assurance_customer: Specifies if this machine is licensed as part of a Software
+     Assurance agreement.
+    :vartype software_assurance_customer: bool
     """
 
     _attribute_map = {
         "tags": {"key": "tags", "type": "{str}"},
+        "subscription_status": {"key": "properties.productProfile.subscriptionStatus", "type": "str"},
+        "product_type": {"key": "properties.productProfile.productType", "type": "str"},
+        "product_features": {"key": "properties.productProfile.productFeatures", "type": "[ProductFeatureUpdate]"},
         "assigned_license": {"key": "properties.esuProfile.assignedLicense", "type": "str"},
+        "software_assurance_customer": {
+            "key": "properties.softwareAssurance.softwareAssuranceCustomer",
+            "type": "bool",
+        },
     }
 
     def __init__(
-        self, *, tags: Optional[Dict[str, str]] = None, assigned_license: Optional[str] = None, **kwargs: Any
+        self,
+        *,
+        tags: Optional[Dict[str, str]] = None,
+        subscription_status: Optional[Union[str, "_models.LicenseProfileSubscriptionStatusUpdate"]] = None,
+        product_type: Optional[Union[str, "_models.LicenseProfileProductType"]] = None,
+        product_features: Optional[List["_models.ProductFeatureUpdate"]] = None,
+        assigned_license: Optional[str] = None,
+        software_assurance_customer: Optional[bool] = None,
+        **kwargs: Any
     ) -> None:
         """
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
+        :keyword subscription_status: Indicates the subscription status of the product. Known values
+         are: "Enable" and "Disable".
+        :paramtype subscription_status: str or
+         ~azure.mgmt.hybridcompute.models.LicenseProfileSubscriptionStatusUpdate
+        :keyword product_type: Indicates the product type of the license. Known values are:
+         "WindowsServer" and "WindowsIoTEnterprise".
+        :paramtype product_type: str or ~azure.mgmt.hybridcompute.models.LicenseProfileProductType
+        :keyword product_features: The list of product feature updates.
+        :paramtype product_features: list[~azure.mgmt.hybridcompute.models.ProductFeatureUpdate]
         :keyword assigned_license: The resource id of the license.
         :paramtype assigned_license: str
+        :keyword software_assurance_customer: Specifies if this machine is licensed as part of a
+         Software Assurance agreement.
+        :paramtype software_assurance_customer: bool
         """
         super().__init__(tags=tags, **kwargs)
+        self.subscription_status = subscription_status
+        self.product_type = product_type
+        self.product_features = product_features
         self.assigned_license = assigned_license
+        self.software_assurance_customer = software_assurance_customer
 
 
 class LicensesListResult(_serialization.Model):
     """The List license operation response.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar value: The list of licenses. Required.
     :vartype value: list[~azure.mgmt.hybridcompute.models.License]
     :ivar next_link: The URI to fetch the next page of Machines. Call ListNext() with this URI to
      fetch the next page of license profile.
     :vartype next_link: str
     """
@@ -1848,15 +2078,15 @@
         self.package_name_masks_to_include = package_name_masks_to_include
         self.package_name_masks_to_exclude = package_name_masks_to_exclude
 
 
 class LocationData(_serialization.Model):
     """Metadata pertaining to the geographic location of the resource.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar name: A canonical name for the geographic or physical location. Required.
     :vartype name: str
     :ivar city: The city or locality where the resource is located.
     :vartype city: str
     :ivar district: The district, state, or province where the resource is located.
     :vartype district: str
@@ -1902,18 +2132,18 @@
 
 
 class Machine(TrackedResource):  # pylint: disable=too-many-instance-attributes
     """Describes a hybrid machine.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -1939,15 +2169,15 @@
     :vartype service_statuses: ~azure.mgmt.hybridcompute.models.ServiceStatuses
     :ivar cloud_metadata: The metadata of the cloud environment (Azure/GCP/AWS/OCI...).
     :vartype cloud_metadata: ~azure.mgmt.hybridcompute.models.CloudMetadata
     :ivar agent_upgrade: The info of the machine w.r.t Agent Upgrade.
     :vartype agent_upgrade: ~azure.mgmt.hybridcompute.models.AgentUpgrade
     :ivar os_profile: Specifies the operating system settings for the hybrid machine.
     :vartype os_profile: ~azure.mgmt.hybridcompute.models.OSProfile
-    :ivar license_profile: Specifies the ESU related properties for a machine.
+    :ivar license_profile: Specifies the License related properties for a machine.
     :vartype license_profile: ~azure.mgmt.hybridcompute.models.LicenseProfileMachineInstanceView
     :ivar provisioning_state: The provisioning state, which only appears in the response.
     :vartype provisioning_state: str
     :ivar status: The status of the hybrid machine agent. Known values are: "Connected",
      "Disconnected", and "Error".
     :vartype status: str or ~azure.mgmt.hybridcompute.models.StatusTypes
     :ivar last_status_change: The time of the last status change.
@@ -1973,14 +2203,16 @@
     :vartype os_type: str
     :ivar vm_uuid: Specifies the Arc Machine's unique SMBIOS ID.
     :vartype vm_uuid: str
     :ivar extensions: Machine Extensions information (deprecated field).
     :vartype extensions: list[~azure.mgmt.hybridcompute.models.MachineExtensionInstanceView]
     :ivar os_sku: Specifies the Operating System product SKU.
     :vartype os_sku: str
+    :ivar os_edition: The edition of the Operating System.
+    :vartype os_edition: str
     :ivar domain_name: Specifies the Windows domain name.
     :vartype domain_name: str
     :ivar ad_fqdn: Specifies the AD fully qualified display name.
     :vartype ad_fqdn: str
     :ivar dns_fqdn: Specifies the DNS fully qualified display name.
     :vartype dns_fqdn: str
     :ivar private_link_scope_resource_id: The resource id of the private link scope this machine is
@@ -2012,14 +2244,15 @@
         "agent_version": {"readonly": True},
         "display_name": {"readonly": True},
         "machine_fqdn": {"readonly": True},
         "os_name": {"readonly": True},
         "os_version": {"readonly": True},
         "vm_uuid": {"readonly": True},
         "os_sku": {"readonly": True},
+        "os_edition": {"readonly": True},
         "domain_name": {"readonly": True},
         "ad_fqdn": {"readonly": True},
         "dns_fqdn": {"readonly": True},
         "detected_properties": {"readonly": True},
         "network_profile": {"readonly": True},
     }
 
@@ -2051,14 +2284,15 @@
         "client_public_key": {"key": "properties.clientPublicKey", "type": "str"},
         "os_name": {"key": "properties.osName", "type": "str"},
         "os_version": {"key": "properties.osVersion", "type": "str"},
         "os_type": {"key": "properties.osType", "type": "str"},
         "vm_uuid": {"key": "properties.vmUuid", "type": "str"},
         "extensions": {"key": "properties.extensions", "type": "[MachineExtensionInstanceView]"},
         "os_sku": {"key": "properties.osSku", "type": "str"},
+        "os_edition": {"key": "properties.osEdition", "type": "str"},
         "domain_name": {"key": "properties.domainName", "type": "str"},
         "ad_fqdn": {"key": "properties.adFqdn", "type": "str"},
         "dns_fqdn": {"key": "properties.dnsFqdn", "type": "str"},
         "private_link_scope_resource_id": {"key": "properties.privateLinkScopeResourceId", "type": "str"},
         "parent_cluster_resource_id": {"key": "properties.parentClusterResourceId", "type": "str"},
         "mssql_discovered": {"key": "properties.mssqlDiscovered", "type": "str"},
         "detected_properties": {"key": "properties.detectedProperties", "type": "{str}"},
@@ -2103,15 +2337,15 @@
         :paramtype service_statuses: ~azure.mgmt.hybridcompute.models.ServiceStatuses
         :keyword cloud_metadata: The metadata of the cloud environment (Azure/GCP/AWS/OCI...).
         :paramtype cloud_metadata: ~azure.mgmt.hybridcompute.models.CloudMetadata
         :keyword agent_upgrade: The info of the machine w.r.t Agent Upgrade.
         :paramtype agent_upgrade: ~azure.mgmt.hybridcompute.models.AgentUpgrade
         :keyword os_profile: Specifies the operating system settings for the hybrid machine.
         :paramtype os_profile: ~azure.mgmt.hybridcompute.models.OSProfile
-        :keyword license_profile: Specifies the ESU related properties for a machine.
+        :keyword license_profile: Specifies the License related properties for a machine.
         :paramtype license_profile: ~azure.mgmt.hybridcompute.models.LicenseProfileMachineInstanceView
         :keyword vm_id: Specifies the hybrid machine unique ID.
         :paramtype vm_id: str
         :keyword client_public_key: Public Key that the client provides to be used during initial
          resource onboarding.
         :paramtype client_public_key: str
         :keyword os_type: The type of Operating System (windows/linux).
@@ -2149,14 +2383,15 @@
         self.client_public_key = client_public_key
         self.os_name = None
         self.os_version = None
         self.os_type = os_type
         self.vm_uuid = None
         self.extensions = extensions
         self.os_sku = None
+        self.os_edition = None
         self.domain_name = None
         self.ad_fqdn = None
         self.dns_fqdn = None
         self.private_link_scope_resource_id = private_link_scope_resource_id
         self.parent_cluster_resource_id = parent_cluster_resource_id
         self.mssql_discovered = mssql_discovered
         self.detected_properties = None
@@ -2255,18 +2490,18 @@
 
 
 class MachineExtension(TrackedResource):
     """Describes a Machine Extension.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -2665,19 +2900,19 @@
         super().__init__(**kwargs)
         self.extension_targets = extension_targets
 
 
 class MachineInstallPatchesParameters(_serialization.Model):
     """Input for InstallPatches as directly received by the API.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar maximum_duration: Specifies the maximum amount of time that the operation will run. It
      must be an ISO 8601-compliant duration string such as PT4H (4 hours). Required.
-    :vartype maximum_duration: str
+    :vartype maximum_duration: ~datetime.timedelta
     :ivar reboot_setting: Defines when it is acceptable to reboot a VM during a software update
      operation. Required. Known values are: "IfRequired", "Never", and "Always".
     :vartype reboot_setting: str or ~azure.mgmt.hybridcompute.models.VMGuestPatchRebootSetting
     :ivar windows_parameters: Input for InstallPatches on a Windows VM, as directly received by the
      API.
     :vartype windows_parameters: ~azure.mgmt.hybridcompute.models.WindowsParameters
     :ivar linux_parameters: Input for InstallPatches on a Linux VM, as directly received by the
@@ -2687,33 +2922,33 @@
 
     _validation = {
         "maximum_duration": {"required": True},
         "reboot_setting": {"required": True},
     }
 
     _attribute_map = {
-        "maximum_duration": {"key": "maximumDuration", "type": "str"},
+        "maximum_duration": {"key": "maximumDuration", "type": "duration"},
         "reboot_setting": {"key": "rebootSetting", "type": "str"},
         "windows_parameters": {"key": "windowsParameters", "type": "WindowsParameters"},
         "linux_parameters": {"key": "linuxParameters", "type": "LinuxParameters"},
     }
 
     def __init__(
         self,
         *,
-        maximum_duration: str,
+        maximum_duration: datetime.timedelta,
         reboot_setting: Union[str, "_models.VMGuestPatchRebootSetting"],
         windows_parameters: Optional["_models.WindowsParameters"] = None,
         linux_parameters: Optional["_models.LinuxParameters"] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword maximum_duration: Specifies the maximum amount of time that the operation will run. It
          must be an ISO 8601-compliant duration string such as PT4H (4 hours). Required.
-        :paramtype maximum_duration: str
+        :paramtype maximum_duration: ~datetime.timedelta
         :keyword reboot_setting: Defines when it is acceptable to reboot a VM during a software update
          operation. Required. Known values are: "IfRequired", "Never", and "Always".
         :paramtype reboot_setting: str or ~azure.mgmt.hybridcompute.models.VMGuestPatchRebootSetting
         :keyword windows_parameters: Input for InstallPatches on a Windows VM, as directly received by
          the API.
         :paramtype windows_parameters: ~azure.mgmt.hybridcompute.models.WindowsParameters
         :keyword linux_parameters: Input for InstallPatches on a Linux VM, as directly received by the
@@ -2833,15 +3068,15 @@
         self.os_type = None
         self.error_details = None
 
 
 class MachineListResult(_serialization.Model):
     """The List hybrid machine operation response.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar value: The list of hybrid machines. Required.
     :vartype value: list[~azure.mgmt.hybridcompute.models.Machine]
     :ivar next_link: The URI to fetch the next page of Machines. Call ListNext() with this URI to
      fetch the next page of hybrid machines.
     :vartype next_link: str
     """
@@ -2864,14 +3099,379 @@
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
 
+class MachineRunCommand(TrackedResource):  # pylint: disable=too-many-instance-attributes
+    """Describes a Run Command.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar id: Fully qualified resource ID for the resource. Ex -
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.hybridcompute.models.SystemData
+    :ivar tags: Resource tags.
+    :vartype tags: dict[str, str]
+    :ivar location: The geo-location where the resource lives. Required.
+    :vartype location: str
+    :ivar source: The source of the run command script.
+    :vartype source: ~azure.mgmt.hybridcompute.models.MachineRunCommandScriptSource
+    :ivar parameters: The parameters used by the script.
+    :vartype parameters: list[~azure.mgmt.hybridcompute.models.RunCommandInputParameter]
+    :ivar protected_parameters: The parameters used by the script.
+    :vartype protected_parameters: list[~azure.mgmt.hybridcompute.models.RunCommandInputParameter]
+    :ivar async_execution: Optional. If set to true, provisioning will complete as soon as script
+     starts and will not wait for script to complete.
+    :vartype async_execution: bool
+    :ivar run_as_user: Specifies the user account on the machine when executing the run command.
+    :vartype run_as_user: str
+    :ivar run_as_password: Specifies the user account password on the machine when executing the
+     run command.
+    :vartype run_as_password: str
+    :ivar timeout_in_seconds: The timeout in seconds to execute the run command.
+    :vartype timeout_in_seconds: int
+    :ivar output_blob_uri: Specifies the Azure storage blob where script output stream will be
+     uploaded. Use a SAS URI with read, append, create, write access OR use managed identity to
+     provide the VM access to the blob. Refer outputBlobManagedIdentity parameter.
+    :vartype output_blob_uri: str
+    :ivar error_blob_uri: Specifies the Azure storage blob where script error stream will be
+     uploaded. Use a SAS URI with read, append, create, write access OR use managed identity to
+     provide the VM access to the blob. Refer errorBlobManagedIdentity parameter.
+    :vartype error_blob_uri: str
+    :ivar output_blob_managed_identity: User-assigned managed identity that has access to
+     outputBlobUri storage blob. Use an empty object in case of system-assigned identity. Make sure
+     managed identity has been given access to blob's container with 'Storage Blob Data Contributor'
+     role assignment. In case of user-assigned identity, make sure you add it under VM's identity.
+     For more info on managed identity and Run Command, refer https://aka.ms/ManagedIdentity and
+     https://aka.ms/RunCommandManaged.
+    :vartype output_blob_managed_identity:
+     ~azure.mgmt.hybridcompute.models.RunCommandManagedIdentity
+    :ivar error_blob_managed_identity: User-assigned managed identity that has access to
+     errorBlobUri storage blob. Use an empty object in case of system-assigned identity. Make sure
+     managed identity has been given access to blob's container with 'Storage Blob Data Contributor'
+     role assignment. In case of user-assigned identity, make sure you add it under VM's identity.
+     For more info on managed identity and Run Command, refer https://aka.ms/ManagedIdentity and
+     https://aka.ms/RunCommandManaged.
+    :vartype error_blob_managed_identity:
+     ~azure.mgmt.hybridcompute.models.RunCommandManagedIdentity
+    :ivar provisioning_state: The provisioning state, which only appears in the response.
+    :vartype provisioning_state: str
+    :ivar instance_view: The machine run command instance view.
+    :vartype instance_view: ~azure.mgmt.hybridcompute.models.MachineRunCommandInstanceView
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+        "location": {"required": True},
+        "provisioning_state": {"readonly": True},
+        "instance_view": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+        "tags": {"key": "tags", "type": "{str}"},
+        "location": {"key": "location", "type": "str"},
+        "source": {"key": "properties.source", "type": "MachineRunCommandScriptSource"},
+        "parameters": {"key": "properties.parameters", "type": "[RunCommandInputParameter]"},
+        "protected_parameters": {"key": "properties.protectedParameters", "type": "[RunCommandInputParameter]"},
+        "async_execution": {"key": "properties.asyncExecution", "type": "bool"},
+        "run_as_user": {"key": "properties.runAsUser", "type": "str"},
+        "run_as_password": {"key": "properties.runAsPassword", "type": "str"},
+        "timeout_in_seconds": {"key": "properties.timeoutInSeconds", "type": "int"},
+        "output_blob_uri": {"key": "properties.outputBlobUri", "type": "str"},
+        "error_blob_uri": {"key": "properties.errorBlobUri", "type": "str"},
+        "output_blob_managed_identity": {
+            "key": "properties.outputBlobManagedIdentity",
+            "type": "RunCommandManagedIdentity",
+        },
+        "error_blob_managed_identity": {
+            "key": "properties.errorBlobManagedIdentity",
+            "type": "RunCommandManagedIdentity",
+        },
+        "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
+        "instance_view": {"key": "properties.instanceView", "type": "MachineRunCommandInstanceView"},
+    }
+
+    def __init__(
+        self,
+        *,
+        location: str,
+        tags: Optional[Dict[str, str]] = None,
+        source: Optional["_models.MachineRunCommandScriptSource"] = None,
+        parameters: Optional[List["_models.RunCommandInputParameter"]] = None,
+        protected_parameters: Optional[List["_models.RunCommandInputParameter"]] = None,
+        async_execution: bool = False,
+        run_as_user: Optional[str] = None,
+        run_as_password: Optional[str] = None,
+        timeout_in_seconds: Optional[int] = None,
+        output_blob_uri: Optional[str] = None,
+        error_blob_uri: Optional[str] = None,
+        output_blob_managed_identity: Optional["_models.RunCommandManagedIdentity"] = None,
+        error_blob_managed_identity: Optional["_models.RunCommandManagedIdentity"] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword tags: Resource tags.
+        :paramtype tags: dict[str, str]
+        :keyword location: The geo-location where the resource lives. Required.
+        :paramtype location: str
+        :keyword source: The source of the run command script.
+        :paramtype source: ~azure.mgmt.hybridcompute.models.MachineRunCommandScriptSource
+        :keyword parameters: The parameters used by the script.
+        :paramtype parameters: list[~azure.mgmt.hybridcompute.models.RunCommandInputParameter]
+        :keyword protected_parameters: The parameters used by the script.
+        :paramtype protected_parameters:
+         list[~azure.mgmt.hybridcompute.models.RunCommandInputParameter]
+        :keyword async_execution: Optional. If set to true, provisioning will complete as soon as
+         script starts and will not wait for script to complete.
+        :paramtype async_execution: bool
+        :keyword run_as_user: Specifies the user account on the machine when executing the run command.
+        :paramtype run_as_user: str
+        :keyword run_as_password: Specifies the user account password on the machine when executing the
+         run command.
+        :paramtype run_as_password: str
+        :keyword timeout_in_seconds: The timeout in seconds to execute the run command.
+        :paramtype timeout_in_seconds: int
+        :keyword output_blob_uri: Specifies the Azure storage blob where script output stream will be
+         uploaded. Use a SAS URI with read, append, create, write access OR use managed identity to
+         provide the VM access to the blob. Refer outputBlobManagedIdentity parameter.
+        :paramtype output_blob_uri: str
+        :keyword error_blob_uri: Specifies the Azure storage blob where script error stream will be
+         uploaded. Use a SAS URI with read, append, create, write access OR use managed identity to
+         provide the VM access to the blob. Refer errorBlobManagedIdentity parameter.
+        :paramtype error_blob_uri: str
+        :keyword output_blob_managed_identity: User-assigned managed identity that has access to
+         outputBlobUri storage blob. Use an empty object in case of system-assigned identity. Make sure
+         managed identity has been given access to blob's container with 'Storage Blob Data Contributor'
+         role assignment. In case of user-assigned identity, make sure you add it under VM's identity.
+         For more info on managed identity and Run Command, refer https://aka.ms/ManagedIdentity and
+         https://aka.ms/RunCommandManaged.
+        :paramtype output_blob_managed_identity:
+         ~azure.mgmt.hybridcompute.models.RunCommandManagedIdentity
+        :keyword error_blob_managed_identity: User-assigned managed identity that has access to
+         errorBlobUri storage blob. Use an empty object in case of system-assigned identity. Make sure
+         managed identity has been given access to blob's container with 'Storage Blob Data Contributor'
+         role assignment. In case of user-assigned identity, make sure you add it under VM's identity.
+         For more info on managed identity and Run Command, refer https://aka.ms/ManagedIdentity and
+         https://aka.ms/RunCommandManaged.
+        :paramtype error_blob_managed_identity:
+         ~azure.mgmt.hybridcompute.models.RunCommandManagedIdentity
+        """
+        super().__init__(tags=tags, location=location, **kwargs)
+        self.source = source
+        self.parameters = parameters
+        self.protected_parameters = protected_parameters
+        self.async_execution = async_execution
+        self.run_as_user = run_as_user
+        self.run_as_password = run_as_password
+        self.timeout_in_seconds = timeout_in_seconds
+        self.output_blob_uri = output_blob_uri
+        self.error_blob_uri = error_blob_uri
+        self.output_blob_managed_identity = output_blob_managed_identity
+        self.error_blob_managed_identity = error_blob_managed_identity
+        self.provisioning_state = None
+        self.instance_view = None
+
+
+class MachineRunCommandInstanceView(_serialization.Model):
+    """The instance view of a machine run command.
+
+    :ivar execution_state: Script execution status. Known values are: "Unknown", "Pending",
+     "Running", "Failed", "Succeeded", "TimedOut", and "Canceled".
+    :vartype execution_state: str or ~azure.mgmt.hybridcompute.models.ExecutionState
+    :ivar execution_message: Communicate script configuration errors or execution messages.
+    :vartype execution_message: str
+    :ivar exit_code: Exit code returned from script execution.
+    :vartype exit_code: int
+    :ivar output: Script output stream.
+    :vartype output: str
+    :ivar error: Script error stream.
+    :vartype error: str
+    :ivar start_time: Script start time.
+    :vartype start_time: ~datetime.datetime
+    :ivar end_time: Script end time.
+    :vartype end_time: ~datetime.datetime
+    :ivar statuses: The  status information.
+    :vartype statuses: list[~azure.mgmt.hybridcompute.models.ExtensionsResourceStatus]
+    """
+
+    _attribute_map = {
+        "execution_state": {"key": "executionState", "type": "str"},
+        "execution_message": {"key": "executionMessage", "type": "str"},
+        "exit_code": {"key": "exitCode", "type": "int"},
+        "output": {"key": "output", "type": "str"},
+        "error": {"key": "error", "type": "str"},
+        "start_time": {"key": "startTime", "type": "iso-8601"},
+        "end_time": {"key": "endTime", "type": "iso-8601"},
+        "statuses": {"key": "statuses", "type": "[ExtensionsResourceStatus]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        execution_state: Optional[Union[str, "_models.ExecutionState"]] = None,
+        execution_message: Optional[str] = None,
+        exit_code: Optional[int] = None,
+        output: Optional[str] = None,
+        error: Optional[str] = None,
+        start_time: Optional[datetime.datetime] = None,
+        end_time: Optional[datetime.datetime] = None,
+        statuses: Optional[List["_models.ExtensionsResourceStatus"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword execution_state: Script execution status. Known values are: "Unknown", "Pending",
+         "Running", "Failed", "Succeeded", "TimedOut", and "Canceled".
+        :paramtype execution_state: str or ~azure.mgmt.hybridcompute.models.ExecutionState
+        :keyword execution_message: Communicate script configuration errors or execution messages.
+        :paramtype execution_message: str
+        :keyword exit_code: Exit code returned from script execution.
+        :paramtype exit_code: int
+        :keyword output: Script output stream.
+        :paramtype output: str
+        :keyword error: Script error stream.
+        :paramtype error: str
+        :keyword start_time: Script start time.
+        :paramtype start_time: ~datetime.datetime
+        :keyword end_time: Script end time.
+        :paramtype end_time: ~datetime.datetime
+        :keyword statuses: The  status information.
+        :paramtype statuses: list[~azure.mgmt.hybridcompute.models.ExtensionsResourceStatus]
+        """
+        super().__init__(**kwargs)
+        self.execution_state = execution_state
+        self.execution_message = execution_message
+        self.exit_code = exit_code
+        self.output = output
+        self.error = error
+        self.start_time = start_time
+        self.end_time = end_time
+        self.statuses = statuses
+
+
+class MachineRunCommandScriptSource(_serialization.Model):
+    """Describes the script sources for run command. Use only one of script, scriptUri, commandId.
+
+    :ivar script: Specifies the script content to be executed on the machine.
+    :vartype script: str
+    :ivar script_uri: Specifies the script download location. It can be either SAS URI of an Azure
+     storage blob with read access or public URI.
+    :vartype script_uri: str
+    :ivar command_id: Specifies the commandId of predefined built-in script.
+    :vartype command_id: str
+    :ivar script_uri_managed_identity: User-assigned managed identity that has access to scriptUri
+     in case of Azure storage blob. Use an empty object in case of system-assigned identity. Make
+     sure the Azure storage blob exists, and managed identity has been given access to blob's
+     container with 'Storage Blob Data Reader' role assignment. In case of user-assigned identity,
+     make sure you add it under VM's identity. For more info on managed identity and Run Command,
+     refer https://aka.ms/ManagedIdentity and https://aka.ms/RunCommandManaged.
+    :vartype script_uri_managed_identity:
+     ~azure.mgmt.hybridcompute.models.RunCommandManagedIdentity
+    """
+
+    _attribute_map = {
+        "script": {"key": "script", "type": "str"},
+        "script_uri": {"key": "scriptUri", "type": "str"},
+        "command_id": {"key": "commandId", "type": "str"},
+        "script_uri_managed_identity": {"key": "scriptUriManagedIdentity", "type": "RunCommandManagedIdentity"},
+    }
+
+    def __init__(
+        self,
+        *,
+        script: Optional[str] = None,
+        script_uri: Optional[str] = None,
+        command_id: Optional[str] = None,
+        script_uri_managed_identity: Optional["_models.RunCommandManagedIdentity"] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword script: Specifies the script content to be executed on the machine.
+        :paramtype script: str
+        :keyword script_uri: Specifies the script download location. It can be either SAS URI of an
+         Azure storage blob with read access or public URI.
+        :paramtype script_uri: str
+        :keyword command_id: Specifies the commandId of predefined built-in script.
+        :paramtype command_id: str
+        :keyword script_uri_managed_identity: User-assigned managed identity that has access to
+         scriptUri in case of Azure storage blob. Use an empty object in case of system-assigned
+         identity. Make sure the Azure storage blob exists, and managed identity has been given access
+         to blob's container with 'Storage Blob Data Reader' role assignment. In case of user-assigned
+         identity, make sure you add it under VM's identity. For more info on managed identity and Run
+         Command, refer https://aka.ms/ManagedIdentity and https://aka.ms/RunCommandManaged.
+        :paramtype script_uri_managed_identity:
+         ~azure.mgmt.hybridcompute.models.RunCommandManagedIdentity
+        """
+        super().__init__(**kwargs)
+        self.script = script
+        self.script_uri = script_uri
+        self.command_id = command_id
+        self.script_uri_managed_identity = script_uri_managed_identity
+
+
+class MachineRunCommandsListResult(_serialization.Model):
+    """Describes the Run Commands List Result.
+
+    :ivar value: The list of run commands.
+    :vartype value: list[~azure.mgmt.hybridcompute.models.MachineRunCommand]
+    :ivar next_link: The uri to fetch the next page of run commands. Call ListNext() with this to
+     fetch the next page of run commands.
+    :vartype next_link: str
+    """
+
+    _attribute_map = {
+        "value": {"key": "value", "type": "[MachineRunCommand]"},
+        "next_link": {"key": "nextLink", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        value: Optional[List["_models.MachineRunCommand"]] = None,
+        next_link: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword value: The list of run commands.
+        :paramtype value: list[~azure.mgmt.hybridcompute.models.MachineRunCommand]
+        :keyword next_link: The uri to fetch the next page of run commands. Call ListNext() with this
+         to fetch the next page of run commands.
+        :paramtype next_link: str
+        """
+        super().__init__(**kwargs)
+        self.value = value
+        self.next_link = next_link
+
+
+class MachineRunCommandUpdate(ResourceUpdate):
+    """Describes a Machine Extension Update.
+
+    :ivar tags: Resource tags.
+    :vartype tags: dict[str, str]
+    """
+
+
 class MachineUpdate(ResourceUpdate):
     """Describes a hybrid machine Update.
 
     :ivar tags: Resource tags.
     :vartype tags: dict[str, str]
     :ivar identity: Identity for the resource.
     :vartype identity: ~azure.mgmt.hybridcompute.models.Identity
@@ -2950,14 +3550,92 @@
         self.os_profile = os_profile
         self.cloud_metadata = cloud_metadata
         self.agent_upgrade = agent_upgrade
         self.parent_cluster_resource_id = parent_cluster_resource_id
         self.private_link_scope_resource_id = private_link_scope_resource_id
 
 
+class NetworkConfiguration(ProxyResource):
+    """NetworkConfiguration.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar id: Fully qualified resource ID for the resource. Ex -
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.hybridcompute.models.SystemData
+    :ivar location: Resource location.
+    :vartype location: str
+    :ivar tenant_id: Azure resource tenant Id.
+    :vartype tenant_id: str
+    :ivar network_configuration_scope_id: Associated Network Configuration Scope Id (GUID).
+    :vartype network_configuration_scope_id: str
+    :ivar network_configuration_scope_resource_id: Associated Network Configuration Scope Resource
+     Id.
+    :vartype network_configuration_scope_resource_id: str
+    :ivar key_properties: Public key information for client authentication.
+    :vartype key_properties: ~azure.mgmt.hybridcompute.models.KeyProperties
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+        "tenant_id": {"readonly": True},
+        "key_properties": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+        "location": {"key": "properties.location", "type": "str"},
+        "tenant_id": {"key": "properties.tenantId", "type": "str"},
+        "network_configuration_scope_id": {"key": "properties.networkConfigurationScopeId", "type": "str"},
+        "network_configuration_scope_resource_id": {
+            "key": "properties.networkConfigurationScopeResourceId",
+            "type": "str",
+        },
+        "key_properties": {"key": "properties.keyProperties", "type": "KeyProperties"},
+    }
+
+    def __init__(
+        self,
+        *,
+        location: Optional[str] = None,
+        network_configuration_scope_id: Optional[str] = None,
+        network_configuration_scope_resource_id: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword location: Resource location.
+        :paramtype location: str
+        :keyword network_configuration_scope_id: Associated Network Configuration Scope Id (GUID).
+        :paramtype network_configuration_scope_id: str
+        :keyword network_configuration_scope_resource_id: Associated Network Configuration Scope
+         Resource Id.
+        :paramtype network_configuration_scope_resource_id: str
+        """
+        super().__init__(**kwargs)
+        self.location = location
+        self.tenant_id = None
+        self.network_configuration_scope_id = network_configuration_scope_id
+        self.network_configuration_scope_resource_id = network_configuration_scope_resource_id
+        self.key_properties = None
+
+
 class NetworkInterface(_serialization.Model):
     """Describes a network interface.
 
     :ivar ip_addresses: The list of IP addresses in this interface.
     :vartype ip_addresses: list[~azure.mgmt.hybridcompute.models.IpAddress]
     """
 
@@ -2990,14 +3668,195 @@
         :keyword network_interfaces: The list of network interfaces.
         :paramtype network_interfaces: list[~azure.mgmt.hybridcompute.models.NetworkInterface]
         """
         super().__init__(**kwargs)
         self.network_interfaces = network_interfaces
 
 
+class NetworkSecurityPerimeter(_serialization.Model):
+    """Properties that define a Network Security Perimeter resource.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar id: Azure resource Id.
+    :vartype id: str
+    :ivar perimeter_guid: Guid of the Network Security Perimeter.
+    :vartype perimeter_guid: str
+    :ivar location: Regional location of the perimeter.
+    :vartype location: str
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "perimeter_guid": {"readonly": True},
+        "location": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "perimeter_guid": {"key": "perimeterGuid", "type": "str"},
+        "location": {"key": "location", "type": "str"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.id = None
+        self.perimeter_guid = None
+        self.location = None
+
+
+class NetworkSecurityPerimeterConfiguration(_serialization.Model):
+    """Properties that define a Network Security Perimeter resource.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar id: Azure resource Id.
+    :vartype id: str
+    :ivar name: Azure resource name.
+    :vartype name: str
+    :ivar type: Azure resource type.
+    :vartype type: str
+    :ivar provisioning_state: Current state of this NetworkSecurityPerimeter: whether or not is has
+     been provisioned within the resource group it is defined. Users cannot change this value but
+     are able to read from it. Values will include Provisioning ,Succeeded, Canceled and Failed.
+    :vartype provisioning_state: str
+    :ivar provisioning_issues: Provisioning issues.
+    :vartype provisioning_issues: list[~azure.mgmt.hybridcompute.models.ProvisioningIssue]
+    :ivar network_security_perimeter: The Network Security Perimeter associated with this
+     configuration.
+    :vartype network_security_perimeter: ~azure.mgmt.hybridcompute.models.NetworkSecurityPerimeter
+    :ivar resource_association: The Resource Association.
+    :vartype resource_association: ~azure.mgmt.hybridcompute.models.ResourceAssociation
+    :ivar profile: Network Security Perimeter profile.
+    :vartype profile: ~azure.mgmt.hybridcompute.models.NetworkSecurityPerimeterProfile
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "provisioning_state": {"readonly": True},
+        "provisioning_issues": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
+        "provisioning_issues": {"key": "properties.provisioningIssues", "type": "[ProvisioningIssue]"},
+        "network_security_perimeter": {
+            "key": "properties.networkSecurityPerimeter",
+            "type": "NetworkSecurityPerimeter",
+        },
+        "resource_association": {"key": "properties.resourceAssociation", "type": "ResourceAssociation"},
+        "profile": {"key": "properties.profile", "type": "NetworkSecurityPerimeterProfile"},
+    }
+
+    def __init__(
+        self,
+        *,
+        network_security_perimeter: Optional["_models.NetworkSecurityPerimeter"] = None,
+        resource_association: Optional["_models.ResourceAssociation"] = None,
+        profile: Optional["_models.NetworkSecurityPerimeterProfile"] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword network_security_perimeter: The Network Security Perimeter associated with this
+         configuration.
+        :paramtype network_security_perimeter:
+         ~azure.mgmt.hybridcompute.models.NetworkSecurityPerimeter
+        :keyword resource_association: The Resource Association.
+        :paramtype resource_association: ~azure.mgmt.hybridcompute.models.ResourceAssociation
+        :keyword profile: Network Security Perimeter profile.
+        :paramtype profile: ~azure.mgmt.hybridcompute.models.NetworkSecurityPerimeterProfile
+        """
+        super().__init__(**kwargs)
+        self.id = None
+        self.name = None
+        self.type = None
+        self.provisioning_state = None
+        self.provisioning_issues = None
+        self.network_security_perimeter = network_security_perimeter
+        self.resource_association = resource_association
+        self.profile = profile
+
+
+class NetworkSecurityPerimeterConfigurationListResult(_serialization.Model):  # pylint: disable=name-too-long
+    """A list of network security perimeter configurations.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar value: Array of results.
+    :vartype value: list[~azure.mgmt.hybridcompute.models.NetworkSecurityPerimeterConfiguration]
+    :ivar next_link: Link to retrieve next page of results.
+    :vartype next_link: str
+    """
+
+    _validation = {
+        "value": {"readonly": True},
+        "next_link": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "value": {"key": "value", "type": "[NetworkSecurityPerimeterConfiguration]"},
+        "next_link": {"key": "nextLink", "type": "str"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.value = None
+        self.next_link = None
+
+
+class NetworkSecurityPerimeterProfile(_serialization.Model):
+    """Network Security Perimeter profile.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar name: Name of the resource.
+    :vartype name: str
+    :ivar access_rules_version: Access rules version number.
+    :vartype access_rules_version: str
+    :ivar access_rules: Collection of access rules for the profile.
+    :vartype access_rules: list[~azure.mgmt.hybridcompute.models.AccessRule]
+    :ivar diagnostic_settings_version: Diagnostic settings version number.
+    :vartype diagnostic_settings_version: str
+    :ivar enabled_log_categories: Collection of enabled log categories for the profile.
+    :vartype enabled_log_categories: list[str]
+    """
+
+    _validation = {
+        "name": {"readonly": True},
+        "access_rules_version": {"readonly": True},
+        "access_rules": {"readonly": True},
+        "diagnostic_settings_version": {"readonly": True},
+        "enabled_log_categories": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "name": {"key": "name", "type": "str"},
+        "access_rules_version": {"key": "accessRulesVersion", "type": "str"},
+        "access_rules": {"key": "accessRules", "type": "[AccessRule]"},
+        "diagnostic_settings_version": {"key": "diagnosticSettingsVersion", "type": "str"},
+        "enabled_log_categories": {"key": "enabledLogCategories", "type": "[str]"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.name = None
+        self.access_rules_version = None
+        self.access_rules = None
+        self.diagnostic_settings_version = None
+        self.enabled_log_categories = None
+
+
 class OperationListResult(_serialization.Model):
     """The List Compute Operation operation response.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar value: The list of compute operations.
     :vartype value: list[~azure.mgmt.hybridcompute.models.OperationValue]
@@ -3212,15 +4071,15 @@
 
 class PrivateEndpointConnection(ProxyResource):
     """A private endpoint connection.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -3402,15 +4261,15 @@
 
 class PrivateLinkResource(ProxyResource):
     """A private link resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -3547,20 +4406,20 @@
         """
         super().__init__(**kwargs)
         self.id = None
         self.public_network_access = public_network_access
         self.connection_details = connection_details
 
 
-class PrivateLinkServiceConnectionStateProperty(_serialization.Model):
+class PrivateLinkServiceConnectionStateProperty(_serialization.Model):  # pylint: disable=name-too-long
     """State of the private endpoint connection.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to Azure.
+    All required parameters must be populated in order to send to server.
 
     :ivar status: The private link service connection status. Required.
     :vartype status: str
     :ivar description: The private link service connection description. Required.
     :vartype description: str
     :ivar actions_required: The actions required for private link service connection.
     :vartype actions_required: str
@@ -3587,14 +4446,255 @@
         """
         super().__init__(**kwargs)
         self.status = status
         self.description = description
         self.actions_required = None
 
 
+class ProductFeature(_serialization.Model):
+    """Product Feature.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar name: Product feature name.
+    :vartype name: str
+    :ivar subscription_status: Indicates the current status of the product features. Known values
+     are: "Unknown", "Enabling", "Enabled", and "Disabled".
+    :vartype subscription_status: str or
+     ~azure.mgmt.hybridcompute.models.LicenseProfileSubscriptionStatus
+    :ivar billing_start_date: The timestamp in UTC when the billing starts.
+    :vartype billing_start_date: ~datetime.datetime
+    :ivar enrollment_date: The timestamp in UTC when the user enrolls the feature.
+    :vartype enrollment_date: ~datetime.datetime
+    :ivar disenrollment_date: The timestamp in UTC when the user disenrolled the feature.
+    :vartype disenrollment_date: ~datetime.datetime
+    """
+
+    _validation = {
+        "billing_start_date": {"readonly": True},
+        "enrollment_date": {"readonly": True},
+        "disenrollment_date": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "name": {"key": "name", "type": "str"},
+        "subscription_status": {"key": "subscriptionStatus", "type": "str"},
+        "billing_start_date": {"key": "billingStartDate", "type": "iso-8601"},
+        "enrollment_date": {"key": "enrollmentDate", "type": "iso-8601"},
+        "disenrollment_date": {"key": "disenrollmentDate", "type": "iso-8601"},
+    }
+
+    def __init__(
+        self,
+        *,
+        name: Optional[str] = None,
+        subscription_status: Optional[Union[str, "_models.LicenseProfileSubscriptionStatus"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword name: Product feature name.
+        :paramtype name: str
+        :keyword subscription_status: Indicates the current status of the product features. Known
+         values are: "Unknown", "Enabling", "Enabled", and "Disabled".
+        :paramtype subscription_status: str or
+         ~azure.mgmt.hybridcompute.models.LicenseProfileSubscriptionStatus
+        """
+        super().__init__(**kwargs)
+        self.name = name
+        self.subscription_status = subscription_status
+        self.billing_start_date = None
+        self.enrollment_date = None
+        self.disenrollment_date = None
+
+
+class ProductFeatureUpdate(_serialization.Model):
+    """Product Feature.
+
+    :ivar name: Product feature name.
+    :vartype name: str
+    :ivar subscription_status: Indicates the new status of the product feature. Known values are:
+     "Enable" and "Disable".
+    :vartype subscription_status: str or
+     ~azure.mgmt.hybridcompute.models.LicenseProfileSubscriptionStatusUpdate
+    """
+
+    _attribute_map = {
+        "name": {"key": "name", "type": "str"},
+        "subscription_status": {"key": "subscriptionStatus", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        name: Optional[str] = None,
+        subscription_status: Optional[Union[str, "_models.LicenseProfileSubscriptionStatusUpdate"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword name: Product feature name.
+        :paramtype name: str
+        :keyword subscription_status: Indicates the new status of the product feature. Known values
+         are: "Enable" and "Disable".
+        :paramtype subscription_status: str or
+         ~azure.mgmt.hybridcompute.models.LicenseProfileSubscriptionStatusUpdate
+        """
+        super().__init__(**kwargs)
+        self.name = name
+        self.subscription_status = subscription_status
+
+
+class ProvisioningIssue(_serialization.Model):
+    """Details on issues that occurred during provisioning.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar name: Name of the provisioning issue.
+    :vartype name: str
+    :ivar issue_type: Issue type. Known values are: "MissingPerimeterConfiguration",
+     "MissingIdentityConfiguration", "ConfigurationPropagationFailure", and "Other".
+    :vartype issue_type: str or ~azure.mgmt.hybridcompute.models.ProvisioningIssueType
+    :ivar severity: Severity of the provisioning issue. Known values are: "Warning" and "Error".
+    :vartype severity: str or ~azure.mgmt.hybridcompute.models.ProvisioningIssueSeverity
+    :ivar description: Description of the provisioning issue.
+    :vartype description: str
+    :ivar suggested_resource_ids: ARM Ids of the resources that can be associated to the same
+     perimeter to remediate the issue.
+    :vartype suggested_resource_ids: list[str]
+    :ivar suggested_access_rules: Access rules that can be added to the perimeter to remediate the
+     issue.
+    :vartype suggested_access_rules: list[~azure.mgmt.hybridcompute.models.AccessRule]
+    """
+
+    _validation = {
+        "name": {"readonly": True},
+        "issue_type": {"readonly": True},
+        "severity": {"readonly": True},
+        "description": {"readonly": True},
+        "suggested_resource_ids": {"readonly": True},
+        "suggested_access_rules": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "name": {"key": "name", "type": "str"},
+        "issue_type": {"key": "properties.issueType", "type": "str"},
+        "severity": {"key": "properties.severity", "type": "str"},
+        "description": {"key": "properties.description", "type": "str"},
+        "suggested_resource_ids": {"key": "properties.suggestedResourceIds", "type": "[str]"},
+        "suggested_access_rules": {"key": "properties.suggestedAccessRules", "type": "[AccessRule]"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.name = None
+        self.issue_type = None
+        self.severity = None
+        self.description = None
+        self.suggested_resource_ids = None
+        self.suggested_access_rules = None
+
+
+class ResourceAssociation(_serialization.Model):
+    """Properties that define a Resource Association.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar name: Name of the Resource Association.
+    :vartype name: str
+    :ivar access_mode: The access mode. Known values are: "enforced", "audit", and "learning".
+    :vartype access_mode: str or ~azure.mgmt.hybridcompute.models.AccessMode
+    """
+
+    _validation = {
+        "name": {"readonly": True},
+        "access_mode": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "name": {"key": "name", "type": "str"},
+        "access_mode": {"key": "accessMode", "type": "str"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.name = None
+        self.access_mode = None
+
+
+class RunCommandInputParameter(_serialization.Model):
+    """Describes the properties of a run command parameter.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar name: The run command parameter name. Required.
+    :vartype name: str
+    :ivar value: The run command parameter value. Required.
+    :vartype value: str
+    """
+
+    _validation = {
+        "name": {"required": True},
+        "value": {"required": True},
+    }
+
+    _attribute_map = {
+        "name": {"key": "name", "type": "str"},
+        "value": {"key": "value", "type": "str"},
+    }
+
+    def __init__(self, *, name: str, value: str, **kwargs: Any) -> None:
+        """
+        :keyword name: The run command parameter name. Required.
+        :paramtype name: str
+        :keyword value: The run command parameter value. Required.
+        :paramtype value: str
+        """
+        super().__init__(**kwargs)
+        self.name = name
+        self.value = value
+
+
+class RunCommandManagedIdentity(_serialization.Model):
+    """Contains clientId or objectId (use only one, not both) of a user-assigned managed identity that
+    has access to storage blob used in Run Command. Use an empty RunCommandManagedIdentity object
+    in case of system-assigned identity. Make sure the Azure storage blob exists in case of
+    scriptUri, and managed identity has been given access to blob's container with 'Storage Blob
+    Data Reader' role assignment with scriptUri blob and 'Storage Blob Data Contributor' for Append
+    blobs(outputBlobUri, errorBlobUri). In case of user assigned identity, make sure you add it
+    under VM's identity. For more info on managed identity and Run Command, refer
+    https://aka.ms/ManagedIdentity and https://aka.ms/RunCommandManaged.
+
+    :ivar client_id: Client Id (GUID value) of the user-assigned managed identity. ObjectId should
+     not be used if this is provided.
+    :vartype client_id: str
+    :ivar object_id: Object Id (GUID value) of the user-assigned managed identity. ClientId should
+     not be used if this is provided.
+    :vartype object_id: str
+    """
+
+    _attribute_map = {
+        "client_id": {"key": "clientId", "type": "str"},
+        "object_id": {"key": "objectId", "type": "str"},
+    }
+
+    def __init__(self, *, client_id: Optional[str] = None, object_id: Optional[str] = None, **kwargs: Any) -> None:
+        """
+        :keyword client_id: Client Id (GUID value) of the user-assigned managed identity. ObjectId
+         should not be used if this is provided.
+        :paramtype client_id: str
+        :keyword object_id: Object Id (GUID value) of the user-assigned managed identity. ClientId
+         should not be used if this is provided.
+        :paramtype object_id: str
+        """
+        super().__init__(**kwargs)
+        self.client_id = client_id
+        self.object_id = object_id
+
+
 class ServiceStatus(_serialization.Model):
     """Describes the status and behavior of a service.
 
     :ivar status: The current status of the service.
     :vartype status: str
     :ivar startup_type: The behavior of the service when the Arc-enabled machine starts up.
     :vartype startup_type: str
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/models/_patch.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/__init__.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,42 +2,36 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._licenses_operations import LicensesOperations
 from ._machines_operations import MachinesOperations
-from ._license_profiles_operations import LicenseProfilesOperations
 from ._machine_extensions_operations import MachineExtensionsOperations
 from ._hybrid_compute_management_client_operations import HybridComputeManagementClientOperationsMixin
 from ._extension_metadata_operations import ExtensionMetadataOperations
 from ._operations import Operations
 from ._network_profile_operations import NetworkProfileOperations
-from ._hybrid_identity_metadata_operations import HybridIdentityMetadataOperations
-from ._agent_version_operations import AgentVersionOperations
+from ._machine_run_commands_operations import MachineRunCommandsOperations
 from ._private_link_scopes_operations import PrivateLinkScopesOperations
 from ._private_link_resources_operations import PrivateLinkResourcesOperations
 from ._private_endpoint_connections_operations import PrivateEndpointConnectionsOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
-    "LicensesOperations",
     "MachinesOperations",
-    "LicenseProfilesOperations",
     "MachineExtensionsOperations",
     "HybridComputeManagementClientOperationsMixin",
     "ExtensionMetadataOperations",
     "Operations",
     "NetworkProfileOperations",
-    "HybridIdentityMetadataOperations",
-    "AgentVersionOperations",
+    "MachineRunCommandsOperations",
     "PrivateLinkScopesOperations",
     "PrivateLinkResourcesOperations",
     "PrivateEndpointConnectionsOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/_agent_version_operations.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_private_link_resources_operations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, Callable, Dict, Optional, TypeVar
+from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
+import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
+from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
@@ -30,190 +32,240 @@
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
-def build_list_request(os_type: str, **kwargs: Any) -> HttpRequest:
+def build_list_by_private_link_scope_request(
+    resource_group_name: str, scope_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-20-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
-    _url = kwargs.pop("template_url", "/providers/Microsoft.HybridCompute/osType/{osType}/agentVersions")
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateLinkResources",
+    )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "osType": _SERIALIZER.url("os_type", os_type, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "scopeName": _SERIALIZER.url("scope_name", scope_name, "str", pattern=r"[a-zA-Z0-9-_\.]+"),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_get_request(os_type: str, version: str, **kwargs: Any) -> HttpRequest:
+def build_get_request(
+    resource_group_name: str, scope_name: str, group_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-20-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
-    _url = kwargs.pop("template_url", "/providers/Microsoft.HybridCompute/osType/{osType}/agentVersions/{version}")
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateLinkResources/{groupName}",
+    )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "osType": _SERIALIZER.url("os_type", os_type, "str"),
-        "version": _SERIALIZER.url("version", version, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "scopeName": _SERIALIZER.url("scope_name", scope_name, "str", pattern=r"[a-zA-Z0-9-_\.]+"),
+        "groupName": _SERIALIZER.url("group_name", group_name, "str"),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class AgentVersionOperations:
+class PrivateLinkResourcesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.hybridcompute.HybridComputeManagementClient`'s
-        :attr:`agent_version` attribute.
+        :attr:`private_link_resources` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(self, os_type: str, **kwargs: Any) -> _models.AgentVersionsList:
-        """Gets all Agent Versions along with the download link currently present.
-
-        :param os_type: Defines the os type. Required.
-        :type os_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: AgentVersionsList or the result of cls(response)
-        :rtype: ~azure.mgmt.hybridcompute.models.AgentVersionsList
+    def list_by_private_link_scope(
+        self, resource_group_name: str, scope_name: str, **kwargs: Any
+    ) -> Iterable["_models.PrivateLinkResource"]:
+        """Gets the private link resources that need to be created for a Azure Monitor PrivateLinkScope.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
+        :type scope_name: str
+        :return: An iterator like instance of either PrivateLinkResource or the result of cls(response)
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.hybridcompute.models.PrivateLinkResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.PrivateLinkResourceListResult] = kwargs.pop("cls", None)
+
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+        def prepare_request(next_link=None):
+            if not next_link:
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.AgentVersionsList] = kwargs.pop("cls", None)
+                _request = build_list_by_private_link_scope_request(
+                    resource_group_name=resource_group_name,
+                    scope_name=scope_name,
+                    subscription_id=self._config.subscription_id,
+                    api_version=api_version,
+                    headers=_headers,
+                    params=_params,
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+
+            else:
+                # make call to next link with the client's api-version
+                _parsed_next_link = urllib.parse.urlparse(next_link)
+                _next_request_params = case_insensitive_dict(
+                    {
+                        key: [urllib.parse.quote(v) for v in value]
+                        for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
+                    }
+                )
+                _next_request_params["api-version"] = self._config.api_version
+                _request = HttpRequest(
+                    "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
+                )
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
+
+        def extract_data(pipeline_response):
+            deserialized = self._deserialize("PrivateLinkResourceListResult", pipeline_response)
+            list_of_elem = deserialized.value
+            if cls:
+                list_of_elem = cls(list_of_elem)  # type: ignore
+            return deserialized.next_link or None, iter(list_of_elem)
+
+        def get_next(next_link=None):
+            _request = prepare_request(next_link)
+
+            _stream = False
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+            response = pipeline_response.http_response
+
+            if response.status_code not in [200]:
+                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        request = build_list_request(
-            os_type=os_type,
-            api_version=api_version,
-            template_url=self.list.metadata["url"],
-            headers=_headers,
-            params=_params,
-        )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+            return pipeline_response
 
-        _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.ErrorResponseAutoGenerated, pipeline_response)
-            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-        deserialized = self._deserialize("AgentVersionsList", pipeline_response)
-
-        if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
-
-    list.metadata = {"url": "/providers/Microsoft.HybridCompute/osType/{osType}/agentVersions"}
+        return ItemPaged(get_next, extract_data)
 
     @distributed_trace
-    def get(self, os_type: str, version: str, **kwargs: Any) -> _models.AgentVersion:
-        """Gets an Agent Version along with the download link currently present.
-
-        :param os_type: Defines the os type. Required.
-        :type os_type: str
-        :param version: Defines the agent version. To get latest, use latest or else a specific agent
-         version. Required.
-        :type version: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: AgentVersion or the result of cls(response)
-        :rtype: ~azure.mgmt.hybridcompute.models.AgentVersion
+    def get(
+        self, resource_group_name: str, scope_name: str, group_name: str, **kwargs: Any
+    ) -> _models.PrivateLinkResource:
+        """Gets the private link resources that need to be created for a Azure Monitor PrivateLinkScope.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
+        :type scope_name: str
+        :param group_name: The name of the private link resource. Required.
+        :type group_name: str
+        :return: PrivateLinkResource or the result of cls(response)
+        :rtype: ~azure.mgmt.hybridcompute.models.PrivateLinkResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.AgentVersion] = kwargs.pop("cls", None)
+        cls: ClsType[_models.PrivateLinkResource] = kwargs.pop("cls", None)
 
-        request = build_get_request(
-            os_type=os_type,
-            version=version,
+        _request = build_get_request(
+            resource_group_name=resource_group_name,
+            scope_name=scope_name,
+            group_name=group_name,
+            subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.ErrorResponseAutoGenerated, pipeline_response)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("AgentVersion", pipeline_response)
+        deserialized = self._deserialize("PrivateLinkResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {"url": "/providers/Microsoft.HybridCompute/osType/{osType}/agentVersions/{version}"}
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/_extension_metadata_operations.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_extension_metadata_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -38,15 +38,15 @@
 
 def build_get_request(
     location: str, publisher: str, extension_type: str, version: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-20-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.HybridCompute/locations/{location}/publishers/{publisher}/extensionTypes/{extensionType}/versions/{version}",
     )  # pylint: disable=line-too-long
@@ -71,15 +71,15 @@
 
 def build_list_request(
     location: str, publisher: str, extension_type: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-20-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.HybridCompute/locations/{location}/publishers/{publisher}/extensionTypes/{extensionType}/versions",
     )  # pylint: disable=line-too-long
@@ -130,15 +130,14 @@
         :type location: str
         :param publisher: The publisher of the Extension being received. Required.
         :type publisher: str
         :param extension_type: The extensionType of the Extension being received. Required.
         :type extension_type: str
         :param version: The version of the Extension being received. Required.
         :type version: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ExtensionValue or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.ExtensionValue
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -149,64 +148,58 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ExtensionValue] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             location=location,
             publisher=publisher,
             extension_type=extension_type,
             version=version,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ExtensionValue", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.HybridCompute/locations/{location}/publishers/{publisher}/extensionTypes/{extensionType}/versions/{version}"
-    }
+        return deserialized  # type: ignore
 
     @distributed_trace
     def list(
         self, location: str, publisher: str, extension_type: str, **kwargs: Any
     ) -> Iterable["_models.ExtensionValue"]:
         """Gets all Extension versions based on location, publisher, extensionType.
 
         :param location: The location of the Extension being received. Required.
         :type location: str
         :param publisher: The publisher of the Extension being received. Required.
         :type publisher: str
         :param extension_type: The extensionType of the Extension being received. Required.
         :type extension_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ExtensionValue or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.hybridcompute.models.ExtensionValue]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -220,66 +213,61 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     location=location,
                     publisher=publisher,
                     extension_type=extension_type,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ExtensionValueListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
-
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.HybridCompute/locations/{location}/publishers/{publisher}/extensionTypes/{extensionType}/versions"
-    }
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/_license_profiles_operations.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_machine_extensions_operations.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-import sys
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -29,48 +28,45 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import HybridComputeManagementClientMixinABC, _convert_request
 
-if sys.version_info >= (3, 8):
-    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
-else:
-    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_create_or_update_request(
-    resource_group_name: str, machine_name: str, subscription_id: str, **kwargs: Any
+    resource_group_name: str, machine_name: str, extension_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-20-preview"))
-    license_profile_name: Literal["default"] = kwargs.pop("license_profile_name", "default")
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/licenseProfiles/{licenseProfileName}",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/extensions/{extensionName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
-        "machineName": _SERIALIZER.url("machine_name", machine_name, "str", pattern=r"[a-zA-Z0-9-_\.]+"),
-        "licenseProfileName": _SERIALIZER.url("license_profile_name", license_profile_name, "str"),
+        "machineName": _SERIALIZER.url(
+            "machine_name", machine_name, "str", max_length=54, min_length=1, pattern=r"^[a-zA-Z0-9-_\.]{1,54}$"
+        ),
+        "extensionName": _SERIALIZER.url("extension_name", extension_name, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -79,36 +75,37 @@
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_update_request(
-    resource_group_name: str, machine_name: str, subscription_id: str, **kwargs: Any
+    resource_group_name: str, machine_name: str, extension_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-20-preview"))
-    license_profile_name: Literal["default"] = kwargs.pop("license_profile_name", "default")
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/licenseProfiles/{licenseProfileName}",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/extensions/{extensionName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
-        "machineName": _SERIALIZER.url("machine_name", machine_name, "str", pattern=r"[a-zA-Z0-9-_\.]+"),
-        "licenseProfileName": _SERIALIZER.url("license_profile_name", license_profile_name, "str"),
+        "machineName": _SERIALIZER.url(
+            "machine_name", machine_name, "str", max_length=54, min_length=1, pattern=r"^[a-zA-Z0-9-_\.]{1,54}$"
+        ),
+        "extensionName": _SERIALIZER.url("extension_name", extension_name, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -116,894 +113,817 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_get_request(resource_group_name: str, machine_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
+def build_delete_request(
+    resource_group_name: str, machine_name: str, extension_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-20-preview"))
-    license_profile_name: Literal["default"] = kwargs.pop("license_profile_name", "default")
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/licenseProfiles/{licenseProfileName}",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/extensions/{extensionName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
-        "machineName": _SERIALIZER.url("machine_name", machine_name, "str", pattern=r"[a-zA-Z0-9-_\.]+"),
-        "licenseProfileName": _SERIALIZER.url("license_profile_name", license_profile_name, "str"),
+        "machineName": _SERIALIZER.url(
+            "machine_name", machine_name, "str", max_length=54, min_length=1, pattern=r"^[a-zA-Z0-9-_\.]{1,54}$"
+        ),
+        "extensionName": _SERIALIZER.url("extension_name", extension_name, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+    return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_delete_request(
-    resource_group_name: str, machine_name: str, subscription_id: str, **kwargs: Any
+def build_get_request(
+    resource_group_name: str, machine_name: str, extension_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-20-preview"))
-    license_profile_name: Literal["default"] = kwargs.pop("license_profile_name", "default")
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/licenseProfiles/{licenseProfileName}",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/extensions/{extensionName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
-        "machineName": _SERIALIZER.url("machine_name", machine_name, "str", pattern=r"[a-zA-Z0-9-_\.]+"),
-        "licenseProfileName": _SERIALIZER.url("license_profile_name", license_profile_name, "str"),
+        "machineName": _SERIALIZER.url(
+            "machine_name", machine_name, "str", max_length=54, min_length=1, pattern=r"^[a-zA-Z0-9-_\.]{1,54}$"
+        ),
+        "extensionName": _SERIALIZER.url("extension_name", extension_name, "str"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_list_request(resource_group_name: str, machine_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
+def build_list_request(
+    resource_group_name: str, machine_name: str, subscription_id: str, *, expand: Optional[str] = None, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-20-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/licenseProfiles",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/extensions",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "machineName": _SERIALIZER.url(
-            "machine_name", machine_name, "str", max_length=54, min_length=1, pattern=r"[a-zA-Z0-9-_\.]"
+            "machine_name", machine_name, "str", max_length=54, min_length=1, pattern=r"^[a-zA-Z0-9-_\.]{1,54}$"
         ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
+    if expand is not None:
+        _params["$expand"] = _SERIALIZER.query("expand", expand, "str")
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class LicenseProfilesOperations:
+class MachineExtensionsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.hybridcompute.HybridComputeManagementClient`'s
-        :attr:`license_profiles` attribute.
+        :attr:`machine_extensions` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     def _create_or_update_initial(
-        self, resource_group_name: str, machine_name: str, parameters: Union[_models.LicenseProfile, IO], **kwargs: Any
-    ) -> _models.LicenseProfile:
+        self,
+        resource_group_name: str,
+        machine_name: str,
+        extension_name: str,
+        extension_parameters: Union[_models.MachineExtension, IO[bytes]],
+        **kwargs: Any
+    ) -> Optional[_models.MachineExtension]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        license_profile_name: Literal["default"] = kwargs.pop("license_profile_name", "default")
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.LicenseProfile] = kwargs.pop("cls", None)
+        cls: ClsType[Optional[_models.MachineExtension]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
-            _content = parameters
+        if isinstance(extension_parameters, (IOBase, bytes)):
+            _content = extension_parameters
         else:
-            _json = self._serialize.body(parameters, "LicenseProfile")
+            _json = self._serialize.body(extension_parameters, "MachineExtension")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             machine_name=machine_name,
+            extension_name=extension_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            license_profile_name=license_profile_name,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 201]:
+        if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        response_headers = {}
+        deserialized = None
         if response.status_code == 200:
-            deserialized = self._deserialize("LicenseProfile", pipeline_response)
-
-        if response.status_code == 201:
-            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
-            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
-            response_headers["Azure-AsyncOperation"] = self._deserialize(
-                "str", response.headers.get("Azure-AsyncOperation")
-            )
-
-            deserialized = self._deserialize("LicenseProfile", pipeline_response)
+            deserialized = self._deserialize("MachineExtension", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/licenseProfiles/{licenseProfileName}"
-    }
-
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         machine_name: str,
-        parameters: _models.LicenseProfile,
+        extension_name: str,
+        extension_parameters: _models.MachineExtension,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> LROPoller[_models.LicenseProfile]:
-        """The operation to create or update a license profile.
+    ) -> LROPoller[_models.MachineExtension]:
+        """The operation to create or update the extension.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param machine_name: The name of the hybrid machine. Required.
+        :param machine_name: The name of the machine where the extension should be created or updated.
+         Required.
         :type machine_name: str
-        :param parameters: Parameters supplied to the Create license profile operation. Required.
-        :type parameters: ~azure.mgmt.hybridcompute.models.LicenseProfile
+        :param extension_name: The name of the machine extension. Required.
+        :type extension_name: str
+        :param extension_parameters: Parameters supplied to the Create Machine Extension operation.
+         Required.
+        :type extension_parameters: ~azure.mgmt.hybridcompute.models.MachineExtension
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword license_profile_name: The name of the license profile. Default value is "default".
-         Note that overriding this default value may result in unsupported behavior.
-        :paramtype license_profile_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either LicenseProfile or the result of
+        :return: An instance of LROPoller that returns either MachineExtension or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.LicenseProfile]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.MachineExtension]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         machine_name: str,
-        parameters: IO,
+        extension_name: str,
+        extension_parameters: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> LROPoller[_models.LicenseProfile]:
-        """The operation to create or update a license profile.
+    ) -> LROPoller[_models.MachineExtension]:
+        """The operation to create or update the extension.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param machine_name: The name of the hybrid machine. Required.
+        :param machine_name: The name of the machine where the extension should be created or updated.
+         Required.
         :type machine_name: str
-        :param parameters: Parameters supplied to the Create license profile operation. Required.
-        :type parameters: IO
+        :param extension_name: The name of the machine extension. Required.
+        :type extension_name: str
+        :param extension_parameters: Parameters supplied to the Create Machine Extension operation.
+         Required.
+        :type extension_parameters: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword license_profile_name: The name of the license profile. Default value is "default".
-         Note that overriding this default value may result in unsupported behavior.
-        :paramtype license_profile_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either LicenseProfile or the result of
+        :return: An instance of LROPoller that returns either MachineExtension or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.LicenseProfile]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.MachineExtension]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create_or_update(
-        self, resource_group_name: str, machine_name: str, parameters: Union[_models.LicenseProfile, IO], **kwargs: Any
-    ) -> LROPoller[_models.LicenseProfile]:
-        """The operation to create or update a license profile.
+        self,
+        resource_group_name: str,
+        machine_name: str,
+        extension_name: str,
+        extension_parameters: Union[_models.MachineExtension, IO[bytes]],
+        **kwargs: Any
+    ) -> LROPoller[_models.MachineExtension]:
+        """The operation to create or update the extension.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param machine_name: The name of the hybrid machine. Required.
+        :param machine_name: The name of the machine where the extension should be created or updated.
+         Required.
         :type machine_name: str
-        :param parameters: Parameters supplied to the Create license profile operation. Is either a
-         LicenseProfile type or a IO type. Required.
-        :type parameters: ~azure.mgmt.hybridcompute.models.LicenseProfile or IO
-        :keyword license_profile_name: The name of the license profile. Default value is "default".
-         Note that overriding this default value may result in unsupported behavior.
-        :paramtype license_profile_name: str
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either LicenseProfile or the result of
+        :param extension_name: The name of the machine extension. Required.
+        :type extension_name: str
+        :param extension_parameters: Parameters supplied to the Create Machine Extension operation. Is
+         either a MachineExtension type or a IO[bytes] type. Required.
+        :type extension_parameters: ~azure.mgmt.hybridcompute.models.MachineExtension or IO[bytes]
+        :return: An instance of LROPoller that returns either MachineExtension or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.LicenseProfile]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.MachineExtension]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        license_profile_name: Literal["default"] = kwargs.pop("license_profile_name", "default")
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.LicenseProfile] = kwargs.pop("cls", None)
+        cls: ClsType[_models.MachineExtension] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._create_or_update_initial(
                 resource_group_name=resource_group_name,
                 machine_name=machine_name,
-                parameters=parameters,
+                extension_name=extension_name,
+                extension_parameters=extension_parameters,
                 api_version=api_version,
-                license_profile_name=license_profile_name,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("LicenseProfile", pipeline_response)
+            deserialized = self._deserialize("MachineExtension", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[_models.MachineExtension].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/licenseProfiles/{licenseProfileName}"
-    }
+        return LROPoller[_models.MachineExtension](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     def _update_initial(
         self,
         resource_group_name: str,
         machine_name: str,
-        parameters: Union[_models.LicenseProfileUpdate, IO],
+        extension_name: str,
+        extension_parameters: Union[_models.MachineExtensionUpdate, IO[bytes]],
         **kwargs: Any
-    ) -> Optional[_models.LicenseProfile]:
+    ) -> Optional[_models.MachineExtension]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        license_profile_name: Literal["default"] = kwargs.pop("license_profile_name", "default")
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[Optional[_models.LicenseProfile]] = kwargs.pop("cls", None)
+        cls: ClsType[Optional[_models.MachineExtension]] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(parameters, (IOBase, bytes)):
-            _content = parameters
+        if isinstance(extension_parameters, (IOBase, bytes)):
+            _content = extension_parameters
         else:
-            _json = self._serialize.body(parameters, "LicenseProfileUpdate")
+            _json = self._serialize.body(extension_parameters, "MachineExtensionUpdate")
 
-        request = build_update_request(
+        _request = build_update_request(
             resource_group_name=resource_group_name,
             machine_name=machine_name,
+            extension_name=extension_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            license_profile_name=license_profile_name,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
         response_headers = {}
         if response.status_code == 200:
-            deserialized = self._deserialize("LicenseProfile", pipeline_response)
+            deserialized = self._deserialize("MachineExtension", pipeline_response)
 
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)
-
-        return deserialized
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
-    _update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/licenseProfiles/{licenseProfileName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     def begin_update(
         self,
         resource_group_name: str,
         machine_name: str,
-        parameters: _models.LicenseProfileUpdate,
+        extension_name: str,
+        extension_parameters: _models.MachineExtensionUpdate,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> LROPoller[_models.LicenseProfile]:
-        """The operation to update a license profile.
+    ) -> LROPoller[_models.MachineExtension]:
+        """The operation to create or update the extension.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param machine_name: The name of the hybrid machine. Required.
+        :param machine_name: The name of the machine where the extension should be created or updated.
+         Required.
         :type machine_name: str
-        :param parameters: Parameters supplied to the Update license profile operation. Required.
-        :type parameters: ~azure.mgmt.hybridcompute.models.LicenseProfileUpdate
+        :param extension_name: The name of the machine extension. Required.
+        :type extension_name: str
+        :param extension_parameters: Parameters supplied to the Create Machine Extension operation.
+         Required.
+        :type extension_parameters: ~azure.mgmt.hybridcompute.models.MachineExtensionUpdate
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword license_profile_name: The name of the license profile. Default value is "default".
-         Note that overriding this default value may result in unsupported behavior.
-        :paramtype license_profile_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either LicenseProfile or the result of
+        :return: An instance of LROPoller that returns either MachineExtension or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.LicenseProfile]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.MachineExtension]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_update(
         self,
         resource_group_name: str,
         machine_name: str,
-        parameters: IO,
+        extension_name: str,
+        extension_parameters: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> LROPoller[_models.LicenseProfile]:
-        """The operation to update a license profile.
+    ) -> LROPoller[_models.MachineExtension]:
+        """The operation to create or update the extension.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param machine_name: The name of the hybrid machine. Required.
+        :param machine_name: The name of the machine where the extension should be created or updated.
+         Required.
         :type machine_name: str
-        :param parameters: Parameters supplied to the Update license profile operation. Required.
-        :type parameters: IO
+        :param extension_name: The name of the machine extension. Required.
+        :type extension_name: str
+        :param extension_parameters: Parameters supplied to the Create Machine Extension operation.
+         Required.
+        :type extension_parameters: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword license_profile_name: The name of the license profile. Default value is "default".
-         Note that overriding this default value may result in unsupported behavior.
-        :paramtype license_profile_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either LicenseProfile or the result of
+        :return: An instance of LROPoller that returns either MachineExtension or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.LicenseProfile]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.MachineExtension]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_update(
         self,
         resource_group_name: str,
         machine_name: str,
-        parameters: Union[_models.LicenseProfileUpdate, IO],
+        extension_name: str,
+        extension_parameters: Union[_models.MachineExtensionUpdate, IO[bytes]],
         **kwargs: Any
-    ) -> LROPoller[_models.LicenseProfile]:
-        """The operation to update a license profile.
+    ) -> LROPoller[_models.MachineExtension]:
+        """The operation to create or update the extension.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param machine_name: The name of the hybrid machine. Required.
+        :param machine_name: The name of the machine where the extension should be created or updated.
+         Required.
         :type machine_name: str
-        :param parameters: Parameters supplied to the Update license profile operation. Is either a
-         LicenseProfileUpdate type or a IO type. Required.
-        :type parameters: ~azure.mgmt.hybridcompute.models.LicenseProfileUpdate or IO
-        :keyword license_profile_name: The name of the license profile. Default value is "default".
-         Note that overriding this default value may result in unsupported behavior.
-        :paramtype license_profile_name: str
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
-        :return: An instance of LROPoller that returns either LicenseProfile or the result of
+        :param extension_name: The name of the machine extension. Required.
+        :type extension_name: str
+        :param extension_parameters: Parameters supplied to the Create Machine Extension operation. Is
+         either a MachineExtensionUpdate type or a IO[bytes] type. Required.
+        :type extension_parameters: ~azure.mgmt.hybridcompute.models.MachineExtensionUpdate or
+         IO[bytes]
+        :return: An instance of LROPoller that returns either MachineExtension or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.LicenseProfile]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.MachineExtension]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        license_profile_name: Literal["default"] = kwargs.pop("license_profile_name", "default")
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.LicenseProfile] = kwargs.pop("cls", None)
+        cls: ClsType[_models.MachineExtension] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._update_initial(
                 resource_group_name=resource_group_name,
                 machine_name=machine_name,
-                parameters=parameters,
+                extension_name=extension_name,
+                extension_parameters=extension_parameters,
                 api_version=api_version,
-                license_profile_name=license_profile_name,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
-            deserialized = self._deserialize("LicenseProfile", pipeline_response)
+            deserialized = self._deserialize("MachineExtension", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[_models.MachineExtension].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/licenseProfiles/{licenseProfileName}"
-    }
-
-    @distributed_trace
-    def get(self, resource_group_name: str, machine_name: str, **kwargs: Any) -> _models.LicenseProfile:
-        """Retrieves information about the view of a license profile.
-
-        :param resource_group_name: The name of the resource group. The name is case insensitive.
-         Required.
-        :type resource_group_name: str
-        :param machine_name: The name of the hybrid machine. Required.
-        :type machine_name: str
-        :keyword license_profile_name: The name of the license profile. Default value is "default".
-         Note that overriding this default value may result in unsupported behavior.
-        :paramtype license_profile_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: LicenseProfile or the result of cls(response)
-        :rtype: ~azure.mgmt.hybridcompute.models.LicenseProfile
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        license_profile_name: Literal["default"] = kwargs.pop("license_profile_name", "default")
-        cls: ClsType[_models.LicenseProfile] = kwargs.pop("cls", None)
-
-        request = build_get_request(
-            resource_group_name=resource_group_name,
-            machine_name=machine_name,
-            subscription_id=self._config.subscription_id,
-            api_version=api_version,
-            license_profile_name=license_profile_name,
-            template_url=self.get.metadata["url"],
-            headers=_headers,
-            params=_params,
-        )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
-
-        _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        return LROPoller[_models.MachineExtension](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
         )
 
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
-
-        deserialized = self._deserialize("LicenseProfile", pipeline_response)
-
-        if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
-
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/licenseProfiles/{licenseProfileName}"
-    }
-
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
-        self, resource_group_name: str, machine_name: str, **kwargs: Any
+        self, resource_group_name: str, machine_name: str, extension_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        license_profile_name: Literal["default"] = kwargs.pop("license_profile_name", "default")
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             machine_name=machine_name,
+            extension_name=extension_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            license_profile_name=license_profile_name,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [202, 204]:
+        if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         if response.status_code == 202:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/licenseProfiles/{licenseProfileName}"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
-    def begin_delete(self, resource_group_name: str, machine_name: str, **kwargs: Any) -> LROPoller[None]:
-        """The operation to delete a license profile.
+    def begin_delete(
+        self, resource_group_name: str, machine_name: str, extension_name: str, **kwargs: Any
+    ) -> LROPoller[None]:
+        """The operation to delete the extension.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param machine_name: The name of the hybrid machine. Required.
+        :param machine_name: The name of the machine where the extension should be deleted. Required.
         :type machine_name: str
-        :keyword license_profile_name: The name of the license profile. Default value is "default".
-         Note that overriding this default value may result in unsupported behavior.
-        :paramtype license_profile_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+        :param extension_name: The name of the machine extension. Required.
+        :type extension_name: str
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        license_profile_name: Literal["default"] = kwargs.pop("license_profile_name", "default")
         cls: ClsType[None] = kwargs.pop("cls", None)
         polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
             raw_result = self._delete_initial(  # type: ignore
                 resource_group_name=resource_group_name,
                 machine_name=machine_name,
+                extension_name=extension_name,
                 api_version=api_version,
-                license_profile_name=license_profile_name,
                 cls=lambda x, y, z: x,
                 headers=_headers,
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+        return LROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/licenseProfiles/{licenseProfileName}"
-    }
+    @distributed_trace
+    def get(
+        self, resource_group_name: str, machine_name: str, extension_name: str, **kwargs: Any
+    ) -> _models.MachineExtension:
+        """The operation to get the extension.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param machine_name: The name of the machine containing the extension. Required.
+        :type machine_name: str
+        :param extension_name: The name of the machine extension. Required.
+        :type extension_name: str
+        :return: MachineExtension or the result of cls(response)
+        :rtype: ~azure.mgmt.hybridcompute.models.MachineExtension
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.MachineExtension] = kwargs.pop("cls", None)
+
+        _request = build_get_request(
+            resource_group_name=resource_group_name,
+            machine_name=machine_name,
+            extension_name=extension_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            headers=_headers,
+            params=_params,
+        )
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = self._deserialize("MachineExtension", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
 
     @distributed_trace
-    def list(self, resource_group_name: str, machine_name: str, **kwargs: Any) -> Iterable["_models.LicenseProfile"]:
-        """The operation to get all license profiles of a non-Azure machine.
+    def list(
+        self, resource_group_name: str, machine_name: str, expand: Optional[str] = None, **kwargs: Any
+    ) -> Iterable["_models.MachineExtension"]:
+        """The operation to get all extensions of a non-Azure machine.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :param machine_name: The name of the machine. Required.
+        :param machine_name: The name of the machine containing the extension. Required.
         :type machine_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either LicenseProfile or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.hybridcompute.models.LicenseProfile]
+        :param expand: The expand expression to apply on the operation. Default value is None.
+        :type expand: str
+        :return: An iterator like instance of either MachineExtension or the result of cls(response)
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.hybridcompute.models.MachineExtension]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.LicenseProfilesListResult] = kwargs.pop("cls", None)
+        cls: ClsType[_models.MachineExtensionsListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     resource_group_name=resource_group_name,
                     machine_name=machine_name,
                     subscription_id=self._config.subscription_id,
+                    expand=expand,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
-            deserialized = self._deserialize("LicenseProfilesListResult", pipeline_response)
+            deserialized = self._deserialize("MachineExtensionsListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
-
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/licenseProfiles"
-    }
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/_network_profile_operations.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_network_profile_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -34,29 +34,29 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_get_request(resource_group_name: str, machine_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-20-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/networkProfile",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "machineName": _SERIALIZER.url(
-            "machine_name", machine_name, "str", max_length=54, min_length=1, pattern=r"[a-zA-Z0-9-_\.]"
+            "machine_name", machine_name, "str", max_length=54, min_length=1, pattern=r"^[a-zA-Z0-9-_\.]{1,54}$"
         ),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -91,15 +91,14 @@
         """The operation to get network information of hybrid machine.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param machine_name: The name of the hybrid machine. Required.
         :type machine_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: NetworkProfile or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.NetworkProfile
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -110,41 +109,36 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.NetworkProfile] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             machine_name=machine_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("NetworkProfile", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/networkProfile"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/_patch.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/_private_endpoint_connections_operations.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_private_endpoint_connections_operations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -45,28 +45,28 @@
     private_endpoint_connection_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-20-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateEndpointConnections/{privateEndpointConnectionName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
-        "scopeName": _SERIALIZER.url("scope_name", scope_name, "str"),
+        "scopeName": _SERIALIZER.url("scope_name", scope_name, "str", pattern=r"[a-zA-Z0-9-_\.]+"),
         "privateEndpointConnectionName": _SERIALIZER.url(
             "private_endpoint_connection_name", private_endpoint_connection_name, "str"
         ),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
@@ -85,29 +85,29 @@
     private_endpoint_connection_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-20-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateEndpointConnections/{privateEndpointConnectionName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
-        "scopeName": _SERIALIZER.url("scope_name", scope_name, "str"),
+        "scopeName": _SERIALIZER.url("scope_name", scope_name, "str", pattern=r"[a-zA-Z0-9-_\.]+"),
         "privateEndpointConnectionName": _SERIALIZER.url(
             "private_endpoint_connection_name", private_endpoint_connection_name, "str"
         ),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
@@ -128,28 +128,28 @@
     private_endpoint_connection_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-20-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateEndpointConnections/{privateEndpointConnectionName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
-        "scopeName": _SERIALIZER.url("scope_name", scope_name, "str"),
+        "scopeName": _SERIALIZER.url("scope_name", scope_name, "str", pattern=r"[a-zA-Z0-9-_\.]+"),
         "privateEndpointConnectionName": _SERIALIZER.url(
             "private_endpoint_connection_name", private_endpoint_connection_name, "str"
         ),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
@@ -164,28 +164,28 @@
 
 def build_list_by_private_link_scope_request(
     resource_group_name: str, scope_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-20-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateEndpointConnections",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
-        "scopeName": _SERIALIZER.url("scope_name", scope_name, "str"),
+        "scopeName": _SERIALIZER.url("scope_name", scope_name, "str", pattern=r"[a-zA-Z0-9-_\.]+"),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -223,15 +223,14 @@
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
         :type private_endpoint_connection_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateEndpointConnection or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.PrivateEndpointConnection
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -242,56 +241,51 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateEndpointConnection] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             scope_name=scope_name,
             private_endpoint_connection_name=private_endpoint_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+        return deserialized  # type: ignore
 
     def _create_or_update_initial(
         self,
         resource_group_name: str,
         scope_name: str,
         private_endpoint_connection_name: str,
-        parameters: Union[_models.PrivateEndpointConnection, IO],
+        parameters: Union[_models.PrivateEndpointConnection, IO[bytes]],
         **kwargs: Any
     ) -> Optional[_models.PrivateEndpointConnection]:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -309,54 +303,49 @@
         _json = None
         _content = None
         if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "PrivateEndpointConnection")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             scope_name=scope_name,
             private_endpoint_connection_name=private_endpoint_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_or_update_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
         if response.status_code == 200:
             deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    _create_or_update_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         scope_name: str,
         private_endpoint_connection_name: str,
@@ -375,100 +364,73 @@
         :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
         :type private_endpoint_connection_name: str
         :param parameters: Required.
         :type parameters: ~azure.mgmt.hybridcompute.models.PrivateEndpointConnection
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either PrivateEndpointConnection or the result
          of cls(response)
         :rtype:
          ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.PrivateEndpointConnection]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_create_or_update(
         self,
         resource_group_name: str,
         scope_name: str,
         private_endpoint_connection_name: str,
-        parameters: IO,
+        parameters: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.PrivateEndpointConnection]:
         """Approve or reject a private endpoint connection with a given name.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
         :type private_endpoint_connection_name: str
         :param parameters: Required.
-        :type parameters: IO
+        :type parameters: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either PrivateEndpointConnection or the result
          of cls(response)
         :rtype:
          ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.PrivateEndpointConnection]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create_or_update(
         self,
         resource_group_name: str,
         scope_name: str,
         private_endpoint_connection_name: str,
-        parameters: Union[_models.PrivateEndpointConnection, IO],
+        parameters: Union[_models.PrivateEndpointConnection, IO[bytes]],
         **kwargs: Any
     ) -> LROPoller[_models.PrivateEndpointConnection]:
         """Approve or reject a private endpoint connection with a given name.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
         :type private_endpoint_connection_name: str
-        :param parameters: Is either a PrivateEndpointConnection type or a IO type. Required.
-        :type parameters: ~azure.mgmt.hybridcompute.models.PrivateEndpointConnection or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
+        :param parameters: Is either a PrivateEndpointConnection type or a IO[bytes] type. Required.
+        :type parameters: ~azure.mgmt.hybridcompute.models.PrivateEndpointConnection or IO[bytes]
         :return: An instance of LROPoller that returns either PrivateEndpointConnection or the result
          of cls(response)
         :rtype:
          ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.PrivateEndpointConnection]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
@@ -494,35 +456,33 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("PrivateEndpointConnection", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[_models.PrivateEndpointConnection].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+        return LROPoller[_models.PrivateEndpointConnection](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, scope_name: str, private_endpoint_connection_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -533,30 +493,29 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             scope_name=scope_name,
             private_endpoint_connection_name=private_endpoint_connection_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -567,41 +526,29 @@
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(
         self, resource_group_name: str, scope_name: str, private_endpoint_connection_name: str, **kwargs: Any
     ) -> LROPoller[None]:
         """Deletes a private endpoint connection with a given name.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
         :type private_endpoint_connection_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -621,47 +568,42 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateEndpointConnections/{privateEndpointConnectionName}"
-    }
+        return LROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     @distributed_trace
     def list_by_private_link_scope(
         self, resource_group_name: str, scope_name: str, **kwargs: Any
     ) -> Iterable["_models.PrivateEndpointConnection"]:
         """Gets all private endpoint connections on a private link scope.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PrivateEndpointConnection or the result of
          cls(response)
         :rtype:
          ~azure.core.paging.ItemPaged[~azure.mgmt.hybridcompute.models.PrivateEndpointConnection]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
@@ -677,65 +619,60 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_private_link_scope_request(
+                _request = build_list_by_private_link_scope_request(
                     resource_group_name=resource_group_name,
                     scope_name=scope_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_private_link_scope.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("PrivateEndpointConnectionListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
-
-    list_by_private_link_scope.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateEndpointConnections"
-    }
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure/mgmt/hybridcompute/operations/_private_link_scopes_operations.py` & `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_private_link_scopes_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -39,15 +39,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-20-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.HybridCompute/privateLinkScopes"
     )
     path_format_arguments = {
@@ -65,15 +65,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_resource_group_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-20-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes",
     )  # pylint: disable=line-too-long
@@ -95,28 +95,28 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_delete_request(resource_group_name: str, scope_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-20-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
-        "scopeName": _SERIALIZER.url("scope_name", scope_name, "str"),
+        "scopeName": _SERIALIZER.url("scope_name", scope_name, "str", pattern=r"[a-zA-Z0-9-_\.]+"),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -126,28 +126,28 @@
     return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(resource_group_name: str, scope_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-20-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
-        "scopeName": _SERIALIZER.url("scope_name", scope_name, "str"),
+        "scopeName": _SERIALIZER.url("scope_name", scope_name, "str", pattern=r"[a-zA-Z0-9-_\.]+"),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -159,29 +159,29 @@
 
 def build_create_or_update_request(
     resource_group_name: str, scope_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-20-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
-        "scopeName": _SERIALIZER.url("scope_name", scope_name, "str"),
+        "scopeName": _SERIALIZER.url("scope_name", scope_name, "str", pattern=r"[a-zA-Z0-9-_\.]+"),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -195,29 +195,29 @@
 
 def build_update_tags_request(
     resource_group_name: str, scope_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-20-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}",
     )  # pylint: disable=line-too-long
     path_format_arguments = {
         "resourceGroupName": _SERIALIZER.url(
             "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
         ),
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
-        "scopeName": _SERIALIZER.url("scope_name", scope_name, "str"),
+        "scopeName": _SERIALIZER.url("scope_name", scope_name, "str", pattern=r"[a-zA-Z0-9-_\.]+"),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
@@ -231,15 +231,15 @@
 
 def build_get_validation_details_request(
     location: str, private_link_scope_id: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-20-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.HybridCompute/locations/{location}/privateLinkScopes/{privateLinkScopeId}",
     )  # pylint: disable=line-too-long
@@ -256,21 +256,21 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_get_validation_details_for_machine_request(
+def build_get_validation_details_for_machine_request(  # pylint: disable=name-too-long
     resource_group_name: str, machine_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-20-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/privateLinkScopes/current",
     )  # pylint: disable=line-too-long
@@ -312,15 +312,14 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, **kwargs: Any) -> Iterable["_models.HybridComputePrivateLinkScope"]:
         """Gets a list of all Azure Arc PrivateLinkScopes within a subscription.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either HybridComputePrivateLinkScope or the result of
          cls(response)
         :rtype:
          ~azure.core.paging.ItemPaged[~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
@@ -336,79 +335,75 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("HybridComputePrivateLinkScopeListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.HybridCompute/privateLinkScopes"}
-
     @distributed_trace
     def list_by_resource_group(
         self, resource_group_name: str, **kwargs: Any
     ) -> Iterable["_models.HybridComputePrivateLinkScope"]:
         """Gets a list of Azure Arc PrivateLinkScopes within a resource group.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either HybridComputePrivateLinkScope or the result of
          cls(response)
         :rtype:
          ~azure.core.paging.ItemPaged[~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
@@ -424,72 +419,67 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_by_resource_group_request(
+                _request = build_list_by_resource_group_request(
                     resource_group_name=resource_group_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_by_resource_group.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("HybridComputePrivateLinkScopeListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return deserialized.next_link or None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list_by_resource_group.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes"
-    }
-
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, scope_name: str, **kwargs: Any
     ) -> None:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -499,29 +489,28 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             scope_name=scope_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self._delete_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -532,37 +521,25 @@
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
             response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
             response_headers["Azure-AsyncOperation"] = self._deserialize(
                 "str", response.headers.get("Azure-AsyncOperation")
             )
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    _delete_initial.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def begin_delete(self, resource_group_name: str, scope_name: str, **kwargs: Any) -> LROPoller[None]:
         """Deletes a Azure Arc PrivateLinkScope.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: By default, your polling method will be ARMPolling. Pass in False for this
-         operation to not poll, or pass in your own initialized polling object for a personal polling
-         strategy.
-        :paramtype polling: bool or ~azure.core.polling.PollingMethod
-        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
-         Retry-After header is present.
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -581,45 +558,40 @@
                 params=_params,
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):  # pylint: disable=inconsistent-return-statements
             if cls:
-                return cls(pipeline_response, None, {})
+                return cls(pipeline_response, None, {})  # type: ignore
 
         if polling is True:
             polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[None].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}"
-    }
+        return LROPoller[None](self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
 
     @distributed_trace
     def get(self, resource_group_name: str, scope_name: str, **kwargs: Any) -> _models.HybridComputePrivateLinkScope:
         """Returns a Azure Arc PrivateLinkScope.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: HybridComputePrivateLinkScope or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -630,48 +602,43 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.HybridComputePrivateLinkScope] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             scope_name=scope_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("HybridComputePrivateLinkScope", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     def create_or_update(
         self,
         resource_group_name: str,
         scope_name: str,
         parameters: _models.HybridComputePrivateLinkScope,
@@ -689,74 +656,68 @@
         :type scope_name: str
         :param parameters: Properties that need to be specified to create or update a Azure Arc for
          Servers and Clusters PrivateLinkScope. Required.
         :type parameters: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: HybridComputePrivateLinkScope or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def create_or_update(
         self,
         resource_group_name: str,
         scope_name: str,
-        parameters: IO,
+        parameters: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.HybridComputePrivateLinkScope:
         """Creates (or updates) a Azure Arc PrivateLinkScope. Note: You cannot specify a different value
         for InstrumentationKey nor AppId in the Put operation.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
         :param parameters: Properties that need to be specified to create or update a Azure Arc for
          Servers and Clusters PrivateLinkScope. Required.
-        :type parameters: IO
+        :type parameters: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: HybridComputePrivateLinkScope or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def create_or_update(
         self,
         resource_group_name: str,
         scope_name: str,
-        parameters: Union[_models.HybridComputePrivateLinkScope, IO],
+        parameters: Union[_models.HybridComputePrivateLinkScope, IO[bytes]],
         **kwargs: Any
     ) -> _models.HybridComputePrivateLinkScope:
         """Creates (or updates) a Azure Arc PrivateLinkScope. Note: You cannot specify a different value
         for InstrumentationKey nor AppId in the Put operation.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
         :param parameters: Properties that need to be specified to create or update a Azure Arc for
-         Servers and Clusters PrivateLinkScope. Is either a HybridComputePrivateLinkScope type or a IO
-         type. Required.
-        :type parameters: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         Servers and Clusters PrivateLinkScope. Is either a HybridComputePrivateLinkScope type or a
+         IO[bytes] type. Required.
+        :type parameters: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope or IO[bytes]
         :return: HybridComputePrivateLinkScope or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -776,32 +737,31 @@
         _json = None
         _content = None
         if isinstance(parameters, (IOBase, bytes)):
             _content = parameters
         else:
             _json = self._serialize.body(parameters, "HybridComputePrivateLinkScope")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             scope_name=scope_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -814,18 +774,14 @@
             deserialized = self._deserialize("HybridComputePrivateLinkScope", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}"
-    }
-
     @overload
     def update_tags(
         self,
         resource_group_name: str,
         scope_name: str,
         private_link_scope_tags: _models.TagsResource,
         *,
@@ -842,73 +798,67 @@
         :type scope_name: str
         :param private_link_scope_tags: Updated tag information to set into the PrivateLinkScope
          instance. Required.
         :type private_link_scope_tags: ~azure.mgmt.hybridcompute.models.TagsResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: HybridComputePrivateLinkScope or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def update_tags(
         self,
         resource_group_name: str,
         scope_name: str,
-        private_link_scope_tags: IO,
+        private_link_scope_tags: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.HybridComputePrivateLinkScope:
         """Updates an existing PrivateLinkScope's tags. To update other fields use the CreateOrUpdate
         method.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
         :param private_link_scope_tags: Updated tag information to set into the PrivateLinkScope
          instance. Required.
-        :type private_link_scope_tags: IO
+        :type private_link_scope_tags: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: HybridComputePrivateLinkScope or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def update_tags(
         self,
         resource_group_name: str,
         scope_name: str,
-        private_link_scope_tags: Union[_models.TagsResource, IO],
+        private_link_scope_tags: Union[_models.TagsResource, IO[bytes]],
         **kwargs: Any
     ) -> _models.HybridComputePrivateLinkScope:
         """Updates an existing PrivateLinkScope's tags. To update other fields use the CreateOrUpdate
         method.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
         :param private_link_scope_tags: Updated tag information to set into the PrivateLinkScope
-         instance. Is either a TagsResource type or a IO type. Required.
-        :type private_link_scope_tags: ~azure.mgmt.hybridcompute.models.TagsResource or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         instance. Is either a TagsResource type or a IO[bytes] type. Required.
+        :type private_link_scope_tags: ~azure.mgmt.hybridcompute.models.TagsResource or IO[bytes]
         :return: HybridComputePrivateLinkScope or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -928,64 +878,58 @@
         _json = None
         _content = None
         if isinstance(private_link_scope_tags, (IOBase, bytes)):
             _content = private_link_scope_tags
         else:
             _json = self._serialize.body(private_link_scope_tags, "TagsResource")
 
-        request = build_update_tags_request(
+        _request = build_update_tags_request(
             resource_group_name=resource_group_name,
             scope_name=scope_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.update_tags.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("HybridComputePrivateLinkScope", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    update_tags.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}"
-    }
+        return deserialized  # type: ignore
 
     @distributed_trace
     def get_validation_details(
         self, location: str, private_link_scope_id: str, **kwargs: Any
     ) -> _models.PrivateLinkScopeValidationDetails:
         """Returns a Azure Arc PrivateLinkScope's validation details.
 
         :param location: The location of the target resource. Required.
         :type location: str
         :param private_link_scope_id: The id (Guid) of the Azure Arc PrivateLinkScope resource.
          Required.
         :type private_link_scope_id: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateLinkScopeValidationDetails or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.PrivateLinkScopeValidationDetails
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -996,62 +940,56 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateLinkScopeValidationDetails] = kwargs.pop("cls", None)
 
-        request = build_get_validation_details_request(
+        _request = build_get_validation_details_request(
             location=location,
             private_link_scope_id=private_link_scope_id,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get_validation_details.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("PrivateLinkScopeValidationDetails", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get_validation_details.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.HybridCompute/locations/{location}/privateLinkScopes/{privateLinkScopeId}"
-    }
+        return deserialized  # type: ignore
 
     @distributed_trace
     def get_validation_details_for_machine(
         self, resource_group_name: str, machine_name: str, **kwargs: Any
     ) -> _models.PrivateLinkScopeValidationDetails:
         """Returns a Azure Arc PrivateLinkScope's validation details for a given machine.
 
         :param resource_group_name: The name of the resource group. The name is case insensitive.
          Required.
         :type resource_group_name: str
         :param machine_name: The name of the target machine to get the private link scope validation
          details for. Required.
         :type machine_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateLinkScopeValidationDetails or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.PrivateLinkScopeValidationDetails
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -1062,41 +1000,36 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateLinkScopeValidationDetails] = kwargs.pop("cls", None)
 
-        request = build_get_validation_details_for_machine_request(
+        _request = build_get_validation_details_for_machine_request(
             resource_group_name=resource_group_name,
             machine_name=machine_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get_validation_details_for_machine.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("PrivateLinkScopeValidationDetails", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get_validation_details_for_machine.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/privateLinkScopes/current"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure_mgmt_hybridcompute.egg-info/PKG-INFO` & `azure-mgmt-hybridcompute-9.0.0b2/azure_mgmt_hybridcompute.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-hybridcompute
-Version: 9.0.0b1
+Version: 9.0.0b2
 Summary: Microsoft Azure Hybrid Compute Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: isodate<1.0.0,>=0.6.1
-Requires-Dist: azure-common~=1.1
-Requires-Dist: azure-mgmt-core<2.0.0,>=1.3.2
-Requires-Dist: typing-extensions>=4.3.0; python_version < "3.8.0"
 
 # Microsoft Azure SDK for Python
 
 This is the Microsoft Azure Hybrid Compute Management Client Library.
-This package has been tested with Python 3.7+.
+This package has been tested with Python 3.8+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
 ## Getting started
 
 ### Prerequisites
 
-- Python 3.7+ is required to use this package.
+- Python 3.8+ is required to use this package.
 - [Azure subscription](https://azure.microsoft.com/free/)
 
 ### Install the package
 
 ```bash
 pip install azure-mgmt-hybridcompute
 pip install azure-identity
@@ -86,14 +82,48 @@
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 # Release History
 
+## 9.0.0b2 (2024-04-22)
+
+### Features Added
+
+  - Added operation group MachineRunCommandsOperations
+  - Model LicenseProfile has a new parameter billing_start_date
+  - Model LicenseProfile has a new parameter disenrollment_date
+  - Model LicenseProfile has a new parameter enrollment_date
+  - Model LicenseProfile has a new parameter product_features
+  - Model LicenseProfile has a new parameter product_type
+  - Model LicenseProfile has a new parameter software_assurance_customer
+  - Model LicenseProfile has a new parameter subscription_status
+  - Model LicenseProfileMachineInstanceView has a new parameter billing_start_date
+  - Model LicenseProfileMachineInstanceView has a new parameter disenrollment_date
+  - Model LicenseProfileMachineInstanceView has a new parameter enrollment_date
+  - Model LicenseProfileMachineInstanceView has a new parameter license_channel
+  - Model LicenseProfileMachineInstanceView has a new parameter license_status
+  - Model LicenseProfileMachineInstanceView has a new parameter product_features
+  - Model LicenseProfileMachineInstanceView has a new parameter product_type
+  - Model LicenseProfileMachineInstanceView has a new parameter software_assurance_customer
+  - Model LicenseProfileMachineInstanceView has a new parameter subscription_status
+  - Model LicenseProfileUpdate has a new parameter product_features
+  - Model LicenseProfileUpdate has a new parameter product_type
+  - Model LicenseProfileUpdate has a new parameter software_assurance_customer
+  - Model LicenseProfileUpdate has a new parameter subscription_status
+  - Model Machine has a new parameter os_edition
+
+### Breaking Changes
+
+  - Removed operation group AgentVersionOperations
+  - Removed operation group HybridIdentityMetadataOperations
+  - Removed operation group LicenseProfilesOperations
+  - Removed operation group LicensesOperations
+
 ## 9.0.0b1 (2023-11-20)
 
 ### Features Added
 
   - Added operation MachinesOperations.begin_assess_patches
   - Added operation MachinesOperations.begin_install_patches
   - Added operation group AgentVersionOperations
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/azure_mgmt_hybridcompute.egg-info/SOURCES.txt` & `azure-mgmt-hybridcompute-9.0.0b2/azure_mgmt_hybridcompute.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -16,40 +16,34 @@
 azure/mgmt/hybridcompute/py.typed
 azure/mgmt/hybridcompute/aio/__init__.py
 azure/mgmt/hybridcompute/aio/_configuration.py
 azure/mgmt/hybridcompute/aio/_hybrid_compute_management_client.py
 azure/mgmt/hybridcompute/aio/_patch.py
 azure/mgmt/hybridcompute/aio/_vendor.py
 azure/mgmt/hybridcompute/aio/operations/__init__.py
-azure/mgmt/hybridcompute/aio/operations/_agent_version_operations.py
 azure/mgmt/hybridcompute/aio/operations/_extension_metadata_operations.py
 azure/mgmt/hybridcompute/aio/operations/_hybrid_compute_management_client_operations.py
-azure/mgmt/hybridcompute/aio/operations/_hybrid_identity_metadata_operations.py
-azure/mgmt/hybridcompute/aio/operations/_license_profiles_operations.py
-azure/mgmt/hybridcompute/aio/operations/_licenses_operations.py
 azure/mgmt/hybridcompute/aio/operations/_machine_extensions_operations.py
+azure/mgmt/hybridcompute/aio/operations/_machine_run_commands_operations.py
 azure/mgmt/hybridcompute/aio/operations/_machines_operations.py
 azure/mgmt/hybridcompute/aio/operations/_network_profile_operations.py
 azure/mgmt/hybridcompute/aio/operations/_operations.py
 azure/mgmt/hybridcompute/aio/operations/_patch.py
 azure/mgmt/hybridcompute/aio/operations/_private_endpoint_connections_operations.py
 azure/mgmt/hybridcompute/aio/operations/_private_link_resources_operations.py
 azure/mgmt/hybridcompute/aio/operations/_private_link_scopes_operations.py
 azure/mgmt/hybridcompute/models/__init__.py
 azure/mgmt/hybridcompute/models/_hybrid_compute_management_client_enums.py
 azure/mgmt/hybridcompute/models/_models_py3.py
 azure/mgmt/hybridcompute/models/_patch.py
 azure/mgmt/hybridcompute/operations/__init__.py
-azure/mgmt/hybridcompute/operations/_agent_version_operations.py
 azure/mgmt/hybridcompute/operations/_extension_metadata_operations.py
 azure/mgmt/hybridcompute/operations/_hybrid_compute_management_client_operations.py
-azure/mgmt/hybridcompute/operations/_hybrid_identity_metadata_operations.py
-azure/mgmt/hybridcompute/operations/_license_profiles_operations.py
-azure/mgmt/hybridcompute/operations/_licenses_operations.py
 azure/mgmt/hybridcompute/operations/_machine_extensions_operations.py
+azure/mgmt/hybridcompute/operations/_machine_run_commands_operations.py
 azure/mgmt/hybridcompute/operations/_machines_operations.py
 azure/mgmt/hybridcompute/operations/_network_profile_operations.py
 azure/mgmt/hybridcompute/operations/_operations.py
 azure/mgmt/hybridcompute/operations/_patch.py
 azure/mgmt/hybridcompute/operations/_private_endpoint_connections_operations.py
 azure/mgmt/hybridcompute/operations/_private_link_resources_operations.py
 azure/mgmt/hybridcompute/operations/_private_link_scopes_operations.py
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/setup.py` & `azure-mgmt-hybridcompute-9.0.0b2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,19 +49,19 @@
     url="https://github.com/Azure/azure-sdk-for-python",
     keywords="azure, azure sdk",  # update with search keywords relevant to the azure service / product
     classifiers=[
         "Development Status :: 4 - Beta",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
     ],
     zip_safe=False,
     packages=find_packages(
         exclude=[
             "tests",
             # Exclude packages that will be covered by PEP420 or nspkg
@@ -70,14 +70,13 @@
         ]
     ),
     include_package_data=True,
     package_data={
         "pytyped": ["py.typed"],
     },
     install_requires=[
-        "isodate<1.0.0,>=0.6.1",
-        "azure-common~=1.1",
-        "azure-mgmt-core>=1.3.2,<2.0.0",
-        "typing-extensions>=4.3.0; python_version<'3.8.0'",
+        "isodate>=0.6.1",
+        "azure-common>=1.1",
+        "azure-mgmt-core>=1.3.2",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
 )
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/tests/conftest.py` & `azure-mgmt-hybridcompute-9.0.0b2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/tests/disable_test_hybridcompute.py` & `azure-mgmt-hybridcompute-9.0.0b2/tests/disable_test_hybridcompute.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b1/tests/test_mgmt_hybridcompute.py` & `azure-mgmt-hybridcompute-9.0.0b2/tests/test_mgmt_hybridcompute.py`

 * *Files identical despite different names*

