# Comparing `tmp/azure-mgmt-support-6.1.0b3.tar.gz` & `tmp/azure-mgmt-support-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-mgmt-support-6.1.0b3.tar", last modified: Thu Mar 21 03:04:14 2024, max compression
+gzip compressed data, was "azure-mgmt-support-7.0.0.tar", last modified: Wed Apr 24 04:42:19 2024, max compression
```

## Comparing `azure-mgmt-support-6.1.0b3.tar` & `azure-mgmt-support-7.0.0.tar`

### file list

```diff
@@ -1,81 +1,73 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-21 03:04:14.328320 azure-mgmt-support-6.1.0b3/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5030 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      213 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/MANIFEST.in
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     8014 2024-03-21 03:04:14.328320 azure-mgmt-support-6.1.0b3/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1993 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/README.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      624 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/_meta.json
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-21 03:04:14.316320 azure-mgmt-support-6.1.0b3/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-21 03:04:14.316320 azure-mgmt-support-6.1.0b3/azure/mgmt/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-21 03:04:14.316320 azure-mgmt-support-6.1.0b3/azure/mgmt/support/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      887 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3456 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10972 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/_microsoft_support.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/_serialization.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/_vendor.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      488 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-21 03:04:14.320320 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      834 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3504 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11196 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/_microsoft_support.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-21 03:04:14.324320 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2670 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8407 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_chat_transcripts_no_subscription_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8509 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_chat_transcripts_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    24375 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_communications_no_subscription_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    24382 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_communications_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6514 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_file_workspaces_no_subscription_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6640 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_file_workspaces_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18204 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_files_no_subscription_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18491 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_files_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7027 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_look_up_resource_id_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5558 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8327 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_problem_classifications_no_subscription_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    14950 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_problem_classifications_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6942 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_service_classifications_no_subscription_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6921 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_service_classifications_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8372 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_services_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    32662 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_support_tickets_no_subscription_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    34582 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_support_tickets_operations.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-21 03:04:14.324320 azure-mgmt-support-6.1.0b3/azure/mgmt/support/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4896 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2768 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/models/_microsoft_support_enums.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    86797 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/models/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-21 03:04:14.328320 azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2670 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10439 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_chat_transcripts_no_subscription_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10897 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_chat_transcripts_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    29115 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_communications_no_subscription_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    29791 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_communications_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8500 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_file_workspaces_no_subscription_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9014 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_file_workspaces_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    22803 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_files_no_subscription_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    23811 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_files_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7971 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_look_up_resource_id_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6265 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9568 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_problem_classifications_no_subscription_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18383 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_problem_classifications_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7866 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_service_classifications_no_subscription_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8106 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_service_classifications_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9921 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_services_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    37582 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_support_tickets_no_subscription_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    40586 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_support_tickets_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/azure/mgmt/support/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-21 03:04:14.328320 azure-mgmt-support-6.1.0b3/azure_mgmt_support.egg-info/
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     8014 2024-03-21 03:04:14.000000 azure-mgmt-support-6.1.0b3/azure_mgmt_support.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3503 2024-03-21 03:04:14.000000 azure-mgmt-support-6.1.0b3/azure_mgmt_support.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-03-21 03:04:14.000000 azure-mgmt-support-6.1.0b3/azure_mgmt_support.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-03-21 03:04:14.000000 azure-mgmt-support-6.1.0b3/azure_mgmt_support.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       56 2024-03-21 03:04:14.000000 azure-mgmt-support-6.1.0b3/azure_mgmt_support.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-03-21 03:04:14.000000 azure-mgmt-support-6.1.0b3/azure_mgmt_support.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-03-21 03:04:14.328320 azure-mgmt-support-6.1.0b3/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2767 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-21 03:04:14.328320 azure-mgmt-support-6.1.0b3/tests/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25903 2024-03-21 03:02:30.000000 azure-mgmt-support-6.1.0b3/tests/disable_test_cli_mgmt_support.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:42:19.225532 azure-mgmt-support-7.0.0/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6876 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      213 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/MANIFEST.in
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9770 2024-04-24 04:42:19.225532 azure-mgmt-support-7.0.0/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1993 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/README.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      624 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/_meta.json
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:42:19.217532 azure-mgmt-support-7.0.0/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:42:19.217532 azure-mgmt-support-7.0.0/azure/mgmt/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:42:19.217532 azure-mgmt-support-7.0.0/azure/mgmt/support/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      887 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3440 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9263 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/_microsoft_support.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/_serialization.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/_vendor.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      486 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:42:19.217532 azure-mgmt-support-7.0.0/azure/mgmt/support/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      834 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3488 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9471 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/aio/_microsoft_support.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/aio/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:42:19.221532 azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2110 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8407 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_chat_transcripts_no_subscription_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8509 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_chat_transcripts_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    24375 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_communications_no_subscription_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    24382 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_communications_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6514 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_file_workspaces_no_subscription_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6640 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_file_workspaces_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18204 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_files_no_subscription_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18491 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_files_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5558 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8686 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_problem_classifications_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8304 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_services_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    32662 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_support_tickets_no_subscription_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    34582 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_support_tickets_operations.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:42:19.221532 azure-mgmt-support-7.0.0/azure/mgmt/support/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4040 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2768 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/models/_microsoft_support_enums.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    74137 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/models/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:42:19.225532 azure-mgmt-support-7.0.0/azure/mgmt/support/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2110 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10423 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_chat_transcripts_no_subscription_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10881 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_chat_transcripts_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    29083 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_communications_no_subscription_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    29759 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_communications_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8484 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_file_workspaces_no_subscription_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8998 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_file_workspaces_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    22771 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_files_no_subscription_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    23779 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_files_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6257 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10682 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_problem_classifications_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9837 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_services_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    37542 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_support_tickets_no_subscription_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    40546 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_support_tickets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/azure/mgmt/support/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:42:19.225532 azure-mgmt-support-7.0.0/azure_mgmt_support.egg-info/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9770 2024-04-24 04:42:19.000000 azure-mgmt-support-7.0.0/azure_mgmt_support.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2879 2024-04-24 04:42:19.000000 azure-mgmt-support-7.0.0/azure_mgmt_support.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-24 04:42:19.000000 azure-mgmt-support-7.0.0/azure_mgmt_support.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-24 04:42:18.000000 azure-mgmt-support-7.0.0/azure_mgmt_support.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       56 2024-04-24 04:42:19.000000 azure-mgmt-support-7.0.0/azure_mgmt_support.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-04-24 04:42:19.000000 azure-mgmt-support-7.0.0/azure_mgmt_support.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-04-24 04:42:19.225532 azure-mgmt-support-7.0.0/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2780 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:42:19.225532 azure-mgmt-support-7.0.0/tests/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25903 2024-04-24 04:40:41.000000 azure-mgmt-support-7.0.0/tests/disable_test_cli_mgmt_support.py
```

### Comparing `azure-mgmt-support-6.1.0b3/LICENSE` & `azure-mgmt-support-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-mgmt-support-6.1.0b3/PKG-INFO` & `azure-mgmt-support-7.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-support
-Version: 6.1.0b3
+Version: 7.0.0
 Summary: Microsoft Azure Support Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: isodate>=0.6.1
-Requires-Dist: azure-common>=1.1
-Requires-Dist: azure-mgmt-core>=1.3.2
 
 # Microsoft Azure SDK for Python
 
 This is the Microsoft Azure Support Management Client Library.
 This package has been tested with Python 3.8+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
@@ -85,14 +82,48 @@
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 # Release History
 
+## 7.0.0 (2024-04-22)
+
+### Features Added
+
+  - Added operation group ChatTranscriptsNoSubscriptionOperations
+  - Added operation group ChatTranscriptsOperations
+  - Added operation group CommunicationsNoSubscriptionOperations
+  - Added operation group FileWorkspacesNoSubscriptionOperations
+  - Added operation group FileWorkspacesOperations
+  - Added operation group FilesNoSubscriptionOperations
+  - Added operation group FilesOperations
+  - Added operation group SupportTicketsNoSubscriptionOperations
+  - Model ProblemClassification has a new parameter secondary_consent_enabled
+  - Model SupportTicketDetails has a new parameter file_workspace_name
+  - Model SupportTicketDetails has a new parameter is_temporary_ticket
+  - Model SupportTicketDetails has a new parameter problem_scoping_questions
+  - Model SupportTicketDetails has a new parameter secondary_consent
+  - Model SupportTicketDetails has a new parameter support_plan_display_name
+  - Model SupportTicketDetails has a new parameter support_plan_id
+  - Model UpdateSupportTicket has a new parameter advanced_diagnostic_consent
+  - Model UpdateSupportTicket has a new parameter secondary_consent
+
+### Breaking Changes
+
+  - Model SupportTicketDetails has a new required parameter advanced_diagnostic_consent
+  - Parameter body of model CommunicationDetails is now required
+  - Parameter contact_details of model SupportTicketDetails is now required
+  - Parameter description of model SupportTicketDetails is now required
+  - Parameter problem_classification_id of model SupportTicketDetails is now required
+  - Parameter service_id of model SupportTicketDetails is now required
+  - Parameter severity of model SupportTicketDetails is now required
+  - Parameter subject of model CommunicationDetails is now required
+  - Parameter title of model SupportTicketDetails is now required
+
 ## 6.1.0b3 (2024-03-18)
 
 ### Features Added
 
   - Added operation ChatTranscriptsNoSubscriptionOperations.list
   - Added operation CommunicationsNoSubscriptionOperations.list
   - Added operation ProblemClassificationsOperations.classify_problems
```

### Comparing `azure-mgmt-support-6.1.0b3/README.md` & `azure-mgmt-support-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/__init__.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/_configuration.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,21 +24,21 @@
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2023-06-01-preview". Note that overriding
-     this default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2024-04-01". Note that overriding this
+     default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        api_version: str = kwargs.pop("api_version", "2023-06-01-preview")
+        api_version: str = kwargs.pop("api_version", "2024-04-01")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
```

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/_microsoft_support.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/_microsoft_support.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,20 +22,16 @@
     ChatTranscriptsOperations,
     CommunicationsNoSubscriptionOperations,
     CommunicationsOperations,
     FileWorkspacesNoSubscriptionOperations,
     FileWorkspacesOperations,
     FilesNoSubscriptionOperations,
     FilesOperations,
-    LookUpResourceIdOperations,
     Operations,
-    ProblemClassificationsNoSubscriptionOperations,
     ProblemClassificationsOperations,
-    ServiceClassificationsNoSubscriptionOperations,
-    ServiceClassificationsOperations,
     ServicesOperations,
     SupportTicketsNoSubscriptionOperations,
     SupportTicketsOperations,
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
@@ -45,25 +41,14 @@
 class MicrosoftSupport:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
     """Microsoft Azure Support Resource Provider.
 
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.support.operations.Operations
     :ivar services: ServicesOperations operations
     :vartype services: azure.mgmt.support.operations.ServicesOperations
-    :ivar service_classifications_no_subscription: ServiceClassificationsNoSubscriptionOperations
-     operations
-    :vartype service_classifications_no_subscription:
-     azure.mgmt.support.operations.ServiceClassificationsNoSubscriptionOperations
-    :ivar service_classifications: ServiceClassificationsOperations operations
-    :vartype service_classifications:
-     azure.mgmt.support.operations.ServiceClassificationsOperations
-    :ivar problem_classifications_no_subscription: ProblemClassificationsNoSubscriptionOperations
-     operations
-    :vartype problem_classifications_no_subscription:
-     azure.mgmt.support.operations.ProblemClassificationsNoSubscriptionOperations
     :ivar problem_classifications: ProblemClassificationsOperations operations
     :vartype problem_classifications:
      azure.mgmt.support.operations.ProblemClassificationsOperations
     :ivar support_tickets: SupportTicketsOperations operations
     :vartype support_tickets: azure.mgmt.support.operations.SupportTicketsOperations
     :ivar support_tickets_no_subscription: SupportTicketsNoSubscriptionOperations operations
     :vartype support_tickets_no_subscription:
@@ -83,24 +68,22 @@
     :ivar file_workspaces_no_subscription: FileWorkspacesNoSubscriptionOperations operations
     :vartype file_workspaces_no_subscription:
      azure.mgmt.support.operations.FileWorkspacesNoSubscriptionOperations
     :ivar files: FilesOperations operations
     :vartype files: azure.mgmt.support.operations.FilesOperations
     :ivar files_no_subscription: FilesNoSubscriptionOperations operations
     :vartype files_no_subscription: azure.mgmt.support.operations.FilesNoSubscriptionOperations
-    :ivar look_up_resource_id: LookUpResourceIdOperations operations
-    :vartype look_up_resource_id: azure.mgmt.support.operations.LookUpResourceIdOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2023-06-01-preview". Note that overriding
-     this default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2024-04-01". Note that overriding this
+     default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
@@ -132,23 +115,14 @@
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.services = ServicesOperations(self._client, self._config, self._serialize, self._deserialize)
-        self.service_classifications_no_subscription = ServiceClassificationsNoSubscriptionOperations(
-            self._client, self._config, self._serialize, self._deserialize
-        )
-        self.service_classifications = ServiceClassificationsOperations(
-            self._client, self._config, self._serialize, self._deserialize
-        )
-        self.problem_classifications_no_subscription = ProblemClassificationsNoSubscriptionOperations(
-            self._client, self._config, self._serialize, self._deserialize
-        )
         self.problem_classifications = ProblemClassificationsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.support_tickets = SupportTicketsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.support_tickets_no_subscription = SupportTicketsNoSubscriptionOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
@@ -166,17 +140,14 @@
         self.file_workspaces_no_subscription = FileWorkspacesNoSubscriptionOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.files = FilesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.files_no_subscription = FilesNoSubscriptionOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
-        self.look_up_resource_id = LookUpResourceIdOperations(
-            self._client, self._config, self._serialize, self._deserialize
-        )
 
     def _send_request(self, request: HttpRequest, *, stream: bool = False, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
```

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/_patch.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/_serialization.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/_serialization.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/_vendor.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/__init__.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/_configuration.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/aio/_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,21 +24,21 @@
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2023-06-01-preview". Note that overriding
-     this default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2024-04-01". Note that overriding this
+     default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        api_version: str = kwargs.pop("api_version", "2023-06-01-preview")
+        api_version: str = kwargs.pop("api_version", "2024-04-01")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
```

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/_microsoft_support.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/aio/_microsoft_support.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,20 +22,16 @@
     ChatTranscriptsOperations,
     CommunicationsNoSubscriptionOperations,
     CommunicationsOperations,
     FileWorkspacesNoSubscriptionOperations,
     FileWorkspacesOperations,
     FilesNoSubscriptionOperations,
     FilesOperations,
-    LookUpResourceIdOperations,
     Operations,
-    ProblemClassificationsNoSubscriptionOperations,
     ProblemClassificationsOperations,
-    ServiceClassificationsNoSubscriptionOperations,
-    ServiceClassificationsOperations,
     ServicesOperations,
     SupportTicketsNoSubscriptionOperations,
     SupportTicketsOperations,
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
@@ -45,25 +41,14 @@
 class MicrosoftSupport:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
     """Microsoft Azure Support Resource Provider.
 
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.support.aio.operations.Operations
     :ivar services: ServicesOperations operations
     :vartype services: azure.mgmt.support.aio.operations.ServicesOperations
-    :ivar service_classifications_no_subscription: ServiceClassificationsNoSubscriptionOperations
-     operations
-    :vartype service_classifications_no_subscription:
-     azure.mgmt.support.aio.operations.ServiceClassificationsNoSubscriptionOperations
-    :ivar service_classifications: ServiceClassificationsOperations operations
-    :vartype service_classifications:
-     azure.mgmt.support.aio.operations.ServiceClassificationsOperations
-    :ivar problem_classifications_no_subscription: ProblemClassificationsNoSubscriptionOperations
-     operations
-    :vartype problem_classifications_no_subscription:
-     azure.mgmt.support.aio.operations.ProblemClassificationsNoSubscriptionOperations
     :ivar problem_classifications: ProblemClassificationsOperations operations
     :vartype problem_classifications:
      azure.mgmt.support.aio.operations.ProblemClassificationsOperations
     :ivar support_tickets: SupportTicketsOperations operations
     :vartype support_tickets: azure.mgmt.support.aio.operations.SupportTicketsOperations
     :ivar support_tickets_no_subscription: SupportTicketsNoSubscriptionOperations operations
     :vartype support_tickets_no_subscription:
@@ -83,24 +68,22 @@
     :ivar file_workspaces_no_subscription: FileWorkspacesNoSubscriptionOperations operations
     :vartype file_workspaces_no_subscription:
      azure.mgmt.support.aio.operations.FileWorkspacesNoSubscriptionOperations
     :ivar files: FilesOperations operations
     :vartype files: azure.mgmt.support.aio.operations.FilesOperations
     :ivar files_no_subscription: FilesNoSubscriptionOperations operations
     :vartype files_no_subscription: azure.mgmt.support.aio.operations.FilesNoSubscriptionOperations
-    :ivar look_up_resource_id: LookUpResourceIdOperations operations
-    :vartype look_up_resource_id: azure.mgmt.support.aio.operations.LookUpResourceIdOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2023-06-01-preview". Note that overriding
-     this default value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2024-04-01". Note that overriding this
+     default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
         self,
@@ -132,23 +115,14 @@
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.services = ServicesOperations(self._client, self._config, self._serialize, self._deserialize)
-        self.service_classifications_no_subscription = ServiceClassificationsNoSubscriptionOperations(
-            self._client, self._config, self._serialize, self._deserialize
-        )
-        self.service_classifications = ServiceClassificationsOperations(
-            self._client, self._config, self._serialize, self._deserialize
-        )
-        self.problem_classifications_no_subscription = ProblemClassificationsNoSubscriptionOperations(
-            self._client, self._config, self._serialize, self._deserialize
-        )
         self.problem_classifications = ProblemClassificationsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.support_tickets = SupportTicketsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.support_tickets_no_subscription = SupportTicketsNoSubscriptionOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
@@ -166,17 +140,14 @@
         self.file_workspaces_no_subscription = FileWorkspacesNoSubscriptionOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.files = FilesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.files_no_subscription = FilesNoSubscriptionOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
-        self.look_up_resource_id = LookUpResourceIdOperations(
-            self._client, self._config, self._serialize, self._deserialize
-        )
 
     def _send_request(
         self, request: HttpRequest, *, stream: bool = False, **kwargs: Any
     ) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
```

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/_patch.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/__init__.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,48 +4,40 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._operations import Operations
 from ._services_operations import ServicesOperations
-from ._service_classifications_no_subscription_operations import ServiceClassificationsNoSubscriptionOperations
-from ._service_classifications_operations import ServiceClassificationsOperations
-from ._problem_classifications_no_subscription_operations import ProblemClassificationsNoSubscriptionOperations
 from ._problem_classifications_operations import ProblemClassificationsOperations
 from ._support_tickets_operations import SupportTicketsOperations
 from ._support_tickets_no_subscription_operations import SupportTicketsNoSubscriptionOperations
 from ._communications_operations import CommunicationsOperations
 from ._communications_no_subscription_operations import CommunicationsNoSubscriptionOperations
 from ._chat_transcripts_operations import ChatTranscriptsOperations
 from ._chat_transcripts_no_subscription_operations import ChatTranscriptsNoSubscriptionOperations
 from ._file_workspaces_operations import FileWorkspacesOperations
 from ._file_workspaces_no_subscription_operations import FileWorkspacesNoSubscriptionOperations
 from ._files_operations import FilesOperations
 from ._files_no_subscription_operations import FilesNoSubscriptionOperations
-from ._look_up_resource_id_operations import LookUpResourceIdOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "Operations",
     "ServicesOperations",
-    "ServiceClassificationsNoSubscriptionOperations",
-    "ServiceClassificationsOperations",
-    "ProblemClassificationsNoSubscriptionOperations",
     "ProblemClassificationsOperations",
     "SupportTicketsOperations",
     "SupportTicketsNoSubscriptionOperations",
     "CommunicationsOperations",
     "CommunicationsNoSubscriptionOperations",
     "ChatTranscriptsOperations",
     "ChatTranscriptsNoSubscriptionOperations",
     "FileWorkspacesOperations",
     "FileWorkspacesNoSubscriptionOperations",
     "FilesOperations",
     "FilesNoSubscriptionOperations",
-    "LookUpResourceIdOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_chat_transcripts_no_subscription_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_chat_transcripts_no_subscription_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_chat_transcripts_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_chat_transcripts_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_communications_no_subscription_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_communications_no_subscription_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_communications_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_communications_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_file_workspaces_no_subscription_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_file_workspaces_no_subscription_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_file_workspaces_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_file_workspaces_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_files_no_subscription_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_files_no_subscription_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_files_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_files_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_look_up_resource_id_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_operations.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,160 +2,150 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
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
-from ...operations._look_up_resource_id_operations import build_post_request
+from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import _convert_request
 
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
 
-class LookUpResourceIdOperations:
+
+def build_list_request(**kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop("template_url", "/providers/Microsoft.Support/operations")
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
-        :class:`~azure.mgmt.support.aio.MicrosoftSupport`'s
-        :attr:`look_up_resource_id` attribute.
+        :class:`~azure.mgmt.support.MicrosoftSupport`'s
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
 
-    @overload
-    async def post(
-        self,
-        look_up_resource_id_request: _models.LookUpResourceIdRequest,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> _models.LookUpResourceIdResponse:
-        """This operation fetches ARM resource id of support resource type.
-
-        This operation fetches ARM resource id of support resource type.
-
-        :param look_up_resource_id_request: Look up resource id request body. Required.
-        :type look_up_resource_id_request: ~azure.mgmt.support.models.LookUpResourceIdRequest
-        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :return: LookUpResourceIdResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.support.models.LookUpResourceIdResponse
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
+    @distributed_trace
+    def list(self, **kwargs: Any) -> Iterable["_models.Operation"]:
+        """This lists all the available Microsoft Support REST API operations.
 
-    @overload
-    async def post(
-        self, look_up_resource_id_request: IO[bytes], *, content_type: str = "application/json", **kwargs: Any
-    ) -> _models.LookUpResourceIdResponse:
-        """This operation fetches ARM resource id of support resource type.
-
-        This operation fetches ARM resource id of support resource type.
-
-        :param look_up_resource_id_request: Look up resource id request body. Required.
-        :type look_up_resource_id_request: IO[bytes]
-        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :return: LookUpResourceIdResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.support.models.LookUpResourceIdResponse
+        :return: An iterator like instance of either Operation or the result of cls(response)
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.support.models.Operation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.OperationsListResult] = kwargs.pop("cls", None)
 
-    @distributed_trace_async
-    async def post(
-        self, look_up_resource_id_request: Union[_models.LookUpResourceIdRequest, IO[bytes]], **kwargs: Any
-    ) -> _models.LookUpResourceIdResponse:
-        """This operation fetches ARM resource id of support resource type.
-
-        This operation fetches ARM resource id of support resource type.
-
-        :param look_up_resource_id_request: Look up resource id request body. Is either a
-         LookUpResourceIdRequest type or a IO[bytes] type. Required.
-        :type look_up_resource_id_request: ~azure.mgmt.support.models.LookUpResourceIdRequest or
-         IO[bytes]
-        :return: LookUpResourceIdResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.support.models.LookUpResourceIdResponse
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
-        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.LookUpResourceIdResponse] = kwargs.pop("cls", None)
-
-        content_type = content_type or "application/json"
-        _json = None
-        _content = None
-        if isinstance(look_up_resource_id_request, (IOBase, bytes)):
-            _content = look_up_resource_id_request
-        else:
-            _json = self._serialize.body(look_up_resource_id_request, "LookUpResourceIdRequest")
-
-        _request = build_post_request(
-            api_version=api_version,
-            content_type=content_type,
-            json=_json,
-            content=_content,
-            headers=_headers,
-            params=_params,
-        )
-        _request = _convert_request(_request)
-        _request.url = self._client.format_url(_request.url)
-
-        _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            _request, stream=_stream, **kwargs
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+        def prepare_request(next_link=None):
+            if not next_link:
 
-        deserialized = self._deserialize("LookUpResourceIdResponse", pipeline_response)
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
+            deserialized = self._deserialize("OperationsListResult", pipeline_response)
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
 
-        if cls:
-            return cls(pipeline_response, deserialized, {})  # type: ignore
+            return pipeline_response
 
-        return deserialized  # type: ignore
+        return ItemPaged(get_next, extract_data)
```

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_patch.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_problem_classifications_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_problem_classifications_operations.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,207 +2,127 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from io import IOBase
-from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, overload
+from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
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
+from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
-from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
-from ... import models as _models
-from ..._vendor import _convert_request
-from ...operations._problem_classifications_operations import (
-    build_classify_problems_request,
-    build_get_request,
-    build_list_request,
-)
+from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import _convert_request
 
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
 
-class ProblemClassificationsOperations:
-    """
-    .. warning::
-        **DO NOT** instantiate this class directly.
 
-        Instead, you should access the following operations through
-        :class:`~azure.mgmt.support.aio.MicrosoftSupport`'s
-        :attr:`problem_classifications` attribute.
-    """
+def build_list_request(service_name: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    models = _models
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
+    accept = _headers.pop("Accept", "application/json")
 
-    def __init__(self, *args, **kwargs) -> None:
-        input_args = list(args)
-        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
-        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
-        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
-        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+    # Construct URL
+    _url = kwargs.pop("template_url", "/providers/Microsoft.Support/services/{serviceName}/problemClassifications")
+    path_format_arguments = {
+        "serviceName": _SERIALIZER.url("service_name", service_name, "str"),
+    }
 
-    @overload
-    async def classify_problems(
-        self,
-        problem_service_name: str,
-        problem_classifications_classification_input: _models.ProblemClassificationsClassificationInput,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> _models.ProblemClassificationsClassificationOutput:
-        """Classify the right problem classifications (categories) available for a specific Azure service.
-
-        :param problem_service_name: Name of the Azure service for which the problem classifications
-         need to be retrieved. Required.
-        :type problem_service_name: str
-        :param problem_classifications_classification_input: Input to check. Required.
-        :type problem_classifications_classification_input:
-         ~azure.mgmt.support.models.ProblemClassificationsClassificationInput
-        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :return: ProblemClassificationsClassificationOutput or the result of cls(response)
-        :rtype: ~azure.mgmt.support.models.ProblemClassificationsClassificationOutput
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
-    @overload
-    async def classify_problems(
-        self,
-        problem_service_name: str,
-        problem_classifications_classification_input: IO[bytes],
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> _models.ProblemClassificationsClassificationOutput:
-        """Classify the right problem classifications (categories) available for a specific Azure service.
-
-        :param problem_service_name: Name of the Azure service for which the problem classifications
-         need to be retrieved. Required.
-        :type problem_service_name: str
-        :param problem_classifications_classification_input: Input to check. Required.
-        :type problem_classifications_classification_input: IO[bytes]
-        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :return: ProblemClassificationsClassificationOutput or the result of cls(response)
-        :rtype: ~azure.mgmt.support.models.ProblemClassificationsClassificationOutput
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
-    @distributed_trace_async
-    async def classify_problems(
-        self,
-        problem_service_name: str,
-        problem_classifications_classification_input: Union[
-            _models.ProblemClassificationsClassificationInput, IO[bytes]
-        ],
-        **kwargs: Any
-    ) -> _models.ProblemClassificationsClassificationOutput:
-        """Classify the right problem classifications (categories) available for a specific Azure service.
-
-        :param problem_service_name: Name of the Azure service for which the problem classifications
-         need to be retrieved. Required.
-        :type problem_service_name: str
-        :param problem_classifications_classification_input: Input to check. Is either a
-         ProblemClassificationsClassificationInput type or a IO[bytes] type. Required.
-        :type problem_classifications_classification_input:
-         ~azure.mgmt.support.models.ProblemClassificationsClassificationInput or IO[bytes]
-        :return: ProblemClassificationsClassificationOutput or the result of cls(response)
-        :rtype: ~azure.mgmt.support.models.ProblemClassificationsClassificationOutput
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
-        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-        cls: ClsType[_models.ProblemClassificationsClassificationOutput] = kwargs.pop("cls", None)
 
-        content_type = content_type or "application/json"
-        _json = None
-        _content = None
-        if isinstance(problem_classifications_classification_input, (IOBase, bytes)):
-            _content = problem_classifications_classification_input
-        else:
-            _json = self._serialize.body(
-                problem_classifications_classification_input, "ProblemClassificationsClassificationInput"
-            )
+def build_get_request(service_name: str, problem_classification_name: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-        _request = build_classify_problems_request(
-            problem_service_name=problem_service_name,
-            subscription_id=self._config.subscription_id,
-            api_version=api_version,
-            content_type=content_type,
-            json=_json,
-            content=_content,
-            headers=_headers,
-            params=_params,
-        )
-        _request = _convert_request(_request)
-        _request.url = self._client.format_url(_request.url)
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
+    accept = _headers.pop("Accept", "application/json")
 
-        _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            _request, stream=_stream, **kwargs
-        )
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/providers/Microsoft.Support/services/{serviceName}/problemClassifications/{problemClassificationName}",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "serviceName": _SERIALIZER.url("service_name", service_name, "str"),
+        "problemClassificationName": _SERIALIZER.url("problem_classification_name", problem_classification_name, "str"),
+    }
 
-        response = pipeline_response.http_response
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
-        if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
-            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
-            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-        deserialized = self._deserialize("ProblemClassificationsClassificationOutput", pipeline_response)
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
-        if cls:
-            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized  # type: ignore
+class ProblemClassificationsOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~azure.mgmt.support.MicrosoftSupport`'s
+        :attr:`problem_classifications` attribute.
+    """
+
+    models = _models
+
+    def __init__(self, *args, **kwargs):
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(self, service_name: str, **kwargs: Any) -> AsyncIterable["_models.ProblemClassification"]:
+    def list(self, service_name: str, **kwargs: Any) -> Iterable["_models.ProblemClassification"]:
         """Lists all the problem classifications (categories) available for a specific Azure service.
         Always use the service and problem classifications obtained programmatically. This practice
         ensures that you always have the most recent set of service and problem classification Ids.
 
         :param service_name: Name of the Azure service for which the problem classifications need to be
          retrieved. Required.
         :type service_name: str
         :return: An iterator like instance of either ProblemClassification or the result of
          cls(response)
-        :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.support.models.ProblemClassification]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.support.models.ProblemClassification]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ProblemClassificationsListResult] = kwargs.pop("cls", None)
@@ -241,47 +161,44 @@
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
                 _request = _convert_request(_request)
                 _request.url = self._client.format_url(_request.url)
                 _request.method = "GET"
             return _request
 
-        async def extract_data(pipeline_response):
+        def extract_data(pipeline_response):
             deserialized = self._deserialize("ProblemClassificationsListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
-            return None, AsyncList(list_of_elem)
+            return None, iter(list_of_elem)
 
-        async def get_next(next_link=None):
+        def get_next(next_link=None):
             _request = prepare_request(next_link)
 
             _stream = False
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
                 _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return AsyncItemPaged(get_next, extract_data)
+        return ItemPaged(get_next, extract_data)
 
-    @distributed_trace_async
-    async def get(
-        self, service_name: str, problem_classification_name: str, **kwargs: Any
-    ) -> _models.ProblemClassification:
+    @distributed_trace
+    def get(self, service_name: str, problem_classification_name: str, **kwargs: Any) -> _models.ProblemClassification:
         """Get problem classification details for a specific Azure service.
 
-        :param service_name: Name of the Azure service for which the problem classifications need to be
-         retrieved. Required.
+        :param service_name: Name of the Azure service available for support. Required.
         :type service_name: str
         :param problem_classification_name: Name of problem classification. Required.
         :type problem_classification_name: str
         :return: ProblemClassification or the result of cls(response)
         :rtype: ~azure.mgmt.support.models.ProblemClassification
         :raises ~azure.core.exceptions.HttpResponseError:
         """
@@ -306,15 +223,15 @@
             headers=_headers,
             params=_params,
         )
         _request = _convert_request(_request)
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
```

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_services_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_services_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,16 +135,15 @@
 
         return AsyncItemPaged(get_next, extract_data)
 
     @distributed_trace_async
     async def get(self, service_name: str, **kwargs: Any) -> _models.Service:
         """Gets a specific Azure service for support ticket creation.
 
-        :param service_name: Name of the Azure service for which the problem classifications need to be
-         retrieved. Required.
+        :param service_name: Name of the Azure service. Required.
         :type service_name: str
         :return: Service or the result of cls(response)
         :rtype: ~azure.mgmt.support.models.Service
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
```

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_support_tickets_no_subscription_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_support_tickets_no_subscription_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/aio/operations/_support_tickets_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_support_tickets_operations.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/models/_microsoft_support_enums.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/models/_microsoft_support_enums.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/models/_models_py3.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/models/_models_py3.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 import datetime
-from typing import Any, List, Literal, Optional, TYPE_CHECKING, Union
+from typing import Any, List, Optional, TYPE_CHECKING, Union
 
 from .. import _serialization
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from .. import models as _models
 
@@ -223,82 +223,51 @@
         """ """
         super().__init__(**kwargs)
         self.name_available = None
         self.reason = None
         self.message = None
 
 
-class ClassificationService(_serialization.Model):
-    """Service Classification result object.
-
-    Variables are only populated by the server, and will be ignored when sending a request.
-
-    :ivar service_id: Azure resource Id of the service.
-    :vartype service_id: str
-    :ivar display_name: Localized name of the azure service.
-    :vartype display_name: str
-    :ivar resource_types: List of applicable ARM resource types for this service.
-    :vartype resource_types: list[str]
-    """
-
-    _validation = {
-        "service_id": {"readonly": True},
-        "display_name": {"readonly": True},
-    }
-
-    _attribute_map = {
-        "service_id": {"key": "serviceId", "type": "str"},
-        "display_name": {"key": "displayName", "type": "str"},
-        "resource_types": {"key": "resourceTypes", "type": "[str]"},
-    }
-
-    def __init__(self, *, resource_types: Optional[List[str]] = None, **kwargs: Any) -> None:
-        """
-        :keyword resource_types: List of applicable ARM resource types for this service.
-        :paramtype resource_types: list[str]
-        """
-        super().__init__(**kwargs)
-        self.service_id = None
-        self.display_name = None
-        self.resource_types = resource_types
-
-
 class CommunicationDetails(_serialization.Model):
     """Object that represents a Communication resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
+    All required parameters must be populated in order to send to server.
+
     :ivar id: Id of the resource.
     :vartype id: str
     :ivar name: Name of the resource.
     :vartype name: str
     :ivar type: Type of the resource 'Microsoft.Support/communications'.
     :vartype type: str
     :ivar communication_type: Communication type. Known values are: "web" and "phone".
     :vartype communication_type: str or ~azure.mgmt.support.models.CommunicationType
     :ivar communication_direction: Direction of communication. Known values are: "inbound" and
      "outbound".
     :vartype communication_direction: str or ~azure.mgmt.support.models.CommunicationDirection
     :ivar sender: Email address of the sender. This property is required if called by a service
      principal.
     :vartype sender: str
-    :ivar subject: Subject of the communication.
+    :ivar subject: Subject of the communication. Required.
     :vartype subject: str
-    :ivar body: Body of the communication.
+    :ivar body: Body of the communication. Required.
     :vartype body: str
     :ivar created_date: Time in UTC (ISO 8601 format) when the communication was created.
     :vartype created_date: ~datetime.datetime
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
         "communication_type": {"readonly": True},
         "communication_direction": {"readonly": True},
+        "subject": {"required": True},
+        "body": {"required": True},
         "created_date": {"readonly": True},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
@@ -306,24 +275,22 @@
         "communication_direction": {"key": "properties.communicationDirection", "type": "str"},
         "sender": {"key": "properties.sender", "type": "str"},
         "subject": {"key": "properties.subject", "type": "str"},
         "body": {"key": "properties.body", "type": "str"},
         "created_date": {"key": "properties.createdDate", "type": "iso-8601"},
     }
 
-    def __init__(
-        self, *, sender: Optional[str] = None, subject: Optional[str] = None, body: Optional[str] = None, **kwargs: Any
-    ) -> None:
+    def __init__(self, *, subject: str, body: str, sender: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword sender: Email address of the sender. This property is required if called by a service
          principal.
         :paramtype sender: str
-        :keyword subject: Subject of the communication.
+        :keyword subject: Subject of the communication. Required.
         :paramtype subject: str
-        :keyword body: Body of the communication.
+        :keyword body: Body of the communication. Required.
         :paramtype body: str
         """
         super().__init__(**kwargs)
         self.id = None
         self.name = None
         self.type = None
         self.communication_type = None
@@ -585,19 +552,22 @@
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
      information.
     :vartype system_data: ~azure.mgmt.support.models.SystemData
     :ivar created_on: Time in UTC (ISO 8601 format) when file workspace was created.
     :vartype created_on: ~datetime.datetime
-    :ivar chunk_size: Size of each chunk.
+    :ivar chunk_size: Size of each chunk. The size of each chunk should be provided in bytes and
+     must not exceed 2.5 megabytes (MB).
     :vartype chunk_size: int
-    :ivar file_size: Size of the file to be uploaded.
+    :ivar file_size: Size of the file to be uploaded. The file size must not exceed 5 MB and should
+     be provided in bytes.
     :vartype file_size: int
-    :ivar number_of_chunks: Number of chunks to be uploaded.
+    :ivar number_of_chunks: Number of chunks to be uploaded. The maximum number of allowed chunks
+     is 2.
     :vartype number_of_chunks: int
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
@@ -621,19 +591,22 @@
         *,
         chunk_size: Optional[int] = None,
         file_size: Optional[int] = None,
         number_of_chunks: Optional[int] = None,
         **kwargs: Any
     ) -> None:
         """
-        :keyword chunk_size: Size of each chunk.
+        :keyword chunk_size: Size of each chunk. The size of each chunk should be provided in bytes and
+         must not exceed 2.5 megabytes (MB).
         :paramtype chunk_size: int
-        :keyword file_size: Size of the file to be uploaded.
+        :keyword file_size: Size of the file to be uploaded. The file size must not exceed 5 MB and
+         should be provided in bytes.
         :paramtype file_size: int
-        :keyword number_of_chunks: Number of chunks to be uploaded.
+        :keyword number_of_chunks: Number of chunks to be uploaded. The maximum number of allowed
+         chunks is 2.
         :paramtype number_of_chunks: int
         """
         super().__init__(**kwargs)
         self.created_on = None
         self.chunk_size = chunk_size
         self.file_size = file_size
         self.number_of_chunks = number_of_chunks
@@ -710,108 +683,51 @@
     def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.created_on = None
         self.expiration_time = None
 
 
-class LookUpResourceIdRequest(_serialization.Model):
-    """The look up resource Id request body.
-
-    :ivar identifier: The System generated Id that is unique. Use supportTicketId property for
-     Microsoft.Support/supportTickets resource type.
-    :vartype identifier: str
-    :ivar type: The type of resource. Default value is "Microsoft.Support/supportTickets".
-    :vartype type: str
-    """
-
-    _attribute_map = {
-        "identifier": {"key": "identifier", "type": "str"},
-        "type": {"key": "type", "type": "str"},
-    }
-
-    def __init__(
-        self,
-        *,
-        identifier: Optional[str] = None,
-        type: Optional[Literal["Microsoft.Support/supportTickets"]] = None,
-        **kwargs: Any
-    ) -> None:
-        """
-        :keyword identifier: The System generated Id that is unique. Use supportTicketId property for
-         Microsoft.Support/supportTickets resource type.
-        :paramtype identifier: str
-        :keyword type: The type of resource. Default value is "Microsoft.Support/supportTickets".
-        :paramtype type: str
-        """
-        super().__init__(**kwargs)
-        self.identifier = identifier
-        self.type = type
-
-
-class LookUpResourceIdResponse(_serialization.Model):
-    """The look up resource id response.
-
-    :ivar resource_id: The resource Id of support resource type.
-    :vartype resource_id: str
-    """
-
-    _attribute_map = {
-        "resource_id": {"key": "resourceId", "type": "str"},
-    }
-
-    def __init__(self, *, resource_id: Optional[str] = None, **kwargs: Any) -> None:
-        """
-        :keyword resource_id: The resource Id of support resource type.
-        :paramtype resource_id: str
-        """
-        super().__init__(**kwargs)
-        self.resource_id = resource_id
-
-
 class MessageProperties(_serialization.Model):
     """Describes the properties of a Message Details resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    All required parameters must be populated in order to send to server.
-
     :ivar content_type: Content type.
     :vartype content_type: str or ~azure.mgmt.support.models.TranscriptContentType
     :ivar communication_direction: Direction of communication. Known values are: "inbound" and
      "outbound".
     :vartype communication_direction: str or ~azure.mgmt.support.models.CommunicationDirection
     :ivar sender: Name of the sender.
     :vartype sender: str
-    :ivar body: Body of the communication. Required.
+    :ivar body: Body of the communication.
     :vartype body: str
     :ivar created_date: Time in UTC (ISO 8601 format) when the communication was created.
     :vartype created_date: ~datetime.datetime
     """
 
     _validation = {
         "content_type": {"readonly": True},
         "communication_direction": {"readonly": True},
-        "body": {"required": True},
         "created_date": {"readonly": True},
     }
 
     _attribute_map = {
         "content_type": {"key": "contentType", "type": "str"},
         "communication_direction": {"key": "communicationDirection", "type": "str"},
         "sender": {"key": "sender", "type": "str"},
         "body": {"key": "body", "type": "str"},
         "created_date": {"key": "createdDate", "type": "iso-8601"},
     }
 
-    def __init__(self, *, body: str, sender: Optional[str] = None, **kwargs: Any) -> None:
+    def __init__(self, *, sender: Optional[str] = None, body: Optional[str] = None, **kwargs: Any) -> None:
         """
         :keyword sender: Name of the sender.
         :paramtype sender: str
-        :keyword body: Body of the communication. Required.
+        :keyword body: Body of the communication.
         :paramtype body: str
         """
         super().__init__(**kwargs)
         self.content_type = None
         self.communication_direction = None
         self.sender = sender
         self.body = body
@@ -918,189 +834,50 @@
     :ivar type: Type of the resource 'Microsoft.Support/problemClassification'.
     :vartype type: str
     :ivar display_name: Localized name of problem classification.
     :vartype display_name: str
     :ivar secondary_consent_enabled: This property indicates whether secondary consent is present
      for problem classification.
     :vartype secondary_consent_enabled: list[~azure.mgmt.support.models.SecondaryConsentEnabled]
-    :ivar metadata: String-to-string dictionary for additional metadata.
-    :vartype metadata: dict[str, str]
-    :ivar parent_problem_classification: Reference to the parent problem classification which has
-     same structure as problem classification.
-    :vartype parent_problem_classification: ~azure.mgmt.support.models.ProblemClassification
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
-        "metadata": {"readonly": True},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "display_name": {"key": "properties.displayName", "type": "str"},
         "secondary_consent_enabled": {"key": "properties.secondaryConsentEnabled", "type": "[SecondaryConsentEnabled]"},
-        "metadata": {"key": "properties.metadata", "type": "{str}"},
-        "parent_problem_classification": {
-            "key": "properties.parentProblemClassification",
-            "type": "ProblemClassification",
-        },
     }
 
     def __init__(
         self,
         *,
         display_name: Optional[str] = None,
         secondary_consent_enabled: Optional[List["_models.SecondaryConsentEnabled"]] = None,
-        parent_problem_classification: Optional["_models.ProblemClassification"] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword display_name: Localized name of problem classification.
         :paramtype display_name: str
         :keyword secondary_consent_enabled: This property indicates whether secondary consent is
          present for problem classification.
         :paramtype secondary_consent_enabled: list[~azure.mgmt.support.models.SecondaryConsentEnabled]
-        :keyword parent_problem_classification: Reference to the parent problem classification which
-         has same structure as problem classification.
-        :paramtype parent_problem_classification: ~azure.mgmt.support.models.ProblemClassification
         """
         super().__init__(**kwargs)
         self.id = None
         self.name = None
         self.type = None
         self.display_name = display_name
         self.secondary_consent_enabled = secondary_consent_enabled
-        self.metadata = None
-        self.parent_problem_classification = parent_problem_classification
-
-
-class ProblemClassificationsClassificationInput(_serialization.Model):  # pylint: disable=name-too-long
-    """Input to problem classification Classification API.
-
-    All required parameters must be populated in order to send to server.
-
-    :ivar issue_summary: Natural language description of the customer’s issue. Required.
-    :vartype issue_summary: str
-    :ivar resource_id: ARM resource Id of the resource that is having the issue.
-    :vartype resource_id: str
-    """
-
-    _validation = {
-        "issue_summary": {"required": True},
-    }
-
-    _attribute_map = {
-        "issue_summary": {"key": "issueSummary", "type": "str"},
-        "resource_id": {"key": "resourceId", "type": "str"},
-    }
-
-    def __init__(self, *, issue_summary: str, resource_id: Optional[str] = None, **kwargs: Any) -> None:
-        """
-        :keyword issue_summary: Natural language description of the customer’s issue. Required.
-        :paramtype issue_summary: str
-        :keyword resource_id: ARM resource Id of the resource that is having the issue.
-        :paramtype resource_id: str
-        """
-        super().__init__(**kwargs)
-        self.issue_summary = issue_summary
-        self.resource_id = resource_id
-
-
-class ProblemClassificationsClassificationOutput(_serialization.Model):  # pylint: disable=name-too-long
-    """Output of the problem classification Classification API.
-
-    :ivar problem_classification_results: Set of problem classification objects classified.
-    :vartype problem_classification_results:
-     list[~azure.mgmt.support.models.ProblemClassificationsClassificationResult]
-    """
-
-    _attribute_map = {
-        "problem_classification_results": {
-            "key": "problemClassificationResults",
-            "type": "[ProblemClassificationsClassificationResult]",
-        },
-    }
-
-    def __init__(
-        self,
-        *,
-        problem_classification_results: Optional[List["_models.ProblemClassificationsClassificationResult"]] = None,
-        **kwargs: Any
-    ) -> None:
-        """
-        :keyword problem_classification_results: Set of problem classification objects classified.
-        :paramtype problem_classification_results:
-         list[~azure.mgmt.support.models.ProblemClassificationsClassificationResult]
-        """
-        super().__init__(**kwargs)
-        self.problem_classification_results = problem_classification_results
-
-
-class ProblemClassificationsClassificationResult(_serialization.Model):  # pylint: disable=name-too-long
-    """ProblemClassification Classification result object.
-
-    Variables are only populated by the server, and will be ignored when sending a request.
-
-    :ivar problem_id: Identifier that may be used for solution discovery or some other purposes.
-    :vartype problem_id: str
-    :ivar title: Title of the problem classification result.
-    :vartype title: str
-    :ivar description: Description of the problem classification result.
-    :vartype description: str
-    :ivar service_id: Identifier of the service associated with this problem classification result.
-    :vartype service_id: str
-    :ivar problem_classification_id: Identifier that may be used for support ticket creation.
-    :vartype problem_classification_id: str
-    :ivar service_id_related_service_id: Azure resource Id of the service.
-    :vartype service_id_related_service_id: str
-    :ivar display_name: Localized name of the azure service.
-    :vartype display_name: str
-    :ivar resource_types: List of applicable ARM resource types for this service.
-    :vartype resource_types: list[str]
-    """
-
-    _validation = {
-        "problem_id": {"readonly": True},
-        "title": {"readonly": True},
-        "description": {"readonly": True},
-        "service_id": {"readonly": True},
-        "problem_classification_id": {"readonly": True},
-        "service_id_related_service_id": {"readonly": True},
-        "display_name": {"readonly": True},
-    }
-
-    _attribute_map = {
-        "problem_id": {"key": "problemId", "type": "str"},
-        "title": {"key": "title", "type": "str"},
-        "description": {"key": "description", "type": "str"},
-        "service_id": {"key": "serviceId", "type": "str"},
-        "problem_classification_id": {"key": "problemClassificationId", "type": "str"},
-        "service_id_related_service_id": {"key": "relatedService.serviceId", "type": "str"},
-        "display_name": {"key": "relatedService.displayName", "type": "str"},
-        "resource_types": {"key": "relatedService.resourceTypes", "type": "[str]"},
-    }
-
-    def __init__(self, *, resource_types: Optional[List[str]] = None, **kwargs: Any) -> None:
-        """
-        :keyword resource_types: List of applicable ARM resource types for this service.
-        :paramtype resource_types: list[str]
-        """
-        super().__init__(**kwargs)
-        self.problem_id = None
-        self.title = None
-        self.description = None
-        self.service_id = None
-        self.problem_classification_id = None
-        self.service_id_related_service_id = None
-        self.display_name = None
-        self.resource_types = resource_types
 
 
 class ProblemClassificationsListResult(_serialization.Model):
     """Collection of ProblemClassification resources.
 
     :ivar value: List of ProblemClassification resources.
     :vartype value: list[~azure.mgmt.support.models.ProblemClassification]
@@ -1261,32 +1038,28 @@
     :vartype name: str
     :ivar type: Type of the resource 'Microsoft.Support/services'.
     :vartype type: str
     :ivar display_name: Localized name of the Azure service.
     :vartype display_name: str
     :ivar resource_types: ARM Resource types.
     :vartype resource_types: list[str]
-    :ivar metadata: Metadata about the service, only visible for 1P clients.
-    :vartype metadata: dict[str, str]
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
-        "metadata": {"readonly": True},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "display_name": {"key": "properties.displayName", "type": "str"},
         "resource_types": {"key": "properties.resourceTypes", "type": "[str]"},
-        "metadata": {"key": "properties.metadata", "type": "{str}"},
     }
 
     def __init__(
         self, *, display_name: Optional[str] = None, resource_types: Optional[List[str]] = None, **kwargs: Any
     ) -> None:
         """
         :keyword display_name: Localized name of the Azure service.
@@ -1296,128 +1069,14 @@
         """
         super().__init__(**kwargs)
         self.id = None
         self.name = None
         self.type = None
         self.display_name = display_name
         self.resource_types = resource_types
-        self.metadata = None
-
-
-class ServiceClassificationAnswer(ClassificationService):
-    """Service Classification result object.
-
-    Variables are only populated by the server, and will be ignored when sending a request.
-
-    :ivar service_id: Azure resource Id of the service.
-    :vartype service_id: str
-    :ivar display_name: Localized name of the azure service.
-    :vartype display_name: str
-    :ivar resource_types: List of applicable ARM resource types for this service.
-    :vartype resource_types: list[str]
-    :ivar child_service: Child service.
-    :vartype child_service: ~azure.mgmt.support.models.ClassificationService
-    """
-
-    _validation = {
-        "service_id": {"readonly": True},
-        "display_name": {"readonly": True},
-    }
-
-    _attribute_map = {
-        "service_id": {"key": "serviceId", "type": "str"},
-        "display_name": {"key": "displayName", "type": "str"},
-        "resource_types": {"key": "resourceTypes", "type": "[str]"},
-        "child_service": {"key": "childService", "type": "ClassificationService"},
-    }
-
-    def __init__(
-        self,
-        *,
-        resource_types: Optional[List[str]] = None,
-        child_service: Optional["_models.ClassificationService"] = None,
-        **kwargs: Any
-    ) -> None:
-        """
-        :keyword resource_types: List of applicable ARM resource types for this service.
-        :paramtype resource_types: list[str]
-        :keyword child_service: Child service.
-        :paramtype child_service: ~azure.mgmt.support.models.ClassificationService
-        """
-        super().__init__(resource_types=resource_types, **kwargs)
-        self.child_service = child_service
-
-
-class ServiceClassificationOutput(_serialization.Model):
-    """Output of the service classification API.
-
-    :ivar service_classification_results: Set of problem classification objects classified.
-    :vartype service_classification_results:
-     list[~azure.mgmt.support.models.ServiceClassificationAnswer]
-    """
-
-    _attribute_map = {
-        "service_classification_results": {
-            "key": "serviceClassificationResults",
-            "type": "[ServiceClassificationAnswer]",
-        },
-    }
-
-    def __init__(
-        self,
-        *,
-        service_classification_results: Optional[List["_models.ServiceClassificationAnswer"]] = None,
-        **kwargs: Any
-    ) -> None:
-        """
-        :keyword service_classification_results: Set of problem classification objects classified.
-        :paramtype service_classification_results:
-         list[~azure.mgmt.support.models.ServiceClassificationAnswer]
-        """
-        super().__init__(**kwargs)
-        self.service_classification_results = service_classification_results
-
-
-class ServiceClassificationRequest(_serialization.Model):
-    """Input to problem classification Classification API.
-
-    :ivar issue_summary: Natural language description of the customer’s issue.
-    :vartype issue_summary: str
-    :ivar resource_id: ARM resource Id of the resource that is having the issue.
-    :vartype resource_id: str
-    :ivar additional_context: Additional information in the form of a string.
-    :vartype additional_context: str
-    """
-
-    _attribute_map = {
-        "issue_summary": {"key": "issueSummary", "type": "str"},
-        "resource_id": {"key": "resourceId", "type": "str"},
-        "additional_context": {"key": "additionalContext", "type": "str"},
-    }
-
-    def __init__(
-        self,
-        *,
-        issue_summary: Optional[str] = None,
-        resource_id: Optional[str] = None,
-        additional_context: Optional[str] = None,
-        **kwargs: Any
-    ) -> None:
-        """
-        :keyword issue_summary: Natural language description of the customer’s issue.
-        :paramtype issue_summary: str
-        :keyword resource_id: ARM resource Id of the resource that is having the issue.
-        :paramtype resource_id: str
-        :keyword additional_context: Additional information in the form of a string.
-        :paramtype additional_context: str
-        """
-        super().__init__(**kwargs)
-        self.issue_summary = issue_summary
-        self.resource_id = resource_id
-        self.additional_context = additional_context
 
 
 class ServiceLevelAgreement(_serialization.Model):
     """Service Level Agreement details for a support ticket.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
@@ -1494,63 +1153,66 @@
 
 
 class SupportTicketDetails(_serialization.Model):  # pylint: disable=too-many-instance-attributes
     """Object that represents SupportTicketDetails resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
+    All required parameters must be populated in order to send to server.
+
     :ivar id: Id of the resource.
     :vartype id: str
     :ivar name: Name of the resource.
     :vartype name: str
     :ivar type: Type of the resource 'Microsoft.Support/supportTickets'.
     :vartype type: str
     :ivar support_ticket_id: System generated support ticket Id that is unique.
     :vartype support_ticket_id: str
-    :ivar description: Detailed description of the question or issue.
+    :ivar description: Detailed description of the question or issue. Required.
     :vartype description: str
     :ivar problem_classification_id: Each Azure service has its own set of issue categories, also
      known as problem classification. This parameter is the unique Id for the type of problem you
-     are experiencing.
+     are experiencing. Required.
     :vartype problem_classification_id: str
     :ivar problem_classification_display_name: Localized name of problem classification.
     :vartype problem_classification_display_name: str
     :ivar severity: A value that indicates the urgency of the case, which in turn determines the
      response time according to the service level agreement of the technical support plan you have
      with Azure. Note: 'Highest critical impact', also known as the 'Emergency - Severe impact'
-     level in the Azure portal is reserved only for our Premium customers. Known values are:
-     "minimal", "moderate", "critical", and "highestcriticalimpact".
+     level in the Azure portal is reserved only for our Premium customers. Required. Known values
+     are: "minimal", "moderate", "critical", and "highestcriticalimpact".
     :vartype severity: str or ~azure.mgmt.support.models.SeverityLevel
     :ivar enrollment_id: Enrollment Id associated with the support ticket.
     :vartype enrollment_id: str
     :ivar require24_x7_response: Indicates if this requires a 24x7 response from Azure.
     :vartype require24_x7_response: bool
     :ivar advanced_diagnostic_consent: Advanced diagnostic consent to be updated on the support
-     ticket. Known values are: "Yes" and "No".
+     ticket. Required. Known values are: "Yes" and "No".
     :vartype advanced_diagnostic_consent: str or ~azure.mgmt.support.models.Consent
     :ivar problem_scoping_questions: Problem scoping questions associated with the support ticket.
     :vartype problem_scoping_questions: str
     :ivar support_plan_id: Support plan id associated with the support ticket.
     :vartype support_plan_id: str
     :ivar contact_details: Contact information of the user requesting to create a support ticket.
+     Required.
     :vartype contact_details: ~azure.mgmt.support.models.ContactProfile
     :ivar service_level_agreement: Service Level Agreement information for this support ticket.
     :vartype service_level_agreement: ~azure.mgmt.support.models.ServiceLevelAgreement
     :ivar support_engineer: Information about the support engineer working on this support ticket.
     :vartype support_engineer: ~azure.mgmt.support.models.SupportEngineer
     :ivar support_plan_type: Support plan type associated with the support ticket.
     :vartype support_plan_type: str
     :ivar support_plan_display_name: Support plan type associated with the support ticket.
     :vartype support_plan_display_name: str
-    :ivar title: Title of the support ticket.
+    :ivar title: Title of the support ticket. Required.
     :vartype title: str
     :ivar problem_start_time: Time in UTC (ISO 8601 format) when the problem started.
     :vartype problem_start_time: ~datetime.datetime
     :ivar service_id: This is the resource Id of the Azure service resource associated with the
-     support ticket.
+     support ticket. Required.
     :vartype service_id: str
     :ivar service_display_name: Localized name of the Azure service.
     :vartype service_display_name: str
     :ivar status: Status of the support ticket.
     :vartype status: str
     :ivar created_date: Time in UTC (ISO 8601 format) when the support ticket was created.
     :vartype created_date: ~datetime.datetime
@@ -1571,17 +1233,24 @@
     :vartype secondary_consent: list[~azure.mgmt.support.models.SecondaryConsent]
     """
 
     _validation = {
         "id": {"readonly": True},
         "name": {"readonly": True},
         "type": {"readonly": True},
+        "description": {"required": True},
+        "problem_classification_id": {"required": True},
         "problem_classification_display_name": {"readonly": True},
+        "severity": {"required": True},
+        "advanced_diagnostic_consent": {"required": True},
+        "contact_details": {"required": True},
         "support_plan_type": {"readonly": True},
         "support_plan_display_name": {"readonly": True},
+        "title": {"required": True},
+        "service_id": {"required": True},
         "service_display_name": {"readonly": True},
         "status": {"readonly": True},
         "created_date": {"readonly": True},
         "modified_date": {"readonly": True},
         "is_temporary_ticket": {"readonly": True},
     }
 
@@ -1617,76 +1286,76 @@
         "quota_ticket_details": {"key": "properties.quotaTicketDetails", "type": "QuotaTicketDetails"},
         "secondary_consent": {"key": "properties.secondaryConsent", "type": "[SecondaryConsent]"},
     }
 
     def __init__(  # pylint: disable=too-many-locals
         self,
         *,
+        description: str,
+        problem_classification_id: str,
+        severity: Union[str, "_models.SeverityLevel"],
+        advanced_diagnostic_consent: Union[str, "_models.Consent"],
+        contact_details: "_models.ContactProfile",
+        title: str,
+        service_id: str,
         support_ticket_id: Optional[str] = None,
-        description: Optional[str] = None,
-        problem_classification_id: Optional[str] = None,
-        severity: Optional[Union[str, "_models.SeverityLevel"]] = None,
         enrollment_id: Optional[str] = None,
         require24_x7_response: Optional[bool] = None,
-        advanced_diagnostic_consent: Optional[Union[str, "_models.Consent"]] = None,
         problem_scoping_questions: Optional[str] = None,
         support_plan_id: Optional[str] = None,
-        contact_details: Optional["_models.ContactProfile"] = None,
         service_level_agreement: Optional["_models.ServiceLevelAgreement"] = None,
         support_engineer: Optional["_models.SupportEngineer"] = None,
-        title: Optional[str] = None,
         problem_start_time: Optional[datetime.datetime] = None,
-        service_id: Optional[str] = None,
         file_workspace_name: Optional[str] = None,
         technical_ticket_details: Optional["_models.TechnicalTicketDetails"] = None,
         quota_ticket_details: Optional["_models.QuotaTicketDetails"] = None,
         secondary_consent: Optional[List["_models.SecondaryConsent"]] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword support_ticket_id: System generated support ticket Id that is unique.
         :paramtype support_ticket_id: str
-        :keyword description: Detailed description of the question or issue.
+        :keyword description: Detailed description of the question or issue. Required.
         :paramtype description: str
         :keyword problem_classification_id: Each Azure service has its own set of issue categories,
          also known as problem classification. This parameter is the unique Id for the type of problem
-         you are experiencing.
+         you are experiencing. Required.
         :paramtype problem_classification_id: str
         :keyword severity: A value that indicates the urgency of the case, which in turn determines the
          response time according to the service level agreement of the technical support plan you have
          with Azure. Note: 'Highest critical impact', also known as the 'Emergency - Severe impact'
-         level in the Azure portal is reserved only for our Premium customers. Known values are:
-         "minimal", "moderate", "critical", and "highestcriticalimpact".
+         level in the Azure portal is reserved only for our Premium customers. Required. Known values
+         are: "minimal", "moderate", "critical", and "highestcriticalimpact".
         :paramtype severity: str or ~azure.mgmt.support.models.SeverityLevel
         :keyword enrollment_id: Enrollment Id associated with the support ticket.
         :paramtype enrollment_id: str
         :keyword require24_x7_response: Indicates if this requires a 24x7 response from Azure.
         :paramtype require24_x7_response: bool
         :keyword advanced_diagnostic_consent: Advanced diagnostic consent to be updated on the support
-         ticket. Known values are: "Yes" and "No".
+         ticket. Required. Known values are: "Yes" and "No".
         :paramtype advanced_diagnostic_consent: str or ~azure.mgmt.support.models.Consent
         :keyword problem_scoping_questions: Problem scoping questions associated with the support
          ticket.
         :paramtype problem_scoping_questions: str
         :keyword support_plan_id: Support plan id associated with the support ticket.
         :paramtype support_plan_id: str
         :keyword contact_details: Contact information of the user requesting to create a support
-         ticket.
+         ticket. Required.
         :paramtype contact_details: ~azure.mgmt.support.models.ContactProfile
         :keyword service_level_agreement: Service Level Agreement information for this support ticket.
         :paramtype service_level_agreement: ~azure.mgmt.support.models.ServiceLevelAgreement
         :keyword support_engineer: Information about the support engineer working on this support
          ticket.
         :paramtype support_engineer: ~azure.mgmt.support.models.SupportEngineer
-        :keyword title: Title of the support ticket.
+        :keyword title: Title of the support ticket. Required.
         :paramtype title: str
         :keyword problem_start_time: Time in UTC (ISO 8601 format) when the problem started.
         :paramtype problem_start_time: ~datetime.datetime
         :keyword service_id: This is the resource Id of the Azure service resource associated with the
-         support ticket.
+         support ticket. Required.
         :paramtype service_id: str
         :keyword file_workspace_name: File workspace name.
         :paramtype file_workspace_name: str
         :keyword technical_ticket_details: Additional ticket details associated with a technical
          support ticket request.
         :paramtype technical_ticket_details: ~azure.mgmt.support.models.TechnicalTicketDetails
         :keyword quota_ticket_details: Additional ticket details associated with a quota support ticket
@@ -1943,15 +1612,16 @@
         self.phone_number = phone_number
         self.preferred_time_zone = preferred_time_zone
         self.country = country
         self.preferred_support_language = preferred_support_language
 
 
 class UpdateSupportTicket(_serialization.Model):
-    """Updates severity, ticket status, and contact details in the support ticket.
+    """Updates severity, ticket status, contact details, advanced diagnostic consent and secondary
+    consent in the support ticket.
 
     :ivar severity: Severity level. Known values are: "minimal", "moderate", "critical", and
      "highestcriticalimpact".
     :vartype severity: str or ~azure.mgmt.support.models.SeverityLevel
     :ivar status: Status to be updated on the ticket. Known values are: "open" and "closed".
     :vartype status: str or ~azure.mgmt.support.models.Status
     :ivar contact_details: Contact details to be updated on the support ticket.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/models/_patch.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/__init__.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/operations/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,48 +4,40 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._operations import Operations
 from ._services_operations import ServicesOperations
-from ._service_classifications_no_subscription_operations import ServiceClassificationsNoSubscriptionOperations
-from ._service_classifications_operations import ServiceClassificationsOperations
-from ._problem_classifications_no_subscription_operations import ProblemClassificationsNoSubscriptionOperations
 from ._problem_classifications_operations import ProblemClassificationsOperations
 from ._support_tickets_operations import SupportTicketsOperations
 from ._support_tickets_no_subscription_operations import SupportTicketsNoSubscriptionOperations
 from ._communications_operations import CommunicationsOperations
 from ._communications_no_subscription_operations import CommunicationsNoSubscriptionOperations
 from ._chat_transcripts_operations import ChatTranscriptsOperations
 from ._chat_transcripts_no_subscription_operations import ChatTranscriptsNoSubscriptionOperations
 from ._file_workspaces_operations import FileWorkspacesOperations
 from ._file_workspaces_no_subscription_operations import FileWorkspacesNoSubscriptionOperations
 from ._files_operations import FilesOperations
 from ._files_no_subscription_operations import FilesNoSubscriptionOperations
-from ._look_up_resource_id_operations import LookUpResourceIdOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "Operations",
     "ServicesOperations",
-    "ServiceClassificationsNoSubscriptionOperations",
-    "ServiceClassificationsOperations",
-    "ProblemClassificationsNoSubscriptionOperations",
     "ProblemClassificationsOperations",
     "SupportTicketsOperations",
     "SupportTicketsNoSubscriptionOperations",
     "CommunicationsOperations",
     "CommunicationsNoSubscriptionOperations",
     "ChatTranscriptsOperations",
     "ChatTranscriptsNoSubscriptionOperations",
     "FileWorkspacesOperations",
     "FileWorkspacesNoSubscriptionOperations",
     "FilesOperations",
     "FilesNoSubscriptionOperations",
-    "LookUpResourceIdOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_chat_transcripts_no_subscription_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_chat_transcripts_no_subscription_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(support_ticket_name: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.Support/supportTickets/{supportTicketName}/chatTranscripts")
     path_format_arguments = {
         "supportTicketName": _SERIALIZER.url("support_ticket_name", support_ticket_name, "str"),
     }
@@ -60,15 +60,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(support_ticket_name: str, chat_transcript_name: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/providers/Microsoft.Support/supportTickets/{supportTicketName}/chatTranscripts/{chatTranscriptName}",
     )  # pylint: disable=line-too-long
```

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_chat_transcripts_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_chat_transcripts_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(support_ticket_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.Support/supportTickets/{supportTicketName}/chatTranscripts",
     )  # pylint: disable=line-too-long
@@ -66,15 +66,15 @@
 
 def build_get_request(
     support_ticket_name: str, chat_transcript_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.Support/supportTickets/{supportTicketName}/chatTranscripts/{chatTranscriptName}",
     )  # pylint: disable=line-too-long
```

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_communications_no_subscription_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_communications_no_subscription_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_check_name_availability_request(support_ticket_name: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/providers/Microsoft.Support/supportTickets/{supportTicketName}/checkNameAvailability"
     )  # pylint: disable=line-too-long
@@ -70,15 +70,15 @@
 
 def build_list_request(
     support_ticket_name: str, *, top: Optional[int] = None, filter: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.Support/supportTickets/{supportTicketName}/communications")
     path_format_arguments = {
         "supportTicketName": _SERIALIZER.url("support_ticket_name", support_ticket_name, "str"),
     }
@@ -98,15 +98,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(support_ticket_name: str, communication_name: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/providers/Microsoft.Support/supportTickets/{supportTicketName}/communications/{communicationName}",
     )  # pylint: disable=line-too-long
@@ -126,15 +126,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_create_request(support_ticket_name: str, communication_name: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/providers/Microsoft.Support/supportTickets/{supportTicketName}/communications/{communicationName}",
```

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_communications_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_communications_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_check_name_availability_request(support_ticket_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.Support/supportTickets/{supportTicketName}/checkNameAvailability",
@@ -77,15 +77,15 @@
     top: Optional[int] = None,
     filter: Optional[str] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.Support/supportTickets/{supportTicketName}/communications",
     )  # pylint: disable=line-too-long
@@ -111,15 +111,15 @@
 
 def build_get_request(
     support_ticket_name: str, communication_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.Support/supportTickets/{supportTicketName}/communications/{communicationName}",
     )  # pylint: disable=line-too-long
@@ -142,15 +142,15 @@
 
 def build_create_request(
     support_ticket_name: str, communication_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.Support/supportTickets/{supportTicketName}/communications/{communicationName}",
```

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_file_workspaces_no_subscription_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_file_workspaces_no_subscription_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_get_request(file_workspace_name: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.Support/fileWorkspaces/{fileWorkspaceName}")
     path_format_arguments = {
         "fileWorkspaceName": _SERIALIZER.url("file_workspace_name", file_workspace_name, "str"),
     }
@@ -58,15 +58,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_create_request(file_workspace_name: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.Support/fileWorkspaces/{fileWorkspaceName}")
     path_format_arguments = {
         "fileWorkspaceName": _SERIALIZER.url(
             "file_workspace_name", file_workspace_name, "str", pattern=r"^[0-9a-zA-Z_\-. ]+$"
```

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_file_workspaces_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_file_workspaces_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_get_request(file_workspace_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.Support/fileWorkspaces/{fileWorkspaceName}"
     )  # pylint: disable=line-too-long
     path_format_arguments = {
@@ -61,15 +61,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_create_request(file_workspace_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.Support/fileWorkspaces/{fileWorkspaceName}"
     )  # pylint: disable=line-too-long
     path_format_arguments = {
```

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_files_no_subscription_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_files_no_subscription_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(file_workspace_name: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.Support/fileWorkspaces/{fileWorkspaceName}/files")
     path_format_arguments = {
         "fileWorkspaceName": _SERIALIZER.url("file_workspace_name", file_workspace_name, "str"),
     }
@@ -61,15 +61,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(file_workspace_name: str, file_name: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/providers/Microsoft.Support/fileWorkspaces/{fileWorkspaceName}/files/{fileName}"
     )
     path_format_arguments = {
@@ -88,15 +88,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_create_request(file_workspace_name: str, file_name: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/providers/Microsoft.Support/fileWorkspaces/{fileWorkspaceName}/files/{fileName}"
     )
@@ -120,15 +120,15 @@
     return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_upload_request(file_workspace_name: str, file_name: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/providers/Microsoft.Support/fileWorkspaces/{fileWorkspaceName}/files/{fileName}/upload"
     )  # pylint: disable=line-too-long
```

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_files_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_files_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(file_workspace_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.Support/fileWorkspaces/{fileWorkspaceName}/files",
     )  # pylint: disable=line-too-long
@@ -65,15 +65,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(file_workspace_name: str, file_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.Support/fileWorkspaces/{fileWorkspaceName}/files/{fileName}",
     )  # pylint: disable=line-too-long
@@ -94,15 +94,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_create_request(file_workspace_name: str, file_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.Support/fileWorkspaces/{fileWorkspaceName}/files/{fileName}",
@@ -128,15 +128,15 @@
     return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_upload_request(file_workspace_name: str, file_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.Support/fileWorkspaces/{fileWorkspaceName}/files/{fileName}/upload",
```

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_look_up_resource_id_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/aio/operations/_problem_classifications_operations.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,185 +2,194 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
+from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
+import urllib.parse
 
+from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import HttpResponse
+from azure.core.pipeline.transport import AsyncHttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
+from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
-from .. import models as _models
-from .._serialization import Serializer
-from .._vendor import _convert_request
+from ... import models as _models
+from ..._vendor import _convert_request
+from ...operations._problem_classifications_operations import build_get_request, build_list_request
 
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
-_SERIALIZER = Serializer()
-_SERIALIZER.client_side_validation = False
 
-
-def build_post_request(**kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
-    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = kwargs.pop("template_url", "/providers/Microsoft.Support/lookUpResourceId")
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    if content_type is not None:
-        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-class LookUpResourceIdOperations:
+class ProblemClassificationsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.support.MicrosoftSupport`'s
-        :attr:`look_up_resource_id` attribute.
+        :class:`~azure.mgmt.support.aio.MicrosoftSupport`'s
+        :attr:`problem_classifications` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
-    @overload
-    def post(
-        self,
-        look_up_resource_id_request: _models.LookUpResourceIdRequest,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any
-    ) -> _models.LookUpResourceIdResponse:
-        """This operation fetches ARM resource id of support resource type.
-
-        This operation fetches ARM resource id of support resource type.
-
-        :param look_up_resource_id_request: Look up resource id request body. Required.
-        :type look_up_resource_id_request: ~azure.mgmt.support.models.LookUpResourceIdRequest
-        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :return: LookUpResourceIdResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.support.models.LookUpResourceIdResponse
+    @distributed_trace
+    def list(self, service_name: str, **kwargs: Any) -> AsyncIterable["_models.ProblemClassification"]:
+        """Lists all the problem classifications (categories) available for a specific Azure service.
+        Always use the service and problem classifications obtained programmatically. This practice
+        ensures that you always have the most recent set of service and problem classification Ids.
+
+        :param service_name: Name of the Azure service for which the problem classifications need to be
+         retrieved. Required.
+        :type service_name: str
+        :return: An iterator like instance of either ProblemClassification or the result of
+         cls(response)
+        :rtype:
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.support.models.ProblemClassification]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    @overload
-    def post(
-        self, look_up_resource_id_request: IO[bytes], *, content_type: str = "application/json", **kwargs: Any
-    ) -> _models.LookUpResourceIdResponse:
-        """This operation fetches ARM resource id of support resource type.
-
-        This operation fetches ARM resource id of support resource type.
-
-        :param look_up_resource_id_request: Look up resource id request body. Required.
-        :type look_up_resource_id_request: IO[bytes]
-        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :return: LookUpResourceIdResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.support.models.LookUpResourceIdResponse
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        cls: ClsType[_models.ProblemClassificationsListResult] = kwargs.pop("cls", None)
 
-    @distributed_trace
-    def post(
-        self, look_up_resource_id_request: Union[_models.LookUpResourceIdRequest, IO[bytes]], **kwargs: Any
-    ) -> _models.LookUpResourceIdResponse:
-        """This operation fetches ARM resource id of support resource type.
-
-        This operation fetches ARM resource id of support resource type.
-
-        :param look_up_resource_id_request: Look up resource id request body. Is either a
-         LookUpResourceIdRequest type or a IO[bytes] type. Required.
-        :type look_up_resource_id_request: ~azure.mgmt.support.models.LookUpResourceIdRequest or
-         IO[bytes]
-        :return: LookUpResourceIdResponse or the result of cls(response)
-        :rtype: ~azure.mgmt.support.models.LookUpResourceIdResponse
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        def prepare_request(next_link=None):
+            if not next_link:
+
+                _request = build_list_request(
+                    service_name=service_name,
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
+        async def extract_data(pipeline_response):
+            deserialized = self._deserialize("ProblemClassificationsListResult", pipeline_response)
+            list_of_elem = deserialized.value
+            if cls:
+                list_of_elem = cls(list_of_elem)  # type: ignore
+            return None, AsyncList(list_of_elem)
+
+        async def get_next(next_link=None):
+            _request = prepare_request(next_link)
+
+            _stream = False
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+            response = pipeline_response.http_response
+
+            if response.status_code not in [200]:
+                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+                raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+            return pipeline_response
+
+        return AsyncItemPaged(get_next, extract_data)
+
+    @distributed_trace_async
+    async def get(
+        self, service_name: str, problem_classification_name: str, **kwargs: Any
+    ) -> _models.ProblemClassification:
+        """Get problem classification details for a specific Azure service.
+
+        :param service_name: Name of the Azure service available for support. Required.
+        :type service_name: str
+        :param problem_classification_name: Name of problem classification. Required.
+        :type problem_classification_name: str
+        :return: ProblemClassification or the result of cls(response)
+        :rtype: ~azure.mgmt.support.models.ProblemClassification
         :raises ~azure.core.exceptions.HttpResponseError:
         """
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
-        cls: ClsType[_models.LookUpResourceIdResponse] = kwargs.pop("cls", None)
-
-        content_type = content_type or "application/json"
-        _json = None
-        _content = None
-        if isinstance(look_up_resource_id_request, (IOBase, bytes)):
-            _content = look_up_resource_id_request
-        else:
-            _json = self._serialize.body(look_up_resource_id_request, "LookUpResourceIdRequest")
+        cls: ClsType[_models.ProblemClassification] = kwargs.pop("cls", None)
 
-        _request = build_post_request(
+        _request = build_get_request(
+            service_name=service_name,
+            problem_classification_name=problem_classification_name,
             api_version=api_version,
-            content_type=content_type,
-            json=_json,
-            content=_content,
             headers=_headers,
             params=_params,
         )
         _request = _convert_request(_request)
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
-        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize("LookUpResourceIdResponse", pipeline_response)
+        deserialized = self._deserialize("ProblemClassification", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
```

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_services_operations.py`

 * *Files 22% similar despite different names*

```diff
@@ -36,61 +36,91 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
-    _url = kwargs.pop("template_url", "/providers/Microsoft.Support/operations")
+    _url = kwargs.pop("template_url", "/providers/Microsoft.Support/services")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class Operations:
+def build_get_request(service_name: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop("template_url", "/providers/Microsoft.Support/services/{serviceName}")
+    path_format_arguments = {
+        "serviceName": _SERIALIZER.url("service_name", service_name, "str"),
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
+class ServicesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.support.MicrosoftSupport`'s
-        :attr:`operations` attribute.
+        :attr:`services` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(self, **kwargs: Any) -> Iterable["_models.Operation"]:
-        """This lists all the available Microsoft Support REST API operations.
+    def list(self, **kwargs: Any) -> Iterable["_models.Service"]:
+        """Lists all the Azure services available for support ticket creation. For **Technical** issues,
+        select the Service Id that maps to the Azure service/product as displayed in the **Services**
+        drop-down list on the Azure portal's `New support request
+        <https://portal.azure.com/#blade/Microsoft_Azure_Support/HelpAndSupportBlade/overview>`_ page.
+        Always use the service and its corresponding problem classification(s) obtained
+        programmatically for support ticket creation. This practice ensures that you always have the
+        most recent set of service and problem classification Ids.
 
-        :return: An iterator like instance of either Operation or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.support.models.Operation]
+        :return: An iterator like instance of either Service or the result of cls(response)
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.support.models.Service]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.OperationsListResult] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ServicesListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
@@ -122,15 +152,15 @@
                 )
                 _request = _convert_request(_request)
                 _request.url = self._client.format_url(_request.url)
                 _request.method = "GET"
             return _request
 
         def extract_data(pipeline_response):
-            deserialized = self._deserialize("OperationsListResult", pipeline_response)
+            deserialized = self._deserialize("ServicesListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, iter(list_of_elem)
 
         def get_next(next_link=None):
             _request = prepare_request(next_link)
@@ -145,7 +175,59 @@
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
+
+    @distributed_trace
+    def get(self, service_name: str, **kwargs: Any) -> _models.Service:
+        """Gets a specific Azure service for support ticket creation.
+
+        :param service_name: Name of the Azure service. Required.
+        :type service_name: str
+        :return: Service or the result of cls(response)
+        :rtype: ~azure.mgmt.support.models.Service
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
+        cls: ClsType[_models.Service] = kwargs.pop("cls", None)
+
+        _request = build_get_request(
+            service_name=service_name,
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
+        deserialized = self._deserialize("Service", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})  # type: ignore
+
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_patch.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_support_tickets_no_subscription_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_support_tickets_no_subscription_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_check_name_availability_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.Support/checkNameAvailability")
 
     # Construct parameters
@@ -61,15 +61,15 @@
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_request(*, top: Optional[int] = None, filter: Optional[str] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.Support/supportTickets")
 
     # Construct parameters
     if top is not None:
@@ -84,15 +84,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(support_ticket_name: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.Support/supportTickets/{supportTicketName}")
     path_format_arguments = {
         "supportTicketName": _SERIALIZER.url("support_ticket_name", support_ticket_name, "str"),
     }
@@ -108,15 +108,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_update_request(support_ticket_name: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.Support/supportTickets/{supportTicketName}")
     path_format_arguments = {
         "supportTicketName": _SERIALIZER.url("support_ticket_name", support_ticket_name, "str"),
@@ -135,15 +135,15 @@
     return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_create_request(support_ticket_name: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.Support/supportTickets/{supportTicketName}")
     path_format_arguments = {
         "supportTicketName": _SERIALIZER.url("support_ticket_name", support_ticket_name, "str"),
```

### Comparing `azure-mgmt-support-6.1.0b3/azure/mgmt/support/operations/_support_tickets_operations.py` & `azure-mgmt-support-7.0.0/azure/mgmt/support/operations/_support_tickets_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_check_name_availability_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.Support/checkNameAvailability"
     )
@@ -70,15 +70,15 @@
 
 def build_list_request(
     subscription_id: str, *, top: Optional[int] = None, filter: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.Support/supportTickets")
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
@@ -98,15 +98,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(support_ticket_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.Support/supportTickets/{supportTicketName}"
     )  # pylint: disable=line-too-long
     path_format_arguments = {
@@ -125,15 +125,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_update_request(support_ticket_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.Support/supportTickets/{supportTicketName}"
     )  # pylint: disable=line-too-long
@@ -155,15 +155,15 @@
     return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_create_request(support_ticket_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-06-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-04-01"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.Support/supportTickets/{supportTicketName}"
     )  # pylint: disable=line-too-long
```

### Comparing `azure-mgmt-support-6.1.0b3/azure_mgmt_support.egg-info/PKG-INFO` & `azure-mgmt-support-7.0.0/azure_mgmt_support.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-support
-Version: 6.1.0b3
+Version: 7.0.0
 Summary: Microsoft Azure Support Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: isodate>=0.6.1
-Requires-Dist: azure-common>=1.1
-Requires-Dist: azure-mgmt-core>=1.3.2
 
 # Microsoft Azure SDK for Python
 
 This is the Microsoft Azure Support Management Client Library.
 This package has been tested with Python 3.8+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
@@ -85,14 +82,48 @@
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 # Release History
 
+## 7.0.0 (2024-04-22)
+
+### Features Added
+
+  - Added operation group ChatTranscriptsNoSubscriptionOperations
+  - Added operation group ChatTranscriptsOperations
+  - Added operation group CommunicationsNoSubscriptionOperations
+  - Added operation group FileWorkspacesNoSubscriptionOperations
+  - Added operation group FileWorkspacesOperations
+  - Added operation group FilesNoSubscriptionOperations
+  - Added operation group FilesOperations
+  - Added operation group SupportTicketsNoSubscriptionOperations
+  - Model ProblemClassification has a new parameter secondary_consent_enabled
+  - Model SupportTicketDetails has a new parameter file_workspace_name
+  - Model SupportTicketDetails has a new parameter is_temporary_ticket
+  - Model SupportTicketDetails has a new parameter problem_scoping_questions
+  - Model SupportTicketDetails has a new parameter secondary_consent
+  - Model SupportTicketDetails has a new parameter support_plan_display_name
+  - Model SupportTicketDetails has a new parameter support_plan_id
+  - Model UpdateSupportTicket has a new parameter advanced_diagnostic_consent
+  - Model UpdateSupportTicket has a new parameter secondary_consent
+
+### Breaking Changes
+
+  - Model SupportTicketDetails has a new required parameter advanced_diagnostic_consent
+  - Parameter body of model CommunicationDetails is now required
+  - Parameter contact_details of model SupportTicketDetails is now required
+  - Parameter description of model SupportTicketDetails is now required
+  - Parameter problem_classification_id of model SupportTicketDetails is now required
+  - Parameter service_id of model SupportTicketDetails is now required
+  - Parameter severity of model SupportTicketDetails is now required
+  - Parameter subject of model CommunicationDetails is now required
+  - Parameter title of model SupportTicketDetails is now required
+
 ## 6.1.0b3 (2024-03-18)
 
 ### Features Added
 
   - Added operation ChatTranscriptsNoSubscriptionOperations.list
   - Added operation CommunicationsNoSubscriptionOperations.list
   - Added operation ProblemClassificationsOperations.classify_problems
```

### Comparing `azure-mgmt-support-6.1.0b3/azure_mgmt_support.egg-info/SOURCES.txt` & `azure-mgmt-support-7.0.0/azure_mgmt_support.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -23,21 +23,17 @@
 azure/mgmt/support/aio/operations/_chat_transcripts_operations.py
 azure/mgmt/support/aio/operations/_communications_no_subscription_operations.py
 azure/mgmt/support/aio/operations/_communications_operations.py
 azure/mgmt/support/aio/operations/_file_workspaces_no_subscription_operations.py
 azure/mgmt/support/aio/operations/_file_workspaces_operations.py
 azure/mgmt/support/aio/operations/_files_no_subscription_operations.py
 azure/mgmt/support/aio/operations/_files_operations.py
-azure/mgmt/support/aio/operations/_look_up_resource_id_operations.py
 azure/mgmt/support/aio/operations/_operations.py
 azure/mgmt/support/aio/operations/_patch.py
-azure/mgmt/support/aio/operations/_problem_classifications_no_subscription_operations.py
 azure/mgmt/support/aio/operations/_problem_classifications_operations.py
-azure/mgmt/support/aio/operations/_service_classifications_no_subscription_operations.py
-azure/mgmt/support/aio/operations/_service_classifications_operations.py
 azure/mgmt/support/aio/operations/_services_operations.py
 azure/mgmt/support/aio/operations/_support_tickets_no_subscription_operations.py
 azure/mgmt/support/aio/operations/_support_tickets_operations.py
 azure/mgmt/support/models/__init__.py
 azure/mgmt/support/models/_microsoft_support_enums.py
 azure/mgmt/support/models/_models_py3.py
 azure/mgmt/support/models/_patch.py
@@ -46,21 +42,17 @@
 azure/mgmt/support/operations/_chat_transcripts_operations.py
 azure/mgmt/support/operations/_communications_no_subscription_operations.py
 azure/mgmt/support/operations/_communications_operations.py
 azure/mgmt/support/operations/_file_workspaces_no_subscription_operations.py
 azure/mgmt/support/operations/_file_workspaces_operations.py
 azure/mgmt/support/operations/_files_no_subscription_operations.py
 azure/mgmt/support/operations/_files_operations.py
-azure/mgmt/support/operations/_look_up_resource_id_operations.py
 azure/mgmt/support/operations/_operations.py
 azure/mgmt/support/operations/_patch.py
-azure/mgmt/support/operations/_problem_classifications_no_subscription_operations.py
 azure/mgmt/support/operations/_problem_classifications_operations.py
-azure/mgmt/support/operations/_service_classifications_no_subscription_operations.py
-azure/mgmt/support/operations/_service_classifications_operations.py
 azure/mgmt/support/operations/_services_operations.py
 azure/mgmt/support/operations/_support_tickets_no_subscription_operations.py
 azure/mgmt/support/operations/_support_tickets_operations.py
 azure_mgmt_support.egg-info/PKG-INFO
 azure_mgmt_support.egg-info/SOURCES.txt
 azure_mgmt_support.egg-info/dependency_links.txt
 azure_mgmt_support.egg-info/not-zip-safe
```

### Comparing `azure-mgmt-support-6.1.0b3/setup.py` & `azure-mgmt-support-7.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     long_description_content_type="text/markdown",
     license="MIT License",
     author="Microsoft Corporation",
     author_email="azpysdkhelp@microsoft.com",
     url="https://github.com/Azure/azure-sdk-for-python",
     keywords="azure, azure sdk",  # update with search keywords relevant to the azure service / product
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
```

### Comparing `azure-mgmt-support-6.1.0b3/tests/disable_test_cli_mgmt_support.py` & `azure-mgmt-support-7.0.0/tests/disable_test_cli_mgmt_support.py`

 * *Files identical despite different names*

