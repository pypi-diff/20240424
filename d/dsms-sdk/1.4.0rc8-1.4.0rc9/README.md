# Comparing `tmp/dsms_sdk-1.4.0rc8.tar.gz` & `tmp/dsms_sdk-1.4.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsms_sdk-1.4.0rc8.tar", last modified: Tue Apr 23 00:32:22 2024, max compression
+gzip compressed data, was "dsms_sdk-1.4.0rc9.tar", last modified: Tue Apr 23 21:05:02 2024, max compression
```

## Comparing `dsms_sdk-1.4.0rc8.tar` & `dsms_sdk-1.4.0rc9.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.572747 dsms_sdk-1.4.0rc8/
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-23 00:32:22.572747 dsms_sdk-1.4.0rc8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.560747 dsms_sdk-1.4.0rc8/dsms/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.560747 dsms_sdk-1.4.0rc8/dsms/apps/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/apps/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/apps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.560747 dsms_sdk-1.4.0rc8/dsms/core/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/core/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/core/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/core/dsms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.564747 dsms_sdk-1.4.0rc8/dsms/knowledge/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    16768 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/kitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/ktype.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.564747 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/affiliations.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/authors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/contacts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.564747 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/custom_datatype/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/custom_datatype/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/custom_datatype/numerical.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/external_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/linked_kitems.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/properties/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.564747 dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.564747 dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/queries/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/queries/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.568747 dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/units/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/units/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/units/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/units/sparql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/units/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.568747 dsms_sdk-1.4.0rc8/dsms/knowledge/sparql_interface/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/sparql_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/sparql_interface/sparql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/sparql_interface/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/sparql_interface/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17151 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/dsms/knowledge/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.568747 dsms_sdk-1.4.0rc8/dsms_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-23 00:32:22.000000 dsms_sdk-1.4.0rc8/dsms_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-23 00:32:22.000000 dsms_sdk-1.4.0rc8/dsms_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 00:32:22.000000 dsms_sdk-1.4.0rc8/dsms_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 00:32:22.000000 dsms_sdk-1.4.0rc8/dsms_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-23 00:32:22.000000 dsms_sdk-1.4.0rc8/dsms_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 00:32:22.000000 dsms_sdk-1.4.0rc8/dsms_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-23 00:32:22.572747 dsms_sdk-1.4.0rc8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:22.568747 dsms_sdk-1.4.0rc8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6432 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/tests/test_kitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-23 00:32:19.000000 dsms_sdk-1.4.0rc8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:05:02.740387 dsms_sdk-1.4.0rc9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-23 21:05:02.740387 dsms_sdk-1.4.0rc9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:05:02.728387 dsms_sdk-1.4.0rc9/dsms/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:05:02.728387 dsms_sdk-1.4.0rc9/dsms/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/apps/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/apps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:05:02.732387 dsms_sdk-1.4.0rc9/dsms/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/core/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/core/dsms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:05:02.732387 dsms_sdk-1.4.0rc9/dsms/knowledge/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18887 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/kitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/ktype.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:05:02.736387 dsms_sdk-1.4.0rc9/dsms/knowledge/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/properties/affiliations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/properties/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/properties/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/properties/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/properties/authors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/properties/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/properties/contacts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:05:02.736387 dsms_sdk-1.4.0rc9/dsms/knowledge/properties/custom_datatype/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/properties/custom_datatype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/properties/custom_datatype/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/properties/external_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/properties/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/properties/linked_kitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/properties/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/properties/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/properties/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:05:02.736387 dsms_sdk-1.4.0rc9/dsms/knowledge/semantics/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/semantics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:05:02.736387 dsms_sdk-1.4.0rc9/dsms/knowledge/semantics/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/semantics/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/semantics/queries/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:05:02.736387 dsms_sdk-1.4.0rc9/dsms/knowledge/semantics/units/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/semantics/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/semantics/units/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/semantics/units/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/semantics/units/sparql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/semantics/units/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:05:02.736387 dsms_sdk-1.4.0rc9/dsms/knowledge/sparql_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/sparql_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/sparql_interface/sparql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/sparql_interface/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/sparql_interface/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17206 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/dsms/knowledge/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:05:02.740387 dsms_sdk-1.4.0rc9/dsms_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-23 21:05:02.000000 dsms_sdk-1.4.0rc9/dsms_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-23 21:05:02.000000 dsms_sdk-1.4.0rc9/dsms_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 21:05:02.000000 dsms_sdk-1.4.0rc9/dsms_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 21:05:02.000000 dsms_sdk-1.4.0rc9/dsms_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-23 21:05:02.000000 dsms_sdk-1.4.0rc9/dsms_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 21:05:02.000000 dsms_sdk-1.4.0rc9/dsms_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-23 21:05:02.740387 dsms_sdk-1.4.0rc9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:05:02.740387 dsms_sdk-1.4.0rc9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6432 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/tests/test_kitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-23 21:04:59.000000 dsms_sdk-1.4.0rc9/tests/test_utils.py
```

### Comparing `dsms_sdk-1.4.0rc8/LICENSE` & `dsms_sdk-1.4.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc8/PKG-INFO` & `dsms_sdk-1.4.0rc9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsms_sdk
-Version: 1.4.0rc8
+Version: 1.4.0rc9
 Summary: Python SDK core-package for working with the Dataspace Management System (DSMS).
 Home-page: https://github.com/MI-FraunhoferIWM/dsms-python-sdk
 Author: Matthias Büschelberger, Yoav Nahshon, Pablo De Andres
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `dsms_sdk-1.4.0rc8/README.md` & `dsms_sdk-1.4.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc8/dsms/apps/apps.py` & `dsms_sdk-1.4.0rc9/dsms/apps/apps.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc8/dsms/apps/utils.py` & `dsms_sdk-1.4.0rc9/dsms/apps/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc8/dsms/core/configuration.py` & `dsms_sdk-1.4.0rc9/dsms/core/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 """General config for the DSMS Python SDK"""
 
 import urllib
 import warnings
-from typing import TYPE_CHECKING, Optional
+from typing import Callable, List, Optional, Set, Union
 
 import requests
 from pydantic import AnyUrl, Field, SecretStr, field_validator
 from pydantic_core.core_schema import ValidationInfo
 from pydantic_settings import BaseSettings, SettingsConfigDict
 
 from .utils import get_callable
 
-if TYPE_CHECKING:
-    from typing import Callable
-
 MODULE_REGEX = r"^[a-zA-Z_][a-zA-Z0-9_]*(\.[a-zA-Z_][a-zA-Z0-9_]*)*:[a-zA-Z_][a-zA-Z0-9_]*$"
 DEFAULT_UNIT_SPARQL = "dsms.knowledge.semantics.units.sparql:UnitSparqlQuery"
 DEFAULT_REPO = "knowledge-items"
 
 
 class Configuration(BaseSettings):
     """General config for DSMS-SDK"""
@@ -102,19 +99,40 @@
         DEFAULT_UNIT_SPARQL,
         pattern=MODULE_REGEX,
         description="""Class and Module specification in Python for a subclass of
           `dsms.knowledge.semantics.units.base:BaseUnitSparqlQuery` in order to retrieve
           the units of a HDF5 column/ custom property of a KItem.""",
     )
 
+    filter_bad_hdf5_types: Optional[List[Callable]] = Field(
+        [str, type(None)],
+        description="""A list of classes which should be filtered out
+        from a column of an hdf5 when fetched""",
+    )
+
+    hide_properties: Set[Union[str, None]] = Field(
+        set(),
+        description="Properties to hide while printing, e.g {'external_links'}",
+    )
+
     @field_validator("units_sparql_object")
     def get_unit_sparql_object(cls, val: str) -> "Callable":
         """Source the class from the given module"""
         return get_callable(val)
 
+    @field_validator("hide_properties")
+    def validate_hide_properties(cls, val: Set) -> "Callable":
+        """Source the class from the given module"""
+        from dsms import KItem
+
+        for key in val:
+            if key not in KItem.model_fields:
+                raise KeyError(f"Property `{key}` not in KItem schema")
+        return val
+
     @field_validator("token")
     def validate_auth(cls, val, info: ValidationInfo):
         """Validate the provided authentication/authorization secrets."""
         username = info.data.get("username")
         passwd = info.data.get("password")
         host_url = info.data.get("host_url")
         timeout = info.data.get("request_timeout")
```

### Comparing `dsms_sdk-1.4.0rc8/dsms/core/context.py` & `dsms_sdk-1.4.0rc9/dsms/core/context.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc8/dsms/core/dsms.py` & `dsms_sdk-1.4.0rc9/dsms/core/dsms.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc8/dsms/core/utils.py` & `dsms_sdk-1.4.0rc9/dsms/core/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/cli.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/cli.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/kitem.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/kitem.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 from dsms.knowledge.ktype import KType  # isort:skip
 
 from dsms.knowledge.utils import (  # isort:skip
     _kitem_exists,
     _slug_is_available,
     _slugify,
     _inspect_hdf5,
-    _get_ktype_from_id,
+    _make_annotation_schema,
 )
 
 from dsms.knowledge.sparql_interface.utils import _get_subgraph  # isort:skip
 
 if TYPE_CHECKING:
     from dsms import Context
     from dsms.core.dsms import DSMS
@@ -109,14 +109,18 @@
     # public
     name: str = Field(..., description="Human readable name of the KItem")
     id: Optional[UUID] = Field(
         default_factory=uuid4,
         description="ID of the KItem",
     )
     ktype_id: Union[Enum, str] = Field(..., description="Type ID of the KItem")
+    in_backend: bool = Field(
+        False,
+        description="Whether the KItem was already created in the backend.",
+    )
     slug: Optional[str] = Field(
         None, description="Slug of the KContext.dsms", min_length=4
     )
     annotations: List[Annotation] = Field(
         [], description="Annotations of the KItem"
     )
     attachments: List[Union[Attachment, str]] = Field(
@@ -166,14 +170,18 @@
         None, description="KType of the KItem", exclude=True
     )
 
     hdf5: Optional[
         Union[List[Column], pd.DataFrame, Dict[str, Union[List, Dict]]]
     ] = Field(None, description="HDF5 interface.")
 
+    rdf_exists: bool = Field(
+        False, description="Whether the KItem holds an RDF Graph or not."
+    )
+
     model_config = ConfigDict(
         extra="forbid",
         validate_assignment=True,
         validate_default=True,
         exclude={"ktype"},
         arbitrary_types_allowed=True,
     )
@@ -186,18 +194,15 @@
         if not self.dsms:
             self.dsms = DSMS()
 
         # initialize the kitem
         super().__init__(**kwargs)
 
         # add kitem to buffer
-        if (
-            _slug_is_available(self._get_ktype_as_str(), self.slug)
-            and self.id not in self.context.buffers.created
-        ):
+        if not self.in_backend and self.id not in self.context.buffers.created:
             self.context.buffers.created.update({self.id: self})
             self.context.buffers.updated.update({self.id: self})
 
         self._set_kitem_for_properties()
 
     def __setattr__(self, name, value) -> None:
         """Add kitem to updated-buffer if an attribute is set"""
@@ -212,37 +217,66 @@
 
     def __str__(self) -> str:
         """Pretty print the kitem fields"""
         fields = ", \n".join(
             [
                 f"\n\t{key} = {value}"
                 for key, value in self.__dict__.items()
-                if key not in self.model_config["exclude"]
+                if (
+                    key not in self.model_config["exclude"]
+                    and key not in self.dsms.config.hide_properties
+                )
             ]
         )
         return f"{self.__class__.__name__}(\n{fields}\n)"
 
     def __repr__(self) -> str:
         """Pretty print the kitem Fields"""
         return str(self)
 
     def __hash__(self) -> int:
         return hash(str(self))
 
+    @field_validator("affiliations", mode="before")
+    @classmethod
+    def validate_affiliations_before(
+        cls, value: List[Union[str, Affiliation]]
+    ) -> List[Affiliation]:
+        """Validate affiliations Field"""
+        return [
+            Affiliation(name=affiliation)
+            if isinstance(affiliation, str)
+            else affiliation
+            for affiliation in value
+        ]
+
     @field_validator("affiliations", mode="after")
     @classmethod
-    def validate_affiliation(
+    def validate_affiliation_after(
         cls, value: List[Affiliation]
     ) -> AffiliationsProperty:
         """Validate affiliations Field"""
         return AffiliationsProperty(value)
 
+    @field_validator("annotations", mode="before")
+    @classmethod
+    def validate_annotations_before(
+        cls, value: List[Union[str, Annotation]]
+    ) -> List[Annotation]:
+        """Validate annotations Field"""
+        return [
+            Annotation(**_make_annotation_schema(annotation))
+            if isinstance(annotation, str)
+            else annotation
+            for annotation in value
+        ]
+
     @field_validator("annotations", mode="after")
     @classmethod
-    def validate_annotations(
+    def validate_annotations_after(
         cls, value: List[Annotation]
     ) -> AnnotationsProperty:
         """Validate annotations Field"""
         return AnnotationsProperty(value)
 
     @field_validator("attachments", mode="before")
     @classmethod
@@ -361,41 +395,63 @@
             )
         return value
 
     @field_validator("ktype")
     @classmethod
     def validate_ktype(cls, value: KType, info: ValidationInfo) -> KType:
         """Validate the data attribute of the KItem"""
+        from dsms import Context
 
         if not value:
             ktype_id = info.data.get("ktype_id")
-            value = _get_ktype_from_id(ktype_id)
+            if not isinstance(ktype_id, str):
+                value = Context.ktypes.get(ktype_id.value)
+            else:
+                value = Context.ktypes.get(ktype_id)
+
+            if not value:
+                raise TypeError(
+                    f"KType for `ktype_id={ktype_id}` does not exist."
+                )
+        return value
 
+    @field_validator("in_backend")
+    @classmethod
+    def validate_in_backend(cls, value: bool, info: ValidationInfo) -> bool:
+        """Checks whether the kitem already exists"""
+        kitem_id = info.data["id"]
+        if _kitem_exists(kitem_id):
+            value = True
         return value
 
     @field_validator("slug")
     @classmethod
     def validate_slug(cls, value: str, info: ValidationInfo) -> str:
         """Validate slug"""
         from dsms import Context
 
         ktype_id = info.data["ktype_id"]
-        name = info.data.get("name")
         kitem_id = info.data.get("id")
+        kitem_exists = info.data.get("in_backend")
+
+        if not isinstance(ktype_id, str):
+            ktype = ktype_id.value
+        else:
+            ktype = ktype_id
+        name = info.data.get("name")
+
         if not value:
             value = _slugify(name)
             if len(value) < 4:
                 raise ValueError(
                     "Slug length must have a minimum length of 4."
                 )
             if Context.dsms.config.individual_slugs:
                 value += f"-{str(kitem_id).split('-', maxsplit=1)[0]}"
-        if not _kitem_exists(kitem_id) and not _slug_is_available(
-            ktype_id.value, value
-        ):
+        if not kitem_exists and not _slug_is_available(ktype, value):
             raise ValueError(f"Slug for `{value}` is already taken.")
         return value
 
     @field_validator("summary")
     @classmethod
     def validate_summary(cls, value: Union[str, Summary]) -> Summary:
         """Check whether the summary is a string or the dedicated model"""
@@ -450,15 +506,20 @@
             if isinstance(content, str):
                 try:
                     content = json.loads(content)
                 except Exception as error:
                     raise TypeError(
                         f"Invalid type: {type(content)}"
                     ) from error
+            was_in_buffer = self.id in self.context.buffers.updated
             self.custom_properties = self.ktype.webform(**content)
+            # fix: find a better way to prehebit that properties are
+            # set in the buffer
+            if not was_in_buffer:
+                self.context.buffers.updated.pop(self.id)
         # set kitem id for custom properties
         if isinstance(self.custom_properties, BaseModel):
             self.custom_properties.kitem = self
         return self
 
     def _set_kitem_for_properties(self) -> None:
         """Set kitem for CustomProperties and KProperties in order to
```

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/ktype.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/ktype.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/properties/__init__.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/properties/affiliations.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/properties/affiliations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Affiliation KProperty"""
 
 from typing import TYPE_CHECKING
 
 from pydantic import Field
 
 from dsms.knowledge.properties.base import KProperty, KPropertyItem
+from dsms.knowledge.properties.utils import _str_to_dict
 
 if TYPE_CHECKING:
     from typing import Callable
 
 
 class Affiliation(KPropertyItem):
     """Affiliation of a KItem."""
@@ -19,7 +20,12 @@
 class AffiliationsProperty(KProperty):
     """Affiliations property"""
 
     # OVERRIDE
     @property
     def k_property_item(cls) -> "Callable":
         return Affiliation
+
+    @property
+    def k_property_helper(cls) -> "Callable":
+        """Affiliation property helper"""
+        return _str_to_dict
```

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/properties/annotations.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/properties/annotations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Annotations KProperty"""
 
 from typing import TYPE_CHECKING
 
 from pydantic import Field
 
 from dsms.knowledge.properties.base import KProperty, KPropertyItem
+from dsms.knowledge.utils import _make_annotation_schema
 
 if TYPE_CHECKING:
-    from typing import Callable
+    from typing import Any, Callable, Dict
 
 
 class Annotation(KPropertyItem):
     """KItem annotation model"""
 
     iri: str = Field(..., description="IRI of the annotation")
     name: str = Field(..., description="Name of the annotation")
@@ -22,7 +23,17 @@
     """KProperty for annotations"""
 
     # OVERRIDE
     @property
     def k_property_item(cls) -> "Callable":
         """Annotation data model"""
         return Annotation
+
+    @property
+    def k_property_helper(cls) -> None:
+        """Not defined for Affiliations"""
+        return _make_annotation_schema
+
+    @property
+    def by_iri(cls) -> "Dict[str, Any]":
+        """Return dict of annotations per IRI"""
+        return {annotation.iri for annotation in cls}
```

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/properties/apps.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/properties/apps.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,7 +63,11 @@
     """KProperty for apps"""
 
     # OVERRIDE
     @property
     def k_property_item(cls) -> "Callable":
         """App data model"""
         return App
+
+    @property
+    def k_property_helper(cls) -> None:
+        """Not defined for Apps"""
```

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/properties/attachments.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/properties/attachments.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 from pydantic import Field
 
 from dsms.knowledge.properties.base import KProperty, KPropertyItem
+from dsms.knowledge.properties.utils import _str_to_dict
 from dsms.knowledge.utils import _get_attachment
 
 if TYPE_CHECKING:
     from typing import Any, Callable, Dict, Iterable, List, Union
 
 
 class Attachment(KPropertyItem):
@@ -26,14 +27,20 @@
     """KProperty for managing attachments."""
 
     # OVERRIDE
     @property
     def k_property_item(cls) -> "Callable":
         return Attachment
 
+    # OVERRIDE
+    @property
+    def k_property_helper(cls) -> "Callable":
+        """Helper for constructing attachment property"""
+        return _str_to_dict
+
     def extend(self, iterable: "Iterable") -> None:
         """Extend KProperty with list of KPropertyItem"""
         from dsms import KItem
 
         to_extend = []
         for item in iterable:
             if isinstance(item, (list, tuple)):
```

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/properties/authors.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/properties/authors.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,7 +21,12 @@
     """KProperty for authors"""
 
     # OVERRIDE
     @property
     def k_property_item(cls) -> "Callable":
         """Author data model"""
         return Author
+
+    # OVERRIDE
+    @property
+    def k_property_helper(cls) -> None:
+        """Not defined for Authors"""
```

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/properties/base.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/properties/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,19 +47,23 @@
         )
         return f"{{\n\t\t\t{values}\n\t\t}}"
 
     def __repr__(self) -> str:
         """Pretty print the KProperty"""
         return str(self)
 
-    def __setattr__(self, index: int, item: "Any") -> None:
+    def __setattr__(self, key: str, item: "Any") -> None:
         """Add KItem to updated buffer."""
-        if self.kitem and self.kitem.id not in self.context.buffers.updated:
+        if (
+            self.kitem
+            and self.kitem.id not in self.context.buffers.updated
+            and key not in ["_kitem", "kitem", "id"]
+        ):
             self.context.buffers.updated.update({self.id: self.kitem})
-        super().__setattr__(index, item)
+        super().__setattr__(key, item)
 
     def __hash__(self) -> int:
         return hash(str(self))
 
     @property
     def kitem(cls) -> "KItem":
         """KItem related to the KPropertyItem"""
@@ -94,21 +98,28 @@
 
 
 class KProperty(list):
     """Basic class for an KItem-property."""
 
     def __init__(self, *args) -> None:
         self._kitem: "KItem" = None
-        self.extend(args)
+        to_extend = self._get_extendables(args)
+        self.extend(to_extend)
 
     @property
     @abstractmethod
     def k_property_item(cls) -> "Callable":
         """Return the KPropertyItem-class for the KProperty"""
 
+    @property
+    @abstractmethod
+    def k_property_helper(cls) -> "Optional[Callable]":
+        """Optional helper for transforming a given
+        input into the k property item"""
+
     def __str__(self) -> str:
         """Pretty print the KProperty"""
         values = ", \n".join(["\t\t" + repr(value) for value in self])
         if values:
             values = f"\n{values}\n\t"
         return f"[{values}]"
 
@@ -135,16 +146,15 @@
         super().__delitem__(index)
 
     def __imul__(self, index: int) -> None:
         """Imul the KPropertyItem"""
         self._mark_as_updated()
         super().__imul__(index)
 
-    def extend(self, iterable: "Iterable") -> None:
-        """Extend KProperty with list of KPropertyItem"""
+    def _get_extendables(self, iterable: "Iterable") -> "List[KPropertyItem]":
         from dsms import KItem
 
         to_extend = []
         for item in iterable:
             if isinstance(item, (list, tuple)):
                 for subitem in item:
                     item = self._check_item(subitem)
@@ -153,14 +163,20 @@
             elif isinstance(item, (dict, KPropertyItem, KItem)):
                 item = self._check_item(item)
                 if not item in self:
                     to_extend.append(item)
             else:
                 if not item in self:
                     to_extend.append(item)
+        return to_extend
+
+    def extend(self, iterable: "Iterable") -> None:
+        """Extend KProperty with list of KPropertyItem"""
+        to_extend = self._get_extendables(iterable)
+
         if to_extend:
             self._mark_as_updated()
             super().extend(to_extend)
 
     def append(self, item: "Union[Dict, Any]") -> None:
         """Append KPropertyItem to KProperty"""
 
@@ -197,22 +213,23 @@
             item.kitem = self.kitem
         return item
 
     def _check_k_property_item(
         self, item: "Union[Dict, Any]"
     ) -> KPropertyItem:
         """Check the type of the processsed KPropertyItem"""
-        from dsms import KItem
-
-        if not isinstance(item, (self.k_property_item, dict, KItem, str)):
-            raise TypeError(
-                f"""Item `{item}` must be of type {self.k_property_item}, {KItem}, {str} or {dict},
-                not `{type(item)}`."""
-            )
-        if isinstance(item, dict):
+        if not isinstance(item, BaseModel):
+            if self.k_property_helper and not isinstance(item, dict):
+                item = self.k_property_helper(item)
+            elif not self.k_property_helper and not isinstance(item, dict):
+                raise TypeError(
+                    f"""No `k_propertyhelper` defined for {type(self)}.
+                    Hence, item `{item}` must be of type {self.k_property_item},
+                    {BaseModel} or {dict}, not `{type(item)}`."""
+                )
             item = self.k_property_item(**item)
         return item
 
     def _mark_as_updated(self) -> None:
         """Add KItem of KProperty to updated buffer"""
         if self._kitem and self._kitem.id not in self.context.buffers.updated:
             self.context.buffers.updated.update({self._kitem.id: self._kitem})
```

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/properties/contacts.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/properties/user_groups.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-"""DContacts KProperty"""
+"""UserGroup KProperty"""
 
-
-from typing import TYPE_CHECKING, Optional
-from uuid import UUID
+from typing import TYPE_CHECKING
 
 from pydantic import Field
 
 from dsms.knowledge.properties.base import KProperty, KPropertyItem
 
 if TYPE_CHECKING:
     from typing import Callable
 
 
-class ContactInfo(KPropertyItem):
-    """Contact info"""
+class UserGroup(KPropertyItem):
+    """Users groups related to a KItem."""
 
-    name: str = Field(..., description="Name of the contact person")
-    email: str = Field(..., description="EMail of the contact person")
-    user_id: Optional[UUID] = Field(
-        None, description="User ID of the contact person"
-    )
+    name: str = Field(..., description="Name of the user group")
+    group_id: str = Field(..., description="ID of the user group")
 
 
-class ContactsProperty(KProperty):
-    """KProperty for contacts"""
+class UserGroupsProperty(KProperty):
+    """KProperty for user_groups"""
 
-    # OVERRIDE
     @property
     def k_property_item(cls) -> "Callable":
-        return ContactInfo
+        """UserGroup data model"""
+        return UserGroup
+
+    @property
+    def k_property_helper(cls) -> None:
+        """Not defined for User groups"""
```

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/properties/custom_datatype/numerical.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/properties/custom_datatype/numerical.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/properties/hdf5.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/properties/hdf5.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,14 +107,19 @@
     """HDF5 container of a data frame related to a KItem"""
 
     # OVERRIDE
     @property
     def k_property_item(cls) -> "Callable":
         return Column
 
+    # OVERRIDE
+    @property
+    def k_property_helper(cls) -> None:
+        """Not defined for HDF5"""
+
     def to_df(self) -> pd.DataFrame:
         """Return hdf5 as pandas DataFrame"""
         data = {column.name: column.get() for column in self}
         return pd.DataFrame.from_dict(data)
 
     def get(self, name: str) -> "Optional[Column]":
         """Get a column with a certain name."""
```

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/properties/linked_kitems.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/properties/linked_kitems.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,14 +11,22 @@
 
 if TYPE_CHECKING:
     from typing import Callable, Union
 
     from dsms import KItem
 
 
+def _linked_kitem_helper(kitem: "KItem"):
+    from dsms import KItem
+
+    if not isinstance(kitem, KItem):
+        raise TypeError(f"{kitem} is not of type {KItem}")
+    return {"id": kitem.id}
+
+
 class LinkedKItem(KPropertyItem):
     """Data model of a linked KItem"""
 
     # OVERRIDE
     id: Optional[UUID] = Field(
         None,
         description="ID of the KItem to be linked",
@@ -54,12 +62,18 @@
     """KProperty for linked KItems"""
 
     # OVERRIDE
     @property
     def k_property_item(cls) -> "Callable":
         return LinkedKItem
 
+    # OVERRIDE
+    @property
+    def k_property_helper(cls) -> "Callable":
+        """Linked KItem helper function"""
+        return _linked_kitem_helper
+
     def get(self, kitem_id: "Union[str, UUID]") -> "KItem":
         """Get the kitem with a certain id which is linked to the source KItem."""
         if not str(kitem_id) in [str(item.id) for item in self]:
             raise KeyError(f"A KItem with ID `{kitem_id} is not linked.")
         return _get_kitem(kitem_id)
```

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/properties/summary.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/properties/summary.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/queries/base.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/semantics/queries/base.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/units/base.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/semantics/units/base.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/units/conversion.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/semantics/units/conversion.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/units/sparql.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/semantics/units/sparql.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/semantics/units/utils.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/semantics/units/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/sparql_interface/sparql_interface.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/sparql_interface/sparql_interface.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/sparql_interface/subgraph.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/sparql_interface/subgraph.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/sparql_interface/utils.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/sparql_interface/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc8/dsms/knowledge/utils.py` & `dsms_sdk-1.4.0rc9/dsms/knowledge/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,19 +111,17 @@
 
 
 def __setattr_property__(self, key, value) -> None:
     if _is_number(value):
         # convert to convertable numeric object
         value = _create_numerical_dtype(key, value, self.kitem)
         # mark as updated
-        if self.kitem:
-            self.kitem.context.buffers.updated.update(
-                {self.kitem.id: self.kitem}
-            )
-    if key == "kitem":
+    if key != "kitem" and self.kitem:
+        self.kitem.context.buffers.updated.update({self.kitem.id: self.kitem})
+    elif key == "kitem":
         # set kitem for convertable numeric datatype
         for prop in self.model_dump().values():
             if isinstance(prop, NumericalDataType) and not prop.kitem:
                 prop.kitem = value
     # reassignment of extra fields does not work, seems to be a bug?
     # have this workaround:
     if key in self.__pydantic_extra__:
@@ -147,27 +145,14 @@
         if _is_number(value):
             values[key] = _create_numerical_dtype(
                 key, value, values.get("kitem")
             )
     return values
 
 
-def _get_ktype_from_id(ktype_id: str) -> "KType":
-    from dsms import Context
-
-    if not isinstance(ktype_id, str):
-        value = Context.ktypes.get(ktype_id.value)
-    else:
-        value = Context.ktypes.get(ktype_id)
-
-    if not value:
-        raise TypeError(f"KType for `ktype_id={ktype_id}` does not exist.")
-    return value
-
-
 def _get_remote_ktypes() -> Enum:
     """Get the KTypes from the remote backend"""
     from dsms import (  # isort:skip
         Context,
         KType,
     )
 
@@ -238,25 +223,26 @@
     response = _perform_request("api/knowledge/kitems", "post", json=payload)
     if not response.ok:
         raise ValueError(
             f"KItem with uuid `{kitem.id}` could not be created in DSMS: {response.text}`"
         )
 
 
-def _update_kitem(kitem: "KItem") -> Response:
+def _update_kitem(new_kitem: "KItem", old_kitem: "KItem") -> Response:
     """Update a KItem in the remote backend."""
-    old_kitem = _get_kitem(kitem.id)
-    differences = _get_kitems_diffs(old_kitem, kitem)
-    dumped = kitem.model_dump_json(
+    differences = _get_kitems_diffs(old_kitem, new_kitem)
+    dumped = new_kitem.model_dump_json(
         exclude={
             "authors",
             "annotations",
             "custom_properties",
             "linked_kitems",
             "updated_at",
+            "rdf_exists",
+            "in_backend",
             "avatar_exists",
             "user_groups",
             "ktype_id",
             "attachments",
             "id",
             "kitem_apps",
             "created_at",
@@ -264,53 +250,47 @@
             "hdf5",
         },
         exclude_none=True,
     )
     payload = json.loads(dumped)
     payload.update(
         external_links={
-            link.label: str(link.url) for link in kitem.external_links
+            link.label: str(link.url) for link in new_kitem.external_links
         },
         **differences,
     )
-    if kitem.custom_properties:
-        custom_properties = kitem.custom_properties.model_dump()
+    if new_kitem.custom_properties:
+        custom_properties = new_kitem.custom_properties.model_dump()
         payload.update(custom_properties={"content": custom_properties})
     response = _perform_request(
-        f"api/knowledge/kitems/{kitem.id}", "put", json=payload
+        f"api/knowledge/kitems/{new_kitem.id}", "put", json=payload
     )
     if not response.ok:
         raise ValueError(
-            f"KItem with uuid `{kitem.id}` could not be updated in DSMS: {response.text}`"
+            f"KItem with uuid `{new_kitem.id}` could not be updated in DSMS: {response.text}`"
         )
-    for key, value in _get_kitem(kitem.id).__dict__.items():
-        if key != "attachments":
-            setattr(kitem, key, value)
     return response
 
 
 def _delete_kitem(kitem: "KItem") -> None:
     """Delete a KItem in the remote backend"""
     response = _perform_request(f"api/knowledge/kitems/{kitem.id}", "delete")
     if not response.ok:
         raise ValueError(
             f"KItem with uuid `{kitem.id}` could not be deleted from DSMS: `{response.text}`"
         )
 
 
-def _update_attachments(kitem: "KItem") -> None:
+def _update_attachments(new_kitem: "KItem", old_kitem: "KItem") -> None:
     """Update attachments of the KItem."""
-    old_kitem = _get_kitem(kitem.id)
-    differences = _get_attachment_diffs(old_kitem, kitem)
+    differences = _get_attachment_diffs(old_kitem, new_kitem)
     for upload in differences["add"]:
-        _upload_attachments(kitem, upload.name)
+        _upload_attachments(new_kitem, upload.name)
     for remove in differences["remove"]:
-        _delete_attachments(kitem, remove.name)
-    for key, value in _get_kitem(kitem.id).__dict__.items():
-        setattr(kitem, key, value)
+        _delete_attachments(new_kitem, remove.name)
 
 
 def _upload_attachments(kitem: "KItem", attachment: "str") -> None:
     """Upload the attachments of the KItem"""
     path = Path(attachment)
 
     if path.is_file():
@@ -401,55 +381,68 @@
     _commit_updated(buffers.updated)
     _commit_deleted(buffers.deleted)
 
 
 def _commit_created(buffer: "Dict[str, KItem]") -> dict:
     """Commit the buffer for the `created` buffers"""
     for kitem in buffer.values():
-        exists = _kitem_exists(kitem)
-        if not exists:
-            _create_new_kitem(kitem)
+        _create_new_kitem(kitem)
 
 
 def _commit_updated(buffer: "Dict[str, KItem]") -> None:
     """Commit the buffer for the `updated` buffers"""
-    for kitem in buffer.values():
-        if _kitem_exists(kitem):
-            if isinstance(kitem.hdf5, pd.DataFrame):
-                _update_hdf5(kitem.id, kitem.hdf5)
-            elif isinstance(kitem.hdf5, type(None)) and _inspect_hdf5(
-                kitem.id
+    for new_kitem in buffer.values():
+        old_kitem = _get_kitem(new_kitem.id)
+        if old_kitem:
+            if isinstance(new_kitem.hdf5, pd.DataFrame):
+                _update_hdf5(new_kitem.id, new_kitem.hdf5)
+            elif isinstance(new_kitem.hdf5, type(None)) and _inspect_hdf5(
+                new_kitem.id
             ):
-                _delete_hdf5(kitem.id)
-            _update_kitem(kitem)
-            _update_attachments(kitem)
+                _delete_hdf5(new_kitem.id)
+            _update_kitem(new_kitem, old_kitem)
+            _update_attachments(new_kitem, old_kitem)
+            for key, value in _get_kitem(new_kitem.id).__dict__.items():
+                setattr(new_kitem, key, value)
 
 
 def _commit_deleted(buffer: "Dict[str, KItem]") -> None:
     """Commit the buffer for the `deleted` buffers"""
     for kitem in buffer.values():
-        if _kitem_exists(kitem):
-            _delete_hdf5(kitem.id)
-            _delete_kitem(kitem)
+        _delete_hdf5(kitem.id)
+        _delete_kitem(kitem)
+
+
+def _split_iri(iri: str) -> List[str]:
+    if "#" in iri:
+        namspace, name = iri.rsplit("#", 1)
+    else:
+        namspace, name = iri.rsplit("/", 1)
+    return namspace, name
+
+
+def _make_annotation_schema(iri: str) -> Dict[str, Any]:
+    namespace, name = _split_iri(iri)
+    return {"namespace": namespace, "name": name, "iri": iri}
 
 
 def _search(
     query: Optional[str] = None,
     ktypes: "Optional[List[KType]]" = [],
     annotations: "Optional[List[str]]" = [],
     limit: "Optional[int]" = 10,
     allow_fuzzy: "Optional[bool]" = True,
 ) -> "List[SearchResult]":
     """Search for KItems in the remote backend"""
-    from dsms import KItem  # isort:skip
+    from dsms import KItem
 
     payload = {
         "search_term": query or "",
         "ktypes": [ktype.value for ktype in ktypes],
-        "annotations": annotations,
+        "annotations": [_make_annotation_schema(iri) for iri in annotations],
         "limit": limit,
     }
     response = _perform_request(
         "api/knowledge/kitems/search",
         "post",
         json=payload,
         params={"allow_fuzzy": allow_fuzzy},
@@ -481,19 +474,22 @@
 
 
 def _slug_is_available(ktype_id: Union[str, UUID], value: str) -> bool:
     """Check whether the id of a KItem is available in the DSMS or not"""
     response = _perform_request(
         f"api/knowledge/kitems/{ktype_id}/{value}", "head"
     )
+    if response.status_code == 401:
+        raise RuntimeError("The access token has expired")
     return response.status_code == 404
 
 
 def _get_hdf5_column(kitem_id: str, column_id: int) -> List[Any]:
     """Download the column of a hdf5 container of a certain kitem"""
+
     response = _perform_request(
         f"api/knowledge/data_api/{kitem_id}/column-{column_id}", "get"
     )
     if not response.ok:
         message = f"""Something went wrong fetch column id `{column_id}`
         for kitem `{kitem_id}`: {response.text}"""
         raise ValueError(message)
```

### Comparing `dsms_sdk-1.4.0rc8/dsms_sdk.egg-info/PKG-INFO` & `dsms_sdk-1.4.0rc9/dsms_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsms_sdk
-Version: 1.4.0rc8
+Version: 1.4.0rc9
 Summary: Python SDK core-package for working with the Dataspace Management System (DSMS).
 Home-page: https://github.com/MI-FraunhoferIWM/dsms-python-sdk
 Author: Matthias Büschelberger, Yoav Nahshon, Pablo De Andres
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `dsms_sdk-1.4.0rc8/dsms_sdk.egg-info/SOURCES.txt` & `dsms_sdk-1.4.0rc9/dsms_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 dsms/knowledge/properties/base.py
 dsms/knowledge/properties/contacts.py
 dsms/knowledge/properties/external_links.py
 dsms/knowledge/properties/hdf5.py
 dsms/knowledge/properties/linked_kitems.py
 dsms/knowledge/properties/summary.py
 dsms/knowledge/properties/user_groups.py
+dsms/knowledge/properties/utils.py
 dsms/knowledge/properties/custom_datatype/__init__.py
 dsms/knowledge/properties/custom_datatype/numerical.py
 dsms/knowledge/semantics/__init__.py
 dsms/knowledge/semantics/queries/__init__.py
 dsms/knowledge/semantics/queries/base.py
 dsms/knowledge/semantics/units/__init__.py
 dsms/knowledge/semantics/units/base.py
```

### Comparing `dsms_sdk-1.4.0rc8/setup.cfg` & `dsms_sdk-1.4.0rc9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dsms_sdk
-version = v1.4.0rc8
+version = v1.4.0rc9
 description = Python SDK core-package for working with the Dataspace Management System (DSMS).
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MI-FraunhoferIWM/dsms-python-sdk
 author = Matthias Büschelberger, Yoav Nahshon, Pablo De Andres
 author_email = matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de
 license = BSD-3-Clause
```

### Comparing `dsms_sdk-1.4.0rc8/tests/conftest.py` & `dsms_sdk-1.4.0rc9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc8/tests/test_kitem.py` & `dsms_sdk-1.4.0rc9/tests/test_kitem.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc8/tests/test_utils.py` & `dsms_sdk-1.4.0rc9/tests/test_utils.py`

 * *Files identical despite different names*

