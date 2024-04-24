# Comparing `tmp/azure-mgmt-selfhelp-2.0.0b2.tar.gz` & `tmp/azure-mgmt-selfhelp-2.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-mgmt-selfhelp-2.0.0b2.tar", last modified: Wed Dec 20 02:49:43 2023, max compression
+gzip compressed data, was "azure-mgmt-selfhelp-2.0.0b3.tar", last modified: Wed Apr 24 04:40:26 2024, max compression
```

## Comparing `azure-mgmt-selfhelp-2.0.0b2.tar` & `azure-mgmt-selfhelp-2.0.0b3.tar`

### file list

```diff
@@ -1,60 +1,68 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-20 02:49:43.109042 azure-mgmt-selfhelp-2.0.0b2/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2035 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      214 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/MANIFEST.in
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     5108 2023-12-20 02:49:43.109042 azure-mgmt-selfhelp-2.0.0b2/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2001 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/README.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      616 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/_meta.json
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-20 02:49:43.101041 azure-mgmt-selfhelp-2.0.0b2/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-20 02:49:43.105041 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-20 02:49:43.105041 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      895 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3204 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5346 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/_self_help_mgmt_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    79289 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/_serialization.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/_vendor.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      488 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-20 02:49:43.105041 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      842 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3252 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5502 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/_self_help_mgmt_client.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-20 02:49:43.105041 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1255 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8881 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/operations/_check_name_availability_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18287 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/operations/_diagnostics_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7797 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/operations/_discovery_solution_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5738 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33617 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/operations/_solution_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    28707 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/operations/_troubleshooters_operations.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-20 02:49:43.105041 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4953 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    77650 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/models/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5727 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/models/_self_help_mgmt_client_enums.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-20 02:49:43.109042 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1255 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10023 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/operations/_check_name_availability_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    20806 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/operations/_diagnostics_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8980 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/operations/_discovery_solution_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6442 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    37382 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/operations/_solution_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    35197 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/operations/_troubleshooters_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-20 02:49:43.109042 azure-mgmt-selfhelp-2.0.0b2/azure_mgmt_selfhelp.egg-info/
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     5108 2023-12-20 02:49:43.000000 azure-mgmt-selfhelp-2.0.0b2/azure_mgmt_selfhelp.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1936 2023-12-20 02:49:43.000000 azure-mgmt-selfhelp-2.0.0b2/azure_mgmt_selfhelp.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-12-20 02:49:43.000000 azure-mgmt-selfhelp-2.0.0b2/azure_mgmt_selfhelp.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-12-20 02:49:42.000000 azure-mgmt-selfhelp-2.0.0b2/azure_mgmt_selfhelp.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      124 2023-12-20 02:49:43.000000 azure-mgmt-selfhelp-2.0.0b2/azure_mgmt_selfhelp.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2023-12-20 02:49:43.000000 azure-mgmt-selfhelp-2.0.0b2/azure_mgmt_selfhelp.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2023-12-20 02:49:43.109042 azure-mgmt-selfhelp-2.0.0b2/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2842 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-20 02:49:43.109042 azure-mgmt-selfhelp-2.0.0b2/tests/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2616 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/tests/conftest.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      741 2023-12-20 02:49:02.000000 azure-mgmt-selfhelp-2.0.0b2/tests/test_cli_mgmt_selfhelp.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:40:26.545424 azure-mgmt-selfhelp-2.0.0b3/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2803 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      214 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/MANIFEST.in
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5696 2024-04-24 04:40:26.545424 azure-mgmt-selfhelp-2.0.0b3/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2001 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/README.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      618 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/_meta.json
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:40:26.533424 azure-mgmt-selfhelp-2.0.0b3/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:40:26.533424 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:40:26.537424 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      895 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3461 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8294 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/_self_help_mgmt_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/_serialization.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/_vendor.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      488 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:40:26.537424 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      842 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3509 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8490 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/_self_help_mgmt_client.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:40:26.541424 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1795 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8376 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_check_name_availability_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15277 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_diagnostics_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7368 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_discovery_solution_nlp_subscription_scope_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7241 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_discovery_solution_nlp_tenant_scope_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7283 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_discovery_solution_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5546 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16587 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_simplified_solutions_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    32962 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_solution_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4709 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_solution_self_help_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    26887 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_troubleshooters_operations.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:40:26.541424 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5742 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    98429 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/models/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6275 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/models/_self_help_mgmt_client_enums.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:40:26.541424 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1795 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9518 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_check_name_availability_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    17826 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_diagnostics_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8533 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_discovery_solution_nlp_subscription_scope_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8167 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_discovery_solution_nlp_tenant_scope_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8260 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_discovery_solution_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6250 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19296 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_simplified_solutions_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    38193 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_solution_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5674 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_solution_self_help_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33377 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_troubleshooters_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:40:26.545424 azure-mgmt-selfhelp-2.0.0b3/azure_mgmt_selfhelp.egg-info/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5696 2024-04-24 04:40:26.000000 azure-mgmt-selfhelp-2.0.0b3/azure_mgmt_selfhelp.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2556 2024-04-24 04:40:26.000000 azure-mgmt-selfhelp-2.0.0b3/azure_mgmt_selfhelp.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-24 04:40:26.000000 azure-mgmt-selfhelp-2.0.0b3/azure_mgmt_selfhelp.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-24 04:40:26.000000 azure-mgmt-selfhelp-2.0.0b3/azure_mgmt_selfhelp.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       56 2024-04-24 04:40:26.000000 azure-mgmt-selfhelp-2.0.0b3/azure_mgmt_selfhelp.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-04-24 04:40:26.000000 azure-mgmt-selfhelp-2.0.0b3/azure_mgmt_selfhelp.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-04-24 04:40:26.545424 azure-mgmt-selfhelp-2.0.0b3/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2769 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:40:26.545424 azure-mgmt-selfhelp-2.0.0b3/tests/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2616 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/tests/conftest.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      741 2024-04-24 04:39:04.000000 azure-mgmt-selfhelp-2.0.0b3/tests/test_cli_mgmt_selfhelp.py
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/CHANGELOG.md` & `azure-mgmt-selfhelp-2.0.0b3/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,28 @@
 # Release History
 
+## 2.0.0b3 (2024-04-22)
+
+### Features Added
+
+  - Added operation SolutionOperations.warm_up
+  - Added operation group DiscoverySolutionNLPSubscriptionScopeOperations
+  - Added operation group DiscoverySolutionNLPTenantScopeOperations
+  - Added operation group SimplifiedSolutionsOperations
+  - Added operation group SolutionSelfHelpOperations
+  - Model AutomatedCheckResult has a new parameter status
+  - Model AutomatedCheckResult has a new parameter version
+  - Model ResponseValidationProperties has a new parameter validation_scope
+  - Model SolutionsDiagnostic has a new parameter estimated_completion_time
+  - Model StepInput has a new parameter question_title
+
+### Breaking Changes
+
+  - Operation DiscoverySolutionOperations.list no longer has parameter scope
+
 ## 2.0.0b2 (2023-12-18)
 
 ### Features Added
 
   - Model SolutionPatchRequestBody has a new parameter content
   - Model SolutionPatchRequestBody has a new parameter parameters
   - Model SolutionPatchRequestBody has a new parameter provisioning_state
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/LICENSE` & `azure-mgmt-selfhelp-2.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b2/PKG-INFO` & `azure-mgmt-selfhelp-2.0.0b3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-selfhelp
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: Microsoft Azure Selfhelp Management Client Library for Python
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
 
 This is the Microsoft Azure Selfhelp Management Client Library.
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
 pip install azure-mgmt-selfhelp
 pip install azure-identity
@@ -86,14 +82,33 @@
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 # Release History
 
+## 2.0.0b3 (2024-04-22)
+
+### Features Added
+
+  - Added operation SolutionOperations.warm_up
+  - Added operation group DiscoverySolutionNLPSubscriptionScopeOperations
+  - Added operation group DiscoverySolutionNLPTenantScopeOperations
+  - Added operation group SimplifiedSolutionsOperations
+  - Added operation group SolutionSelfHelpOperations
+  - Model AutomatedCheckResult has a new parameter status
+  - Model AutomatedCheckResult has a new parameter version
+  - Model ResponseValidationProperties has a new parameter validation_scope
+  - Model SolutionsDiagnostic has a new parameter estimated_completion_time
+  - Model StepInput has a new parameter question_title
+
+### Breaking Changes
+
+  - Operation DiscoverySolutionOperations.list no longer has parameter scope
+
 ## 2.0.0b2 (2023-12-18)
 
 ### Features Added
 
   - Model SolutionPatchRequestBody has a new parameter content
   - Model SolutionPatchRequestBody has a new parameter parameters
   - Model SolutionPatchRequestBody has a new parameter provisioning_state
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/README.md` & `azure-mgmt-selfhelp-2.0.0b3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Microsoft Azure SDK for Python
 
 This is the Microsoft Azure Selfhelp Management Client Library.
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
 pip install azure-mgmt-selfhelp
 pip install azure-identity
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/_meta.json` & `azure-mgmt-selfhelp-2.0.0b3/_meta.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'autorest_command'": "'autorest specification/help/resource-manager/readme.md "*

 * *                       '--generate-sample=True --include-x-ms-examples-original-file=True --python '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk '*

 * *                       '--use=@autorest/python@6.13.7 --use=@autorest/modelerfour@4.27.0 '*

 * *                       "--version=3.9.7 --version-tolerant=False'",*

 * * "'commit'": "'835b124ff8160d23823c0e770b4989ca79e7418c'",*

 * * "'use'": "['@autores […]*

```diff
@@ -1,11 +1,11 @@
 {
     "autorest": "3.9.7",
-    "autorest_command": "autorest specification/help/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.7.1 --use=@autorest/modelerfour@4.26.2 --version=3.9.7 --version-tolerant=False",
-    "commit": "df4c0dccbfb696b378dfef8c7e451dfa4b82b175",
+    "autorest_command": "autorest specification/help/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.13.7 --use=@autorest/modelerfour@4.27.0 --version=3.9.7 --version-tolerant=False",
+    "commit": "835b124ff8160d23823c0e770b4989ca79e7418c",
     "readme": "specification/help/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
-        "@autorest/python@6.7.1",
-        "@autorest/modelerfour@4.26.2"
+        "@autorest/python@6.13.7",
+        "@autorest/modelerfour@4.27.0"
     ]
 }
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/__init__.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/_configuration.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/_configuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,58 +4,62 @@
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
 
 
-class SelfHelpMgmtClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+class SelfHelpMgmtClientConfiguration:  # pylint: disable=too-many-instance-attributes,name-too-long
     """Configuration for SelfHelpMgmtClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
-    :keyword api_version: Api Version. Default value is "2023-09-01-preview". Note that overriding
+    :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
+    :type subscription_id: str
+    :keyword api_version: Api Version. Default value is "2024-03-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(self, credential: "TokenCredential", **kwargs: Any) -> None:
-        super(SelfHelpMgmtClientConfiguration, self).__init__(**kwargs)
-        api_version: str = kwargs.pop("api_version", "2023-09-01-preview")
+    def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
+        api_version: str = kwargs.pop("api_version", "2024-03-01-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
+        if subscription_id is None:
+            raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
+        self.subscription_id = subscription_id
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["https://management.azure.com/.default"])
         kwargs.setdefault("sdk_moniker", "mgmt-selfhelp/{}".format(VERSION))
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

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/_patch.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/_serialization.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/_serialization.py`

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

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/_vendor.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/__init__.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/_configuration.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/_configuration.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,58 +4,62 @@
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
 
 
-class SelfHelpMgmtClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+class SelfHelpMgmtClientConfiguration:  # pylint: disable=too-many-instance-attributes,name-too-long
     """Configuration for SelfHelpMgmtClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :keyword api_version: Api Version. Default value is "2023-09-01-preview". Note that overriding
+    :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
+    :type subscription_id: str
+    :keyword api_version: Api Version. Default value is "2024-03-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(self, credential: "AsyncTokenCredential", **kwargs: Any) -> None:
-        super(SelfHelpMgmtClientConfiguration, self).__init__(**kwargs)
-        api_version: str = kwargs.pop("api_version", "2023-09-01-preview")
+    def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
+        api_version: str = kwargs.pop("api_version", "2024-03-01-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
+        if subscription_id is None:
+            raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
+        self.subscription_id = subscription_id
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["https://management.azure.com/.default"])
         kwargs.setdefault("sdk_moniker", "mgmt-selfhelp/{}".format(VERSION))
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

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/_patch.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/_self_help_mgmt_client.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/_self_help_mgmt_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,83 +5,138 @@
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, Awaitable, TYPE_CHECKING
 
+from azure.core.pipeline import policies
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 from azure.mgmt.core import AsyncARMPipelineClient
+from azure.mgmt.core.policies import AsyncARMAutoResourceProviderRegistrationPolicy
 
 from .. import models as _models
 from .._serialization import Deserializer, Serializer
 from ._configuration import SelfHelpMgmtClientConfiguration
 from .operations import (
     CheckNameAvailabilityOperations,
     DiagnosticsOperations,
+    DiscoverySolutionNLPSubscriptionScopeOperations,
+    DiscoverySolutionNLPTenantScopeOperations,
     DiscoverySolutionOperations,
     Operations,
+    SimplifiedSolutionsOperations,
     SolutionOperations,
+    SolutionSelfHelpOperations,
     TroubleshootersOperations,
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
-class SelfHelpMgmtClient:  # pylint: disable=client-accepts-api-version-keyword
+class SelfHelpMgmtClient:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
     """Help RP provider.
 
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.selfhelp.aio.operations.Operations
     :ivar check_name_availability: CheckNameAvailabilityOperations operations
     :vartype check_name_availability:
      azure.mgmt.selfhelp.aio.operations.CheckNameAvailabilityOperations
     :ivar diagnostics: DiagnosticsOperations operations
     :vartype diagnostics: azure.mgmt.selfhelp.aio.operations.DiagnosticsOperations
     :ivar discovery_solution: DiscoverySolutionOperations operations
     :vartype discovery_solution: azure.mgmt.selfhelp.aio.operations.DiscoverySolutionOperations
     :ivar solution: SolutionOperations operations
     :vartype solution: azure.mgmt.selfhelp.aio.operations.SolutionOperations
+    :ivar simplified_solutions: SimplifiedSolutionsOperations operations
+    :vartype simplified_solutions: azure.mgmt.selfhelp.aio.operations.SimplifiedSolutionsOperations
     :ivar troubleshooters: TroubleshootersOperations operations
     :vartype troubleshooters: azure.mgmt.selfhelp.aio.operations.TroubleshootersOperations
+    :ivar solution_self_help: SolutionSelfHelpOperations operations
+    :vartype solution_self_help: azure.mgmt.selfhelp.aio.operations.SolutionSelfHelpOperations
+    :ivar discovery_solution_nlp_tenant_scope: DiscoverySolutionNLPTenantScopeOperations operations
+    :vartype discovery_solution_nlp_tenant_scope:
+     azure.mgmt.selfhelp.aio.operations.DiscoverySolutionNLPTenantScopeOperations
+    :ivar discovery_solution_nlp_subscription_scope:
+     DiscoverySolutionNLPSubscriptionScopeOperations operations
+    :vartype discovery_solution_nlp_subscription_scope:
+     azure.mgmt.selfhelp.aio.operations.DiscoverySolutionNLPSubscriptionScopeOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
+    :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
+    :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2023-09-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2024-03-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
-        self, credential: "AsyncTokenCredential", base_url: str = "https://management.azure.com", **kwargs: Any
+        self,
+        credential: "AsyncTokenCredential",
+        subscription_id: str,
+        base_url: str = "https://management.azure.com",
+        **kwargs: Any
     ) -> None:
-        self._config = SelfHelpMgmtClientConfiguration(credential=credential, **kwargs)
-        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        self._config = SelfHelpMgmtClientConfiguration(credential=credential, subscription_id=subscription_id, **kwargs)
+        _policies = kwargs.pop("policies", None)
+        if _policies is None:
+            _policies = [
+                policies.RequestIdPolicy(**kwargs),
+                self._config.headers_policy,
+                self._config.user_agent_policy,
+                self._config.proxy_policy,
+                policies.ContentDecodePolicy(**kwargs),
+                AsyncARMAutoResourceProviderRegistrationPolicy(),
+                self._config.redirect_policy,
+                self._config.retry_policy,
+                self._config.authentication_policy,
+                self._config.custom_hook_policy,
+                self._config.logging_policy,
+                policies.DistributedTracingPolicy(**kwargs),
+                policies.SensitiveHeaderCleanupPolicy(**kwargs) if self._config.redirect_policy else None,
+                self._config.http_logging_policy,
+            ]
+        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, policies=_policies, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.check_name_availability = CheckNameAvailabilityOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.diagnostics = DiagnosticsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.discovery_solution = DiscoverySolutionOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.solution = SolutionOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.simplified_solutions = SimplifiedSolutionsOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
         self.troubleshooters = TroubleshootersOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.solution_self_help = SolutionSelfHelpOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
+        self.discovery_solution_nlp_tenant_scope = DiscoverySolutionNLPTenantScopeOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
+        self.discovery_solution_nlp_subscription_scope = DiscoverySolutionNLPSubscriptionScopeOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
 
-    def _send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
+    def _send_request(
+        self, request: HttpRequest, *, stream: bool = False, **kwargs: Any
+    ) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
         >>> response = await client._send_request(request)
         <AsyncHttpResponse: 200 OK>
@@ -93,15 +148,15 @@
         :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
         :rtype: ~azure.core.rest.AsyncHttpResponse
         """
 
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
-        return self._client.send_request(request_copy, **kwargs)
+        return self._client.send_request(request_copy, stream=stream, **kwargs)  # type: ignore
 
     async def close(self) -> None:
         await self._client.close()
 
     async def __aenter__(self) -> "SelfHelpMgmtClient":
         await self._client.__aenter__()
         return self
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/operations/__init__.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,23 +7,31 @@
 # --------------------------------------------------------------------------
 
 from ._operations import Operations
 from ._check_name_availability_operations import CheckNameAvailabilityOperations
 from ._diagnostics_operations import DiagnosticsOperations
 from ._discovery_solution_operations import DiscoverySolutionOperations
 from ._solution_operations import SolutionOperations
+from ._simplified_solutions_operations import SimplifiedSolutionsOperations
 from ._troubleshooters_operations import TroubleshootersOperations
+from ._solution_self_help_operations import SolutionSelfHelpOperations
+from ._discovery_solution_nlp_tenant_scope_operations import DiscoverySolutionNLPTenantScopeOperations
+from ._discovery_solution_nlp_subscription_scope_operations import DiscoverySolutionNLPSubscriptionScopeOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "Operations",
     "CheckNameAvailabilityOperations",
     "DiagnosticsOperations",
     "DiscoverySolutionOperations",
     "SolutionOperations",
+    "SimplifiedSolutionsOperations",
     "TroubleshootersOperations",
+    "SolutionSelfHelpOperations",
+    "DiscoverySolutionNLPTenantScopeOperations",
+    "DiscoverySolutionNLPSubscriptionScopeOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/operations/_check_name_availability_operations.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_check_name_availability_operations.py`

 * *Files 9% similar despite different names*

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
@@ -69,70 +69,64 @@
         :type scope: str
         :param check_name_availability_request: The required parameters for availability check. Default
          value is None.
         :type check_name_availability_request: ~azure.mgmt.selfhelp.models.CheckNameAvailabilityRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CheckNameAvailabilityResponse or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.CheckNameAvailabilityResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def post(
         self,
         scope: str,
-        check_name_availability_request: Optional[IO] = None,
+        check_name_availability_request: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.CheckNameAvailabilityResponse:
         """This API is used to check the uniqueness of a resource name used for a diagnostic,
         troubleshooter or solutions.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param check_name_availability_request: The required parameters for availability check. Default
          value is None.
-        :type check_name_availability_request: IO
+        :type check_name_availability_request: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CheckNameAvailabilityResponse or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.CheckNameAvailabilityResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def post(
         self,
         scope: str,
-        check_name_availability_request: Optional[Union[_models.CheckNameAvailabilityRequest, IO]] = None,
+        check_name_availability_request: Optional[Union[_models.CheckNameAvailabilityRequest, IO[bytes]]] = None,
         **kwargs: Any
     ) -> _models.CheckNameAvailabilityResponse:
         """This API is used to check the uniqueness of a resource name used for a diagnostic,
         troubleshooter or solutions.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param check_name_availability_request: The required parameters for availability check. Is
-         either a CheckNameAvailabilityRequest type or a IO type. Default value is None.
+         either a CheckNameAvailabilityRequest type or a IO[bytes] type. Default value is None.
         :type check_name_availability_request: ~azure.mgmt.selfhelp.models.CheckNameAvailabilityRequest
-         or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         or IO[bytes]
         :return: CheckNameAvailabilityResponse or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.CheckNameAvailabilityResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -155,40 +149,37 @@
             _content = check_name_availability_request
         else:
             if check_name_availability_request is not None:
                 _json = self._serialize.body(check_name_availability_request, "CheckNameAvailabilityRequest")
             else:
                 _json = None
 
-        request = build_post_request(
+        _request = build_post_request(
             scope=scope,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.post.metadata["url"],
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
 
         deserialized = self._deserialize("CheckNameAvailabilityResponse", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    post.metadata = {"url": "/{scope}/providers/Microsoft.Help/checkNameAvailability"}
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/operations/_diagnostics_operations.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_diagnostics_operations.py`

 * *Files 12% similar despite different names*

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
@@ -14,54 +14,124 @@
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse
-from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
+from azure.core.pipeline.transport import HttpResponse
+from azure.core.polling import LROPoller, NoPolling, PollingMethod
 from azure.core.rest import HttpRequest
-from azure.core.tracing.decorator_async import distributed_trace_async
+from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
-from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
+from azure.mgmt.core.polling.arm_polling import ARMPolling
 
-from ... import models as _models
-from ..._vendor import _convert_request
-from ...operations._diagnostics_operations import build_create_request, build_get_request
+from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import _convert_request
 
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
+
+
+def build_create_request(scope: str, diagnostics_resource_name: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop("template_url", "/{scope}/providers/Microsoft.Help/diagnostics/{diagnosticsResourceName}")
+    path_format_arguments = {
+        "scope": _SERIALIZER.url("scope", scope, "str", skip_quote=True),
+        "diagnosticsResourceName": _SERIALIZER.url(
+            "diagnostics_resource_name",
+            diagnostics_resource_name,
+            "str",
+            max_length=100,
+            min_length=1,
+            pattern=r"^[A-Za-z0-9-+@()_]+$",
+        ),
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
+def build_get_request(scope: str, diagnostics_resource_name: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-preview"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop("template_url", "/{scope}/providers/Microsoft.Help/diagnostics/{diagnosticsResourceName}")
+    path_format_arguments = {
+        "scope": _SERIALIZER.url("scope", scope, "str", skip_quote=True),
+        "diagnosticsResourceName": _SERIALIZER.url(
+            "diagnostics_resource_name",
+            diagnostics_resource_name,
+            "str",
+            max_length=100,
+            min_length=1,
+            pattern=r"^[A-Za-z0-9-+@()_]+$",
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
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 class DiagnosticsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.selfhelp.aio.SelfHelpMgmtClient`'s
+        :class:`~azure.mgmt.selfhelp.SelfHelpMgmtClient`'s
         :attr:`diagnostics` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    async def _create_initial(
+    def _create_initial(
         self,
         scope: str,
         diagnostics_resource_name: str,
-        diagnostic_resource_request: Optional[Union[_models.DiagnosticResource, IO]] = None,
+        diagnostic_resource_request: Optional[Union[_models.DiagnosticResource, IO[bytes]]] = None,
         **kwargs: Any
     ) -> _models.DiagnosticResource:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -82,31 +152,30 @@
             _content = diagnostic_resource_request
         else:
             if diagnostic_resource_request is not None:
                 _json = self._serialize.body(diagnostic_resource_request, "DiagnosticResource")
             else:
                 _json = None
 
-        request = build_create_request(
+        _request = build_create_request(
             scope=scope,
             diagnostics_resource_name=diagnostics_resource_name,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_initial.metadata["url"],
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
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -119,153 +188,118 @@
             deserialized = self._deserialize("DiagnosticResource", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_initial.metadata = {"url": "/{scope}/providers/Microsoft.Help/diagnostics/{diagnosticsResourceName}"}
-
     @overload
-    async def begin_create(
+    def begin_create(
         self,
         scope: str,
         diagnostics_resource_name: str,
         diagnostic_resource_request: Optional[_models.DiagnosticResource] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.DiagnosticResource]:
-        """Creates a diagnostic for the specific resource using solutionId and requiredInputs* from
-        discovery solutions. :code:`<br/>`Diagnostics are powerful solutions that access product
-        resources or other relevant data and provide the root cause of the issue and the steps to
-        address the issue.:code:`<br/>`:code:`<br/>` :code:`<b>Note: </b>` ‘requiredInputs’ from
-        Discovery solutions response must be passed via ‘additionalParameters’ as an input to
-        Diagnostics API.
+    ) -> LROPoller[_models.DiagnosticResource]:
+        """Creates a diagnostic for the specific resource using solutionId from discovery solutions.
+        :code:`<br/>`Diagnostics are powerful solutions that access product resources or other relevant
+        data and provide the root cause of the issue and the steps to address the
+        issue.:code:`<br/>`:code:`<br/>`.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param diagnostics_resource_name: Unique resource name for insight resources. Required.
         :type diagnostics_resource_name: str
         :param diagnostic_resource_request: The required request body for this insightResource
          invocation. Default value is None.
         :type diagnostic_resource_request: ~azure.mgmt.selfhelp.models.DiagnosticResource
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
-        :return: An instance of AsyncLROPoller that returns either DiagnosticResource or the result of
+        :return: An instance of LROPoller that returns either DiagnosticResource or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.selfhelp.models.DiagnosticResource]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.selfhelp.models.DiagnosticResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    async def begin_create(
+    def begin_create(
         self,
         scope: str,
         diagnostics_resource_name: str,
-        diagnostic_resource_request: Optional[IO] = None,
+        diagnostic_resource_request: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.DiagnosticResource]:
-        """Creates a diagnostic for the specific resource using solutionId and requiredInputs* from
-        discovery solutions. :code:`<br/>`Diagnostics are powerful solutions that access product
-        resources or other relevant data and provide the root cause of the issue and the steps to
-        address the issue.:code:`<br/>`:code:`<br/>` :code:`<b>Note: </b>` ‘requiredInputs’ from
-        Discovery solutions response must be passed via ‘additionalParameters’ as an input to
-        Diagnostics API.
+    ) -> LROPoller[_models.DiagnosticResource]:
+        """Creates a diagnostic for the specific resource using solutionId from discovery solutions.
+        :code:`<br/>`Diagnostics are powerful solutions that access product resources or other relevant
+        data and provide the root cause of the issue and the steps to address the
+        issue.:code:`<br/>`:code:`<br/>`.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param diagnostics_resource_name: Unique resource name for insight resources. Required.
         :type diagnostics_resource_name: str
         :param diagnostic_resource_request: The required request body for this insightResource
          invocation. Default value is None.
-        :type diagnostic_resource_request: IO
+        :type diagnostic_resource_request: IO[bytes]
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
-        :return: An instance of AsyncLROPoller that returns either DiagnosticResource or the result of
+        :return: An instance of LROPoller that returns either DiagnosticResource or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.selfhelp.models.DiagnosticResource]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.selfhelp.models.DiagnosticResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
-    @distributed_trace_async
-    async def begin_create(
+    @distributed_trace
+    def begin_create(
         self,
         scope: str,
         diagnostics_resource_name: str,
-        diagnostic_resource_request: Optional[Union[_models.DiagnosticResource, IO]] = None,
+        diagnostic_resource_request: Optional[Union[_models.DiagnosticResource, IO[bytes]]] = None,
         **kwargs: Any
-    ) -> AsyncLROPoller[_models.DiagnosticResource]:
-        """Creates a diagnostic for the specific resource using solutionId and requiredInputs* from
-        discovery solutions. :code:`<br/>`Diagnostics are powerful solutions that access product
-        resources or other relevant data and provide the root cause of the issue and the steps to
-        address the issue.:code:`<br/>`:code:`<br/>` :code:`<b>Note: </b>` ‘requiredInputs’ from
-        Discovery solutions response must be passed via ‘additionalParameters’ as an input to
-        Diagnostics API.
+    ) -> LROPoller[_models.DiagnosticResource]:
+        """Creates a diagnostic for the specific resource using solutionId from discovery solutions.
+        :code:`<br/>`Diagnostics are powerful solutions that access product resources or other relevant
+        data and provide the root cause of the issue and the steps to address the
+        issue.:code:`<br/>`:code:`<br/>`.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param diagnostics_resource_name: Unique resource name for insight resources. Required.
         :type diagnostics_resource_name: str
         :param diagnostic_resource_request: The required request body for this insightResource
-         invocation. Is either a DiagnosticResource type or a IO type. Default value is None.
-        :type diagnostic_resource_request: ~azure.mgmt.selfhelp.models.DiagnosticResource or IO
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
-        :return: An instance of AsyncLROPoller that returns either DiagnosticResource or the result of
+         invocation. Is either a DiagnosticResource type or a IO[bytes] type. Default value is None.
+        :type diagnostic_resource_request: ~azure.mgmt.selfhelp.models.DiagnosticResource or IO[bytes]
+        :return: An instance of LROPoller that returns either DiagnosticResource or the result of
          cls(response)
-        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.selfhelp.models.DiagnosticResource]
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.selfhelp.models.DiagnosticResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.DiagnosticResource] = kwargs.pop("cls", None)
-        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = await self._create_initial(
+            raw_result = self._create_initial(
                 scope=scope,
                 diagnostics_resource_name=diagnostics_resource_name,
                 diagnostic_resource_request=diagnostic_resource_request,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
@@ -273,49 +307,47 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("DiagnosticResource", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
-            polling_method: AsyncPollingMethod = cast(
-                AsyncPollingMethod,
-                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
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
+            return LROPoller[_models.DiagnosticResource].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create.metadata = {"url": "/{scope}/providers/Microsoft.Help/diagnostics/{diagnosticsResourceName}"}
+        return LROPoller[_models.DiagnosticResource](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
-    @distributed_trace_async
-    async def get(self, scope: str, diagnostics_resource_name: str, **kwargs: Any) -> _models.DiagnosticResource:
+    @distributed_trace
+    def get(self, scope: str, diagnostics_resource_name: str, **kwargs: Any) -> _models.DiagnosticResource:
         """Get the diagnostics using the 'diagnosticsResourceName' you chose while creating the
         diagnostic.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param diagnostics_resource_name: Unique resource name for insight resources. Required.
         :type diagnostics_resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: DiagnosticResource or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.DiagnosticResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -326,38 +358,35 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DiagnosticResource] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             scope=scope,
             diagnostics_resource_name=diagnostics_resource_name,
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
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("DiagnosticResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {"url": "/{scope}/providers/Microsoft.Help/diagnostics/{diagnosticsResourceName}"}
+        return deserialized  # type: ignore
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/operations/_discovery_solution_operations.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_discovery_solution_operations.py`

 * *Files 10% similar despite different names*

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
@@ -50,40 +50,36 @@
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(
-        self, scope: str, filter: Optional[str] = None, skiptoken: Optional[str] = None, **kwargs: Any
+        self, filter: Optional[str] = None, skiptoken: Optional[str] = None, **kwargs: Any
     ) -> AsyncIterable["_models.SolutionMetadataResource"]:
-        """Lists the relevant Azure diagnostics and solutions using `problemClassification API
+        """Lists the relevant Azure Diagnostics, Solutions and Troubleshooters using
+        `problemClassification API
         <https://learn.microsoft.com/rest/api/support/problem-classifications/list?tabs=HTTP>`_\ ) AND
         resourceUri or resourceType.:code:`<br/>` Discovery Solutions is the initial entry point within
         Help API, which identifies relevant Azure diagnostics and solutions. :code:`<br/>`:code:`<br/>`
         Required Input :  problemClassificationId (Use the `problemClassification API
         <https://learn.microsoft.com/rest/api/support/problem-classifications/list?tabs=HTTP>`_\ )
         :code:`<br/>`Optional input: resourceUri OR resource Type :code:`<br/>`:code:`<br/>`
         :code:`<b>Note: </b>`  ‘requiredInputs’ from Discovery solutions response must be passed via
         ‘additionalParameters’ as an input to Diagnostics and Solutions API.
 
-        :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
-         /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
-         Required.
-        :type scope: str
         :param filter: 'ProblemClassificationId' is a mandatory filter to get solutions ids. It also
          supports optional 'ResourceType' and 'SolutionType' filters. The `$filter
          <https://learn.microsoft.com/en-us/odata/webapi/first-odata-api#filter>`_ supports only 'and',
          'or' and 'eq' operators. Example: $filter=ProblemClassificationId eq
          '1ddda5b4-cf6c-4d4f-91ad-bc38ab0e811e'. Default value is None.
         :type filter: str
         :param skiptoken: Skiptoken is only used if a previous operation returned a partial result.
          Default value is None.
         :type skiptoken: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either SolutionMetadataResource or the result of
          cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.selfhelp.models.SolutionMetadataResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
@@ -99,63 +95,59 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
-                    scope=scope,
+                _request = build_list_request(
                     filter=filter,
                     skiptoken=skiptoken,
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
             deserialized = self._deserialize("DiscoveryResponse", pipeline_response)
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
-    list.metadata = {"url": "/{scope}/providers/Microsoft.Help/discoverySolutions"}
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/operations/_operations.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_operations.py`

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
@@ -52,15 +52,14 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, **kwargs: Any) -> AsyncIterable["_models.Operation"]:
         """Returns list of operations.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Operation or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.selfhelp.models.Operation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -74,60 +73,57 @@
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
-    list.metadata = {"url": "/providers/Microsoft.Help/operations"}
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/operations/_patch.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/operations/_solution_operations.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_solution_operations.py`

 * *Files 10% similar despite different names*

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
@@ -24,15 +24,20 @@
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._solution_operations import build_create_request, build_get_request, build_update_request
+from ...operations._solution_operations import (
+    build_create_request,
+    build_get_request,
+    build_update_request,
+    build_warm_up_request,
+)
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class SolutionOperations:
     """
@@ -53,15 +58,15 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     async def _create_initial(
         self,
         scope: str,
         solution_resource_name: str,
-        solution_request_body: Optional[Union[_models.SolutionResource, IO]] = None,
+        solution_request_body: Optional[Union[_models.SolutionResource, IO[bytes]]] = None,
         **kwargs: Any
     ) -> _models.SolutionResource:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -82,31 +87,30 @@
             _content = solution_request_body
         else:
             if solution_request_body is not None:
                 _json = self._serialize.body(solution_request_body, "SolutionResource")
             else:
                 _json = None
 
-        request = build_create_request(
+        _request = build_create_request(
             scope=scope,
             solution_resource_name=solution_resource_name,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_initial.metadata["url"],
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
@@ -119,170 +123,117 @@
             deserialized = self._deserialize("SolutionResource", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_initial.metadata = {"url": "/{scope}/providers/Microsoft.Help/solutions/{solutionResourceName}"}
-
     @overload
     async def begin_create(
         self,
         scope: str,
         solution_resource_name: str,
         solution_request_body: Optional[_models.SolutionResource] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.SolutionResource]:
         """Creates a solution for the specific Azure resource or subscription using the inputs ‘solutionId
         and requiredInputs’ from discovery solutions. :code:`<br/>` Azure solutions comprise a
         comprehensive library of self-help resources that have been thoughtfully curated by Azure
         engineers to aid customers in resolving typical troubleshooting issues. These solutions
-        encompass (1.) dynamic and context-aware diagnostics, guided troubleshooting wizards, and data
-        visualizations, (2.) rich instructional video tutorials and illustrative diagrams and images,
-        and (3.) thoughtfully assembled textual troubleshooting instructions. All these components are
-        seamlessly converged into unified solutions tailored to address a specific support problem
-        area. Each solution type may require one or more ‘requiredParameters’ that are required to
-        execute the individual solution component. In the absence of the ‘requiredParameters’ it is
-        likely that some of the solutions might fail execution, and you might see an empty response.
-        :code:`<br/>`:code:`<br/>` :code:`<b>Note:</b>`  :code:`<br/>`1. ‘requiredInputs’ from
-        Discovery solutions response must be passed via ‘parameters’ in the request body of Solutions
-        API. :code:`<br/>`2. ‘requiredParameters’ from the Solutions response is the same as ‘
-        additionalParameters’ in the request for diagnostics :code:`<br/>`3. ‘requiredParameters’ from
-        the Solutions response is the same as ‘properties.parameters’ in the request for
-        Troubleshooters.
+        encompass: :code:`<br/>` (1.) Dynamic and context-aware diagnostics, guided troubleshooting
+        wizards, and data visualizations. :code:`<br/>` (2.) Rich instructional video tutorials and
+        illustrative diagrams and images. :code:`<br/>` (3.) Thoughtfully assembled textual
+        troubleshooting instructions. :code:`<br/>` All these components are seamlessly converged into
+        unified solutions tailored to address a specific support problem area.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param solution_resource_name: Solution resource Name. Required.
         :type solution_resource_name: str
         :param solution_request_body: The required request body for this solution resource creation.
          Default value is None.
         :type solution_request_body: ~azure.mgmt.selfhelp.models.SolutionResource
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
         :return: An instance of AsyncLROPoller that returns either SolutionResource or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.selfhelp.models.SolutionResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_create(
         self,
         scope: str,
         solution_resource_name: str,
-        solution_request_body: Optional[IO] = None,
+        solution_request_body: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.SolutionResource]:
         """Creates a solution for the specific Azure resource or subscription using the inputs ‘solutionId
         and requiredInputs’ from discovery solutions. :code:`<br/>` Azure solutions comprise a
         comprehensive library of self-help resources that have been thoughtfully curated by Azure
         engineers to aid customers in resolving typical troubleshooting issues. These solutions
-        encompass (1.) dynamic and context-aware diagnostics, guided troubleshooting wizards, and data
-        visualizations, (2.) rich instructional video tutorials and illustrative diagrams and images,
-        and (3.) thoughtfully assembled textual troubleshooting instructions. All these components are
-        seamlessly converged into unified solutions tailored to address a specific support problem
-        area. Each solution type may require one or more ‘requiredParameters’ that are required to
-        execute the individual solution component. In the absence of the ‘requiredParameters’ it is
-        likely that some of the solutions might fail execution, and you might see an empty response.
-        :code:`<br/>`:code:`<br/>` :code:`<b>Note:</b>`  :code:`<br/>`1. ‘requiredInputs’ from
-        Discovery solutions response must be passed via ‘parameters’ in the request body of Solutions
-        API. :code:`<br/>`2. ‘requiredParameters’ from the Solutions response is the same as ‘
-        additionalParameters’ in the request for diagnostics :code:`<br/>`3. ‘requiredParameters’ from
-        the Solutions response is the same as ‘properties.parameters’ in the request for
-        Troubleshooters.
+        encompass: :code:`<br/>` (1.) Dynamic and context-aware diagnostics, guided troubleshooting
+        wizards, and data visualizations. :code:`<br/>` (2.) Rich instructional video tutorials and
+        illustrative diagrams and images. :code:`<br/>` (3.) Thoughtfully assembled textual
+        troubleshooting instructions. :code:`<br/>` All these components are seamlessly converged into
+        unified solutions tailored to address a specific support problem area.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param solution_resource_name: Solution resource Name. Required.
         :type solution_resource_name: str
         :param solution_request_body: The required request body for this solution resource creation.
          Default value is None.
-        :type solution_request_body: IO
+        :type solution_request_body: IO[bytes]
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
         :return: An instance of AsyncLROPoller that returns either SolutionResource or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.selfhelp.models.SolutionResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_create(
         self,
         scope: str,
         solution_resource_name: str,
-        solution_request_body: Optional[Union[_models.SolutionResource, IO]] = None,
+        solution_request_body: Optional[Union[_models.SolutionResource, IO[bytes]]] = None,
         **kwargs: Any
     ) -> AsyncLROPoller[_models.SolutionResource]:
         """Creates a solution for the specific Azure resource or subscription using the inputs ‘solutionId
         and requiredInputs’ from discovery solutions. :code:`<br/>` Azure solutions comprise a
         comprehensive library of self-help resources that have been thoughtfully curated by Azure
         engineers to aid customers in resolving typical troubleshooting issues. These solutions
-        encompass (1.) dynamic and context-aware diagnostics, guided troubleshooting wizards, and data
-        visualizations, (2.) rich instructional video tutorials and illustrative diagrams and images,
-        and (3.) thoughtfully assembled textual troubleshooting instructions. All these components are
-        seamlessly converged into unified solutions tailored to address a specific support problem
-        area. Each solution type may require one or more ‘requiredParameters’ that are required to
-        execute the individual solution component. In the absence of the ‘requiredParameters’ it is
-        likely that some of the solutions might fail execution, and you might see an empty response.
-        :code:`<br/>`:code:`<br/>` :code:`<b>Note:</b>`  :code:`<br/>`1. ‘requiredInputs’ from
-        Discovery solutions response must be passed via ‘parameters’ in the request body of Solutions
-        API. :code:`<br/>`2. ‘requiredParameters’ from the Solutions response is the same as ‘
-        additionalParameters’ in the request for diagnostics :code:`<br/>`3. ‘requiredParameters’ from
-        the Solutions response is the same as ‘properties.parameters’ in the request for
-        Troubleshooters.
+        encompass: :code:`<br/>` (1.) Dynamic and context-aware diagnostics, guided troubleshooting
+        wizards, and data visualizations. :code:`<br/>` (2.) Rich instructional video tutorials and
+        illustrative diagrams and images. :code:`<br/>` (3.) Thoughtfully assembled textual
+        troubleshooting instructions. :code:`<br/>` All these components are seamlessly converged into
+        unified solutions tailored to address a specific support problem area.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param solution_resource_name: Solution resource Name. Required.
         :type solution_resource_name: str
         :param solution_request_body: The required request body for this solution resource creation. Is
-         either a SolutionResource type or a IO type. Default value is None.
-        :type solution_request_body: ~azure.mgmt.selfhelp.models.SolutionResource or IO
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
+         either a SolutionResource type or a IO[bytes] type. Default value is None.
+        :type solution_request_body: ~azure.mgmt.selfhelp.models.SolutionResource or IO[bytes]
         :return: An instance of AsyncLROPoller that returns either SolutionResource or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.selfhelp.models.SolutionResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -306,48 +257,47 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("SolutionResource", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod,
                 AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
             )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.SolutionResource].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create.metadata = {"url": "/{scope}/providers/Microsoft.Help/solutions/{solutionResourceName}"}
+        return AsyncLROPoller[_models.SolutionResource](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     @distributed_trace_async
     async def get(self, scope: str, solution_resource_name: str, **kwargs: Any) -> _models.SolutionResource:
         """Get the solution using the applicable solutionResourceName while creating the solution.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param solution_resource_name: Solution resource Name. Required.
         :type solution_resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SolutionResource or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.SolutionResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -358,51 +308,48 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.SolutionResource] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             scope=scope,
             solution_resource_name=solution_resource_name,
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
 
         deserialized = self._deserialize("SolutionResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {"url": "/{scope}/providers/Microsoft.Help/solutions/{solutionResourceName}"}
+        return deserialized  # type: ignore
 
     async def _update_initial(
         self,
         scope: str,
         solution_resource_name: str,
-        solution_patch_request_body: Optional[Union[_models.SolutionPatchRequestBody, IO]] = None,
+        solution_patch_request_body: Optional[Union[_models.SolutionPatchRequestBody, IO[bytes]]] = None,
         **kwargs: Any
     ) -> _models.SolutionResource:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -423,31 +370,30 @@
             _content = solution_patch_request_body
         else:
             if solution_patch_request_body is not None:
                 _json = self._serialize.body(solution_patch_request_body, "SolutionPatchRequestBody")
             else:
                 _json = None
 
-        request = build_update_request(
+        _request = build_update_request(
             scope=scope,
             solution_resource_name=solution_resource_name,
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
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -465,16 +411,14 @@
             deserialized = self._deserialize("SolutionResource", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
-    _update_initial.metadata = {"url": "/{scope}/providers/Microsoft.Help/solutions/{solutionResourceName}"}
-
     @overload
     async def begin_update(
         self,
         scope: str,
         solution_resource_name: str,
         solution_patch_request_body: Optional[_models.SolutionPatchRequestBody] = None,
         *,
@@ -491,96 +435,70 @@
         :type solution_resource_name: str
         :param solution_patch_request_body: The required request body for updating a solution resource.
          Default value is None.
         :type solution_patch_request_body: ~azure.mgmt.selfhelp.models.SolutionPatchRequestBody
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
         :return: An instance of AsyncLROPoller that returns either SolutionResource or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.selfhelp.models.SolutionResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def begin_update(
         self,
         scope: str,
         solution_resource_name: str,
-        solution_patch_request_body: Optional[IO] = None,
+        solution_patch_request_body: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> AsyncLROPoller[_models.SolutionResource]:
         """Update the requiredInputs or additional information needed to execute the solution.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param solution_resource_name: Solution resource Name. Required.
         :type solution_resource_name: str
         :param solution_patch_request_body: The required request body for updating a solution resource.
          Default value is None.
-        :type solution_patch_request_body: IO
+        :type solution_patch_request_body: IO[bytes]
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
         :return: An instance of AsyncLROPoller that returns either SolutionResource or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.selfhelp.models.SolutionResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def begin_update(
         self,
         scope: str,
         solution_resource_name: str,
-        solution_patch_request_body: Optional[Union[_models.SolutionPatchRequestBody, IO]] = None,
+        solution_patch_request_body: Optional[Union[_models.SolutionPatchRequestBody, IO[bytes]]] = None,
         **kwargs: Any
     ) -> AsyncLROPoller[_models.SolutionResource]:
         """Update the requiredInputs or additional information needed to execute the solution.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param solution_resource_name: Solution resource Name. Required.
         :type solution_resource_name: str
         :param solution_patch_request_body: The required request body for updating a solution resource.
-         Is either a SolutionPatchRequestBody type or a IO type. Default value is None.
-        :type solution_patch_request_body: ~azure.mgmt.selfhelp.models.SolutionPatchRequestBody or IO
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
+         Is either a SolutionPatchRequestBody type or a IO[bytes] type. Default value is None.
+        :type solution_patch_request_body: ~azure.mgmt.selfhelp.models.SolutionPatchRequestBody or
+         IO[bytes]
         :return: An instance of AsyncLROPoller that returns either SolutionResource or the result of
          cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.selfhelp.models.SolutionResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -608,29 +526,166 @@
         def get_long_running_output(pipeline_response):
             response_headers = {}
             response = pipeline_response.http_response
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
 
             deserialized = self._deserialize("SolutionResource", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, response_headers)
+                return cls(pipeline_response, deserialized, response_headers)  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: AsyncPollingMethod = cast(
                 AsyncPollingMethod,
                 AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
             )
         elif polling is False:
             polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return AsyncLROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.SolutionResource].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+        return AsyncLROPoller[_models.SolutionResource](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
+
+    @overload
+    async def warm_up(  # pylint: disable=inconsistent-return-statements
+        self,
+        scope: str,
+        solution_resource_name: str,
+        solution_warm_up_request_body: Optional[_models.SolutionWarmUpRequestBody] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """Warm up the solution resource by preloading asynchronous diagnostics results into cache.
 
-    begin_update.metadata = {"url": "/{scope}/providers/Microsoft.Help/solutions/{solutionResourceName}"}
+        :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
+         /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
+         Required.
+        :type scope: str
+        :param solution_resource_name: Solution resource Name. Required.
+        :type solution_resource_name: str
+        :param solution_warm_up_request_body: The required request body for warming up a solution
+         resource. Default value is None.
+        :type solution_warm_up_request_body: ~azure.mgmt.selfhelp.models.SolutionWarmUpRequestBody
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None or the result of cls(response)
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def warm_up(  # pylint: disable=inconsistent-return-statements
+        self,
+        scope: str,
+        solution_resource_name: str,
+        solution_warm_up_request_body: Optional[IO[bytes]] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """Warm up the solution resource by preloading asynchronous diagnostics results into cache.
+
+        :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
+         /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
+         Required.
+        :type scope: str
+        :param solution_resource_name: Solution resource Name. Required.
+        :type solution_resource_name: str
+        :param solution_warm_up_request_body: The required request body for warming up a solution
+         resource. Default value is None.
+        :type solution_warm_up_request_body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None or the result of cls(response)
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def warm_up(  # pylint: disable=inconsistent-return-statements
+        self,
+        scope: str,
+        solution_resource_name: str,
+        solution_warm_up_request_body: Optional[Union[_models.SolutionWarmUpRequestBody, IO[bytes]]] = None,
+        **kwargs: Any
+    ) -> None:
+        """Warm up the solution resource by preloading asynchronous diagnostics results into cache.
+
+        :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
+         /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
+         Required.
+        :type scope: str
+        :param solution_resource_name: Solution resource Name. Required.
+        :type solution_resource_name: str
+        :param solution_warm_up_request_body: The required request body for warming up a solution
+         resource. Is either a SolutionWarmUpRequestBody type or a IO[bytes] type. Default value is
+         None.
+        :type solution_warm_up_request_body: ~azure.mgmt.selfhelp.models.SolutionWarmUpRequestBody or
+         IO[bytes]
+        :return: None or the result of cls(response)
+        :rtype: None
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
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(solution_warm_up_request_body, (IOBase, bytes)):
+            _content = solution_warm_up_request_body
+        else:
+            if solution_warm_up_request_body is not None:
+                _json = self._serialize.body(solution_warm_up_request_body, "SolutionWarmUpRequestBody")
+            else:
+                _json = None
+
+        _request = build_warm_up_request(
+            scope=scope,
+            solution_resource_name=solution_resource_name,
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
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
+        if response.status_code not in [204]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/aio/operations/_troubleshooters_operations.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_troubleshooters_operations.py`

 * *Files 3% similar despite different names*

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
@@ -85,26 +85,25 @@
         :type troubleshooter_name: str
         :param create_troubleshooter_request_body: The required request body for this Troubleshooter
          resource creation. Default value is None.
         :type create_troubleshooter_request_body: ~azure.mgmt.selfhelp.models.TroubleshooterResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: TroubleshooterResource or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.TroubleshooterResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def create(
         self,
         scope: str,
         troubleshooter_name: str,
-        create_troubleshooter_request_body: Optional[IO] = None,
+        create_troubleshooter_request_body: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.TroubleshooterResource:
         """Creates the specific troubleshooter action under a resource or subscription using the
         ‘solutionId’ and  ‘properties.parameters’ as the trigger. :code:`<br/>` Azure Troubleshooters
         help with hard to classify issues, reducing the gap between customer observed problems and
@@ -119,30 +118,29 @@
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param troubleshooter_name: Troubleshooter resource Name. Required.
         :type troubleshooter_name: str
         :param create_troubleshooter_request_body: The required request body for this Troubleshooter
          resource creation. Default value is None.
-        :type create_troubleshooter_request_body: IO
+        :type create_troubleshooter_request_body: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: TroubleshooterResource or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.TroubleshooterResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def create(
         self,
         scope: str,
         troubleshooter_name: str,
-        create_troubleshooter_request_body: Optional[Union[_models.TroubleshooterResource, IO]] = None,
+        create_troubleshooter_request_body: Optional[Union[_models.TroubleshooterResource, IO[bytes]]] = None,
         **kwargs: Any
     ) -> _models.TroubleshooterResource:
         """Creates the specific troubleshooter action under a resource or subscription using the
         ‘solutionId’ and  ‘properties.parameters’ as the trigger. :code:`<br/>` Azure Troubleshooters
         help with hard to classify issues, reducing the gap between customer observed problems and
         solutions by guiding the user effortlessly through the troubleshooting process. Each
         Troubleshooter flow represents a problem area within Azure and has a complex tree-like
@@ -154,21 +152,18 @@
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param troubleshooter_name: Troubleshooter resource Name. Required.
         :type troubleshooter_name: str
         :param create_troubleshooter_request_body: The required request body for this Troubleshooter
-         resource creation. Is either a TroubleshooterResource type or a IO type. Default value is None.
+         resource creation. Is either a TroubleshooterResource type or a IO[bytes] type. Default value
+         is None.
         :type create_troubleshooter_request_body: ~azure.mgmt.selfhelp.models.TroubleshooterResource or
-         IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         IO[bytes]
         :return: TroubleshooterResource or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.TroubleshooterResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -191,31 +186,30 @@
             _content = create_troubleshooter_request_body
         else:
             if create_troubleshooter_request_body is not None:
                 _json = self._serialize.body(create_troubleshooter_request_body, "TroubleshooterResource")
             else:
                 _json = None
 
-        request = build_create_request(
+        _request = build_create_request(
             scope=scope,
             troubleshooter_name=troubleshooter_name,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.create.metadata["url"],
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
@@ -228,31 +222,28 @@
             deserialized = self._deserialize("TroubleshooterResource", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    create.metadata = {"url": "/{scope}/providers/Microsoft.Help/troubleshooters/{troubleshooterName}"}
-
     @distributed_trace_async
     async def get(self, scope: str, troubleshooter_name: str, **kwargs: Any) -> _models.TroubleshooterResource:
         """Gets troubleshooter instance result which includes the step status/result of the troubleshooter
         resource name that is being executed.:code:`<br/>` Get API is used to retrieve the result of a
         Troubleshooter instance, which includes the status and result of each step in the
         Troubleshooter workflow. This API requires the Troubleshooter resource name that was created
         using the Create API.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param troubleshooter_name: Troubleshooter resource Name. Required.
         :type troubleshooter_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: TroubleshooterResource or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.TroubleshooterResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -263,45 +254,42 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.TroubleshooterResource] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             scope=scope,
             troubleshooter_name=troubleshooter_name,
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
 
         deserialized = self._deserialize("TroubleshooterResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {"url": "/{scope}/providers/Microsoft.Help/troubleshooters/{troubleshooterName}"}
+        return deserialized  # type: ignore
 
     @overload
     async def continue_method(  # pylint: disable=inconsistent-return-statements
         self,
         scope: str,
         troubleshooter_name: str,
         continue_request_body: Optional[_models.ContinueRequestBody] = None,
@@ -322,26 +310,25 @@
         :type troubleshooter_name: str
         :param continue_request_body: The required request body for going to next step in
          Troubleshooter resource. Default value is None.
         :type continue_request_body: ~azure.mgmt.selfhelp.models.ContinueRequestBody
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def continue_method(  # pylint: disable=inconsistent-return-statements
         self,
         scope: str,
         troubleshooter_name: str,
-        continue_request_body: Optional[IO] = None,
+        continue_request_body: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> None:
         """Uses ‘stepId’ and ‘responses’ as the trigger to continue the troubleshooting steps for the
         respective troubleshooter resource name. :code:`<br/>`Continue API is used to provide inputs
         that are required for the specific troubleshooter to progress into the next step in the
@@ -351,51 +338,46 @@
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param troubleshooter_name: Troubleshooter resource Name. Required.
         :type troubleshooter_name: str
         :param continue_request_body: The required request body for going to next step in
          Troubleshooter resource. Default value is None.
-        :type continue_request_body: IO
+        :type continue_request_body: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def continue_method(  # pylint: disable=inconsistent-return-statements
         self,
         scope: str,
         troubleshooter_name: str,
-        continue_request_body: Optional[Union[_models.ContinueRequestBody, IO]] = None,
+        continue_request_body: Optional[Union[_models.ContinueRequestBody, IO[bytes]]] = None,
         **kwargs: Any
     ) -> None:
         """Uses ‘stepId’ and ‘responses’ as the trigger to continue the troubleshooting steps for the
         respective troubleshooter resource name. :code:`<br/>`Continue API is used to provide inputs
         that are required for the specific troubleshooter to progress into the next step in the
         process. This API is used after the Troubleshooter has been created using the Create API.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param troubleshooter_name: Troubleshooter resource Name. Required.
         :type troubleshooter_name: str
         :param continue_request_body: The required request body for going to next step in
-         Troubleshooter resource. Is either a ContinueRequestBody type or a IO type. Default value is
-         None.
-        :type continue_request_body: ~azure.mgmt.selfhelp.models.ContinueRequestBody or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         Troubleshooter resource. Is either a ContinueRequestBody type or a IO[bytes] type. Default
+         value is None.
+        :type continue_request_body: ~azure.mgmt.selfhelp.models.ContinueRequestBody or IO[bytes]
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -418,63 +400,57 @@
             _content = continue_request_body
         else:
             if continue_request_body is not None:
                 _json = self._serialize.body(continue_request_body, "ContinueRequestBody")
             else:
                 _json = None
 
-        request = build_continue_method_request(
+        _request = build_continue_method_request(
             scope=scope,
             troubleshooter_name=troubleshooter_name,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.continue_method.metadata["url"],
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
 
         if response.status_code not in [204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    continue_method.metadata = {
-        "url": "/{scope}/providers/Microsoft.Help/troubleshooters/{troubleshooterName}/continue"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def end(  # pylint: disable=inconsistent-return-statements
         self, scope: str, troubleshooter_name: str, **kwargs: Any
     ) -> None:
         """Ends the troubleshooter action.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param troubleshooter_name: Troubleshooter resource Name. Required.
         :type troubleshooter_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -485,44 +461,41 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_end_request(
+        _request = build_end_request(
             scope=scope,
             troubleshooter_name=troubleshooter_name,
             api_version=api_version,
-            template_url=self.end.metadata["url"],
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
 
         if response.status_code not in [204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    end.metadata = {"url": "/{scope}/providers/Microsoft.Help/troubleshooters/{troubleshooterName}/end"}
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace_async
     async def restart(
         self, scope: str, troubleshooter_name: str, **kwargs: Any
     ) -> _models.RestartTroubleshooterResponse:
         """Restarts the troubleshooter API using applicable troubleshooter resource name as the
         input.:code:`<br/>` It returns new resource name which should be used in subsequent request.
@@ -530,15 +503,14 @@
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param troubleshooter_name: Troubleshooter resource Name. Required.
         :type troubleshooter_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RestartTroubleshooterResponse or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.RestartTroubleshooterResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -549,28 +521,27 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.RestartTroubleshooterResponse] = kwargs.pop("cls", None)
 
-        request = build_restart_request(
+        _request = build_restart_request(
             scope=scope,
             troubleshooter_name=troubleshooter_name,
             api_version=api_version,
-            template_url=self.restart.metadata["url"],
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
@@ -578,12 +549,10 @@
 
         response_headers = {}
         response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
 
         deserialized = self._deserialize("RestartTroubleshooterResponse", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
-        return deserialized
-
-    restart.metadata = {"url": "/{scope}/providers/Microsoft.Help/troubleshooters/{troubleshooterName}/restart"}
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/models/__init__.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/models/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,42 +5,51 @@
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._models_py3 import AutomatedCheckResult
 from ._models_py3 import CheckNameAvailabilityRequest
 from ._models_py3 import CheckNameAvailabilityResponse
+from ._models_py3 import ClassificationService
 from ._models_py3 import ContinueRequestBody
 from ._models_py3 import Diagnostic
 from ._models_py3 import DiagnosticInvocation
 from ._models_py3 import DiagnosticResource
+from ._models_py3 import DiscoveryNlpRequest
+from ._models_py3 import DiscoveryNlpResponse
 from ._models_py3 import DiscoveryResponse
 from ._models_py3 import Error
 from ._models_py3 import ErrorAdditionalInfo
 from ._models_py3 import ErrorDetail
 from ._models_py3 import ErrorResponse
 from ._models_py3 import Filter
 from ._models_py3 import FilterGroup
 from ._models_py3 import Insight
 from ._models_py3 import MetricsBasedChart
 from ._models_py3 import Operation
 from ._models_py3 import OperationDisplay
 from ._models_py3 import OperationListResult
 from ._models_py3 import ProxyResource
 from ._models_py3 import ReplacementMaps
+from ._models_py3 import ReplacementMapsSelfHelp
 from ._models_py3 import Resource
 from ._models_py3 import ResponseOption
 from ._models_py3 import ResponseValidationProperties
 from ._models_py3 import RestartTroubleshooterResponse
 from ._models_py3 import SearchResult
 from ._models_py3 import Section
+from ._models_py3 import SectionSelfHelp
+from ._models_py3 import SimplifiedSolutionsResource
 from ._models_py3 import SolutionMetadataProperties
 from ._models_py3 import SolutionMetadataResource
+from ._models_py3 import SolutionNlpMetadataResource
 from ._models_py3 import SolutionPatchRequestBody
 from ._models_py3 import SolutionResource
+from ._models_py3 import SolutionResourceSelfHelp
+from ._models_py3 import SolutionWarmUpRequestBody
 from ._models_py3 import SolutionsDiagnostic
 from ._models_py3 import SolutionsTroubleshooters
 from ._models_py3 import Step
 from ._models_py3 import StepInput
 from ._models_py3 import SystemData
 from ._models_py3 import TriggerCriterion
 from ._models_py3 import TroubleshooterResource
@@ -64,50 +73,60 @@
 from ._self_help_mgmt_client_enums import QuestionType
 from ._self_help_mgmt_client_enums import ResultType
 from ._self_help_mgmt_client_enums import SolutionProvisioningState
 from ._self_help_mgmt_client_enums import SolutionType
 from ._self_help_mgmt_client_enums import Status
 from ._self_help_mgmt_client_enums import TroubleshooterProvisioningState
 from ._self_help_mgmt_client_enums import Type
+from ._self_help_mgmt_client_enums import ValidationScope
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "AutomatedCheckResult",
     "CheckNameAvailabilityRequest",
     "CheckNameAvailabilityResponse",
+    "ClassificationService",
     "ContinueRequestBody",
     "Diagnostic",
     "DiagnosticInvocation",
     "DiagnosticResource",
+    "DiscoveryNlpRequest",
+    "DiscoveryNlpResponse",
     "DiscoveryResponse",
     "Error",
     "ErrorAdditionalInfo",
     "ErrorDetail",
     "ErrorResponse",
     "Filter",
     "FilterGroup",
     "Insight",
     "MetricsBasedChart",
     "Operation",
     "OperationDisplay",
     "OperationListResult",
     "ProxyResource",
     "ReplacementMaps",
+    "ReplacementMapsSelfHelp",
     "Resource",
     "ResponseOption",
     "ResponseValidationProperties",
     "RestartTroubleshooterResponse",
     "SearchResult",
     "Section",
+    "SectionSelfHelp",
+    "SimplifiedSolutionsResource",
     "SolutionMetadataProperties",
     "SolutionMetadataResource",
+    "SolutionNlpMetadataResource",
     "SolutionPatchRequestBody",
     "SolutionResource",
+    "SolutionResourceSelfHelp",
+    "SolutionWarmUpRequestBody",
     "SolutionsDiagnostic",
     "SolutionsTroubleshooters",
     "Step",
     "StepInput",
     "SystemData",
     "TriggerCriterion",
     "TroubleshooterResource",
@@ -130,10 +149,11 @@
     "QuestionType",
     "ResultType",
     "SolutionProvisioningState",
     "SolutionType",
     "Status",
     "TroubleshooterProvisioningState",
     "Type",
+    "ValidationScope",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/models/_models_py3.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/models/_models_py3.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,40 +16,54 @@
     # pylint: disable=unused-import,ungrouped-imports
     from .. import models as _models
 
 
 class AutomatedCheckResult(_serialization.Model):
     """Only for AutomatedStep type.
 
+    :ivar version: Version for automated check result.
+    :vartype version: str
+    :ivar status: Status for automated check result.
+    :vartype status: str
     :ivar result: Insight Article Content.
     :vartype result: str
     :ivar type: Type of Result. Known values are: "Success", "Warning", "Error", and "Information".
     :vartype type: str or ~azure.mgmt.selfhelp.models.AutomatedCheckResultType
     """
 
     _attribute_map = {
+        "version": {"key": "version", "type": "str"},
+        "status": {"key": "status", "type": "str"},
         "result": {"key": "result", "type": "str"},
         "type": {"key": "type", "type": "str"},
     }
 
     def __init__(
         self,
         *,
+        version: Optional[str] = None,
+        status: Optional[str] = None,
         result: Optional[str] = None,
         type: Optional[Union[str, "_models.AutomatedCheckResultType"]] = None,
         **kwargs: Any
     ) -> None:
         """
+        :keyword version: Version for automated check result.
+        :paramtype version: str
+        :keyword status: Status for automated check result.
+        :paramtype status: str
         :keyword result: Insight Article Content.
         :paramtype result: str
         :keyword type: Type of Result. Known values are: "Success", "Warning", "Error", and
          "Information".
         :paramtype type: str or ~azure.mgmt.selfhelp.models.AutomatedCheckResultType
         """
         super().__init__(**kwargs)
+        self.version = version
+        self.status = status
         self.result = result
         self.type = type
 
 
 class CheckNameAvailabilityRequest(_serialization.Model):
     """The check availability request body.
 
@@ -115,14 +129,49 @@
         """
         super().__init__(**kwargs)
         self.name_available = name_available
         self.reason = reason
         self.message = message
 
 
+class ClassificationService(_serialization.Model):
+    """Service Classification result object.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar service_id: Azure resource Id of the service.
+    :vartype service_id: str
+    :ivar display_name: Localized name of the azure service.
+    :vartype display_name: str
+    :ivar resource_types: List of applicable ARM resource types for this service.
+    :vartype resource_types: list[str]
+    """
+
+    _validation = {
+        "service_id": {"readonly": True},
+        "display_name": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "service_id": {"key": "serviceId", "type": "str"},
+        "display_name": {"key": "displayName", "type": "str"},
+        "resource_types": {"key": "resourceTypes", "type": "[str]"},
+    }
+
+    def __init__(self, *, resource_types: Optional[List[str]] = None, **kwargs: Any) -> None:
+        """
+        :keyword resource_types: List of applicable ARM resource types for this service.
+        :paramtype resource_types: list[str]
+        """
+        super().__init__(**kwargs)
+        self.service_id = None
+        self.display_name = None
+        self.resource_types = resource_types
+
+
 class ContinueRequestBody(_serialization.Model):
     """Troubleshooter ContinueRequest body.
 
     :ivar step_id: Unique id of the result.
     :vartype step_id: str
     :ivar responses:
     :vartype responses: list[~azure.mgmt.selfhelp.models.TroubleshooterResponse]
@@ -233,15 +282,15 @@
 
 class Resource(_serialization.Model):
     """Common fields that are returned in the response for all Azure Resource Manager resources.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. E.g.
-     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -275,52 +324,34 @@
 class ProxyResource(Resource):
     """The resource model definition for a Azure Resource Manager proxy resource. It will not have
     tags and a location.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. E.g.
-     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
     :vartype system_data: ~azure.mgmt.selfhelp.models.SystemData
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
 
 class DiagnosticResource(ProxyResource):
     """Diagnostic resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. E.g.
-     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -380,14 +411,89 @@
         self.global_parameters = global_parameters
         self.insights = insights
         self.accepted_at = None
         self.provisioning_state = None
         self.diagnostics = None
 
 
+class DiscoveryNlpRequest(_serialization.Model):
+    """Discover NLP request.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar issue_summary: Natural language description of the issue. Required.
+    :vartype issue_summary: str
+    :ivar resource_id: ARM resource Id of the resource that is having the issue.
+    :vartype resource_id: str
+    :ivar service_id: ARM service Id of the service that is having the issue. For more information
+     on service Id see https://learn.microsoft.com/rest/api/support/services/list?tabs=HTTP.
+    :vartype service_id: str
+    :ivar additional_context: Additional information in the form of a string.
+    :vartype additional_context: str
+    """
+
+    _validation = {
+        "issue_summary": {"required": True},
+    }
+
+    _attribute_map = {
+        "issue_summary": {"key": "issueSummary", "type": "str"},
+        "resource_id": {"key": "resourceId", "type": "str"},
+        "service_id": {"key": "serviceId", "type": "str"},
+        "additional_context": {"key": "additionalContext", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        issue_summary: str,
+        resource_id: Optional[str] = None,
+        service_id: Optional[str] = None,
+        additional_context: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword issue_summary: Natural language description of the issue. Required.
+        :paramtype issue_summary: str
+        :keyword resource_id: ARM resource Id of the resource that is having the issue.
+        :paramtype resource_id: str
+        :keyword service_id: ARM service Id of the service that is having the issue. For more
+         information on service Id see
+         https://learn.microsoft.com/rest/api/support/services/list?tabs=HTTP.
+        :paramtype service_id: str
+        :keyword additional_context: Additional information in the form of a string.
+        :paramtype additional_context: str
+        """
+        super().__init__(**kwargs)
+        self.issue_summary = issue_summary
+        self.resource_id = resource_id
+        self.service_id = service_id
+        self.additional_context = additional_context
+
+
+class DiscoveryNlpResponse(_serialization.Model):
+    """Successfully fetched list of solution metadata.
+
+    :ivar value: The list of solution metadata.
+    :vartype value: list[~azure.mgmt.selfhelp.models.SolutionNlpMetadataResource]
+    """
+
+    _attribute_map = {
+        "value": {"key": "value", "type": "[SolutionNlpMetadataResource]"},
+    }
+
+    def __init__(self, *, value: Optional[List["_models.SolutionNlpMetadataResource"]] = None, **kwargs: Any) -> None:
+        """
+        :keyword value: The list of solution metadata.
+        :paramtype value: list[~azure.mgmt.selfhelp.models.SolutionNlpMetadataResource]
+        """
+        super().__init__(**kwargs)
+        self.value = value
+
+
 class DiscoveryResponse(_serialization.Model):
     """Discovery response.
 
     :ivar value: The list of metadata.
     :vartype value: list[~azure.mgmt.selfhelp.models.SolutionMetadataResource]
     :ivar next_link: The link used to get the next page of solution metadata.
     :vartype next_link: str
@@ -896,14 +1002,55 @@
         self.diagnostics = diagnostics
         self.troubleshooters = troubleshooters
         self.metrics_based_charts = metrics_based_charts
         self.videos = videos
         self.video_groups = video_groups
 
 
+class ReplacementMapsSelfHelp(_serialization.Model):
+    """Solution replacement maps.
+
+    :ivar web_results: Solution AzureKB results.
+    :vartype web_results: list[~azure.mgmt.selfhelp.models.WebResult]
+    :ivar videos: Video solutions, which have the power to engage the customer by stimulating their
+     senses.
+    :vartype videos: list[~azure.mgmt.selfhelp.models.Video]
+    :ivar video_groups: Group of Videos.
+    :vartype video_groups: list[~azure.mgmt.selfhelp.models.VideoGroup]
+    """
+
+    _attribute_map = {
+        "web_results": {"key": "webResults", "type": "[WebResult]"},
+        "videos": {"key": "videos", "type": "[Video]"},
+        "video_groups": {"key": "videoGroups", "type": "[VideoGroup]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        web_results: Optional[List["_models.WebResult"]] = None,
+        videos: Optional[List["_models.Video"]] = None,
+        video_groups: Optional[List["_models.VideoGroup"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword web_results: Solution AzureKB results.
+        :paramtype web_results: list[~azure.mgmt.selfhelp.models.WebResult]
+        :keyword videos: Video solutions, which have the power to engage the customer by stimulating
+         their senses.
+        :paramtype videos: list[~azure.mgmt.selfhelp.models.Video]
+        :keyword video_groups: Group of Videos.
+        :paramtype video_groups: list[~azure.mgmt.selfhelp.models.VideoGroup]
+        """
+        super().__init__(**kwargs)
+        self.web_results = web_results
+        self.videos = videos
+        self.video_groups = video_groups
+
+
 class ResponseOption(_serialization.Model):
     """The status of the resource.
 
     :ivar key: Unique string.
     :vartype key: str
     :ivar value: Option description.
     :vartype value: str
@@ -927,50 +1074,59 @@
 
 
 class ResponseValidationProperties(_serialization.Model):
     """Troubleshooter step input response validation properties.
 
     :ivar regex: Regex used for the input validation.
     :vartype regex: str
+    :ivar validation_scope: Validation scope. Known values are: "None", "URLFormat", "GuidFormat",
+     "IpAddressFormat", and "NumberOnlyFormat".
+    :vartype validation_scope: str or ~azure.mgmt.selfhelp.models.ValidationScope
     :ivar is_required: Default True.
     :vartype is_required: bool
     :ivar validation_error_message: Validation Error Message.
     :vartype validation_error_message: str
     :ivar max_length: Max text input (open Ended Text).
     :vartype max_length: int
     """
 
     _attribute_map = {
         "regex": {"key": "regex", "type": "str"},
+        "validation_scope": {"key": "validationScope", "type": "str"},
         "is_required": {"key": "isRequired", "type": "bool"},
         "validation_error_message": {"key": "validationErrorMessage", "type": "str"},
         "max_length": {"key": "maxLength", "type": "int"},
     }
 
     def __init__(
         self,
         *,
         regex: Optional[str] = None,
+        validation_scope: Optional[Union[str, "_models.ValidationScope"]] = None,
         is_required: Optional[bool] = None,
         validation_error_message: Optional[str] = None,
         max_length: Optional[int] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword regex: Regex used for the input validation.
         :paramtype regex: str
+        :keyword validation_scope: Validation scope. Known values are: "None", "URLFormat",
+         "GuidFormat", "IpAddressFormat", and "NumberOnlyFormat".
+        :paramtype validation_scope: str or ~azure.mgmt.selfhelp.models.ValidationScope
         :keyword is_required: Default True.
         :paramtype is_required: bool
         :keyword validation_error_message: Validation Error Message.
         :paramtype validation_error_message: str
         :keyword max_length: Max text input (open Ended Text).
         :paramtype max_length: int
         """
         super().__init__(**kwargs)
         self.regex = regex
+        self.validation_scope = validation_scope
         self.is_required = is_required
         self.validation_error_message = validation_error_message
         self.max_length = max_length
 
 
 class RestartTroubleshooterResponse(_serialization.Model):
     """Troubleshooter restart response.
@@ -1108,22 +1264,135 @@
         """
         super().__init__(**kwargs)
         self.title = title
         self.content = content
         self.replacement_maps = replacement_maps
 
 
+class SectionSelfHelp(_serialization.Model):
+    """Part of the solution and are dividers in the solution rendering.
+
+    :ivar title: Solution sections title.
+    :vartype title: str
+    :ivar content: Solution sections content.
+    :vartype content: str
+    :ivar replacement_maps: Solution replacement maps.
+    :vartype replacement_maps: ~azure.mgmt.selfhelp.models.ReplacementMapsSelfHelp
+    """
+
+    _attribute_map = {
+        "title": {"key": "title", "type": "str"},
+        "content": {"key": "content", "type": "str"},
+        "replacement_maps": {"key": "replacementMaps", "type": "ReplacementMapsSelfHelp"},
+    }
+
+    def __init__(
+        self,
+        *,
+        title: Optional[str] = None,
+        content: Optional[str] = None,
+        replacement_maps: Optional["_models.ReplacementMapsSelfHelp"] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword title: Solution sections title.
+        :paramtype title: str
+        :keyword content: Solution sections content.
+        :paramtype content: str
+        :keyword replacement_maps: Solution replacement maps.
+        :paramtype replacement_maps: ~azure.mgmt.selfhelp.models.ReplacementMapsSelfHelp
+        """
+        super().__init__(**kwargs)
+        self.title = title
+        self.content = content
+        self.replacement_maps = replacement_maps
+
+
+class SimplifiedSolutionsResource(ProxyResource):
+    """Simplified Solutions response.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.selfhelp.models.SystemData
+    :ivar solution_id: Solution Id to identify single Simplified Solution.
+    :vartype solution_id: str
+    :ivar parameters: Client input parameters to run Simplified Solutions.
+    :vartype parameters: dict[str, str]
+    :ivar title: The title.
+    :vartype title: str
+    :ivar appendix: Additional parameter response for Simplified Solutions.
+    :vartype appendix: dict[str, str]
+    :ivar content: The HTML content that needs to be rendered and shown to customer.
+    :vartype content: str
+    :ivar provisioning_state: Status of Simplified Solution provisioning. Known values are:
+     "Succeeded", "PartialComplete", "Failed", "Running", and "Canceled".
+    :vartype provisioning_state: str or ~azure.mgmt.selfhelp.models.SolutionProvisioningState
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+        "title": {"readonly": True},
+        "appendix": {"readonly": True},
+        "content": {"readonly": True},
+        "provisioning_state": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+        "solution_id": {"key": "properties.solutionId", "type": "str"},
+        "parameters": {"key": "properties.parameters", "type": "{str}"},
+        "title": {"key": "properties.title", "type": "str"},
+        "appendix": {"key": "properties.appendix", "type": "{str}"},
+        "content": {"key": "properties.content", "type": "str"},
+        "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
+    }
+
+    def __init__(
+        self, *, solution_id: Optional[str] = None, parameters: Optional[Dict[str, str]] = None, **kwargs: Any
+    ) -> None:
+        """
+        :keyword solution_id: Solution Id to identify single Simplified Solution.
+        :paramtype solution_id: str
+        :keyword parameters: Client input parameters to run Simplified Solutions.
+        :paramtype parameters: dict[str, str]
+        """
+        super().__init__(**kwargs)
+        self.solution_id = solution_id
+        self.parameters = parameters
+        self.title = None
+        self.appendix = None
+        self.content = None
+        self.provisioning_state = None
+
+
 class SolutionMetadataProperties(_serialization.Model):
     """Metadata Properties.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar solution_id: Solution Id.
     :vartype solution_id: str
-    :ivar solution_type: Solution Type. Known values are: "Diagnostics" and "Solutions".
+    :ivar solution_type: Solution Type. Known values are: "Diagnostics", "Solutions",
+     "Troubleshooters", and "SelfHelp".
     :vartype solution_type: str or ~azure.mgmt.selfhelp.models.SolutionType
     :ivar description: A detailed description of solution.
     :vartype description: str
     :ivar required_inputs: Required parameters for invoking this particular solution.
     :vartype required_inputs: list[str]
     """
 
@@ -1154,15 +1423,15 @@
 
 class SolutionMetadataResource(ProxyResource):
     """Metadata resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. E.g.
-     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -1194,16 +1463,112 @@
         :keyword solutions: List of metadata.
         :paramtype solutions: list[~azure.mgmt.selfhelp.models.SolutionMetadataProperties]
         """
         super().__init__(**kwargs)
         self.solutions = solutions
 
 
+class SolutionNlpMetadataResource(ProxyResource):
+    """Nlp Metadata resource.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.selfhelp.models.SystemData
+    :ivar problem_title: Title of the problem classification.
+    :vartype problem_title: str
+    :ivar problem_description: Description of the problem classification.
+    :vartype problem_description: str
+    :ivar service_id: Id of the service
+     (https://learn.microsoft.com/en-us/rest/api/support/services?view=rest-support-2020-04-01) that
+     may be used to create a support ticket.
+    :vartype service_id: str
+    :ivar problem_classification_id: Id of the ProblemClassification
+     (https://learn.microsoft.com/en-us/rest/api/support/problem-classifications?view=rest-support-2020-04-01)
+     that may be used to create a support ticket.
+    :vartype problem_classification_id: str
+    :ivar solutions: The list of solution metadata.
+    :vartype solutions: list[~azure.mgmt.selfhelp.models.SolutionMetadataProperties]
+    :ivar related_services: The set of services that are most likely related to the request. If
+     relatedServices is included in the response then solutions may not be discovered until the
+     client calls a second time specifying one of the service Ids in the relatedServices object.
+    :vartype related_services: list[~azure.mgmt.selfhelp.models.ClassificationService]
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+        "problem_title": {"key": "properties.problemTitle", "type": "str"},
+        "problem_description": {"key": "properties.problemDescription", "type": "str"},
+        "service_id": {"key": "properties.serviceId", "type": "str"},
+        "problem_classification_id": {"key": "properties.problemClassificationId", "type": "str"},
+        "solutions": {"key": "properties.solutions", "type": "[SolutionMetadataProperties]"},
+        "related_services": {"key": "properties.relatedServices", "type": "[ClassificationService]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        problem_title: Optional[str] = None,
+        problem_description: Optional[str] = None,
+        service_id: Optional[str] = None,
+        problem_classification_id: Optional[str] = None,
+        solutions: Optional[List["_models.SolutionMetadataProperties"]] = None,
+        related_services: Optional[List["_models.ClassificationService"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword problem_title: Title of the problem classification.
+        :paramtype problem_title: str
+        :keyword problem_description: Description of the problem classification.
+        :paramtype problem_description: str
+        :keyword service_id: Id of the service
+         (https://learn.microsoft.com/en-us/rest/api/support/services?view=rest-support-2020-04-01) that
+         may be used to create a support ticket.
+        :paramtype service_id: str
+        :keyword problem_classification_id: Id of the ProblemClassification
+         (https://learn.microsoft.com/en-us/rest/api/support/problem-classifications?view=rest-support-2020-04-01)
+         that may be used to create a support ticket.
+        :paramtype problem_classification_id: str
+        :keyword solutions: The list of solution metadata.
+        :paramtype solutions: list[~azure.mgmt.selfhelp.models.SolutionMetadataProperties]
+        :keyword related_services: The set of services that are most likely related to the request. If
+         relatedServices is included in the response then solutions may not be discovered until the
+         client calls a second time specifying one of the service Ids in the relatedServices object.
+        :paramtype related_services: list[~azure.mgmt.selfhelp.models.ClassificationService]
+        """
+        super().__init__(**kwargs)
+        self.problem_title = problem_title
+        self.problem_description = problem_description
+        self.service_id = service_id
+        self.problem_classification_id = problem_classification_id
+        self.solutions = solutions
+        self.related_services = related_services
+
+
 class SolutionPatchRequestBody(_serialization.Model):
-    """Solution response.
+    """Solution PatchRequest body.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar trigger_criteria: Solution request trigger criteria.
     :vartype trigger_criteria: list[~azure.mgmt.selfhelp.models.TriggerCriterion]
     :ivar parameters: Client input parameters to run Solution.
     :vartype parameters: dict[str, str]
@@ -1268,15 +1633,15 @@
 
 class SolutionResource(ProxyResource):  # pylint: disable=too-many-instance-attributes
     """Solution response.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. E.g.
-     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -1349,72 +1714,143 @@
         self.provisioning_state = None
         self.title = None
         self.content = None
         self.replacement_maps = None
         self.sections = None
 
 
+class SolutionResourceSelfHelp(ProxyResource):
+    """Self Help Solution response.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.selfhelp.models.SystemData
+    :ivar solution_id: SolutionId is a unique id to identify a solution. You can retrieve the
+     solution id using the Discovery api -
+     https://learn.microsoft.com/en-us/rest/api/help/discovery-solution/list?view=rest-help-2023-09-01-preview&tabs=HTTP.  # pylint: disable=line-too-long
+    :vartype solution_id: str
+    :ivar title: The title.
+    :vartype title: str
+    :ivar content: The HTML content that needs to be rendered and shown to customer.
+    :vartype content: str
+    :ivar replacement_maps: Solution replacement maps.
+    :vartype replacement_maps: ~azure.mgmt.selfhelp.models.ReplacementMapsSelfHelp
+    :ivar sections: List of section object.
+    :vartype sections: list[~azure.mgmt.selfhelp.models.SectionSelfHelp]
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+        "solution_id": {"readonly": True},
+        "title": {"readonly": True},
+        "content": {"readonly": True},
+        "replacement_maps": {"readonly": True},
+        "sections": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+        "solution_id": {"key": "properties.solutionId", "type": "str"},
+        "title": {"key": "properties.title", "type": "str"},
+        "content": {"key": "properties.content", "type": "str"},
+        "replacement_maps": {"key": "properties.replacementMaps", "type": "ReplacementMapsSelfHelp"},
+        "sections": {"key": "properties.sections", "type": "[SectionSelfHelp]"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.solution_id = None
+        self.title = None
+        self.content = None
+        self.replacement_maps = None
+        self.sections = None
+
+
 class SolutionsDiagnostic(_serialization.Model):
     """Solutions Diagnostic.
 
     :ivar solution_id: Solution Id to identify single Solutions Diagnostic.
     :vartype solution_id: str
     :ivar status: Denotes the status of the diagnostic resource. Known values are: "Failed",
      "MissingInputs", "Running", "Succeeded", and "Timeout".
     :vartype status: str or ~azure.mgmt.selfhelp.models.Status
     :ivar status_details: Details of the status.
     :vartype status_details: str
     :ivar replacement_key: Place holder used in HTML Content replace control with the content.
     :vartype replacement_key: str
+    :ivar estimated_completion_time: Diagnostics estimated completion time in minutes.
+    :vartype estimated_completion_time: str
     :ivar required_parameters: Required parameters of this item.
     :vartype required_parameters: list[str]
     :ivar insights: Diagnostic insights.
     :vartype insights: list[~azure.mgmt.selfhelp.models.Insight]
     """
 
     _attribute_map = {
         "solution_id": {"key": "solutionId", "type": "str"},
         "status": {"key": "status", "type": "str"},
         "status_details": {"key": "statusDetails", "type": "str"},
         "replacement_key": {"key": "replacementKey", "type": "str"},
+        "estimated_completion_time": {"key": "estimatedCompletionTime", "type": "str"},
         "required_parameters": {"key": "requiredParameters", "type": "[str]"},
         "insights": {"key": "insights", "type": "[Insight]"},
     }
 
     def __init__(
         self,
         *,
         solution_id: Optional[str] = None,
         status: Optional[Union[str, "_models.Status"]] = None,
         status_details: Optional[str] = None,
         replacement_key: Optional[str] = None,
+        estimated_completion_time: Optional[str] = None,
         required_parameters: Optional[List[str]] = None,
         insights: Optional[List["_models.Insight"]] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword solution_id: Solution Id to identify single Solutions Diagnostic.
         :paramtype solution_id: str
         :keyword status: Denotes the status of the diagnostic resource. Known values are: "Failed",
          "MissingInputs", "Running", "Succeeded", and "Timeout".
         :paramtype status: str or ~azure.mgmt.selfhelp.models.Status
         :keyword status_details: Details of the status.
         :paramtype status_details: str
         :keyword replacement_key: Place holder used in HTML Content replace control with the content.
         :paramtype replacement_key: str
+        :keyword estimated_completion_time: Diagnostics estimated completion time in minutes.
+        :paramtype estimated_completion_time: str
         :keyword required_parameters: Required parameters of this item.
         :paramtype required_parameters: list[str]
         :keyword insights: Diagnostic insights.
         :paramtype insights: list[~azure.mgmt.selfhelp.models.Insight]
         """
         super().__init__(**kwargs)
         self.solution_id = solution_id
         self.status = status
         self.status_details = status_details
         self.replacement_key = replacement_key
+        self.estimated_completion_time = estimated_completion_time
         self.required_parameters = required_parameters
         self.insights = insights
 
 
 class SolutionsTroubleshooters(_serialization.Model):
     """Troubleshooters in Solutions.
 
@@ -1450,14 +1886,34 @@
         """
         super().__init__(**kwargs)
         self.solution_id = solution_id
         self.title = title
         self.summary = summary
 
 
+class SolutionWarmUpRequestBody(_serialization.Model):
+    """Solution WarmUpRequest body.
+
+    :ivar parameters: Dictionary of :code:`<string>`.
+    :vartype parameters: dict[str, str]
+    """
+
+    _attribute_map = {
+        "parameters": {"key": "parameters", "type": "{str}"},
+    }
+
+    def __init__(self, *, parameters: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
+        """
+        :keyword parameters: Dictionary of :code:`<string>`.
+        :paramtype parameters: dict[str, str]
+        """
+        super().__init__(**kwargs)
+        self.parameters = parameters
+
+
 class Step(_serialization.Model):  # pylint: disable=too-many-instance-attributes
     """Troubleshooter step.
 
     :ivar id: Unique step id.
     :vartype id: str
     :ivar title: Step title.
     :vartype title: str
@@ -1468,15 +1924,15 @@
     :ivar execution_status: Status of Troubleshooter Step execution. Known values are: "Success",
      "Running", "Failed", and "Warning".
     :vartype execution_status: str or ~azure.mgmt.selfhelp.models.ExecutionStatus
     :ivar execution_status_description: This field has more detailed status description of the
      execution status.
     :vartype execution_status_description: str
     :ivar type: Type of Troubleshooting step. Known values are: "Decision", "Solution", "Insight",
-     and "AutomatedCheck".
+     "AutomatedCheck", and "Input".
     :vartype type: str or ~azure.mgmt.selfhelp.models.Type
     :ivar is_last_step: is this last step of the workflow.
     :vartype is_last_step: bool
     :ivar inputs:
     :vartype inputs: list[~azure.mgmt.selfhelp.models.StepInput]
     :ivar automated_check_results: Only for AutomatedStep type.
     :vartype automated_check_results: ~azure.mgmt.selfhelp.models.AutomatedCheckResult
@@ -1530,15 +1986,15 @@
         :keyword execution_status: Status of Troubleshooter Step execution. Known values are:
          "Success", "Running", "Failed", and "Warning".
         :paramtype execution_status: str or ~azure.mgmt.selfhelp.models.ExecutionStatus
         :keyword execution_status_description: This field has more detailed status description of the
          execution status.
         :paramtype execution_status_description: str
         :keyword type: Type of Troubleshooting step. Known values are: "Decision", "Solution",
-         "Insight", and "AutomatedCheck".
+         "Insight", "AutomatedCheck", and "Input".
         :paramtype type: str or ~azure.mgmt.selfhelp.models.Type
         :keyword is_last_step: is this last step of the workflow.
         :paramtype is_last_step: bool
         :keyword inputs:
         :paramtype inputs: list[~azure.mgmt.selfhelp.models.StepInput]
         :keyword automated_check_results: Only for AutomatedStep type.
         :paramtype automated_check_results: ~azure.mgmt.selfhelp.models.AutomatedCheckResult
@@ -1564,16 +2020,18 @@
 
 class StepInput(_serialization.Model):
     """Details of step input.
 
     :ivar question_id: Use Index as QuestionId.
     :vartype question_id: str
     :ivar question_type: Type of Question. Known values are: "RadioButton", "Dropdown",
-     "TextInput", and "MultiLineInfoBox".
+     "TextInput", "MultiLineInfoBox", "DateTimePicker", and "MultiSelect".
     :vartype question_type: str or ~azure.mgmt.selfhelp.models.QuestionType
+    :ivar question_title: Question title.
+    :vartype question_title: str
     :ivar question_content: User question content.
     :vartype question_content: str
     :ivar question_content_type: Default is Text. Known values are: "Text", "Html", and "Markdown".
     :vartype question_content_type: str or ~azure.mgmt.selfhelp.models.QuestionContentType
     :ivar response_hint: Place holder text for response hints.
     :vartype response_hint: str
     :ivar recommended_option: Result of Automate step.
@@ -1586,14 +2044,15 @@
     :ivar response_options:
     :vartype response_options: list[~azure.mgmt.selfhelp.models.ResponseOption]
     """
 
     _attribute_map = {
         "question_id": {"key": "questionId", "type": "str"},
         "question_type": {"key": "questionType", "type": "str"},
+        "question_title": {"key": "questionTitle", "type": "str"},
         "question_content": {"key": "questionContent", "type": "str"},
         "question_content_type": {"key": "questionContentType", "type": "str"},
         "response_hint": {"key": "responseHint", "type": "str"},
         "recommended_option": {"key": "recommendedOption", "type": "str"},
         "selected_option_value": {"key": "selectedOptionValue", "type": "str"},
         "response_validation_properties": {
             "key": "responseValidationProperties",
@@ -1603,29 +2062,32 @@
     }
 
     def __init__(
         self,
         *,
         question_id: Optional[str] = None,
         question_type: Optional[Union[str, "_models.QuestionType"]] = None,
+        question_title: Optional[str] = None,
         question_content: Optional[str] = None,
         question_content_type: Optional[Union[str, "_models.QuestionContentType"]] = None,
         response_hint: Optional[str] = None,
         recommended_option: Optional[str] = None,
         selected_option_value: Optional[str] = None,
         response_validation_properties: Optional["_models.ResponseValidationProperties"] = None,
         response_options: Optional[List["_models.ResponseOption"]] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword question_id: Use Index as QuestionId.
         :paramtype question_id: str
         :keyword question_type: Type of Question. Known values are: "RadioButton", "Dropdown",
-         "TextInput", and "MultiLineInfoBox".
+         "TextInput", "MultiLineInfoBox", "DateTimePicker", and "MultiSelect".
         :paramtype question_type: str or ~azure.mgmt.selfhelp.models.QuestionType
+        :keyword question_title: Question title.
+        :paramtype question_title: str
         :keyword question_content: User question content.
         :paramtype question_content: str
         :keyword question_content_type: Default is Text. Known values are: "Text", "Html", and
          "Markdown".
         :paramtype question_content_type: str or ~azure.mgmt.selfhelp.models.QuestionContentType
         :keyword response_hint: Place holder text for response hints.
         :paramtype response_hint: str
@@ -1639,14 +2101,15 @@
          ~azure.mgmt.selfhelp.models.ResponseValidationProperties
         :keyword response_options:
         :paramtype response_options: list[~azure.mgmt.selfhelp.models.ResponseOption]
         """
         super().__init__(**kwargs)
         self.question_id = question_id
         self.question_type = question_type
+        self.question_title = question_title
         self.question_content = question_content
         self.question_content_type = question_content_type
         self.response_hint = response_hint
         self.recommended_option = recommended_option
         self.selected_option_value = selected_option_value
         self.response_validation_properties = response_validation_properties
         self.response_options = response_options
@@ -1750,15 +2213,15 @@
 
 class TroubleshooterResource(ProxyResource):
     """Troubleshooter response.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. E.g.
-     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -1813,15 +2276,15 @@
 
 class TroubleshooterResponse(_serialization.Model):
     """User Response for Troubleshooter continue request.
 
     :ivar question_id: id of the question.
     :vartype question_id: str
     :ivar question_type: Type of Question. Known values are: "RadioButton", "Dropdown",
-     "TextInput", and "MultiLineInfoBox".
+     "TextInput", "MultiLineInfoBox", "DateTimePicker", and "MultiSelect".
     :vartype question_type: str or ~azure.mgmt.selfhelp.models.QuestionType
     :ivar response: Response key for SingleInput. For Multi-line test/open ended question it is
      free form text.
     :vartype response: str
     """
 
     _attribute_map = {
@@ -1838,15 +2301,15 @@
         response: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword question_id: id of the question.
         :paramtype question_id: str
         :keyword question_type: Type of Question. Known values are: "RadioButton", "Dropdown",
-         "TextInput", and "MultiLineInfoBox".
+         "TextInput", "MultiLineInfoBox", "DateTimePicker", and "MultiSelect".
         :paramtype question_type: str or ~azure.mgmt.selfhelp.models.QuestionType
         :keyword response: Response key for SingleInput. For Multi-line test/open ended question it is
          free form text.
         :paramtype response: str
         """
         super().__init__(**kwargs)
         self.question_id = question_id
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/models/_patch.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/models/_self_help_mgmt_client_enums.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/models/_self_help_mgmt_client_enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,14 +124,18 @@
     """SingleChoice radio button"""
     DROPDOWN = "Dropdown"
     """SingleChoice dropdown."""
     TEXT_INPUT = "TextInput"
     """Text Input"""
     MULTI_LINE_INFO_BOX = "MultiLineInfoBox"
     """MultiLineInfoBox"""
+    DATE_TIME_PICKER = "DateTimePicker"
+    """DateTime Picker"""
+    MULTI_SELECT = "MultiSelect"
+    """Multi Select"""
 
 
 class ResultType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Result type of the search result."""
 
     COMMUNITY = "Community"
     DOCUMENTATION = "Documentation"
@@ -155,14 +159,18 @@
 class SolutionType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Solution Type."""
 
     DIAGNOSTICS = "Diagnostics"
     """Diagnostics resource type."""
     SOLUTIONS = "Solutions"
     """Solutions resource type."""
+    TROUBLESHOOTERS = "Troubleshooters"
+    """Troubleshooters resource type."""
+    SELF_HELP = "SelfHelp"
+    """SelfHelp resource type."""
 
 
 class Status(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Denotes the status of the diagnostic resource."""
 
     FAILED = "Failed"
     """Diagnostic creation failed."""
@@ -189,7 +197,18 @@
 class Type(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Type of Troubleshooting step."""
 
     DECISION = "Decision"
     SOLUTION = "Solution"
     INSIGHT = "Insight"
     AUTOMATED_CHECK = "AutomatedCheck"
+    INPUT = "Input"
+
+
+class ValidationScope(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Validation scope."""
+
+    NONE = "None"
+    URL_FORMAT = "URLFormat"
+    GUID_FORMAT = "GuidFormat"
+    IP_ADDRESS_FORMAT = "IpAddressFormat"
+    NUMBER_ONLY_FORMAT = "NumberOnlyFormat"
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/operations/__init__.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,23 +7,31 @@
 # --------------------------------------------------------------------------
 
 from ._operations import Operations
 from ._check_name_availability_operations import CheckNameAvailabilityOperations
 from ._diagnostics_operations import DiagnosticsOperations
 from ._discovery_solution_operations import DiscoverySolutionOperations
 from ._solution_operations import SolutionOperations
+from ._simplified_solutions_operations import SimplifiedSolutionsOperations
 from ._troubleshooters_operations import TroubleshootersOperations
+from ._solution_self_help_operations import SolutionSelfHelpOperations
+from ._discovery_solution_nlp_tenant_scope_operations import DiscoverySolutionNLPTenantScopeOperations
+from ._discovery_solution_nlp_subscription_scope_operations import DiscoverySolutionNLPSubscriptionScopeOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "Operations",
     "CheckNameAvailabilityOperations",
     "DiagnosticsOperations",
     "DiscoverySolutionOperations",
     "SolutionOperations",
+    "SimplifiedSolutionsOperations",
     "TroubleshootersOperations",
+    "SolutionSelfHelpOperations",
+    "DiscoverySolutionNLPTenantScopeOperations",
+    "DiscoverySolutionNLPSubscriptionScopeOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/operations/_check_name_availability_operations.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_check_name_availability_operations.py`

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
@@ -35,15 +35,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_post_request(scope: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/{scope}/providers/Microsoft.Help/checkNameAvailability")
     path_format_arguments = {
         "scope": _SERIALIZER.url("scope", scope, "str", skip_quote=True),
@@ -99,70 +99,64 @@
         :type scope: str
         :param check_name_availability_request: The required parameters for availability check. Default
          value is None.
         :type check_name_availability_request: ~azure.mgmt.selfhelp.models.CheckNameAvailabilityRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CheckNameAvailabilityResponse or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.CheckNameAvailabilityResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def post(
         self,
         scope: str,
-        check_name_availability_request: Optional[IO] = None,
+        check_name_availability_request: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.CheckNameAvailabilityResponse:
         """This API is used to check the uniqueness of a resource name used for a diagnostic,
         troubleshooter or solutions.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param check_name_availability_request: The required parameters for availability check. Default
          value is None.
-        :type check_name_availability_request: IO
+        :type check_name_availability_request: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CheckNameAvailabilityResponse or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.CheckNameAvailabilityResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def post(
         self,
         scope: str,
-        check_name_availability_request: Optional[Union[_models.CheckNameAvailabilityRequest, IO]] = None,
+        check_name_availability_request: Optional[Union[_models.CheckNameAvailabilityRequest, IO[bytes]]] = None,
         **kwargs: Any
     ) -> _models.CheckNameAvailabilityResponse:
         """This API is used to check the uniqueness of a resource name used for a diagnostic,
         troubleshooter or solutions.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param check_name_availability_request: The required parameters for availability check. Is
-         either a CheckNameAvailabilityRequest type or a IO type. Default value is None.
+         either a CheckNameAvailabilityRequest type or a IO[bytes] type. Default value is None.
         :type check_name_availability_request: ~azure.mgmt.selfhelp.models.CheckNameAvailabilityRequest
-         or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         or IO[bytes]
         :return: CheckNameAvailabilityResponse or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.CheckNameAvailabilityResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -185,40 +179,37 @@
             _content = check_name_availability_request
         else:
             if check_name_availability_request is not None:
                 _json = self._serialize.body(check_name_availability_request, "CheckNameAvailabilityRequest")
             else:
                 _json = None
 
-        request = build_post_request(
+        _request = build_post_request(
             scope=scope,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.post.metadata["url"],
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
 
         deserialized = self._deserialize("CheckNameAvailabilityResponse", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    post.metadata = {"url": "/{scope}/providers/Microsoft.Help/checkNameAvailability"}
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/operations/_diagnostics_operations.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/aio/operations/_diagnostics_operations.py`

 * *Files 22% similar despite different names*

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
@@ -14,124 +14,54 @@
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import HttpResponse
-from azure.core.polling import LROPoller, NoPolling, PollingMethod
+from azure.core.pipeline.transport import AsyncHttpResponse
+from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
 from azure.core.rest import HttpRequest
-from azure.core.tracing.decorator import distributed_trace
+from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
-from azure.mgmt.core.polling.arm_polling import ARMPolling
+from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
-from .. import models as _models
-from .._serialization import Serializer
-from .._vendor import _convert_request
+from ... import models as _models
+from ..._vendor import _convert_request
+from ...operations._diagnostics_operations import build_create_request, build_get_request
 
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
-
-_SERIALIZER = Serializer()
-_SERIALIZER.client_side_validation = False
-
-
-def build_create_request(scope: str, diagnostics_resource_name: str, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
-    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = kwargs.pop("template_url", "/{scope}/providers/Microsoft.Help/diagnostics/{diagnosticsResourceName}")
-    path_format_arguments = {
-        "scope": _SERIALIZER.url("scope", scope, "str", skip_quote=True),
-        "diagnosticsResourceName": _SERIALIZER.url(
-            "diagnostics_resource_name",
-            diagnostics_resource_name,
-            "str",
-            max_length=100,
-            min_length=1,
-            pattern=r"^[A-Za-z0-9-+@()_]+$",
-        ),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    if content_type is not None:
-        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-def build_get_request(scope: str, diagnostics_resource_name: str, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = kwargs.pop("template_url", "/{scope}/providers/Microsoft.Help/diagnostics/{diagnosticsResourceName}")
-    path_format_arguments = {
-        "scope": _SERIALIZER.url("scope", scope, "str", skip_quote=True),
-        "diagnosticsResourceName": _SERIALIZER.url(
-            "diagnostics_resource_name",
-            diagnostics_resource_name,
-            "str",
-            max_length=100,
-            min_length=1,
-            pattern=r"^[A-Za-z0-9-+@()_]+$",
-        ),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class DiagnosticsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.selfhelp.SelfHelpMgmtClient`'s
+        :class:`~azure.mgmt.selfhelp.aio.SelfHelpMgmtClient`'s
         :attr:`diagnostics` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    def _create_initial(
+    async def _create_initial(
         self,
         scope: str,
         diagnostics_resource_name: str,
-        diagnostic_resource_request: Optional[Union[_models.DiagnosticResource, IO]] = None,
+        diagnostic_resource_request: Optional[Union[_models.DiagnosticResource, IO[bytes]]] = None,
         **kwargs: Any
     ) -> _models.DiagnosticResource:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -152,31 +82,30 @@
             _content = diagnostic_resource_request
         else:
             if diagnostic_resource_request is not None:
                 _json = self._serialize.body(diagnostic_resource_request, "DiagnosticResource")
             else:
                 _json = None
 
-        request = build_create_request(
+        _request = build_create_request(
             scope=scope,
             diagnostics_resource_name=diagnostics_resource_name,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_initial.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -189,153 +118,118 @@
             deserialized = self._deserialize("DiagnosticResource", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_initial.metadata = {"url": "/{scope}/providers/Microsoft.Help/diagnostics/{diagnosticsResourceName}"}
-
     @overload
-    def begin_create(
+    async def begin_create(
         self,
         scope: str,
         diagnostics_resource_name: str,
         diagnostic_resource_request: Optional[_models.DiagnosticResource] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> LROPoller[_models.DiagnosticResource]:
-        """Creates a diagnostic for the specific resource using solutionId and requiredInputs* from
-        discovery solutions. :code:`<br/>`Diagnostics are powerful solutions that access product
-        resources or other relevant data and provide the root cause of the issue and the steps to
-        address the issue.:code:`<br/>`:code:`<br/>` :code:`<b>Note: </b>` ‘requiredInputs’ from
-        Discovery solutions response must be passed via ‘additionalParameters’ as an input to
-        Diagnostics API.
+    ) -> AsyncLROPoller[_models.DiagnosticResource]:
+        """Creates a diagnostic for the specific resource using solutionId from discovery solutions.
+        :code:`<br/>`Diagnostics are powerful solutions that access product resources or other relevant
+        data and provide the root cause of the issue and the steps to address the
+        issue.:code:`<br/>`:code:`<br/>`.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param diagnostics_resource_name: Unique resource name for insight resources. Required.
         :type diagnostics_resource_name: str
         :param diagnostic_resource_request: The required request body for this insightResource
          invocation. Default value is None.
         :type diagnostic_resource_request: ~azure.mgmt.selfhelp.models.DiagnosticResource
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
-        :return: An instance of LROPoller that returns either DiagnosticResource or the result of
+        :return: An instance of AsyncLROPoller that returns either DiagnosticResource or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.selfhelp.models.DiagnosticResource]
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.selfhelp.models.DiagnosticResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
-    def begin_create(
+    async def begin_create(
         self,
         scope: str,
         diagnostics_resource_name: str,
-        diagnostic_resource_request: Optional[IO] = None,
+        diagnostic_resource_request: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
-    ) -> LROPoller[_models.DiagnosticResource]:
-        """Creates a diagnostic for the specific resource using solutionId and requiredInputs* from
-        discovery solutions. :code:`<br/>`Diagnostics are powerful solutions that access product
-        resources or other relevant data and provide the root cause of the issue and the steps to
-        address the issue.:code:`<br/>`:code:`<br/>` :code:`<b>Note: </b>` ‘requiredInputs’ from
-        Discovery solutions response must be passed via ‘additionalParameters’ as an input to
-        Diagnostics API.
+    ) -> AsyncLROPoller[_models.DiagnosticResource]:
+        """Creates a diagnostic for the specific resource using solutionId from discovery solutions.
+        :code:`<br/>`Diagnostics are powerful solutions that access product resources or other relevant
+        data and provide the root cause of the issue and the steps to address the
+        issue.:code:`<br/>`:code:`<br/>`.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param diagnostics_resource_name: Unique resource name for insight resources. Required.
         :type diagnostics_resource_name: str
         :param diagnostic_resource_request: The required request body for this insightResource
          invocation. Default value is None.
-        :type diagnostic_resource_request: IO
+        :type diagnostic_resource_request: IO[bytes]
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
-        :return: An instance of LROPoller that returns either DiagnosticResource or the result of
+        :return: An instance of AsyncLROPoller that returns either DiagnosticResource or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.selfhelp.models.DiagnosticResource]
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.selfhelp.models.DiagnosticResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
-    @distributed_trace
-    def begin_create(
+    @distributed_trace_async
+    async def begin_create(
         self,
         scope: str,
         diagnostics_resource_name: str,
-        diagnostic_resource_request: Optional[Union[_models.DiagnosticResource, IO]] = None,
+        diagnostic_resource_request: Optional[Union[_models.DiagnosticResource, IO[bytes]]] = None,
         **kwargs: Any
-    ) -> LROPoller[_models.DiagnosticResource]:
-        """Creates a diagnostic for the specific resource using solutionId and requiredInputs* from
-        discovery solutions. :code:`<br/>`Diagnostics are powerful solutions that access product
-        resources or other relevant data and provide the root cause of the issue and the steps to
-        address the issue.:code:`<br/>`:code:`<br/>` :code:`<b>Note: </b>` ‘requiredInputs’ from
-        Discovery solutions response must be passed via ‘additionalParameters’ as an input to
-        Diagnostics API.
+    ) -> AsyncLROPoller[_models.DiagnosticResource]:
+        """Creates a diagnostic for the specific resource using solutionId from discovery solutions.
+        :code:`<br/>`Diagnostics are powerful solutions that access product resources or other relevant
+        data and provide the root cause of the issue and the steps to address the
+        issue.:code:`<br/>`:code:`<br/>`.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param diagnostics_resource_name: Unique resource name for insight resources. Required.
         :type diagnostics_resource_name: str
         :param diagnostic_resource_request: The required request body for this insightResource
-         invocation. Is either a DiagnosticResource type or a IO type. Default value is None.
-        :type diagnostic_resource_request: ~azure.mgmt.selfhelp.models.DiagnosticResource or IO
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
-        :return: An instance of LROPoller that returns either DiagnosticResource or the result of
+         invocation. Is either a DiagnosticResource type or a IO[bytes] type. Default value is None.
+        :type diagnostic_resource_request: ~azure.mgmt.selfhelp.models.DiagnosticResource or IO[bytes]
+        :return: An instance of AsyncLROPoller that returns either DiagnosticResource or the result of
          cls(response)
-        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.selfhelp.models.DiagnosticResource]
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.selfhelp.models.DiagnosticResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.DiagnosticResource] = kwargs.pop("cls", None)
-        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
         lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
         cont_token: Optional[str] = kwargs.pop("continuation_token", None)
         if cont_token is None:
-            raw_result = self._create_initial(
+            raw_result = await self._create_initial(
                 scope=scope,
                 diagnostics_resource_name=diagnostics_resource_name,
                 diagnostic_resource_request=diagnostic_resource_request,
                 api_version=api_version,
                 content_type=content_type,
                 cls=lambda x, y, z: x,
                 headers=_headers,
@@ -343,48 +237,48 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("DiagnosticResource", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
-            polling_method: PollingMethod = cast(
-                PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
+            polling_method: AsyncPollingMethod = cast(
+                AsyncPollingMethod,
+                AsyncARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs),
             )
         elif polling is False:
-            polling_method = cast(PollingMethod, NoPolling())
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return AsyncLROPoller[_models.DiagnosticResource].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create.metadata = {"url": "/{scope}/providers/Microsoft.Help/diagnostics/{diagnosticsResourceName}"}
+        return AsyncLROPoller[_models.DiagnosticResource](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
-    @distributed_trace
-    def get(self, scope: str, diagnostics_resource_name: str, **kwargs: Any) -> _models.DiagnosticResource:
+    @distributed_trace_async
+    async def get(self, scope: str, diagnostics_resource_name: str, **kwargs: Any) -> _models.DiagnosticResource:
         """Get the diagnostics using the 'diagnosticsResourceName' you chose while creating the
         diagnostic.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param diagnostics_resource_name: Unique resource name for insight resources. Required.
         :type diagnostics_resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: DiagnosticResource or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.DiagnosticResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -395,38 +289,35 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.DiagnosticResource] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             scope=scope,
             diagnostics_resource_name=diagnostics_resource_name,
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
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("DiagnosticResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {"url": "/{scope}/providers/Microsoft.Help/diagnostics/{diagnosticsResourceName}"}
+        return deserialized  # type: ignore
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/operations/_discovery_solution_operations.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_discovery_solution_operations.py`

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
@@ -32,30 +32,23 @@
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
-def build_list_request(
-    scope: str, *, filter: Optional[str] = None, skiptoken: Optional[str] = None, **kwargs: Any
-) -> HttpRequest:
+def build_list_request(*, filter: Optional[str] = None, skiptoken: Optional[str] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
-    _url = kwargs.pop("template_url", "/{scope}/providers/Microsoft.Help/discoverySolutions")
-    path_format_arguments = {
-        "scope": _SERIALIZER.url("scope", scope, "str", skip_quote=True),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
+    _url = kwargs.pop("template_url", "/providers/Microsoft.Help/discoverySolutions")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
     if filter is not None:
         _params["$filter"] = _SERIALIZER.query("filter", filter, "str", skip_quote=True)
     if skiptoken is not None:
         _params["$skiptoken"] = _SERIALIZER.query("skiptoken", skiptoken, "str")
@@ -83,40 +76,36 @@
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(
-        self, scope: str, filter: Optional[str] = None, skiptoken: Optional[str] = None, **kwargs: Any
+        self, filter: Optional[str] = None, skiptoken: Optional[str] = None, **kwargs: Any
     ) -> Iterable["_models.SolutionMetadataResource"]:
-        """Lists the relevant Azure diagnostics and solutions using `problemClassification API
+        """Lists the relevant Azure Diagnostics, Solutions and Troubleshooters using
+        `problemClassification API
         <https://learn.microsoft.com/rest/api/support/problem-classifications/list?tabs=HTTP>`_\ ) AND
         resourceUri or resourceType.:code:`<br/>` Discovery Solutions is the initial entry point within
         Help API, which identifies relevant Azure diagnostics and solutions. :code:`<br/>`:code:`<br/>`
         Required Input :  problemClassificationId (Use the `problemClassification API
         <https://learn.microsoft.com/rest/api/support/problem-classifications/list?tabs=HTTP>`_\ )
         :code:`<br/>`Optional input: resourceUri OR resource Type :code:`<br/>`:code:`<br/>`
         :code:`<b>Note: </b>`  ‘requiredInputs’ from Discovery solutions response must be passed via
         ‘additionalParameters’ as an input to Diagnostics and Solutions API.
 
-        :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
-         /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
-         Required.
-        :type scope: str
         :param filter: 'ProblemClassificationId' is a mandatory filter to get solutions ids. It also
          supports optional 'ResourceType' and 'SolutionType' filters. The `$filter
          <https://learn.microsoft.com/en-us/odata/webapi/first-odata-api#filter>`_ supports only 'and',
          'or' and 'eq' operators. Example: $filter=ProblemClassificationId eq
          '1ddda5b4-cf6c-4d4f-91ad-bc38ab0e811e'. Default value is None.
         :type filter: str
         :param skiptoken: Skiptoken is only used if a previous operation returned a partial result.
          Default value is None.
         :type skiptoken: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either SolutionMetadataResource or the result of
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.selfhelp.models.SolutionMetadataResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -131,63 +120,59 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
-                    scope=scope,
+                _request = build_list_request(
                     filter=filter,
                     skiptoken=skiptoken,
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
             deserialized = self._deserialize("DiscoveryResponse", pipeline_response)
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
-    list.metadata = {"url": "/{scope}/providers/Microsoft.Help/discoverySolutions"}
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/operations/_operations.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_operations.py`

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
@@ -36,15 +36,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.Help/operations")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -74,15 +74,14 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
     def list(self, **kwargs: Any) -> Iterable["_models.Operation"]:
         """Returns list of operations.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Operation or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.selfhelp.models.Operation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -96,60 +95,57 @@
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
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("OperationListResult", pipeline_response)
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
-    list.metadata = {"url": "/providers/Microsoft.Help/operations"}
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/operations/_patch.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/operations/_solution_operations.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_solution_operations.py`

 * *Files 10% similar despite different names*

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
@@ -37,15 +37,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_create_request(scope: str, solution_resource_name: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/{scope}/providers/Microsoft.Help/solutions/{solutionResourceName}")
     path_format_arguments = {
         "scope": _SERIALIZER.url("scope", scope, "str", skip_quote=True),
@@ -72,15 +72,15 @@
     return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(scope: str, solution_resource_name: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/{scope}/providers/Microsoft.Help/solutions/{solutionResourceName}")
     path_format_arguments = {
         "scope": _SERIALIZER.url("scope", scope, "str", skip_quote=True),
         "solutionResourceName": _SERIALIZER.url(
@@ -104,15 +104,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_update_request(scope: str, solution_resource_name: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/{scope}/providers/Microsoft.Help/solutions/{solutionResourceName}")
     path_format_arguments = {
         "scope": _SERIALIZER.url("scope", scope, "str", skip_quote=True),
@@ -135,14 +135,49 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
 
 
+def build_warm_up_request(scope: str, solution_resource_name: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop("template_url", "/{scope}/providers/Microsoft.Help/solutions/{solutionResourceName}/warmup")
+    path_format_arguments = {
+        "scope": _SERIALIZER.url("scope", scope, "str", skip_quote=True),
+        "solutionResourceName": _SERIALIZER.url(
+            "solution_resource_name",
+            solution_resource_name,
+            "str",
+            max_length=100,
+            min_length=1,
+            pattern=r"^[A-Za-z0-9-+@()_]+$",
+        ),
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
 class SolutionOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.selfhelp.SelfHelpMgmtClient`'s
@@ -158,15 +193,15 @@
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     def _create_initial(
         self,
         scope: str,
         solution_resource_name: str,
-        solution_request_body: Optional[Union[_models.SolutionResource, IO]] = None,
+        solution_request_body: Optional[Union[_models.SolutionResource, IO[bytes]]] = None,
         **kwargs: Any
     ) -> _models.SolutionResource:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -187,31 +222,30 @@
             _content = solution_request_body
         else:
             if solution_request_body is not None:
                 _json = self._serialize.body(solution_request_body, "SolutionResource")
             else:
                 _json = None
 
-        request = build_create_request(
+        _request = build_create_request(
             scope=scope,
             solution_resource_name=solution_resource_name,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self._create_initial.metadata["url"],
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
@@ -224,170 +258,117 @@
             deserialized = self._deserialize("SolutionResource", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    _create_initial.metadata = {"url": "/{scope}/providers/Microsoft.Help/solutions/{solutionResourceName}"}
-
     @overload
     def begin_create(
         self,
         scope: str,
         solution_resource_name: str,
         solution_request_body: Optional[_models.SolutionResource] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.SolutionResource]:
         """Creates a solution for the specific Azure resource or subscription using the inputs ‘solutionId
         and requiredInputs’ from discovery solutions. :code:`<br/>` Azure solutions comprise a
         comprehensive library of self-help resources that have been thoughtfully curated by Azure
         engineers to aid customers in resolving typical troubleshooting issues. These solutions
-        encompass (1.) dynamic and context-aware diagnostics, guided troubleshooting wizards, and data
-        visualizations, (2.) rich instructional video tutorials and illustrative diagrams and images,
-        and (3.) thoughtfully assembled textual troubleshooting instructions. All these components are
-        seamlessly converged into unified solutions tailored to address a specific support problem
-        area. Each solution type may require one or more ‘requiredParameters’ that are required to
-        execute the individual solution component. In the absence of the ‘requiredParameters’ it is
-        likely that some of the solutions might fail execution, and you might see an empty response.
-        :code:`<br/>`:code:`<br/>` :code:`<b>Note:</b>`  :code:`<br/>`1. ‘requiredInputs’ from
-        Discovery solutions response must be passed via ‘parameters’ in the request body of Solutions
-        API. :code:`<br/>`2. ‘requiredParameters’ from the Solutions response is the same as ‘
-        additionalParameters’ in the request for diagnostics :code:`<br/>`3. ‘requiredParameters’ from
-        the Solutions response is the same as ‘properties.parameters’ in the request for
-        Troubleshooters.
+        encompass: :code:`<br/>` (1.) Dynamic and context-aware diagnostics, guided troubleshooting
+        wizards, and data visualizations. :code:`<br/>` (2.) Rich instructional video tutorials and
+        illustrative diagrams and images. :code:`<br/>` (3.) Thoughtfully assembled textual
+        troubleshooting instructions. :code:`<br/>` All these components are seamlessly converged into
+        unified solutions tailored to address a specific support problem area.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param solution_resource_name: Solution resource Name. Required.
         :type solution_resource_name: str
         :param solution_request_body: The required request body for this solution resource creation.
          Default value is None.
         :type solution_request_body: ~azure.mgmt.selfhelp.models.SolutionResource
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
         :return: An instance of LROPoller that returns either SolutionResource or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.selfhelp.models.SolutionResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_create(
         self,
         scope: str,
         solution_resource_name: str,
-        solution_request_body: Optional[IO] = None,
+        solution_request_body: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.SolutionResource]:
         """Creates a solution for the specific Azure resource or subscription using the inputs ‘solutionId
         and requiredInputs’ from discovery solutions. :code:`<br/>` Azure solutions comprise a
         comprehensive library of self-help resources that have been thoughtfully curated by Azure
         engineers to aid customers in resolving typical troubleshooting issues. These solutions
-        encompass (1.) dynamic and context-aware diagnostics, guided troubleshooting wizards, and data
-        visualizations, (2.) rich instructional video tutorials and illustrative diagrams and images,
-        and (3.) thoughtfully assembled textual troubleshooting instructions. All these components are
-        seamlessly converged into unified solutions tailored to address a specific support problem
-        area. Each solution type may require one or more ‘requiredParameters’ that are required to
-        execute the individual solution component. In the absence of the ‘requiredParameters’ it is
-        likely that some of the solutions might fail execution, and you might see an empty response.
-        :code:`<br/>`:code:`<br/>` :code:`<b>Note:</b>`  :code:`<br/>`1. ‘requiredInputs’ from
-        Discovery solutions response must be passed via ‘parameters’ in the request body of Solutions
-        API. :code:`<br/>`2. ‘requiredParameters’ from the Solutions response is the same as ‘
-        additionalParameters’ in the request for diagnostics :code:`<br/>`3. ‘requiredParameters’ from
-        the Solutions response is the same as ‘properties.parameters’ in the request for
-        Troubleshooters.
+        encompass: :code:`<br/>` (1.) Dynamic and context-aware diagnostics, guided troubleshooting
+        wizards, and data visualizations. :code:`<br/>` (2.) Rich instructional video tutorials and
+        illustrative diagrams and images. :code:`<br/>` (3.) Thoughtfully assembled textual
+        troubleshooting instructions. :code:`<br/>` All these components are seamlessly converged into
+        unified solutions tailored to address a specific support problem area.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param solution_resource_name: Solution resource Name. Required.
         :type solution_resource_name: str
         :param solution_request_body: The required request body for this solution resource creation.
          Default value is None.
-        :type solution_request_body: IO
+        :type solution_request_body: IO[bytes]
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
         :return: An instance of LROPoller that returns either SolutionResource or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.selfhelp.models.SolutionResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_create(
         self,
         scope: str,
         solution_resource_name: str,
-        solution_request_body: Optional[Union[_models.SolutionResource, IO]] = None,
+        solution_request_body: Optional[Union[_models.SolutionResource, IO[bytes]]] = None,
         **kwargs: Any
     ) -> LROPoller[_models.SolutionResource]:
         """Creates a solution for the specific Azure resource or subscription using the inputs ‘solutionId
         and requiredInputs’ from discovery solutions. :code:`<br/>` Azure solutions comprise a
         comprehensive library of self-help resources that have been thoughtfully curated by Azure
         engineers to aid customers in resolving typical troubleshooting issues. These solutions
-        encompass (1.) dynamic and context-aware diagnostics, guided troubleshooting wizards, and data
-        visualizations, (2.) rich instructional video tutorials and illustrative diagrams and images,
-        and (3.) thoughtfully assembled textual troubleshooting instructions. All these components are
-        seamlessly converged into unified solutions tailored to address a specific support problem
-        area. Each solution type may require one or more ‘requiredParameters’ that are required to
-        execute the individual solution component. In the absence of the ‘requiredParameters’ it is
-        likely that some of the solutions might fail execution, and you might see an empty response.
-        :code:`<br/>`:code:`<br/>` :code:`<b>Note:</b>`  :code:`<br/>`1. ‘requiredInputs’ from
-        Discovery solutions response must be passed via ‘parameters’ in the request body of Solutions
-        API. :code:`<br/>`2. ‘requiredParameters’ from the Solutions response is the same as ‘
-        additionalParameters’ in the request for diagnostics :code:`<br/>`3. ‘requiredParameters’ from
-        the Solutions response is the same as ‘properties.parameters’ in the request for
-        Troubleshooters.
+        encompass: :code:`<br/>` (1.) Dynamic and context-aware diagnostics, guided troubleshooting
+        wizards, and data visualizations. :code:`<br/>` (2.) Rich instructional video tutorials and
+        illustrative diagrams and images. :code:`<br/>` (3.) Thoughtfully assembled textual
+        troubleshooting instructions. :code:`<br/>` All these components are seamlessly converged into
+        unified solutions tailored to address a specific support problem area.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param solution_resource_name: Solution resource Name. Required.
         :type solution_resource_name: str
         :param solution_request_body: The required request body for this solution resource creation. Is
-         either a SolutionResource type or a IO type. Default value is None.
-        :type solution_request_body: ~azure.mgmt.selfhelp.models.SolutionResource or IO
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
+         either a SolutionResource type or a IO[bytes] type. Default value is None.
+        :type solution_request_body: ~azure.mgmt.selfhelp.models.SolutionResource or IO[bytes]
         :return: An instance of LROPoller that returns either SolutionResource or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.selfhelp.models.SolutionResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -411,47 +392,46 @@
                 **kwargs
             )
         kwargs.pop("error_map", None)
 
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize("SolutionResource", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, {})
+                return cls(pipeline_response, deserialized, {})  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: PollingMethod = cast(
                 PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
             )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[_models.SolutionResource].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
-
-    begin_create.metadata = {"url": "/{scope}/providers/Microsoft.Help/solutions/{solutionResourceName}"}
+        return LROPoller[_models.SolutionResource](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
 
     @distributed_trace
     def get(self, scope: str, solution_resource_name: str, **kwargs: Any) -> _models.SolutionResource:
         """Get the solution using the applicable solutionResourceName while creating the solution.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param solution_resource_name: Solution resource Name. Required.
         :type solution_resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SolutionResource or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.SolutionResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -462,51 +442,48 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.SolutionResource] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             scope=scope,
             solution_resource_name=solution_resource_name,
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
 
         deserialized = self._deserialize("SolutionResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {"url": "/{scope}/providers/Microsoft.Help/solutions/{solutionResourceName}"}
+        return deserialized  # type: ignore
 
     def _update_initial(
         self,
         scope: str,
         solution_resource_name: str,
-        solution_patch_request_body: Optional[Union[_models.SolutionPatchRequestBody, IO]] = None,
+        solution_patch_request_body: Optional[Union[_models.SolutionPatchRequestBody, IO[bytes]]] = None,
         **kwargs: Any
     ) -> _models.SolutionResource:
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -527,31 +504,30 @@
             _content = solution_patch_request_body
         else:
             if solution_patch_request_body is not None:
                 _json = self._serialize.body(solution_patch_request_body, "SolutionPatchRequestBody")
             else:
                 _json = None
 
-        request = build_update_request(
+        _request = build_update_request(
             scope=scope,
             solution_resource_name=solution_resource_name,
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
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
@@ -569,16 +545,14 @@
             deserialized = self._deserialize("SolutionResource", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
         return deserialized  # type: ignore
 
-    _update_initial.metadata = {"url": "/{scope}/providers/Microsoft.Help/solutions/{solutionResourceName}"}
-
     @overload
     def begin_update(
         self,
         scope: str,
         solution_resource_name: str,
         solution_patch_request_body: Optional[_models.SolutionPatchRequestBody] = None,
         *,
@@ -595,96 +569,70 @@
         :type solution_resource_name: str
         :param solution_patch_request_body: The required request body for updating a solution resource.
          Default value is None.
         :type solution_patch_request_body: ~azure.mgmt.selfhelp.models.SolutionPatchRequestBody
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
         :return: An instance of LROPoller that returns either SolutionResource or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.selfhelp.models.SolutionResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def begin_update(
         self,
         scope: str,
         solution_resource_name: str,
-        solution_patch_request_body: Optional[IO] = None,
+        solution_patch_request_body: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> LROPoller[_models.SolutionResource]:
         """Update the requiredInputs or additional information needed to execute the solution.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param solution_resource_name: Solution resource Name. Required.
         :type solution_resource_name: str
         :param solution_patch_request_body: The required request body for updating a solution resource.
          Default value is None.
-        :type solution_patch_request_body: IO
+        :type solution_patch_request_body: IO[bytes]
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
         :return: An instance of LROPoller that returns either SolutionResource or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.selfhelp.models.SolutionResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def begin_update(
         self,
         scope: str,
         solution_resource_name: str,
-        solution_patch_request_body: Optional[Union[_models.SolutionPatchRequestBody, IO]] = None,
+        solution_patch_request_body: Optional[Union[_models.SolutionPatchRequestBody, IO[bytes]]] = None,
         **kwargs: Any
     ) -> LROPoller[_models.SolutionResource]:
         """Update the requiredInputs or additional information needed to execute the solution.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param solution_resource_name: Solution resource Name. Required.
         :type solution_resource_name: str
         :param solution_patch_request_body: The required request body for updating a solution resource.
-         Is either a SolutionPatchRequestBody type or a IO type. Default value is None.
-        :type solution_patch_request_body: ~azure.mgmt.selfhelp.models.SolutionPatchRequestBody or IO
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
+         Is either a SolutionPatchRequestBody type or a IO[bytes] type. Default value is None.
+        :type solution_patch_request_body: ~azure.mgmt.selfhelp.models.SolutionPatchRequestBody or
+         IO[bytes]
         :return: An instance of LROPoller that returns either SolutionResource or the result of
          cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.selfhelp.models.SolutionResource]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -712,28 +660,165 @@
         def get_long_running_output(pipeline_response):
             response_headers = {}
             response = pipeline_response.http_response
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
 
             deserialized = self._deserialize("SolutionResource", pipeline_response)
             if cls:
-                return cls(pipeline_response, deserialized, response_headers)
+                return cls(pipeline_response, deserialized, response_headers)  # type: ignore
             return deserialized
 
         if polling is True:
             polling_method: PollingMethod = cast(
                 PollingMethod, ARMPolling(lro_delay, lro_options={"final-state-via": "azure-async-operation"}, **kwargs)
             )
         elif polling is False:
             polling_method = cast(PollingMethod, NoPolling())
         else:
             polling_method = polling
         if cont_token:
-            return LROPoller.from_continuation_token(
+            return LROPoller[_models.SolutionResource].from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
-        return LROPoller(self._client, raw_result, get_long_running_output, polling_method)  # type: ignore
+        return LROPoller[_models.SolutionResource](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
+
+    @overload
+    def warm_up(  # pylint: disable=inconsistent-return-statements
+        self,
+        scope: str,
+        solution_resource_name: str,
+        solution_warm_up_request_body: Optional[_models.SolutionWarmUpRequestBody] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """Warm up the solution resource by preloading asynchronous diagnostics results into cache.
 
-    begin_update.metadata = {"url": "/{scope}/providers/Microsoft.Help/solutions/{solutionResourceName}"}
+        :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
+         /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
+         Required.
+        :type scope: str
+        :param solution_resource_name: Solution resource Name. Required.
+        :type solution_resource_name: str
+        :param solution_warm_up_request_body: The required request body for warming up a solution
+         resource. Default value is None.
+        :type solution_warm_up_request_body: ~azure.mgmt.selfhelp.models.SolutionWarmUpRequestBody
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None or the result of cls(response)
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def warm_up(  # pylint: disable=inconsistent-return-statements
+        self,
+        scope: str,
+        solution_resource_name: str,
+        solution_warm_up_request_body: Optional[IO[bytes]] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """Warm up the solution resource by preloading asynchronous diagnostics results into cache.
+
+        :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
+         /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
+         Required.
+        :type scope: str
+        :param solution_resource_name: Solution resource Name. Required.
+        :type solution_resource_name: str
+        :param solution_warm_up_request_body: The required request body for warming up a solution
+         resource. Default value is None.
+        :type solution_warm_up_request_body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None or the result of cls(response)
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def warm_up(  # pylint: disable=inconsistent-return-statements
+        self,
+        scope: str,
+        solution_resource_name: str,
+        solution_warm_up_request_body: Optional[Union[_models.SolutionWarmUpRequestBody, IO[bytes]]] = None,
+        **kwargs: Any
+    ) -> None:
+        """Warm up the solution resource by preloading asynchronous diagnostics results into cache.
+
+        :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
+         /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
+         Required.
+        :type scope: str
+        :param solution_resource_name: Solution resource Name. Required.
+        :type solution_resource_name: str
+        :param solution_warm_up_request_body: The required request body for warming up a solution
+         resource. Is either a SolutionWarmUpRequestBody type or a IO[bytes] type. Default value is
+         None.
+        :type solution_warm_up_request_body: ~azure.mgmt.selfhelp.models.SolutionWarmUpRequestBody or
+         IO[bytes]
+        :return: None or the result of cls(response)
+        :rtype: None
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
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(solution_warm_up_request_body, (IOBase, bytes)):
+            _content = solution_warm_up_request_body
+        else:
+            if solution_warm_up_request_body is not None:
+                _json = self._serialize.body(solution_warm_up_request_body, "SolutionWarmUpRequestBody")
+            else:
+                _json = None
+
+        _request = build_warm_up_request(
+            scope=scope,
+            solution_resource_name=solution_resource_name,
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
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
+        if response.status_code not in [204]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        if cls:
+            return cls(pipeline_response, None, {})  # type: ignore
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure/mgmt/selfhelp/operations/_troubleshooters_operations.py` & `azure-mgmt-selfhelp-2.0.0b3/azure/mgmt/selfhelp/operations/_troubleshooters_operations.py`

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
@@ -35,15 +35,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_create_request(scope: str, troubleshooter_name: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/{scope}/providers/Microsoft.Help/troubleshooters/{troubleshooterName}")
     path_format_arguments = {
         "scope": _SERIALIZER.url("scope", scope, "str", skip_quote=True),
@@ -70,15 +70,15 @@
     return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(scope: str, troubleshooter_name: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/{scope}/providers/Microsoft.Help/troubleshooters/{troubleshooterName}")
     path_format_arguments = {
         "scope": _SERIALIZER.url("scope", scope, "str", skip_quote=True),
         "troubleshooterName": _SERIALIZER.url(
@@ -102,15 +102,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_continue_method_request(scope: str, troubleshooter_name: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/{scope}/providers/Microsoft.Help/troubleshooters/{troubleshooterName}/continue")
     path_format_arguments = {
         "scope": _SERIALIZER.url("scope", scope, "str", skip_quote=True),
@@ -137,15 +137,15 @@
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_end_request(scope: str, troubleshooter_name: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/{scope}/providers/Microsoft.Help/troubleshooters/{troubleshooterName}/end")
     path_format_arguments = {
         "scope": _SERIALIZER.url("scope", scope, "str", skip_quote=True),
         "troubleshooterName": _SERIALIZER.url(
@@ -169,15 +169,15 @@
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_restart_request(scope: str, troubleshooter_name: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/{scope}/providers/Microsoft.Help/troubleshooters/{troubleshooterName}/restart")
     path_format_arguments = {
         "scope": _SERIALIZER.url("scope", scope, "str", skip_quote=True),
         "troubleshooterName": _SERIALIZER.url(
@@ -248,26 +248,25 @@
         :type troubleshooter_name: str
         :param create_troubleshooter_request_body: The required request body for this Troubleshooter
          resource creation. Default value is None.
         :type create_troubleshooter_request_body: ~azure.mgmt.selfhelp.models.TroubleshooterResource
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: TroubleshooterResource or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.TroubleshooterResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def create(
         self,
         scope: str,
         troubleshooter_name: str,
-        create_troubleshooter_request_body: Optional[IO] = None,
+        create_troubleshooter_request_body: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.TroubleshooterResource:
         """Creates the specific troubleshooter action under a resource or subscription using the
         ‘solutionId’ and  ‘properties.parameters’ as the trigger. :code:`<br/>` Azure Troubleshooters
         help with hard to classify issues, reducing the gap between customer observed problems and
@@ -282,30 +281,29 @@
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param troubleshooter_name: Troubleshooter resource Name. Required.
         :type troubleshooter_name: str
         :param create_troubleshooter_request_body: The required request body for this Troubleshooter
          resource creation. Default value is None.
-        :type create_troubleshooter_request_body: IO
+        :type create_troubleshooter_request_body: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: TroubleshooterResource or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.TroubleshooterResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def create(
         self,
         scope: str,
         troubleshooter_name: str,
-        create_troubleshooter_request_body: Optional[Union[_models.TroubleshooterResource, IO]] = None,
+        create_troubleshooter_request_body: Optional[Union[_models.TroubleshooterResource, IO[bytes]]] = None,
         **kwargs: Any
     ) -> _models.TroubleshooterResource:
         """Creates the specific troubleshooter action under a resource or subscription using the
         ‘solutionId’ and  ‘properties.parameters’ as the trigger. :code:`<br/>` Azure Troubleshooters
         help with hard to classify issues, reducing the gap between customer observed problems and
         solutions by guiding the user effortlessly through the troubleshooting process. Each
         Troubleshooter flow represents a problem area within Azure and has a complex tree-like
@@ -317,21 +315,18 @@
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param troubleshooter_name: Troubleshooter resource Name. Required.
         :type troubleshooter_name: str
         :param create_troubleshooter_request_body: The required request body for this Troubleshooter
-         resource creation. Is either a TroubleshooterResource type or a IO type. Default value is None.
+         resource creation. Is either a TroubleshooterResource type or a IO[bytes] type. Default value
+         is None.
         :type create_troubleshooter_request_body: ~azure.mgmt.selfhelp.models.TroubleshooterResource or
-         IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         IO[bytes]
         :return: TroubleshooterResource or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.TroubleshooterResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -354,31 +349,30 @@
             _content = create_troubleshooter_request_body
         else:
             if create_troubleshooter_request_body is not None:
                 _json = self._serialize.body(create_troubleshooter_request_body, "TroubleshooterResource")
             else:
                 _json = None
 
-        request = build_create_request(
+        _request = build_create_request(
             scope=scope,
             troubleshooter_name=troubleshooter_name,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.create.metadata["url"],
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
@@ -391,31 +385,28 @@
             deserialized = self._deserialize("TroubleshooterResource", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    create.metadata = {"url": "/{scope}/providers/Microsoft.Help/troubleshooters/{troubleshooterName}"}
-
     @distributed_trace
     def get(self, scope: str, troubleshooter_name: str, **kwargs: Any) -> _models.TroubleshooterResource:
         """Gets troubleshooter instance result which includes the step status/result of the troubleshooter
         resource name that is being executed.:code:`<br/>` Get API is used to retrieve the result of a
         Troubleshooter instance, which includes the status and result of each step in the
         Troubleshooter workflow. This API requires the Troubleshooter resource name that was created
         using the Create API.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param troubleshooter_name: Troubleshooter resource Name. Required.
         :type troubleshooter_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: TroubleshooterResource or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.TroubleshooterResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -426,45 +417,42 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.TroubleshooterResource] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             scope=scope,
             troubleshooter_name=troubleshooter_name,
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
 
         deserialized = self._deserialize("TroubleshooterResource", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {"url": "/{scope}/providers/Microsoft.Help/troubleshooters/{troubleshooterName}"}
+        return deserialized  # type: ignore
 
     @overload
     def continue_method(  # pylint: disable=inconsistent-return-statements
         self,
         scope: str,
         troubleshooter_name: str,
         continue_request_body: Optional[_models.ContinueRequestBody] = None,
@@ -485,26 +473,25 @@
         :type troubleshooter_name: str
         :param continue_request_body: The required request body for going to next step in
          Troubleshooter resource. Default value is None.
         :type continue_request_body: ~azure.mgmt.selfhelp.models.ContinueRequestBody
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def continue_method(  # pylint: disable=inconsistent-return-statements
         self,
         scope: str,
         troubleshooter_name: str,
-        continue_request_body: Optional[IO] = None,
+        continue_request_body: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> None:
         """Uses ‘stepId’ and ‘responses’ as the trigger to continue the troubleshooting steps for the
         respective troubleshooter resource name. :code:`<br/>`Continue API is used to provide inputs
         that are required for the specific troubleshooter to progress into the next step in the
@@ -514,51 +501,46 @@
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param troubleshooter_name: Troubleshooter resource Name. Required.
         :type troubleshooter_name: str
         :param continue_request_body: The required request body for going to next step in
          Troubleshooter resource. Default value is None.
-        :type continue_request_body: IO
+        :type continue_request_body: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def continue_method(  # pylint: disable=inconsistent-return-statements
         self,
         scope: str,
         troubleshooter_name: str,
-        continue_request_body: Optional[Union[_models.ContinueRequestBody, IO]] = None,
+        continue_request_body: Optional[Union[_models.ContinueRequestBody, IO[bytes]]] = None,
         **kwargs: Any
     ) -> None:
         """Uses ‘stepId’ and ‘responses’ as the trigger to continue the troubleshooting steps for the
         respective troubleshooter resource name. :code:`<br/>`Continue API is used to provide inputs
         that are required for the specific troubleshooter to progress into the next step in the
         process. This API is used after the Troubleshooter has been created using the Create API.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param troubleshooter_name: Troubleshooter resource Name. Required.
         :type troubleshooter_name: str
         :param continue_request_body: The required request body for going to next step in
-         Troubleshooter resource. Is either a ContinueRequestBody type or a IO type. Default value is
-         None.
-        :type continue_request_body: ~azure.mgmt.selfhelp.models.ContinueRequestBody or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         Troubleshooter resource. Is either a ContinueRequestBody type or a IO[bytes] type. Default
+         value is None.
+        :type continue_request_body: ~azure.mgmt.selfhelp.models.ContinueRequestBody or IO[bytes]
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -581,63 +563,57 @@
             _content = continue_request_body
         else:
             if continue_request_body is not None:
                 _json = self._serialize.body(continue_request_body, "ContinueRequestBody")
             else:
                 _json = None
 
-        request = build_continue_method_request(
+        _request = build_continue_method_request(
             scope=scope,
             troubleshooter_name=troubleshooter_name,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.continue_method.metadata["url"],
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
 
         if response.status_code not in [204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    continue_method.metadata = {
-        "url": "/{scope}/providers/Microsoft.Help/troubleshooters/{troubleshooterName}/continue"
-    }
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def end(  # pylint: disable=inconsistent-return-statements
         self, scope: str, troubleshooter_name: str, **kwargs: Any
     ) -> None:
         """Ends the troubleshooter action.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param troubleshooter_name: Troubleshooter resource Name. Required.
         :type troubleshooter_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -648,58 +624,54 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        request = build_end_request(
+        _request = build_end_request(
             scope=scope,
             troubleshooter_name=troubleshooter_name,
             api_version=api_version,
-            template_url=self.end.metadata["url"],
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
 
         if response.status_code not in [204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         response_headers = {}
         response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
 
         if cls:
-            return cls(pipeline_response, None, response_headers)
-
-    end.metadata = {"url": "/{scope}/providers/Microsoft.Help/troubleshooters/{troubleshooterName}/end"}
+            return cls(pipeline_response, None, response_headers)  # type: ignore
 
     @distributed_trace
     def restart(self, scope: str, troubleshooter_name: str, **kwargs: Any) -> _models.RestartTroubleshooterResponse:
         """Restarts the troubleshooter API using applicable troubleshooter resource name as the
         input.:code:`<br/>` It returns new resource name which should be used in subsequent request.
         The old resource name is obsolete after this API is invoked.
 
         :param scope: scope = resourceUri of affected resource.:code:`<br/>` For example:
          /subscriptions/0d0fcd2e-c4fd-4349-8497-200edb3923c6/resourcegroups/myresourceGroup/providers/Microsoft.KeyVault/vaults/test-keyvault-non-read.
          Required.
         :type scope: str
         :param troubleshooter_name: Troubleshooter resource Name. Required.
         :type troubleshooter_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: RestartTroubleshooterResponse or the result of cls(response)
         :rtype: ~azure.mgmt.selfhelp.models.RestartTroubleshooterResponse
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -710,28 +682,27 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.RestartTroubleshooterResponse] = kwargs.pop("cls", None)
 
-        request = build_restart_request(
+        _request = build_restart_request(
             scope=scope,
             troubleshooter_name=troubleshooter_name,
             api_version=api_version,
-            template_url=self.restart.metadata["url"],
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
@@ -739,12 +710,10 @@
 
         response_headers = {}
         response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
 
         deserialized = self._deserialize("RestartTroubleshooterResponse", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
 
-        return deserialized
-
-    restart.metadata = {"url": "/{scope}/providers/Microsoft.Help/troubleshooters/{troubleshooterName}/restart"}
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure_mgmt_selfhelp.egg-info/PKG-INFO` & `azure-mgmt-selfhelp-2.0.0b3/azure_mgmt_selfhelp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-selfhelp
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: Microsoft Azure Selfhelp Management Client Library for Python
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
 
 This is the Microsoft Azure Selfhelp Management Client Library.
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
 pip install azure-mgmt-selfhelp
 pip install azure-identity
@@ -86,14 +82,33 @@
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 # Release History
 
+## 2.0.0b3 (2024-04-22)
+
+### Features Added
+
+  - Added operation SolutionOperations.warm_up
+  - Added operation group DiscoverySolutionNLPSubscriptionScopeOperations
+  - Added operation group DiscoverySolutionNLPTenantScopeOperations
+  - Added operation group SimplifiedSolutionsOperations
+  - Added operation group SolutionSelfHelpOperations
+  - Model AutomatedCheckResult has a new parameter status
+  - Model AutomatedCheckResult has a new parameter version
+  - Model ResponseValidationProperties has a new parameter validation_scope
+  - Model SolutionsDiagnostic has a new parameter estimated_completion_time
+  - Model StepInput has a new parameter question_title
+
+### Breaking Changes
+
+  - Operation DiscoverySolutionOperations.list no longer has parameter scope
+
 ## 2.0.0b2 (2023-12-18)
 
 ### Features Added
 
   - Model SolutionPatchRequestBody has a new parameter content
   - Model SolutionPatchRequestBody has a new parameter parameters
   - Model SolutionPatchRequestBody has a new parameter provisioning_state
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/azure_mgmt_selfhelp.egg-info/SOURCES.txt` & `azure-mgmt-selfhelp-2.0.0b3/azure_mgmt_selfhelp.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -17,30 +17,38 @@
 azure/mgmt/selfhelp/aio/__init__.py
 azure/mgmt/selfhelp/aio/_configuration.py
 azure/mgmt/selfhelp/aio/_patch.py
 azure/mgmt/selfhelp/aio/_self_help_mgmt_client.py
 azure/mgmt/selfhelp/aio/operations/__init__.py
 azure/mgmt/selfhelp/aio/operations/_check_name_availability_operations.py
 azure/mgmt/selfhelp/aio/operations/_diagnostics_operations.py
+azure/mgmt/selfhelp/aio/operations/_discovery_solution_nlp_subscription_scope_operations.py
+azure/mgmt/selfhelp/aio/operations/_discovery_solution_nlp_tenant_scope_operations.py
 azure/mgmt/selfhelp/aio/operations/_discovery_solution_operations.py
 azure/mgmt/selfhelp/aio/operations/_operations.py
 azure/mgmt/selfhelp/aio/operations/_patch.py
+azure/mgmt/selfhelp/aio/operations/_simplified_solutions_operations.py
 azure/mgmt/selfhelp/aio/operations/_solution_operations.py
+azure/mgmt/selfhelp/aio/operations/_solution_self_help_operations.py
 azure/mgmt/selfhelp/aio/operations/_troubleshooters_operations.py
 azure/mgmt/selfhelp/models/__init__.py
 azure/mgmt/selfhelp/models/_models_py3.py
 azure/mgmt/selfhelp/models/_patch.py
 azure/mgmt/selfhelp/models/_self_help_mgmt_client_enums.py
 azure/mgmt/selfhelp/operations/__init__.py
 azure/mgmt/selfhelp/operations/_check_name_availability_operations.py
 azure/mgmt/selfhelp/operations/_diagnostics_operations.py
+azure/mgmt/selfhelp/operations/_discovery_solution_nlp_subscription_scope_operations.py
+azure/mgmt/selfhelp/operations/_discovery_solution_nlp_tenant_scope_operations.py
 azure/mgmt/selfhelp/operations/_discovery_solution_operations.py
 azure/mgmt/selfhelp/operations/_operations.py
 azure/mgmt/selfhelp/operations/_patch.py
+azure/mgmt/selfhelp/operations/_simplified_solutions_operations.py
 azure/mgmt/selfhelp/operations/_solution_operations.py
+azure/mgmt/selfhelp/operations/_solution_self_help_operations.py
 azure/mgmt/selfhelp/operations/_troubleshooters_operations.py
 azure_mgmt_selfhelp.egg-info/PKG-INFO
 azure_mgmt_selfhelp.egg-info/SOURCES.txt
 azure_mgmt_selfhelp.egg-info/dependency_links.txt
 azure_mgmt_selfhelp.egg-info/not-zip-safe
 azure_mgmt_selfhelp.egg-info/requires.txt
 azure_mgmt_selfhelp.egg-info/top_level.txt
```

### Comparing `azure-mgmt-selfhelp-2.0.0b2/setup.py` & `azure-mgmt-selfhelp-2.0.0b3/setup.py`

 * *Files 2% similar despite different names*

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

### Comparing `azure-mgmt-selfhelp-2.0.0b2/tests/conftest.py` & `azure-mgmt-selfhelp-2.0.0b3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-selfhelp-2.0.0b2/tests/test_cli_mgmt_selfhelp.py` & `azure-mgmt-selfhelp-2.0.0b3/tests/test_cli_mgmt_selfhelp.py`

 * *Files identical despite different names*

