# Comparing `tmp/enbios-2.2.8.tar.gz` & `tmp/enbios-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enbios-2.2.8.tar", last modified: Wed Feb 21 14:05:03 2024, max compression
+gzip compressed data, was "enbios-2.2.9.tar", last modified: Wed Apr 24 11:15:18 2024, max compression
```

## Comparing `enbios-2.2.8.tar` & `enbios-2.2.9.tar`

### file list

```diff
@@ -1,67 +1,70 @@
-drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-02-21 14:05:03.715503 enbios-2.2.8/
--rw-rw-r--   0 ra        (1000) ra        (1000)     1483 2023-10-31 22:54:15.000000 enbios-2.2.8/LICENSE
--rw-r--r--   0 ra        (1000) ra        (1000)    12663 2024-02-21 14:05:03.715503 enbios-2.2.8/PKG-INFO
--rw-rw-r--   0 ra        (1000) ra        (1000)     9418 2024-02-21 14:04:45.000000 enbios-2.2.8/README.md
-drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-02-21 14:05:03.711503 enbios-2.2.8/enbios/
--rw-rw-r--   0 ra        (1000) ra        (1000)      206 2024-01-18 15:52:17.000000 enbios-2.2.8/enbios/__init__.py
-drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-02-21 14:05:03.711503 enbios-2.2.8/enbios/base/
--rw-rw-r--   0 ra        (1000) ra        (1000)        0 2024-01-18 15:52:17.000000 enbios-2.2.8/enbios/base/__init__.py
-drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-02-21 14:05:03.711503 enbios-2.2.8/enbios/base/adapters_aggregators/
--rw-rw-r--   0 ra        (1000) ra        (1000)        0 2024-01-18 15:52:17.000000 enbios-2.2.8/enbios/base/adapters_aggregators/__init__.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     2144 2024-01-22 09:29:34.000000 enbios-2.2.8/enbios/base/adapters_aggregators/adapter.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     1186 2024-01-19 10:01:53.000000 enbios-2.2.8/enbios/base/adapters_aggregators/aggregator.py
-drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-02-21 14:05:03.715503 enbios-2.2.8/enbios/base/adapters_aggregators/builtin/
--rw-rw-r--   0 ra        (1000) ra        (1000)      456 2024-01-19 10:01:53.000000 enbios-2.2.8/enbios/base/adapters_aggregators/builtin/__init__.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     3521 2024-01-19 10:01:53.000000 enbios-2.2.8/enbios/base/adapters_aggregators/builtin/simple_assignment_adapter.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     5393 2024-02-07 12:42:12.000000 enbios-2.2.8/enbios/base/adapters_aggregators/builtin/sum_aggregator.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     2516 2024-02-14 22:39:22.000000 enbios-2.2.8/enbios/base/adapters_aggregators/loader.py
--rw-rw-r--   0 ra        (1000) ra        (1000)    19303 2024-02-21 14:04:45.000000 enbios-2.2.8/enbios/base/experiment.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     3100 2024-02-21 14:04:45.000000 enbios-2.2.8/enbios/base/experiment_io.py
--rw-rw-r--   0 ra        (1000) ra        (1000)    14627 2024-02-14 22:39:22.000000 enbios-2.2.8/enbios/base/plot_experiment.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     1222 2024-01-18 15:52:17.000000 enbios-2.2.8/enbios/base/pydantic_experiment_validation.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     8108 2024-02-14 22:39:22.000000 enbios-2.2.8/enbios/base/result_select.py
--rw-rw-r--   0 ra        (1000) ra        (1000)    13195 2024-02-21 14:04:45.000000 enbios-2.2.8/enbios/base/scenario.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     3457 2024-01-22 09:01:20.000000 enbios-2.2.8/enbios/base/tree_operations.py
--rw-rw-r--   0 ra        (1000) ra        (1000)      533 2024-01-18 15:52:17.000000 enbios-2.2.8/enbios/base/unit_registry.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     5779 2024-02-21 14:04:45.000000 enbios-2.2.8/enbios/base/validation.py
-drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-02-21 14:05:03.715503 enbios-2.2.8/enbios/bw2/
--rw-rw-r--   0 ra        (1000) ra        (1000)     4639 2024-02-21 14:04:45.000000 enbios-2.2.8/enbios/bw2/MultiLCA_util.py
--rw-rw-r--   0 ra        (1000) ra        (1000)        0 2024-01-18 15:52:17.000000 enbios-2.2.8/enbios/bw2/__init__.py
--rw-rw-r--   0 ra        (1000) ra        (1000)    19771 2024-02-21 14:04:45.000000 enbios-2.2.8/enbios/bw2/brightway_experiment_adapter.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     7019 2024-02-21 14:04:45.000000 enbios-2.2.8/enbios/bw2/bw_models.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     1354 2024-02-07 12:42:12.000000 enbios-2.2.8/enbios/bw2/check_bw_acts_normal.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     1167 2024-01-23 09:27:04.000000 enbios-2.2.8/enbios/bw2/import_ecoinvent.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     1997 2024-01-22 09:01:20.000000 enbios-2.2.8/enbios/bw2/regionalization.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     2023 2024-02-14 22:39:22.000000 enbios-2.2.8/enbios/bw2/resolve_lca_bioflows.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     1140 2024-02-16 23:18:45.000000 enbios-2.2.8/enbios/bw2/stacked_MultiLCA.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     3562 2024-02-21 14:04:45.000000 enbios-2.2.8/enbios/bw2/stacked_MultiLCA_regio.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     8387 2024-02-21 14:04:45.000000 enbios-2.2.8/enbios/bw2/util.py
--rw-rw-r--   0 ra        (1000) ra        (1000)      300 2024-01-19 10:01:53.000000 enbios-2.2.8/enbios/const.py
-drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-02-21 14:05:03.715503 enbios-2.2.8/enbios/dev/
--rw-rw-r--   0 ra        (1000) ra        (1000)        0 2024-01-19 10:01:53.000000 enbios-2.2.8/enbios/dev/__init__.py
--rw-rw-r--   0 ra        (1000) ra        (1000)      621 2024-01-19 10:01:53.000000 enbios-2.2.8/enbios/dev/create_experiment_schema.py
-drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-02-21 14:05:03.715503 enbios-2.2.8/enbios/generic/
--rw-rw-r--   0 ra        (1000) ra        (1000)        0 2024-01-18 15:52:17.000000 enbios-2.2.8/enbios/generic/__init__.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     3177 2024-01-18 15:52:17.000000 enbios-2.2.8/enbios/generic/enbios2_logging.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     4065 2024-01-18 15:52:17.000000 enbios-2.2.8/enbios/generic/files.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     8959 2024-02-21 14:04:45.000000 enbios-2.2.8/enbios/generic/mermaid2hierarchy.py
-drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-02-21 14:05:03.715503 enbios-2.2.8/enbios/generic/tree/
--rw-rw-r--   0 ra        (1000) ra        (1000)        0 2024-01-18 15:52:17.000000 enbios-2.2.8/enbios/generic/tree/__init__.py
--rw-rw-r--   0 ra        (1000) ra        (1000)    31524 2024-01-19 10:01:53.000000 enbios-2.2.8/enbios/generic/tree/basic_tree.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     1580 2024-01-18 15:52:17.000000 enbios-2.2.8/enbios/generic/tree/csv2dict.py
--rw-rw-r--   0 ra        (1000) ra        (1000)      934 2024-01-18 15:52:17.000000 enbios-2.2.8/enbios/generic/unit_util.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     4074 2024-02-14 22:39:22.000000 enbios-2.2.8/enbios/generic/util.py
-drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-02-21 14:05:03.715503 enbios-2.2.8/enbios/models/
--rw-rw-r--   0 ra        (1000) ra        (1000)        0 2024-01-18 15:52:17.000000 enbios-2.2.8/enbios/models/__init__.py
--rw-rw-r--   0 ra        (1000) ra        (1000)      182 2024-01-18 15:52:17.000000 enbios-2.2.8/enbios/models/environment_model.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     6506 2024-02-21 14:04:45.000000 enbios-2.2.8/enbios/models/experiment_base_models.py
--rw-rw-r--   0 ra        (1000) ra        (1000)     1282 2024-01-19 10:01:53.000000 enbios-2.2.8/enbios/models/experiment_models.py
-drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-02-21 14:05:03.715503 enbios-2.2.8/enbios.egg-info/
--rw-r--r--   0 ra        (1000) ra        (1000)    12663 2024-02-21 14:05:03.000000 enbios-2.2.8/enbios.egg-info/PKG-INFO
--rw-rw-r--   0 ra        (1000) ra        (1000)     1693 2024-02-21 14:05:03.000000 enbios-2.2.8/enbios.egg-info/SOURCES.txt
--rw-rw-r--   0 ra        (1000) ra        (1000)        1 2024-02-21 14:05:03.000000 enbios-2.2.8/enbios.egg-info/dependency_links.txt
--rw-rw-r--   0 ra        (1000) ra        (1000)     1125 2024-02-21 14:05:03.000000 enbios-2.2.8/enbios.egg-info/requires.txt
--rw-rw-r--   0 ra        (1000) ra        (1000)        7 2024-02-21 14:05:03.000000 enbios-2.2.8/enbios.egg-info/top_level.txt
--rw-rw-r--   0 ra        (1000) ra        (1000)     1388 2024-02-21 14:04:59.000000 enbios-2.2.8/pyproject.toml
--rw-rw-r--   0 ra        (1000) ra        (1000)     1085 2024-02-21 14:04:45.000000 enbios-2.2.8/requirements.txt
--rw-rw-r--   0 ra        (1000) ra        (1000)       38 2024-02-21 14:05:03.715503 enbios-2.2.8/setup.cfg
+drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-04-24 11:15:18.460991 enbios-2.2.9/
+-rw-rw-r--   0 ra        (1000) ra        (1000)     1483 2023-10-31 22:54:15.000000 enbios-2.2.9/LICENSE
+-rw-r--r--   0 ra        (1000) ra        (1000)    14163 2024-04-24 11:15:18.460991 enbios-2.2.9/PKG-INFO
+-rw-rw-r--   0 ra        (1000) ra        (1000)    10459 2024-04-24 11:12:25.000000 enbios-2.2.9/README.md
+drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-04-24 11:15:18.452991 enbios-2.2.9/enbios/
+-rw-rw-r--   0 ra        (1000) ra        (1000)      859 2024-04-16 10:47:16.000000 enbios-2.2.9/enbios/__init__.py
+drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-04-24 11:15:18.456991 enbios-2.2.9/enbios/base/
+-rw-rw-r--   0 ra        (1000) ra        (1000)        0 2024-01-18 15:52:17.000000 enbios-2.2.9/enbios/base/__init__.py
+drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-04-24 11:15:18.456991 enbios-2.2.9/enbios/base/adapters_aggregators/
+-rw-rw-r--   0 ra        (1000) ra        (1000)        0 2024-01-18 15:52:17.000000 enbios-2.2.9/enbios/base/adapters_aggregators/__init__.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)     2131 2024-04-24 11:12:25.000000 enbios-2.2.9/enbios/base/adapters_aggregators/adapter.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)     1205 2024-04-24 11:12:25.000000 enbios-2.2.9/enbios/base/adapters_aggregators/aggregator.py
+drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-04-24 11:15:18.456991 enbios-2.2.9/enbios/base/adapters_aggregators/builtin/
+-rw-rw-r--   0 ra        (1000) ra        (1000)      669 2024-04-16 10:47:16.000000 enbios-2.2.9/enbios/base/adapters_aggregators/builtin/__init__.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)    22455 2024-04-16 10:47:16.000000 enbios-2.2.9/enbios/base/adapters_aggregators/builtin/assignment_adapter.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)     4421 2024-04-22 14:11:59.000000 enbios-2.2.9/enbios/base/adapters_aggregators/builtin/sum_aggregator.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)     2993 2024-04-16 10:47:16.000000 enbios-2.2.9/enbios/base/adapters_aggregators/loader.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)    21172 2024-04-24 11:12:25.000000 enbios-2.2.9/enbios/base/experiment.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)     3124 2024-04-16 10:47:16.000000 enbios-2.2.9/enbios/base/experiment_io.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)    14571 2024-04-16 10:47:16.000000 enbios-2.2.9/enbios/base/plot_experiment.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)     1256 2024-04-16 10:47:16.000000 enbios-2.2.9/enbios/base/pydantic_experiment_validation.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)     8119 2024-04-16 10:47:16.000000 enbios-2.2.9/enbios/base/result_select.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)    14999 2024-04-24 11:12:25.000000 enbios-2.2.9/enbios/base/scenario.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)     6868 2024-04-16 10:47:16.000000 enbios-2.2.9/enbios/base/tree_operations.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)      535 2024-04-16 10:47:16.000000 enbios-2.2.9/enbios/base/unit_registry.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)     5906 2024-04-24 11:12:25.000000 enbios-2.2.9/enbios/base/validation.py
+drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-04-24 11:15:18.456991 enbios-2.2.9/enbios/bw2/
+-rw-rw-r--   0 ra        (1000) ra        (1000)     7340 2024-04-16 10:47:16.000000 enbios-2.2.9/enbios/bw2/MultiLCA_util.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)        0 2024-01-18 15:52:17.000000 enbios-2.2.9/enbios/bw2/__init__.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)    22809 2024-04-24 11:12:25.000000 enbios-2.2.9/enbios/bw2/brightway_experiment_adapter.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)     6762 2024-04-16 10:47:16.000000 enbios-2.2.9/enbios/bw2/bw_models.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)     1354 2024-02-07 12:42:12.000000 enbios-2.2.9/enbios/bw2/check_bw_acts_normal.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)     1167 2024-01-23 09:27:04.000000 enbios-2.2.9/enbios/bw2/import_ecoinvent.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)     1997 2024-01-22 09:01:20.000000 enbios-2.2.9/enbios/bw2/regionalization.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)     2023 2024-02-14 22:39:22.000000 enbios-2.2.9/enbios/bw2/resolve_lca_bioflows.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)     8387 2024-02-21 14:04:45.000000 enbios-2.2.9/enbios/bw2/util.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)      300 2024-01-19 10:01:53.000000 enbios-2.2.9/enbios/const.py
+drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-04-24 11:15:18.456991 enbios-2.2.9/enbios/dev/
+-rw-rw-r--   0 ra        (1000) ra        (1000)        0 2024-01-19 10:01:53.000000 enbios-2.2.9/enbios/dev/__init__.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)      605 2024-04-16 10:47:16.000000 enbios-2.2.9/enbios/dev/create_experiment_schema.py
+drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-04-24 11:15:18.456991 enbios-2.2.9/enbios/generic/
+-rw-rw-r--   0 ra        (1000) ra        (1000)        0 2024-01-18 15:52:17.000000 enbios-2.2.9/enbios/generic/__init__.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)     3177 2024-01-18 15:52:17.000000 enbios-2.2.9/enbios/generic/enbios2_logging.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)     4065 2024-01-18 15:52:17.000000 enbios-2.2.9/enbios/generic/files.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)     8959 2024-02-21 14:04:45.000000 enbios-2.2.9/enbios/generic/mermaid2hierarchy.py
+drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-04-24 11:15:18.456991 enbios-2.2.9/enbios/generic/tree/
+-rw-rw-r--   0 ra        (1000) ra        (1000)        0 2024-01-18 15:52:17.000000 enbios-2.2.9/enbios/generic/tree/__init__.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)    32349 2024-04-24 11:12:25.000000 enbios-2.2.9/enbios/generic/tree/basic_tree.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)     1326 2024-04-16 10:47:16.000000 enbios-2.2.9/enbios/generic/unit_util.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)     4133 2024-04-16 10:47:16.000000 enbios-2.2.9/enbios/generic/util.py
+drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-04-24 11:15:18.456991 enbios-2.2.9/enbios/models/
+-rw-rw-r--   0 ra        (1000) ra        (1000)        0 2024-01-18 15:52:17.000000 enbios-2.2.9/enbios/models/__init__.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)      188 2024-04-16 10:47:16.000000 enbios-2.2.9/enbios/models/environment_model.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)     8299 2024-04-24 11:12:25.000000 enbios-2.2.9/enbios/models/models.py
+drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-04-24 11:15:18.456991 enbios-2.2.9/enbios/util/
+-rw-rw-r--   0 ra        (1000) ra        (1000)       82 2024-04-16 10:47:16.000000 enbios-2.2.9/enbios/util/__init__.py
+drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-04-24 11:15:18.456991 enbios-2.2.9/enbios/util/flatten_dict/
+-rw-rw-r--   0 ra        (1000) ra        (1000)        0 2024-04-16 10:47:16.000000 enbios-2.2.9/enbios/util/flatten_dict/__init__.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)     6274 2024-04-16 10:47:16.000000 enbios-2.2.9/enbios/util/flatten_dict/flatten_dict.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)     1028 2024-04-16 10:47:16.000000 enbios-2.2.9/enbios/util/flatten_dict/reducers.py
+-rw-rw-r--   0 ra        (1000) ra        (1000)      914 2024-04-16 10:47:16.000000 enbios-2.2.9/enbios/util/flatten_dict/splitters.py
+drwxrwxr-x   0 ra        (1000) ra        (1000)        0 2024-04-24 11:15:18.456991 enbios-2.2.9/enbios.egg-info/
+-rw-r--r--   0 ra        (1000) ra        (1000)    14163 2024-04-24 11:15:18.000000 enbios-2.2.9/enbios.egg-info/PKG-INFO
+-rw-rw-r--   0 ra        (1000) ra        (1000)     1712 2024-04-24 11:15:18.000000 enbios-2.2.9/enbios.egg-info/SOURCES.txt
+-rw-rw-r--   0 ra        (1000) ra        (1000)        1 2024-04-24 11:15:18.000000 enbios-2.2.9/enbios.egg-info/dependency_links.txt
+-rw-rw-r--   0 ra        (1000) ra        (1000)     1327 2024-04-24 11:15:18.000000 enbios-2.2.9/enbios.egg-info/requires.txt
+-rw-rw-r--   0 ra        (1000) ra        (1000)        7 2024-04-24 11:15:18.000000 enbios-2.2.9/enbios.egg-info/top_level.txt
+-rw-rw-r--   0 ra        (1000) ra        (1000)     1517 2024-04-24 11:15:16.000000 enbios-2.2.9/pyproject.toml
+-rw-rw-r--   0 ra        (1000) ra        (1000)     1219 2024-04-22 08:08:25.000000 enbios-2.2.9/requirements.txt
+-rw-rw-r--   0 ra        (1000) ra        (1000)       38 2024-04-24 11:15:18.460991 enbios-2.2.9/setup.cfg
```

### Comparing `enbios-2.2.8/LICENSE` & `enbios-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `enbios-2.2.8/PKG-INFO` & `enbios-2.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enbios
-Version: 2.2.8
+Version: 2.2.9
 Summary: Enbios 2
 Author: Ramin Soleymani
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/LIVENlab/enbios
 Project-URL: Bug Tracker, https://github.com/LIVENlab/enbios/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -46,53 +46,65 @@
 Requires-Dist: fonttools==4.47.2
 Requires-Dist: frictionless==5.16.0
 Requires-Dist: fs==2.4.16
 Requires-Dist: idna==3.4
 Requires-Dist: importlib-resources==6.0.0
 Requires-Dist: kiwisolver==1.4.4
 Requires-Dist: lxml==4.9.3
-Requires-Dist: matplotlib==3.7.2
+Requires-Dist: matplotlib==3.8.3
+Requires-Dist: matplotlib-inline==0.1.6
 Requires-Dist: matrix-utils==0.2.5
 Requires-Dist: mrio-common-metadata==0.2.1
 Requires-Dist: numpy==1.26.4
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: packaging==23.1
 Requires-Dist: pandas==2.0.3
-Requires-Dist: peewee==3.17.0
-Requires-Dist: Pillow==10.2.0
-Requires-Dist: Pint==0.22
+Requires-Dist: peewee==3.17.1
+Requires-Dist: pillow==10.2.0
+Requires-Dist: Pint==0.23
+Requires-Dist: pkginfo==1.10.0
 Requires-Dist: platformdirs==3.9.1
-Requires-Dist: pydantic==2.5.2
-Requires-Dist: pyparsing
+Requires-Dist: pydantic==2.6.4
+Requires-Dist: pydantic-settings==2.2.1
+Requires-Dist: pydantic_core==2.16.3
+Requires-Dist: pydoc-markdown==4.8.2
+Requires-Dist: Pygments==2.17.2
+Requires-Dist: pyparsing==3.1.1
 Requires-Dist: PyPrind==2.11.3
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: python-mermaid==0.1.3
 Requires-Dist: pytz==2023.3
 Requires-Dist: pyxlsb==1.0.10
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: requests==2.31.0
-Requires-Dist: scipy==1.11.1
+Requires-Dist: scipy==1.12.0
 Requires-Dist: scikit-learn>=1.4.0
 Requires-Dist: six==1.16.0
 Requires-Dist: stats-arrays==0.6.5
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: tqdm==4.66.1
 Requires-Dist: tzdata==2023.3
 Requires-Dist: Unidecode==1.3.8
-Requires-Dist: urllib3==2.1.0
+Requires-Dist: urllib3==2.2.1
 Requires-Dist: voluptuous==0.13.1
 Requires-Dist: Whoosh==2.7.4
 Requires-Dist: wrapt==1.15.0
 Requires-Dist: xlrd==2.0.1
 Requires-Dist: XlsxWriter==3.1.9
 Requires-Dist: xmltodict==0.13.0
 Requires-Dist: zipp==3.16.2
 Provides-Extra: test
 Requires-Dist: pytest==7.3.2; extra == "test"
-Requires-Dist: Deprecated>=1.2.14; extra == "test"
+Provides-Extra: dev
+Requires-Dist: build==1.2.1; extra == "dev"
+Requires-Dist: twine==4.0.2; extra == "dev"
+Requires-Dist: jupyter==1.0.0; extra == "dev"
+Requires-Dist: ruff==0.3.3; extra == "dev"
+Requires-Dist: black==23.12.1; extra == "dev"
+Requires-Dist: tokenize-rt; extra == "dev"
 
 # ENBIOS2
 
 ## What is ENBIOS 2
 
 ENBIOS2 (Environmental and Bioeconomic System Analysis)  is a [python-based](https://pypi.org/project/enbios/)
 simulation tool for the assessment of environmental impacts and resource requirements of energy system
@@ -198,43 +210,65 @@
 - Environmental impact indicators from the most used LCIA methods (Recipe2016, CML, AWARE, etc.)
 - Environmental externalization rates
 - Forthcoming: Raw Material Recycling rates and Supply risk
 
 ### Features
 
 - Integration of LCA and MuSIASEM evaluation methods
-- Import of .spold LCA inventory data to a multi-level tree-like setting
 - Library of impact assessment methods based on LCIA
 - New impact assessment methods developed for raw materials and circularity
 - Consideration of externalized environmental impacts
 - Takes data from the friendly-data package (other formats under development)
 - High level methods to quickly obtain/refresh analyses
 
 ## Demos
 
 This repository contains a few notebooks (require jupyter notebook) in the demos folder, that can help you get started.
 We are updating and commenting these. Please bear with us while we do it and feel free to give us feedback on those (
 thanks).
 
+You can copy the demos into your project like this:
+
+```python
+from enbios import copy_demos
+
+copy_demos("<destination_path>")
+```
+
 [Getting started](https://github.com/LIVENlab/enbios/blob/main/demos/intro.ipynb)
 
 [Plotting results](https://github.com/LIVENlab/enbios/blob/main/demos/plot_results.ipynb)
 
 [Sorting the results in alternative hierarchies](https://github.com/LIVENlab/enbios/blob/main/demos/multiple_hierarchies.ipynb)
 
+Reevaluate the experiment with alternative hierarchies. For alternative hierarchies the structural nodes (none bottom
+nodes) can be changed/added.
+
+[Assignment Adapter](https://github.com/LIVENlab/enbios/blob/main/demos/assignment_adapter_demo.ipynb)
+
+The Simple Assignment Adapter does not any specific calculations.
+Instead, it allows the user to introduce fixed values, that should come from some external source into the enbios tree
+calculation. This includes not just the outputs of structural nodes, but in particular their impact results.
+These values can be either in the experiment configuration file or for convenience in a referenced csv file. The values
+can be specified in such a way, that scenario outputs and result values have consistent and valid units.
+
 [Splitting the configuration](https://github.com/LIVENlab/enbios/blob/main/demos/multiple_config_files.ipynb)
 
 [Working with trees](https://github.com/LIVENlab/enbios/blob/main/demos/trees.ipynb)
 
 [Experiment with uncertainties](https://github.com/LIVENlab/enbios/blob/main/demos/uncertainty_experiment.ipynb)
 
 [Convert mermaid diagrams to enbios hierarchy](https://github.com/LIVENlab/enbios/blob/main/demos/mermaid.ipynb)
 
 [A complete Brightway adaoter configuration object](https://github.com/LIVENlab/enbios/blob/main/demos/bw_adapter_config.ipynb)
 
+[Specifying the hierarchy in a csv file](https://github.com/LIVENlab/enbios/blob/main/demos/csv_hierarchy.ipynb)
+
+[Exporting to a csv file](https://github.com/LIVENlab/enbios/blob/main/demos/csv_export.ipynb)
+
 ## People
 
 * [Ramin Soleymani](https://es.linkedin.com/in/ramin-soleymani-4703b17). -[ICTA-UAB](https://www.uab.cat/icta/)
 * [Miquel Sierra Montoya](https://portalrecerca.uab.cat/en/persons/miquel-sierra-i-montoya). -[ICTA-UAB](https://www.uab.cat/icta/)
 * [Alexander de Tomás](https://www.linkedin.com/in/alexander-de-tom%C3%A1s-pascual-a85348185/). -[ICTA-UAB](https://www.uab.cat/icta/)
 * [Cristina Madrid-Lopez](https://portalrecerca.uab.cat/en/persons/cristina-madrid-lopez-3). - [ICTA-UAB](https://www.uab.cat/icta/)
```

### Comparing `enbios-2.2.8/README.md` & `enbios-2.2.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -106,43 +106,65 @@
 - Environmental impact indicators from the most used LCIA methods (Recipe2016, CML, AWARE, etc.)
 - Environmental externalization rates
 - Forthcoming: Raw Material Recycling rates and Supply risk
 
 ### Features
 
 - Integration of LCA and MuSIASEM evaluation methods
-- Import of .spold LCA inventory data to a multi-level tree-like setting
 - Library of impact assessment methods based on LCIA
 - New impact assessment methods developed for raw materials and circularity
 - Consideration of externalized environmental impacts
 - Takes data from the friendly-data package (other formats under development)
 - High level methods to quickly obtain/refresh analyses
 
 ## Demos
 
 This repository contains a few notebooks (require jupyter notebook) in the demos folder, that can help you get started.
 We are updating and commenting these. Please bear with us while we do it and feel free to give us feedback on those (
 thanks).
 
+You can copy the demos into your project like this:
+
+```python
+from enbios import copy_demos
+
+copy_demos("<destination_path>")
+```
+
 [Getting started](https://github.com/LIVENlab/enbios/blob/main/demos/intro.ipynb)
 
 [Plotting results](https://github.com/LIVENlab/enbios/blob/main/demos/plot_results.ipynb)
 
 [Sorting the results in alternative hierarchies](https://github.com/LIVENlab/enbios/blob/main/demos/multiple_hierarchies.ipynb)
 
+Reevaluate the experiment with alternative hierarchies. For alternative hierarchies the structural nodes (none bottom
+nodes) can be changed/added.
+
+[Assignment Adapter](https://github.com/LIVENlab/enbios/blob/main/demos/assignment_adapter_demo.ipynb)
+
+The Simple Assignment Adapter does not any specific calculations.
+Instead, it allows the user to introduce fixed values, that should come from some external source into the enbios tree
+calculation. This includes not just the outputs of structural nodes, but in particular their impact results.
+These values can be either in the experiment configuration file or for convenience in a referenced csv file. The values
+can be specified in such a way, that scenario outputs and result values have consistent and valid units.
+
 [Splitting the configuration](https://github.com/LIVENlab/enbios/blob/main/demos/multiple_config_files.ipynb)
 
 [Working with trees](https://github.com/LIVENlab/enbios/blob/main/demos/trees.ipynb)
 
 [Experiment with uncertainties](https://github.com/LIVENlab/enbios/blob/main/demos/uncertainty_experiment.ipynb)
 
 [Convert mermaid diagrams to enbios hierarchy](https://github.com/LIVENlab/enbios/blob/main/demos/mermaid.ipynb)
 
 [A complete Brightway adaoter configuration object](https://github.com/LIVENlab/enbios/blob/main/demos/bw_adapter_config.ipynb)
 
+[Specifying the hierarchy in a csv file](https://github.com/LIVENlab/enbios/blob/main/demos/csv_hierarchy.ipynb)
+
+[Exporting to a csv file](https://github.com/LIVENlab/enbios/blob/main/demos/csv_export.ipynb)
+
 ## People
 
 * [Ramin Soleymani](https://es.linkedin.com/in/ramin-soleymani-4703b17). -[ICTA-UAB](https://www.uab.cat/icta/)
 * [Miquel Sierra Montoya](https://portalrecerca.uab.cat/en/persons/miquel-sierra-i-montoya). -[ICTA-UAB](https://www.uab.cat/icta/)
 * [Alexander de Tomás](https://www.linkedin.com/in/alexander-de-tom%C3%A1s-pascual-a85348185/). -[ICTA-UAB](https://www.uab.cat/icta/)
 * [Cristina Madrid-Lopez](https://portalrecerca.uab.cat/en/persons/cristina-madrid-lopez-3). - [ICTA-UAB](https://www.uab.cat/icta/)
```

### Comparing `enbios-2.2.8/enbios/base/adapters_aggregators/adapter.py` & `enbios-2.2.9/enbios/base/adapters_aggregators/adapter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from abc import ABC, abstractmethod
+from logging import Logger
 from typing import Any, Optional
 
 from enbios.base.scenario import Scenario
 from enbios.generic.enbios2_logging import get_logger
-from enbios.models.experiment_base_models import (
-    NodeOutput,
-    AdapterModel,
-)
-from enbios.models.experiment_models import ResultValue
+from enbios.models.models import AdapterModel, NodeOutput, ResultValue
 
 
 class EnbiosAdapter(ABC):
     def __init__(self):
         self._config = None
 
     @abstractmethod
@@ -32,53 +29,54 @@
         pass
 
     @abstractmethod
     def validate_node(self, node_name: str, node_config: Any):
         pass
 
     @abstractmethod
-    def validate_node_output(self, node_name: str, target_output: NodeOutput) -> float:
+    def validate_scenario_node(
+        self, node_name: str, scenario_name: str, scenario_node_data: Any
+    ):
         pass
 
     @abstractmethod
-    def get_node_output_unit(self, node_name: str) -> str:
+    def get_node_output(self, node_name: str, scenario: str) -> list[NodeOutput]:
         pass
 
     @abstractmethod
     def get_method_unit(self, method_name: str) -> str:
         pass
 
     @abstractmethod
-    def get_default_output_value(self, node_name: str) -> float:
-        pass
-
-    @abstractmethod
     def run_scenario(self, scenario: Scenario) -> dict[str, dict[str, ResultValue]]:
         """
         Run a specific scenario. The adapter should return a dictionary of the form:
             {
                 node_name: {
                     method_name: ResultValue (unit, magnitude)
                 }
             }
         :param scenario:
         :return:
         """
         pass
 
-    def get_logger(self):
-        return get_logger(f"ADAPTER::({self.name()})")
-
     @staticmethod
     @abstractmethod
     def node_indicator() -> str:
         pass
 
     @staticmethod
     @abstractmethod
     def get_config_schemas() -> dict[str, dict[str, Any]]:
         pass
 
     @staticmethod
     @abstractmethod
     def name() -> str:
         pass
+
+    def get_logger(self) -> Logger:
+        return get_logger(f"({self.name()})")
+
+    def result_extras(self, node_name: str) -> dict[str, Any]:
+        return {}
```

### Comparing `enbios-2.2.8/enbios/base/adapters_aggregators/aggregator.py` & `enbios-2.2.9/enbios/base/adapters_aggregators/aggregator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from abc import ABC, abstractmethod
 from typing import Optional, Any
 
 from enbios.generic.enbios2_logging import get_logger
 from enbios.generic.tree.basic_tree import BasicTreeNode
-from enbios.models.experiment_base_models import NodeOutput
-from enbios.models.experiment_models import ScenarioResultNodeData
+from enbios.models.models import NodeOutput, ScenarioResultNodeData
 
 
 class EnbiosAggregator(ABC):
     @abstractmethod
     def validate_config(self, config: Optional[dict[str, Any]]):
         pass
 
@@ -17,15 +16,15 @@
         pass
 
     @abstractmethod
     def aggregate_node_output(
         self,
         node: BasicTreeNode[ScenarioResultNodeData],
         scenario_name: Optional[str] = "",
-    ) -> Optional[NodeOutput]:
+    ) -> list[NodeOutput]:
         pass
 
     @abstractmethod
     def aggregate_node_result(self, node: BasicTreeNode[ScenarioResultNodeData]):
         pass
 
     @staticmethod
@@ -39,9 +38,12 @@
         pass
 
     @staticmethod
     @abstractmethod
     def get_config_schemas() -> dict:
         pass
 
+    def result_extras(self, node_name: str) -> dict[str, Any]:
+        return {}
+
     def get_logger(self):
         return get_logger(f"__name__ ({self.name})")
```

### Comparing `enbios-2.2.8/enbios/base/adapters_aggregators/loader.py` & `enbios-2.2.9/enbios/base/adapters_aggregators/loader.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,58 +1,71 @@
 import inspect
 from pathlib import Path
 from types import ModuleType
-from typing import Union, Type
+from typing import Union, Type, Optional, cast
 
 from enbios.base.adapters_aggregators.adapter import EnbiosAdapter
 from enbios.base.adapters_aggregators.aggregator import EnbiosAggregator
 from enbios.base.adapters_aggregators.builtin import BUILTIN_ADAPTERS, BUILTIN_AGGREGATORS
 from enbios.generic.enbios2_logging import get_logger
 from enbios.generic.util import load_module
-from enbios.models.experiment_base_models import AdapterModel, AggregationModel
+from enbios.models.models import AdapterModel, AggregationModel
 
 logger = get_logger(__name__)
 
 
 def create_module_object(
     model_data: Union[AdapterModel, AggregationModel], base_class: Type
 ) -> Union[EnbiosAdapter, EnbiosAggregator]:
     if model_data.module_path:
+        assert model_data.module_path
         try:
             adapter_module: ModuleType = load_module(model_data.module_path)
         except Exception as err:
             raise ValueError(f"Could not load module '{model_data.module_path}' ({err})")
         # validator makes sure there is no other case
         for inspect_clazz in inspect.getmembers(adapter_module, inspect.isclass):
             # check if cl is subclass of EnbiosAdapter/EnbiosAggregation
-            clazz = inspect_clazz[1]
+            clazz: Optional[Type[Union[EnbiosAdapter, EnbiosAggregator]]] = inspect_clazz[
+                1
+            ]
+            assert clazz
             if any(base.__name__ == base_class.__name__ for base in clazz.__bases__):
                 return clazz()
+        raise ValueError(
+            f"'{Path(model_data.module_path).name}' has no class that inherits from '{base_class.__name__}'"
+        )
     else:
         if base_class.__name__ == EnbiosAdapter.__name__:
+            assert (
+                hasattr(model_data, "adapter_name")
+                and model_data.adapter_name is not None
+            )
             clazz = BUILTIN_ADAPTERS.get(model_data.adapter_name)
             if not clazz:
-                logger.error(
-                    f"Could not find built-in adapter with name '{model_data.adapter_name}'. Candidates are: {BUILTIN_ADAPTERS.keys()}"
+                raise ValueError(
+                    f"Could not find built-in adapter with name '{model_data.adapter_name}'. "
+                    f"Candidates are: {BUILTIN_ADAPTERS.keys()}"
                 )
             else:
                 return clazz()
         else:
             assert base_class.__name__ == EnbiosAggregator.__name__
+            assert hasattr(model_data, "aggregator_name")
             clazz = BUILTIN_AGGREGATORS.get(model_data.aggregator_name)
             if not clazz:
-                logger.error(
-                    f"Could not find built-in aggregator with name '{model_data.aggregator_name}'. Candidates are: {BUILTIN_AGGREGATORS.keys()}"
+                raise ValueError(
+                    f"Could not find built-in aggregator with name '{model_data.aggregator_name}'. "
+                    f"Candidates are: {BUILTIN_AGGREGATORS.keys()}"
                 )
             else:
                 return clazz()
-    raise ValueError(
-        f"'{Path(model_data.module_path).name}' has no class that inherits from '{base_class.__name__}'"
-    )
 
 
 def load_adapter(adapter_model: AdapterModel) -> EnbiosAdapter:
-    return create_module_object(adapter_model, EnbiosAdapter)
+    return cast(EnbiosAdapter, create_module_object(adapter_model, EnbiosAdapter))
 
 
 def load_aggregator(aggregator_model: AggregationModel) -> EnbiosAggregator:
-    return create_module_object(aggregator_model, EnbiosAggregator)
+    return cast(
+        EnbiosAggregator, create_module_object(aggregator_model, EnbiosAggregator)
+    )
```

### Comparing `enbios-2.2.8/enbios/base/experiment.py` & `enbios-2.2.9/enbios/base/experiment.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import csv
+import json
 import math
 import time
 from datetime import timedelta
 from pathlib import Path
 from tempfile import gettempdir
 from typing import Any, Optional, Union, Type, cast
 
@@ -20,38 +21,31 @@
 from enbios.base.validation import (
     validate_run_scenario_setting,
     validate_scenarios,
     validate_scenario,
     validate_adapters,
     validate_aggregators,
 )
-from enbios.bw2.stacked_MultiLCA import StackedMultiLCA
+from enbios.bw2.MultiLCA_util import BaseStackedMultiLCA
 from enbios.generic.enbios2_logging import get_logger
 from enbios.generic.files import PathLike, ReadPath
 from enbios.generic.tree.basic_tree import BasicTreeNode
 from enbios.models.environment_model import Settings
-from enbios.models.experiment_base_models import (
+from enbios.models.models import (
     ExperimentConfig,
     ExperimentScenarioData,
     NodeOutput,
     ExperimentDataResolved,
-)
-from enbios.models.experiment_models import (
-    ScenarioResultNodeData,
     TechTreeNodeData,
+    ScenarioResultNodeData,
 )
 
 logger = get_logger(__name__)
 
 
-# Define a TypeVar that is bound to EnbiosAdapter
-# EnbiosAdapterType = TypeVar("EnbiosAdapterType", bound=EnbiosAdapter)
-# EnbiosAggregatorType = TypeVar("EnbiosAggregatorType", bound=EnbiosAggregator)
-
-
 class Experiment:
     DEFAULT_SCENARIO_NAME = "default scenario"
 
     def __init__(self, data_input: Optional[Union[dict, str]] = None):
         """
         Initialize the experiment
         :param data_input: dictionary or filename to load the data from
@@ -60,54 +54,50 @@
         if not data_input:
             data_input = self.env_settings.CONFIG_FILE
             if not isinstance(data_input, str):
                 raise ValueError(
                     "Experiment config-file-path must be specified as environment "
                     "variable: 'CONFIG_FILE'"
                 )
-        data: dict = {}
         if isinstance(data_input, str):
             config_file_path = ReadPath(data_input)
             data = config_file_path.read_data()
         else:
             data = data_input
         raw_data = validate_experiment_data(data)
         # resolve hierarchy and scenarios filepaths if present
         self.resolved_raw_data: ExperimentDataResolved = resolve_input_files(raw_data)
 
         # load and validate adapters and aggregators
-        adapters, modules = validate_adapters(raw_data.adapters)
+        adapters, methods = validate_adapters(raw_data.adapters)
         self._adapters: dict[str, EnbiosAdapter] = adapters
-        self.methods: list[str] = modules
+        self.methods: list[str] = methods
         self._aggregators: dict[str, EnbiosAggregator] = validate_aggregators(
             raw_data.aggregators
         )
 
         # validate overall hierarchy
-        self.hierarchy_root: BasicTreeNode[TechTreeNodeData] = (
-            validate_experiment_hierarchy(self.resolved_raw_data.hierarchy)
-        )
+        self.hierarchy_root: BasicTreeNode[
+            TechTreeNodeData
+        ] = validate_experiment_hierarchy(self.resolved_raw_data.hierarchy)
         self._structural_nodes: dict[str, BasicTreeNode[TechTreeNodeData]] = {}
         # validate individual nodes based on their adapter/aggregator
         for node in self.hierarchy_root.iter_all_nodes():
             if node.is_leaf:
                 self.get_node_adapter(node).validate_node(node.name, node.data.config)
                 self._structural_nodes[node.name] = node
             else:
                 self.get_node_aggregator(node).validate_node(node.name, node.data.config)
 
         def recursive_convert(
             node_: BasicTreeNode[TechTreeNodeData],
         ) -> BasicTreeNode[ScenarioResultNodeData]:
-            output: Optional[NodeOutput] = None
-            if node_.is_leaf:
-                output = NodeOutput(
-                    unit=self.get_node_adapter(node_).get_node_output_unit(node_.name),
-                    magnitude=0,
-                )
+            output: list[NodeOutput] = []
+            # if node_.is_leaf:
+            #     output = self.get_node_adapter(node_).get_node_output(node_.name, "")
             return BasicTreeNode(
                 name=node_.name,
                 data=ScenarioResultNodeData(
                     output=output,
                     adapter=node_.data.adapter,
                     aggregator=node_.data.aggregator,
                 ),
@@ -119,15 +109,15 @@
         )
 
         self.scenarios: list[Scenario] = validate_scenarios(
             self.resolved_raw_data.scenarios, Experiment.DEFAULT_SCENARIO_NAME, self
         )
         validate_run_scenario_setting(self.env_settings, self.config, self.scenario_names)
 
-        self._lca: Optional[StackedMultiLCA] = None
+        self._lca: Optional[BaseStackedMultiLCA] = None
         self._execution_time: float = float("NaN")
 
     def get_structural_node(self, name: str) -> BasicTreeNode[TechTreeNodeData]:
         """
         Get a node by either its name
         as it is defined in the experiment data
         :param name:
@@ -184,16 +174,17 @@
 
     def _get_module_by_name_or_node_indicator(
         self,
         name_or_indicator: str,
         module_type: Type[Union[EnbiosAdapter, EnbiosAggregator]],
         node_name: Optional[str] = None,
     ) -> Union[EnbiosAdapter, EnbiosAggregator]:
-        modules: dict[str, Union[EnbiosAdapter, EnbiosAggregator]] = (
-            self._adapters if module_type == EnbiosAdapter else self._aggregators
+        modules: dict[str, Union[EnbiosAdapter, EnbiosAggregator]] = cast(
+            dict[str, Union[EnbiosAdapter, EnbiosAggregator]],
+            (self._adapters if module_type == EnbiosAdapter else self._aggregators),
         )
         module = modules.get(name_or_indicator)
         if module:
             return module
         # also check, if the name instead of the indicator was used
         for module in modules.values():
             if module.node_indicator() == name_or_indicator:
@@ -272,70 +263,96 @@
                 return scenario_results
             else:
                 return "not run"
 
     def results_to_csv(
         self,
         file_path: PathLike,
-        scenario_name: Optional[str] = None,
+        scenarios: Optional[Union[str, list[str]]] = None,
         level_names: Optional[list[str]] = None,
         include_method_units: bool = True,
+        include_output: bool = True,
+        flat_hierarchy: Optional[bool] = False,
+        include_extras: Optional[bool] = True,
+        repeat_parent_name: bool = False,
+        alternative_hierarchy: Optional[dict] = None,
     ):
         """
         Turn the results into a csv file. If no scenario name is given,
         it will export all scenarios to the same file,
         :param file_path:
-        :param scenario_name: If no scenario name is given, it will
-        export all scenarios to the same file,
-            with an additional column for the scenario alias
+        :param scenarios: string or list of strings. If no scenario name is given, it will export all scenarios to the same file,
+        with an additional column for the scenario alias
         :param level_names: (list of strings) If given, the results will be
         exported with the given level names
         :param include_method_units:  (Include the units of the methods in the header)
+        :param include_output:
+        :param flat_hierarchy:
+        :param include_extras:
+        :param repeat_parent_name:
+        :param alternative_hierarchy:
+
         :return:
         """
-        if scenario_name:
+        scenario_names: list[str]
+        single_scenario = isinstance(scenarios, str)
+        if single_scenario:
+            scenario_names = [scenarios]
+        elif not scenarios:
+            scenario_names = [s.name for s in self.scenarios]
+        else:
+            scenario_names = scenarios
+        header = []
+        all_rows: list = []
+        for scenario_name in scenario_names:
             scenario = self.get_scenario(scenario_name)
+            temp_file_name = gettempdir() + f"/temp_scenario_{scenario.name}.csv"
             scenario.results_to_csv(
-                file_path,
+                temp_file_name,
                 level_names=level_names,
                 include_method_units=include_method_units,
+                include_output=include_output,
+                flat_hierarchy=flat_hierarchy,
+                repeat_parent_name=repeat_parent_name,
+                include_extras=include_extras,
+                alternative_hierarchy=alternative_hierarchy,
             )
-            return
-        else:
-            header = []
-            all_rows: list = []
-            for scenario in self.scenarios:
-                temp_file_name = gettempdir() + f"/temp_scenario_{scenario.name}.csv"
-                scenario.results_to_csv(
-                    temp_file_name,
-                    level_names=level_names,
-                    include_method_units=include_method_units,
-                )
-                rows = ReadPath(temp_file_name).read_data()
-                rows[0]["scenario"] = scenario.name
-                if not all_rows:
-                    header = list(rows[0].keys())
-                    header.remove("scenario")
-                    header.insert(0, "scenario")
-                all_rows.extend(rows)
-                if (temp_file := Path(temp_file_name)).exists():
-                    temp_file.unlink()
-            with Path(file_path).open("w", newline="") as csvfile:
-                writer = csv.DictWriter(csvfile, header)
-                writer.writeheader()
-                writer.writerows(all_rows)
-
-    def result_to_dict(self, include_output: bool = True) -> list[dict[str, Any]]:
+            rows = ReadPath(temp_file_name).read_data()
+            if not single_scenario:
+                for row in rows:
+                    row["scenario"] = scenario.name
+            # if not all_rows:
+            for row in rows:
+                for k in row.keys():
+                    if k not in header:
+                        header.append(k)
+            all_rows.extend(rows)
+            if (temp_file := Path(temp_file_name)).exists():
+                temp_file.unlink()
+        # put the scenario header at the start
+        if not single_scenario:
+            header.remove("scenario")
+            header.insert(0, "scenario")
+        with Path(file_path).open("w", newline="") as csvfile:
+            writer = csv.DictWriter(csvfile, header)
+            writer.writeheader()
+            writer.writerows(all_rows)
+
+    def result_to_dict(
+        self, include_output: bool = True, alternative_hierarchy: Optional[dict] = None
+    ) -> list[dict[str, Any]]:
         """
         Get the results of all scenarios as a list of dictionaries as dictionaries
         :param include_output: Include the output of each node in the tree
         :return:
         """
         return [
-            scenario.result_to_dict(include_output=include_output)
+            scenario.result_to_dict(
+                include_output=include_output, alternative_hierarchy=alternative_hierarchy
+            )
             for scenario in self.scenarios
         ]
 
     @property
     def config(self) -> ExperimentConfig:
         """
         get the config of the experiment
@@ -378,14 +395,15 @@
         result_as_dict: bool = True,
         append_scenario: bool = True,
     ) -> Union[BasicTreeNode[ScenarioResultNodeData], dict]:
         """
         Run a scenario from a config dictionary. Scenario will be validated and run. An
         :param scenario_config:
         :param result_as_dict:
+        :param append_scenario:
         :return:
         """
         scenario_data = ExperimentScenarioData(**scenario_config)
         scenario_data.name_factory(len(self.scenarios))
 
         extra_index = 1
         if scenario_data.name in self.scenario_names:
@@ -412,27 +430,44 @@
                 module_name = self.get_node_aggregator(node).name()
             node_rows.append(f"{' ' * node.level}{node.name} - {module_name}")
 
         self.hierarchy_root.recursive_apply(print_node, False, False, None)
 
         node_rows_str = "\n".join(node_rows)
         methods_str = "\n".join([f" {m}" for m in self.methods])
+
+        scenarios_done = [scenario.has_run for scenario in self.scenarios]
+        all_scenarios_run = all(scenarios_done)
+        no_scenarios_run = not any(scenarios_done)
+
+        run_status_str = (
+            "all scenarios run"
+            if all_scenarios_run
+            else "no scenarios run"
+            if no_scenarios_run
+            else "some scenarios run"
+        )
+
         return (
             f"Experiment: \n"
             f"Structural nodes: {len(self._structural_nodes)}\n"
             f"{node_rows_str}\n"
             f"Methods: {len(self.methods)}\n"
             f"{methods_str}\n"
             f"Hierarchy (depth): {self.hierarchy_root.depth}\n"
             f"Scenarios: {len(self.scenarios)}\n"
+            f"{run_status_str}\n"
         )
 
     @staticmethod
     def get_module_definition(
-        clazz: Union[EnbiosAdapter, EnbiosAggregator], details: bool = True
+        clazz: Union[
+            Type[EnbiosAdapter], EnbiosAdapter, Type[EnbiosAggregator], EnbiosAggregator
+        ],
+        details: bool = True,
     ) -> dict[str, Any]:
         result: dict = {
             "node_indicator": clazz.node_indicator(),
         }
         if details:
             result["config"] = clazz.get_config_schemas()
         return result
@@ -522,7 +557,24 @@
         for node in self.hierarchy_root.iter_all_nodes():
             mm_node = Node(node.name)
             nodes.append(mm_node)
             mm_nodes_map[node.name] = mm_node
             for child in node.children:
                 links.append(Link(mm_node, mm_nodes_map[child.name]))
         return str(MermaidDiagram(nodes=nodes, links=links, orientation="top-down"))
+
+    def get_simplified_hierarchy(
+        self, print_it: bool = False
+    ) -> dict[str, Optional[dict[str, Any]]]:
+        def rec_nodes(node: BasicTreeNode) -> dict[str, Optional[dict[str, Any]]]:
+            res = {}
+            if node.children:
+                for child in node.children:
+                    res.update(rec_nodes(child))
+                return {node.name: res}
+            else:
+                return {node.name: None}
+
+        result = rec_nodes(self.hierarchy_root)
+        if print_it:
+            print(json.dumps(result, indent=2, ensure_ascii=False))
+        return result
```

### Comparing `enbios-2.2.8/enbios/base/experiment_io.py` & `enbios-2.2.9/enbios/base/experiment_io.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from os import PathLike
 from typing import Union, Optional
 
-from flatten_dict import unflatten
 from frictionless import Schema
 from frictionless.fields import NumberField, StringField
 
+from enbios.base.tree_operations import csv2hierarchy
 from enbios.generic.files import ReadPath
-from enbios.models.experiment_base_models import (
+from enbios.models.models import (
     ExperimentData,
     ExperimentHierarchyNodeData,
     ExperimentScenarioData,
     ExperimentDataResolved,
-    # ExperimentMethodData,
 )
+from enbios.util.flatten_dict.flatten_dict import unflatten
 
 activities_schema = Schema(
     fields=[
         StringField(name="alias"),
         StringField(name="database"),
         StringField(name="code"),
         StringField(name="name"),
@@ -74,16 +74,16 @@
     # hierarchy
     if isinstance(raw_input.hierarchy, str) or isinstance(raw_input.hierarchy, PathLike):
         hierarchy_file: ReadPath = get_abs_path(
             raw_input.hierarchy, raw_input.config.base_directory
         )
         if hierarchy_file.suffix == ".json":
             hierarchy_data = hierarchy_file.read_data()
-        # elif hierarchy_file.suffix == ".csv":
-        #     hierarchy_data = csv_tree2dict(hierarchy_file, False)
+        elif hierarchy_file.suffix == ".csv":
+            hierarchy_data = csv2hierarchy(hierarchy_file)
         else:
             raise Exception(f"Invalid hierarchy file: {raw_input.hierarchy}")
 
         raw_input.hierarchy = ExperimentHierarchyNodeData(**hierarchy_data)
 
     # scenarios
     if isinstance(raw_input.scenarios, str) or isinstance(raw_input.scenarios, PathLike):
```

### Comparing `enbios-2.2.8/enbios/base/plot_experiment.py` & `enbios-2.2.9/enbios/base/plot_experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pandas import DataFrame
 
 from enbios.base.experiment import Experiment
 from enbios.base.result_select import ResultsSelector
 from enbios.generic.enbios2_logging import get_logger
 from enbios.generic.files import PathLike
 from enbios.generic.tree.basic_tree import BasicTreeNode
-from enbios.models.experiment_models import ScenarioResultNodeData
+from enbios import ScenarioResultNodeData
 
 logger = get_logger(__name__)
 
 
 def bar_plot(
     experiment: Union[Experiment, ResultsSelector],
     scenarios: Optional[list[str]] = None,
@@ -216,15 +216,15 @@
     labels = rs.method_label_names(False)
 
     # Create figure and axes
     fig, ax = plt.subplots(figsize=(6, 6), subplot_kw=dict(polar=True))
 
     cmap = plt.colormaps.get_cmap("tab10")
     angles = 0
-    for idx, scenario_name in enumerate(scenarios):
+    for idx, scenario_name in enumerate(scenarios or []):
         values = df.loc[df["scenario"] == scenario_name].values.tolist()[0][1:]
         values.append(values[0])
 
         angles = np.linspace(0, 2 * np.pi, len(values) - 1, endpoint=False).tolist()
         angles.append(0)
 
         _color = list(cmap(idx)[:3]) + [0.3]
@@ -288,16 +288,16 @@
                     va="center",
                     color="black",
                 )
         return ax
 
     df = df.set_index("scenario").transpose()
 
+    fig: Figure
     fig, ax = plt.subplots(figsize=(len(rs.scenarios) * 1.5, len(rs.method_names) * 1.5))
-    fig: Figure = fig
     set_plot_settings(ax, df, rs)
     plot_values_on_grid(ax, df, rs)
     fig.tight_layout()
     if image_file:
         fig.savefig(Path(image_file).as_posix())
     return fig
 
@@ -397,15 +397,14 @@
     level: int = 1,
     methods: Optional[list[str]] = None,
     nodes: Optional[list[str]] = None,
     image_file: Optional[PathLike] = None,
     err_method: Optional[Callable[[np.ndarray], float]] = None,
 ):
     rs = ResultsSelector.get_result_selector(experiment, scenarios, methods)
-    experiment = rs.experiment
 
     nodes = rs.validate_node_selection(level, nodes)
 
     n_rows = len(rs.method_names) * len(rs.scenarios)
     n_cols = 1
 
     fig, axs = plt.subplots(
```

### Comparing `enbios-2.2.8/enbios/base/pydantic_experiment_validation.py` & `enbios-2.2.9/enbios/base/pydantic_experiment_validation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import sys
 
 from pydantic import ValidationError
 
-from enbios.models.experiment_base_models import (
+from enbios.models.models import (
     ExperimentData,
     ExperimentHierarchyNodeData,
     ExperimentScenarioData,
 )
 
 
 def validate_experiment_data(data: dict) -> ExperimentData:
     try:
-        return ExperimentData(**data)
+        return ExperimentData.model_validate(data)
     except ValidationError as err:
         print(err)
 
         try:
-            ExperimentHierarchyNodeData(**data.get("hierarchy"))
+            ExperimentHierarchyNodeData.model_validate(data.get("hierarchy"))
             print("\nHierarchy is valid\n")
         except ValidationError as err:
             print(err)
             print(f"!!!\n!!!\nCheck: 'hierarchy': {err.errors()}\n\n")
+            sys.exit(1)
 
         if scenarios := data.get("scenarios"):
             for idx, scenario in enumerate(scenarios):
                 try:
                     sc = ExperimentScenarioData(**scenario)
                     print(f"Scenario {idx} ({sc.name}) is valid")
                 except ValidationError as err:
```

### Comparing `enbios-2.2.8/enbios/base/result_select.py` & `enbios-2.2.9/enbios/base/result_select.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,23 +22,23 @@
         Initialize the object with experiment, scenarios, and methods.
 
         :param experiment: The Experiment object.
         :param scenarios: A list of scenario names. If None, all scenario names from the experiment will be used.
         :param methods: A list of method names. If None, all method names from the experiment will be used.
         """
         self.experiment = experiment
-
+        self.scenarios: list[str]
         all_scenarios = [sc.name for sc in self.experiment.scenarios]
         if scenarios is not None:
             for scenario in scenarios:
                 if scenario not in all_scenarios:
                     raise ValueError(f"Scenario {scenario} not found in experiment")
-            self.scenarios: list[str] = scenarios
+            self.scenarios = scenarios
         else:
-            self.scenarios: list[str] = all_scenarios
+            self.scenarios = all_scenarios
 
         all_methods: list[str] = self.experiment.method_names
 
         all_method_names: list[str] = self.experiment.method_names
         self.methods: list[str] = []
         self.method_names: list[str] = []
         if methods is not None:
```

### Comparing `enbios-2.2.8/enbios/base/scenario.py` & `enbios-2.2.9/enbios/base/scenario.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,66 @@
 import concurrent.futures
-import json
 import math
 import time
 from dataclasses import dataclass, field
 from datetime import timedelta
-from typing import Optional, Union, TYPE_CHECKING, Any, Callable
+from typing import Optional, Union, TYPE_CHECKING, Any, Callable, cast
 
 from enbios.base.tree_operations import validate_experiment_reference_hierarchy
 from enbios.generic.enbios2_logging import get_logger
 from enbios.generic.files import PathLike
-from enbios.models.experiment_base_models import (
+from enbios.models.models import (
     HierarchyNodeReference,
     ScenarioConfig,
     NodeOutput,
+    TechTreeNodeData,
+    ResultValue,
+    ScenarioResultNodeData,
 )
 
 # for type hinting
 if TYPE_CHECKING:
     from enbios.base.experiment import Experiment
 from enbios.generic.tree.basic_tree import BasicTreeNode
-from enbios.models.experiment_models import (
-    ScenarioResultNodeData,
-    ResultValue,
-    TechTreeNodeData,
-)
 
 logger = get_logger(__name__)
 
 
 @dataclass
 class Scenario:
     experiment: "Experiment"
     name: str
     result_tree: BasicTreeNode[ScenarioResultNodeData]
 
     _has_run: bool = False
     # this should be a simpler type - just str: float
-    structural_nodes_outputs: dict[str, float] = field(default_factory=dict)
+    # structural_nodes_outputs: dict[str, float] = field(default_factory=dict)
     # methods: Optional[dict[str, ExperimentMethodPrepData]] = None
     _execution_time: float = float("NaN")
-    config: ScenarioConfig = field(default_factory=ScenarioConfig)
+    config: ScenarioConfig = field(default_factory=ScenarioConfig)  # type: ignore
 
     def prepare_tree(self):
         """Prepare the result tree for calculating scenario outputs.
         This populates the result tree with ScenarioResultNodeData objects
         for each node, which store the output magnitude and units.
         If config is set, it also stores the BW node dict with the node.
         """
 
-        structural_nodes_names = list(self.structural_nodes_outputs.keys())
+        structural_nodes_names = list(n.name for n in self.result_tree.iter_leaves())
+
         for result_index, node_name in enumerate(structural_nodes_names):
             try:
                 structural_result_node = self.result_tree.find_subnode_by_name(node_name)
             except StopIteration:
                 raise ValueError(f"Node {node_name} not found in result tree")
             structural_node = self.experiment.get_structural_node(node_name)
-            structural_result_node.data.output = NodeOutput(
-                unit=self.experiment.get_node_adapter(
-                    structural_node
-                ).get_node_output_unit(node_name),
-                magnitude=self.structural_nodes_outputs[node_name],
-            )
-            # todo adapter/aggregator specific additional data
-            # if self.experiment.config.include_bw_activity_in_nodes:
-            #     node_node.data.bw_activity = bw_activity
+            # todo: should be dealt returned by the adapter...
+            structural_result_node.data.output = self.experiment.get_node_adapter(
+                structural_node
+            ).get_node_output(structural_node.name, self.name)
 
         if self.config.exclude_defaults:
 
             def remove_empty_nodes(
                 node: BasicTreeNode[ScenarioResultNodeData], cancel_parents_of: set[str]
             ):
                 # aggregators without children are not needed
@@ -89,54 +82,59 @@
             depth_first=True,
             scenario_name=self.name,
             cancel_parents_of=set(),
         )
 
     @staticmethod
     def _propagate_results_upwards(
-        node: BasicTreeNode[ScenarioResultNodeData], experiment: "Experiment"
+        node: BasicTreeNode[ScenarioResultNodeData],
+        experiment: "Experiment",
+        *,
+        include_extras: bool = True,
     ):
         if node.is_leaf:
             return
         else:
-            node.data.results = experiment.get_node_aggregator(
-                node
-            ).aggregate_node_result(node)
+            aggregator = experiment.get_node_aggregator(node)
+            node.data.results = aggregator.aggregate_node_result(node)
+            if include_extras:
+                node.data.extras = aggregator.result_extras(node.name)
 
     def run(
-        self, results_as_dict: bool = True
+        self, results_as_dict: bool = True, include_extras: bool = True
     ) -> Union[BasicTreeNode[ScenarioResultNodeData], dict]:
         # if not self._get_methods():
         #     raise ValueError(f"Scenario '{self.name}' has no methods")
         logger.info(f"Running scenario '{self.name}'")
         # distributions_config = self.experiment.config.use_k_bw_distributions
         # distribution_results = distributions_config > 1
         start_time = time.time()
 
         if self.experiment.config.run_adapters_concurrently:
             # Create a ThreadPoolExecutor
             with concurrent.futures.ThreadPoolExecutor() as executor:
                 # Use a list comprehension to start a thread for each adapter
                 futures = [
-                    executor.submit(adapter.run_scenario, self)
+                    executor.submit(adapter.run_scenario, self)  # type: ignore
                     for adapter in self.experiment.adapters
                 ]
                 # As each future completes, set the results
                 for future in concurrent.futures.as_completed(futures):
                     result_data = future.result()
-                    self.set_results(result_data)
+                    self.set_results(result_data, include_extras)
         else:
             for adapter in self.experiment.adapters:
                 # run in parallel:
-                result_data = adapter.run_scenario(self)
-                self.set_results(result_data)
+                result_data = adapter.run_scenario(self)  # type: ignore
+                self.set_results(result_data, include_extras)
 
         self.result_tree.recursive_apply(
-            Scenario._propagate_results_upwards,
+            Scenario._propagate_results_upwards,  # type: ignore
             experiment=self.experiment,
+            include_extras=include_extras,
             depth_first=True,
         )
 
         self._has_run = True
         self._execution_time = time.time() - start_time
         return self.result_to_dict() if results_as_dict else self.result_tree
 
@@ -146,86 +144,118 @@
             return str(timedelta(seconds=int(self._execution_time)))
         else:
             return "not run"
 
     def reset_execution_time(self):
         self._execution_time = float("NaN")
 
-    def set_results(self, result_data: dict[str, Any]):
+    def set_results(self, result_data: dict[str, Any], include_extras: bool = True):
+        from enbios.base.adapters_aggregators.adapter import EnbiosAdapter
+
         for node_name, node_result in result_data.items():
             node = self.result_tree.find_subnode_by_name(node_name)
             if not node:
                 if self.config.exclude_defaults:
                     logger.warning(
                         f"Structural node '{node_name}' not found in result tree. "
                         f"Make sure that the adapter for does not generate results for default"
                         f"nodes that are not in the scenario."
                     )
                 else:
                     logger.error(f"Node '{node_name}' not found in result tree")
                 continue
             node.data.results = node_result
+            if include_extras:
+                node.data.extras = cast(
+                    EnbiosAdapter, self.experiment.get_node_adapter(node)
+                ).result_extras(node.name)
+        if self.config.exclude_defaults:
+            for leave in self.result_tree.iter_leaves():
+                if not leave.data.results:
+                    parent = leave.parent
+                    leave.remove_self()
+                    while parent:
+                        if parent.get_num_children() == 0:
+                            node = parent
+                            parent = parent.parent
+                            node.remove_self()
+                        else:
+                            break
 
     @staticmethod
     def wrapper_data_serializer(
-        include_output: bool = True, expand_results: bool = False
+        *,
+        include_output: bool = True,
+        include_method_units: bool = True,
+        include_extras: bool = True,
     ) -> Callable[[ScenarioResultNodeData], dict]:
         def _expand_results(results: dict[str, ResultValue]) -> dict:
             """
             brings all results to the data level (one down) which is useful for csv
             :param results:
             :return:
             """
             expanded_results = {}
             for method_name, result_value in results.items():
-                expanded_results[f"{method_name}_magnitude ({result_value.unit})"] = (
-                    result_value.magnitude
+                expanded_results[method_name] = result_value.model_dump(
+                    exclude_defaults=True,
+                    exclude_unset=True,
+                    exclude={} if include_method_units else {"unit"},
                 )
-                if result_value.multi_magnitude:
-                    for idx, magnitude in enumerate(result_value.multi_magnitude):
-                        expanded_results[f"{method_name}_{result_value.unit}_{idx}"] = (
-                            magnitude
-                        )
             return expanded_results
 
         def data_serializer(data: ScenarioResultNodeData) -> dict:
-            if expand_results:
-                result: dict[str, Any] = _expand_results(data.results)
-            else:
-                result: dict[str, Any] = {
-                    "results": {
-                        method_name: result_value.model_dump(exclude_defaults=True)
-                        for method_name, result_value in data.results.items()
-                    }
-                }
-            # there might be no output, when the units dont match
-            if include_output and data.output:
-                if expand_results:
-                    result["output_unit"] = data.output.unit
-                    result["output_magnitude"] = data.output.magnitude
-                else:
-                    result["output"] = data.output.model_dump()
-            # todo: adapter specific additional data
-            # if data.bw_activity:
-            #     result["bw_activity"] = data.bw_activity["code"]
-
+            result: dict[str, Any] = {}
+            result["results"] = _expand_results(data.results)
+            # there might be no output, when the units don't match
+            if include_output:
+                result["output"] = [output.model_dump() for output in data.output]
+            if include_extras and data.extras:
+                extras: dict[str, Any] = data.extras
+                for k in ["name", "results", "output"]:
+                    if k in extras:
+                        logger.warning(
+                            f"node result extras contain key '{k}', which is reserved for the scenario result"
+                        )
+                        extras.pop(k)
+                result.update(extras)
             return result
 
         return data_serializer
 
+    @staticmethod
+    def wrapped_flat_output_list_serializer(
+        serializer: Callable[[ScenarioResultNodeData], dict]
+    ) -> Callable[[ScenarioResultNodeData], dict]:
+        import flatten_dict
+
+        def flattened_wrap(result_data: ScenarioResultNodeData) -> dict:
+            res = serializer(result_data)
+            return flatten_dict.flatten(res, reducer="underscore", enumerate_types={list})
+
+        return flattened_wrap
+
     def results_to_csv(
         self,
         file_path: PathLike,
         level_names: Optional[list[str]] = None,
+        include_output: bool = True,
         include_method_units: bool = True,
         warn_no_results: bool = True,
         alternative_hierarchy: Optional[dict] = None,
+        flat_hierarchy: Optional[bool] = False,
+        repeat_parent_name: bool = False,
+        include_extras: bool = True,
     ):
         """
         Save the results (as tree) to a csv file
+         :param include_extras:
+         :param repeat_parent_name:
+         :param flat_hierarchy:
+         :param include_output:
          :param warn_no_results:
          :param file_path:  path to save the results to
          :param level_names: names of the levels to include in the csv
          (must not match length of levels)
          :param alternative_hierarchy: An alternative hierarchy to use for the results,
           which comes from Scenario.rearrange_results.
          :param include_method_units:
@@ -240,36 +270,47 @@
         if alternative_hierarchy:
             use_tree = self._rearrange_results(alternative_hierarchy)
 
         use_tree.to_csv(
             file_path,
             include_data=True,
             level_names=level_names,
-            data_serializer=self.wrapper_data_serializer(include_method_units, True),
+            data_serializer=self.wrapped_flat_output_list_serializer(
+                self.wrapper_data_serializer(
+                    include_output=include_output,
+                    include_method_units=include_method_units,
+                    include_extras=include_extras,
+                )
+            ),
+            repeat_parent_name=repeat_parent_name,
+            flat_hierarchy=flat_hierarchy,
         )
 
     def result_to_dict(
         self,
         include_output: bool = True,
         warn_no_results: bool = True,
-        alternative_hierarchy: dict = None,
+        alternative_hierarchy: Optional[dict] = None,
     ) -> dict[str, Any]:
         """
         Return the results as a dictionary
         :param include_output:
         :param warn_no_results:
         :param alternative_hierarchy: An alternative hierarchy to use for the results,
         which comes from Scenario.rearrange_results.
         :return:
         """
 
+        # todo params for result_units, extras
         def recursive_transform(node: BasicTreeNode[ScenarioResultNodeData]) -> dict:
             result: dict[str, Any] = {
                 "name": node.name,
-                **Scenario.wrapper_data_serializer(include_output)(node.data),
+                **Scenario.wrapper_data_serializer(include_output=include_output)(
+                    node.data
+                ),
             }
             if node.children:
                 result["children"] = [
                     recursive_transform(child) for child in node.children
                 ]
             return result
 
@@ -282,29 +323,29 @@
             return recursive_transform(self.result_tree.copy())
 
     def _rearrange_results(
         self, hierarchy: dict
     ) -> BasicTreeNode[ScenarioResultNodeData]:
         hierarchy_obj = HierarchyNodeReference(**hierarchy)
 
-        hierarchy_root: BasicTreeNode[TechTreeNodeData] = (
-            validate_experiment_reference_hierarchy(
-                hierarchy_obj,
-                self.experiment.hierarchy_root,
-                self.experiment.get_node_aggregator,
-            )
+        hierarchy_root: BasicTreeNode[
+            TechTreeNodeData
+        ] = validate_experiment_reference_hierarchy(
+            hierarchy_obj,
+            self.experiment.hierarchy_root,
+            self.experiment.get_node_aggregator,
         )
 
         def recursive_convert(
             node_: BasicTreeNode[TechTreeNodeData],
         ) -> BasicTreeNode[ScenarioResultNodeData]:
-            output: Optional[NodeOutput] = None
-            results = {}
+            output: list[NodeOutput] = []
+            results: dict = {}
             if node_.is_leaf:
-                calc_data = self.result_tree.find_subnode_by_name(node_.name).data
+                calc_data = self.result_tree.find_subnode_by_name(node_.name).data  # type: ignore
                 output = calc_data.output
                 results = calc_data.results
             return BasicTreeNode(
                 name=node_.name,
                 data=ScenarioResultNodeData(
                     output=output,
                     results=results,
@@ -317,32 +358,36 @@
         result_tree: BasicTreeNode[ScenarioResultNodeData] = recursive_convert(
             hierarchy_root
         )
 
         from enbios.base.tree_operations import recursive_resolve_outputs
 
         result_tree.recursive_apply(
-            recursive_resolve_outputs,
+            recursive_resolve_outputs,  # type: ignore
             experiment=self.experiment,
             depth_first=True,
             cancel_parents_of=set(),
         )
 
         result_tree.recursive_apply(
-            Scenario._propagate_results_upwards,
+            Scenario._propagate_results_upwards,  # type: ignore
             experiment=self.experiment,
             depth_first=True,
         )
 
         return result_tree
 
     def get_execution_time(self) -> float:
         return self._execution_time
 
     def __repr__(self):
         return f"<Scenario '{self.name}'>"
 
     def describe(self):
         output = f"Scenario '{self.name}'\n"
-        output += json.dumps(self.structural_nodes_outputs, indent=2)
+        # output += json.dumps(self.structural_nodes_outputs, indent=2)
         # todo: the tree instead...
         return output
+
+    @property
+    def has_run(self):
+        return self._has_run
```

### Comparing `enbios-2.2.8/enbios/base/unit_registry.py` & `enbios-2.2.9/enbios/base/unit_registry.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,8 +11,10 @@
         f"Creating 'ecoinvent_pint_unit_match' file at: "
         f"{ecoinvent_units_file_path.as_posix()}"
     )
     ecoinvent_units_file_path.touch()
     ecoinvent_units_file_path.write_text("unspecificEcoinventUnit = []\n")
 
 ureg.load_definitions(ecoinvent_units_file_path)
+
+
 # print("loaded ecoinvent units")
```

### Comparing `enbios-2.2.8/enbios/base/validation.py` & `enbios-2.2.9/enbios/base/validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 
 from enbios.base.adapters_aggregators.adapter import EnbiosAdapter
 from enbios.base.adapters_aggregators.aggregator import EnbiosAggregator
 from enbios.base.adapters_aggregators.builtin import BUILTIN_AGGREGATORS
 from enbios.base.adapters_aggregators.loader import load_adapter, load_aggregator
 from enbios.base.scenario import Scenario
 from enbios.models.environment_model import Settings
-from enbios.models.experiment_base_models import (
+from enbios.models.models import (
     ExperimentConfig,
     ExperimentScenarioData,
-    NodeOutput,
     AdapterModel,
     AggregationModel,
 )
 
 if TYPE_CHECKING:
     from enbios.base.experiment import Experiment
 
@@ -55,17 +54,17 @@
     aggregators = []
     for aggregator_def in experiment_aggregators:
         aggregator = load_aggregator(aggregator_def)
         aggregator.validate_config(aggregator_def.config)
         aggregators.append(aggregator)
 
     aggregator_names = [a.name() for a in aggregators]
-    for builtin_name, aggregator in BUILTIN_AGGREGATORS.items():
+    for builtin_name, aggregator_class in BUILTIN_AGGREGATORS.items():
         if builtin_name not in aggregator_names:
-            aggregator = aggregator()
+            aggregator = aggregator_class()
 
             aggregators.append(aggregator)
 
     return {aggregator.name(): aggregator for aggregator in aggregators}
 
 
 def validate_scenarios(
@@ -73,15 +72,17 @@
     default_scenario_name: str,
     experiment: "Experiment",
 ) -> list[Scenario]:
     scenarios: list[Scenario] = []
 
     # undefined scenarios. just one default scenario
     if not experiment_scenarios:
-        experiment_scenarios = [ExperimentScenarioData(name=default_scenario_name)]
+        experiment_scenarios = [
+            ExperimentScenarioData(name=default_scenario_name, nodes={})
+        ]
 
     # set names if not given
     for index, scenario_data in enumerate(experiment_scenarios):
         scenario_data.name_factory(index)
 
     # check for name duplicates
     name_count = Counter([s.name for s in experiment_scenarios])
@@ -105,41 +106,43 @@
     :param scenario_data:
     :param experiment:
     :return:
     """
 
     def validate_nodes(scenario_: ExperimentScenarioData) -> dict[str, float]:
         nodes = scenario_.nodes or {}
-        result: dict[str, float] = {}
+        outputs: dict[str, float] = {}
 
         for node_name_, node_output in nodes.items():
             node_ = experiment.get_structural_node(node_name_)
             adapter = experiment.get_node_adapter(node_)
+            outputs[node_name_] = adapter.validate_scenario_node(
+                node_name_, str(scenario_.name), node_output
+            )
+        return outputs
 
-            if isinstance(node_output, dict):
-                node_output = NodeOutput(**node_output)
-            result[node_name_] = adapter.validate_node_output(node_name_, node_output)
-        return result
-
-    scenario_nodes_outputs: dict[str, float] = validate_nodes(scenario_data)
-    defined_nodes = list(scenario_nodes_outputs.keys())
+    validate_nodes(scenario_data)
 
     # fill up the missing activities with default values
-    if not scenario_data.config.exclude_defaults:
-        for node_name in experiment.structural_nodes_names:
-            if node_name not in defined_nodes:
-                node = experiment.get_structural_node(node_name)
-                scenario_nodes_outputs[node_name] = experiment.get_node_adapter(
-                    node
-                ).get_default_output_value(node.name)
-
+    # todo bring something like this back...make the data come from the adapter
+    # if not scenario_data.config.exclude_defaults:
+    # for node_name in experiment.structural_nodes_names:
+    #     if node_name not in scenario_data.nodes:
+    #         node = experiment.get_structural_node(node_name)
+    #         output = experiment.get_node_adapter(
+    #             node
+    #         ).get_node_output(node_name, scenario_data.name)
+    #         if not output:
+    #             raise EnbiosValidationException(
+    #                 f"No output for node {node_name} in scenario {scenario_data.name}")
+    assert scenario_data.name
     return Scenario(
         experiment=experiment,  # type: ignore
         name=scenario_data.name,
-        structural_nodes_outputs=scenario_nodes_outputs,
+        # structural_nodes_outputs=scenario_nodes_outputs,
         config=scenario_data.config,
         result_tree=experiment.base_result_tree.copy(),
     )
 
 
 def validate_run_scenario_setting(
     env_settings: Settings, experiment_config: ExperimentConfig, scenario_names: list[str]
```

### Comparing `enbios-2.2.8/enbios/bw2/brightway_experiment_adapter.py` & `enbios-2.2.9/enbios/bw2/brightway_experiment_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,111 +1,110 @@
 import math
 from logging import getLogger
-from typing import Optional, Any, Union, Sequence, Callable
+from typing import Optional, Any, Sequence, Callable
 
-import bw2data
 import bw2data as bd
+import numpy as np
 from bw2calc.dictionary_manager import ReversibleRemappableDictionary
+from bw2data import Method as Bw2Method
 from bw2data.backends import Activity, ActivityDataset
 from numpy import ndarray
 from pint import Quantity, UndefinedUnitError
+from pint.facets.plain import PlainQuantity
 from pydantic.json_schema import GenerateJsonSchema, JsonSchemaValue
 from pydantic_core import core_schema, PydanticOmit
 
-from enbios import get_enbios_ureg
 from enbios.base.adapters_aggregators.adapter import EnbiosAdapter
 from enbios.base.scenario import Scenario
+from enbios.base.unit_registry import ureg
+from enbios.bw2.MultiLCA_util import BaseStackedMultiLCA
 from enbios.bw2.bw_models import (
     ExperimentMethodPrepData,
     BWAdapterConfig,
     BrightwayActivityConfig,
     BWMethodDefinition,
     BWActivityData,
     NonLinearMethodConfig,
+    BWCalculationSetup,
 )
-from enbios.bw2.stacked_MultiLCA import StackedMultiLCA, BWCalculationSetup
-from enbios.bw2.stacked_MultiLCA_regio import RegioStackedMultiLCA
 from enbios.bw2.util import bw_unit_fix, get_activity
 from enbios.generic.util import load_module, get_module_functions
-from enbios.models.experiment_base_models import NodeOutput, AdapterModel
-from enbios.models.experiment_models import (
-    ResultValue,
-)
+from enbios.models.models import NodeOutput, AdapterModel, ResultValue
 
 logger = getLogger(__file__)
 
-ureg = get_enbios_ureg()
-
 
-def _bw_activity_search(activity_id: dict) -> Activity:
+def _bw_activity_search(config: BrightwayActivityConfig) -> Activity:
     """
     Search for the activity in the brightway project
-    :param activity_id:
+    :param config:
     :return: brightway activity
     """
-    id_ = BrightwayActivityConfig(**activity_id)
+
     bw_activity: Optional[Activity] = None
-    if id_.code:
-        if id_.database:
-            bw_activity = bd.Database(id_.database).get(id_.code)
+    if config.code:
+        if config.database:
+            bw_activity = bd.Database(config.database).get(config.code)
         else:
-            bw_activity = get_activity(id_.code)
-    elif id_.name:
+            bw_activity = get_activity(config.code)
+    elif config.name:
         filters = {}
-        search_in_dbs = [id_.database] if id_.database else bd.databases
+        search_in_dbs = [config.database] if config.database else bd.databases
         for db in search_in_dbs:
-            if id_.location:
-                filters["location"] = id_.location
-                search_results = bd.Database(db).search(id_.name, filter=filters)
+            if config.location:
+                filters["location"] = config.location
+                search_results = bd.Database(db).search(config.name, filter=filters)
             else:
-                search_results = bd.Database(db).search(id_.name)
+                search_results = bd.Database(db).search(config.name)
                 # filter exact name
                 search_results = list(
-                    filter(lambda a: a["name"] == id_.name, search_results)
+                    filter(lambda a: a["name"] == config.name, search_results)
                 )
-            if id_.unit:
+            if not search_results:
+                continue
+            if config.unit:
                 search_results = list(
-                    filter(lambda a: a["unit"] == id_.unit, search_results)
+                    filter(lambda a: a["unit"] == config.unit, search_results)
                 )
             if len(search_results) == 1:
                 bw_activity = search_results[0]
                 break
             elif len(search_results) > 1:
                 activities_str = "\n".join(
                     [f'{str(a)} - {a["code"]}' for a in search_results]
                 )
                 raise ValueError(
                     f"There are more than one activity with the same name, "
                     f"try including  "
                     f"the code of the activity you want to use:\n{activities_str}"
                 )
     if not bw_activity:
-        raise ValueError(f"No activity found for {activity_id}")
+        raise ValueError(f"No activity found for {config}")
     return bw_activity
 
 
 class BrightwayAdapter(EnbiosAdapter):
     @staticmethod
     def name() -> str:
         return "brightway-adapter"
 
     def validate_definition(self, definition: AdapterModel):
         pass
 
-    def __init__(self):
+    def __init__(self) -> None:
         super(BrightwayAdapter, self).__init__()
-        self.config: BWAdapterConfig = BWAdapterConfig(bw_project="")
+        self.config = BWAdapterConfig.model_validate({"bw_project": ""})
         self.activityMap: dict[str, BWActivityData] = {}
         self.methods: dict[str, ExperimentMethodPrepData] = {}
-        self.scenario_calc_setups: dict[str, BWCalculationSetup] = (
-            {}
-        )  # scenario_alias to BWCalculationSetup
+        self.scenario_calc_setups: dict[
+            str, BWCalculationSetup
+        ] = {}  # scenario_alias to BWCalculationSetup
         self.raw_results: dict[str, list[ndarray]] = {}  # scenario_alias to results
         self.lca_objects: dict[
-            str, list[Union[StackedMultiLCA, RegioStackedMultiLCA]]
+            str, list[BaseStackedMultiLCA]
         ] = {}  # scenario_alias to lca objects
         self.all_regions_set: bool = (
             False  # as part of first run_scenario, go through set_node_regions
         )
 
     @staticmethod
     def node_indicator() -> str:
@@ -114,15 +113,15 @@
     def assert_all_codes_unique(self):
         all_activities = list(ActivityDataset.select())
         assert len(all_activities) == len(
             set([a.code for a in all_activities])
         ), "It is recommended that all activities have unique codes"
 
     def validate_config(self, config: Optional[dict[str, Any]]):
-        self.config = BWAdapterConfig(**config)
+        self.config = BWAdapterConfig.model_validate(config)
         if self.config.use_k_bw_distributions < 1:
             raise ValueError(
                 f"config.use_k_bw_distributions must be greater than 0, "
                 f"but is {self.config.use_k_bw_distributions}"
             )
 
         if self.config.bw_project not in bd.projects:
@@ -137,20 +136,27 @@
         BWMethodDefinition.model_validate(methods)
 
         def validate_method(method_id: Sequence[str]) -> ExperimentMethodPrepData:
             # todo: should complain, if the same method is passed twice
             bw_method = bd.methods.get(method_id)
             if not bw_method:
                 raise ValueError(f"Method with id: {method_id} does not exist")
-            unit = bw_method.get("unit", "undefined method unit")
+            unit = bw_method.get("unit", None)
+            if not unit:
+                logger.warning(
+                    f"Brightway adapter: No Unit specified for method: {method_id}. "
+                    f"Setting it to: 'undefined method unit'"
+                )
+                unit = "undefined method unit"
             return ExperimentMethodPrepData(id=tuple(method_id), bw_method_unit=unit)
 
         self.methods: dict[str, ExperimentMethodPrepData] = {
             name: validate_method(method) for name, method in methods.items()
         }
+
         return list(self.methods.keys())
 
     def validate_node_output(
         self,
         node_name: str,
         target_output: NodeOutput,
     ) -> float:
@@ -177,47 +183,98 @@
             )
             raise UndefinedUnitError(f"Unit error, {err}; For activity: {node_name}")
 
     def validate_node(self, node_name: str, node_config: Any):
         assert isinstance(
             node_config, dict
         ), f"Activity id (type: dict) must be defined for activity {node_name}"
+        parsed_config = BrightwayActivityConfig(**node_config)
         # get the brightway activity
-        bw_activity = _bw_activity_search(node_config)
-
+        bw_activity = _bw_activity_search(parsed_config)
+        bw_unit = bw_unit_fix(bw_activity["unit"])
         self.activityMap[node_name] = BWActivityData(
-            bw_activity=bw_activity,
-            default_output=NodeOutput(unit=bw_unit_fix(bw_activity["unit"]), magnitude=1),
+            bw_activity=bw_activity, default_output=NodeOutput(unit=bw_unit, magnitude=1)
         )
-        if "default_output" in node_config:
-            self.activityMap[node_name].default_output.magnitude = (
-                self.validate_node_output(
-                    node_name, NodeOutput(**node_config["default_output"])
-                )
-            )
+        if default_out := parsed_config.default_output:
+            unit = bw_unit_fix(default_out.unit)
+            base_q: Quantity = ureg.parse_expression(unit) * default_out.magnitude
+            conv_q: PlainQuantity = base_q.to(bw_unit)
+            self.activityMap[node_name].default_output.from_quantity(conv_q)
         if self.config.simple_regionalization.run_regionalization:
             if "enb_location" in node_config:
                 bw_activity["enb_location"] = node_config["enb_location"]
                 bw_activity.save()
+        # todo, selective methods?
+        # if parsed_config.methods:
+        #     for m in parsed_config.methods:
+        #         if m not in self.methods:
+        #             raise ValueError(f"Brightway-Adapter: node {node_name} specifies a method that "
+        #                              f"was not defined for the adapter: {m}")
 
-    def get_default_output_value(self, node_name: str) -> float:
-        return self.activityMap[node_name].default_output.magnitude
+    def validate_scenario_node(
+        self,
+        node_name: str,
+        scenario_name: str,
+        scenario_node_data: Any,
+    ):
+        """
+        validate and convert to the bw-activity unit
+        :param node_name:
+        :param scenario_name:
+        :param scenario_node_data:
+        :return:
+        """
+        target_output_: NodeOutput = NodeOutput.model_validate(scenario_node_data)
+        try:
+            target_quantity: Quantity = (
+                ureg.parse_expression(bw_unit_fix(target_output_.unit))
+                * target_output_.magnitude
+            )
+            bw_activity_unit = self.get_node_output_unit(node_name)
+            scaled_quantity: PlainQuantity = target_quantity.to(
+                bw_unit_fix(bw_activity_unit)
+            )
+            target_output_.from_quantity(scaled_quantity)
+            self.activityMap[node_name].scenario_outputs[scenario_name] = target_output_
+            #
+        except UndefinedUnitError as err:
+            logger.error(
+                f"Cannot parse output unit '{target_output_.unit}'- "
+                f"of activity {node_name}. {err}. "
+                f"Consider the unit definition to 'enbios2/base/unit_registry.py'"
+            )
+            raise UndefinedUnitError(f"Unit error, {err}; For activity: {node_name}")
 
     def get_node_output_unit(self, node_name: str) -> str:
         return bw_unit_fix(self.activityMap[node_name].bw_activity["unit"])
 
+    def get_node_output(self, node_name: str, scenario: str) -> list[NodeOutput]:
+        # unit = bw_unit_fix(self.activityMap[node_name].bw_activity["unit"])
+        node_data = self.activityMap[node_name]
+        if scenario in self.activityMap[node_name].scenario_outputs:
+            return [node_data.scenario_outputs[scenario]]
+        else:
+            return [node_data.default_output]
+
     def get_method_unit(self, method_name: str) -> str:
         return self.methods[method_name].bw_method_unit
 
     def prepare_scenario(self, scenario: Scenario):
         inventory: list[dict[Activity, float]] = []
         for act_alias, activity in self.activityMap.items():
             try:
-                act_output = scenario.structural_nodes_outputs[act_alias]
-                inventory.append({activity.bw_activity: act_output})
+                if scenario.name in activity.scenario_outputs:
+                    act_output = activity.scenario_outputs[scenario.name].magnitude
+                    inventory.append({activity.bw_activity: act_output})
+                else:
+                    if not scenario.config.exclude_defaults:
+                        inventory.append(
+                            {activity.bw_activity: activity.default_output.magnitude}
+                        )
+
             except KeyError:
                 # todo not sure if that ever happens..
                 if not scenario.config.exclude_defaults:
                     raise Exception(
                         f"Activity {act_alias} not found in scenario {scenario.name}"
                     )
 
@@ -226,15 +283,14 @@
         calculation_setup.register()
         self.scenario_calc_setups[scenario.name] = calculation_setup
         if (
             self.config.simple_regionalization.run_regionalization
             and not self.all_regions_set
         ):
             # memorize nodes from the tree in order to not delete their location
-            keep_locations_of_activities: list[str] = []
             if self.config.simple_regionalization.clear_all_other_node_regions:
                 keep_locations_of_activities = [
                     a.bw_activity["code"] for a in self.activityMap.values()
                 ]
 
                 range_length = 1000
                 activities_to_reset = list(
@@ -284,39 +340,45 @@
 
     def run_scenario(self, scenario: Scenario) -> dict[str, dict[str, ResultValue]]:
         self.prepare_scenario(scenario)
         use_distributions = self.config.use_k_bw_distributions > 1
         raw_results: list[ndarray] = []
         self.lca_objects[scenario.name] = []
         run_regionalization = self.config.simple_regionalization.run_regionalization
+        # non-linear methods
         method_activity_func_maps: Optional[
             dict[tuple[str, ...], dict[int, Callable[[float], float]]]
         ] = None
         if self.config.nonlinear_characterization:
             method_activity_func_maps = self.prepare_nonlinear_methods()
         for i in range(self.config.use_k_bw_distributions):
             if self.config.use_k_bw_distributions > 1:
                 self.get_logger().info(
                     f"Brightway adapter: Run distribution {i + 1}/{self.config.use_k_bw_distributions}"
                 )
+            calc_setup = self.scenario_calc_setups[scenario.name]
+            result_structure = np.zeros((len(calc_setup.inv), len(calc_setup.ia)))
+            subset_labels: Optional[set[str]] = None
+            activity_label_key: Optional[str] = None
             if run_regionalization:
-                _lca = RegioStackedMultiLCA(
-                    self.scenario_calc_setups[scenario.name],
-                    self.config.simple_regionalization.select_regions,
-                    use_distributions=use_distributions,
-                    method_activity_func_maps=method_activity_func_maps,
-                )
-                raw_results.append(_lca.results)
-            else:
-                _lca = StackedMultiLCA(
-                    self.scenario_calc_setups[scenario.name],
-                    use_distributions,
-                    method_activity_func_maps=method_activity_func_maps,
-                )
-                raw_results.append(_lca.results)
+                subset_labels = self.config.simple_regionalization.select_regions
+                result_structure = np.zeros(
+                    (len(calc_setup.inv), len(calc_setup.ia), len(subset_labels))
+                )
+                activity_label_key = "enb_location"
+
+            _lca = BaseStackedMultiLCA(
+                self.scenario_calc_setups[scenario.name],
+                result_structure,
+                subset_labels,
+                activity_label_key,
+                use_distributions=use_distributions,
+                method_activity_func_maps=method_activity_func_maps,
+            )
+            raw_results.append(_lca.results)
             if self.config.store_lca_object:
                 self.lca_objects[scenario.name].append(_lca)
 
         if self.config.store_raw_results:
             self.raw_results[scenario.name] = raw_results
 
         return self._assign_results2nodes(
@@ -328,44 +390,47 @@
         raw_results: list[ndarray],
         scenario: Scenario,
         use_distributions: bool,
         has_regionalization: bool,
     ):
         result_data: dict[str, Any] = {}
         for act_idx, act_alias in enumerate(self.activityMap.keys()):
-            if act_alias not in scenario.structural_nodes_outputs:
-                if not scenario.config.exclude_defaults:
-                    raise ValueError(
-                        f"Activity {act_alias} not found in scenario {scenario.name}"
-                    )
+            if (
+                scenario.name not in self.activityMap[act_alias].scenario_outputs
+                and scenario.config.exclude_defaults
+            ):
                 continue
             result_data[act_alias] = {}
             result_field = "multi_magnitude" if use_distributions else "magnitude"
             for m_idx, method in enumerate(self.methods.items()):
                 method_name, method_data = method
                 if has_regionalization:
                     for region_idx, region in enumerate(
                         self.config.simple_regionalization.select_regions
                     ):
-                        method_result = ResultValue(unit=method_data.bw_method_unit)
+                        method_result = ResultValue.model_validate(
+                            {"unit": method_data.bw_method_unit}
+                        )
                         method_res_values = [
                             res[act_idx, m_idx, region_idx] for res in raw_results
                         ]
                         setattr(
                             method_result,
                             result_field,
                             (
                                 method_res_values
                                 if use_distributions
                                 else method_res_values[0]
                             ),
                         )
                         result_data[act_alias][f"{method_name}.{region}"] = method_result
                 else:
-                    method_result = ResultValue(unit=method_data.bw_method_unit)
+                    method_result = ResultValue.model_validate(
+                        {"unit": method_data.bw_method_unit}
+                    )
                     method_res_values = [res[act_idx, m_idx] for res in raw_results]
                     setattr(
                         method_result,
                         result_field,
                         method_res_values if use_distributions else method_res_values[0],
                     )
                     result_data[act_alias][method_name] = method_result
@@ -383,40 +448,42 @@
             bw_method_id = self.methods[method_name].id
             method_activity2func_maps[bw_method_id] = method_activity2func_map
         return method_activity2func_maps
 
     def prepare_nonlinear_method(
         self, method_name: str, method_config: NonLinearMethodConfig
     ) -> dict[int, Callable[[float], float]]:
-        result_func_map: dict[int, Callable[[float], float]] = (
-            {}
-        )  # [None] * prep_lca.biosphere_matrix.shape[0]
+        result_func_map: dict[
+            int, Callable[[float], float]
+        ] = {}  # [None] * prep_lca.biosphere_matrix.shape[0]
         if method_name not in self.methods:
             raise ValueError(
                 f"Unknown method '{method_name}' specified for nonlinear methods"
             )
         # bw method id (tuple[str,...])
         bw_method_id: tuple[str, ...] = self.methods[method_name].id
         if method_config.module_path_function_name:
             module_path, func_name = method_config.module_path_function_name
-            func: Callable = get_module_functions(load_module(module_path)).get(func_name)
+            func: Optional[Callable] = get_module_functions(load_module(module_path)).get(
+                func_name
+            )
             if not func:
                 raise ValueError(
                     f"Could not find function: '{func_name} in module: {module_path}, which is defined for"
                     f"brightway-adapter non-linear method definition for method: {method_name}"
                 )
             method_config.functions = func()
         # key: (database,code) -> id
         biosphere_keys2ids = self.activities_keys_id_map(
             list(method_config.functions.keys())
         )
         for key, id_ in biosphere_keys2ids.items():
             result_func_map[id_] = method_config.functions[key]
         if method_config.get_defaults_from_original:
-            bw_method_data = bw2data.Method(bw_method_id).load()
+            bw_method_data = Bw2Method(bw_method_id).load()
             bw_cf_activity_key2ids = self.activities_keys_id_map(
                 [tuple[str, str](method_key) for method_key, _ in bw_method_data]
             )
             for method_key, cf in bw_method_data:
                 activity_id = bw_cf_activity_key2ids[tuple(method_key)]
                 result_func_map[activity_id] = lambda v, cf_=cf: v * cf_
         return result_func_map
@@ -450,7 +517,10 @@
         biosphere_activities = list(
             ActivityDataset.select().where(ActivityDataset.code.in_(codes))
         )
         # noinspection PyUnresolvedReferences
         return ReversibleRemappableDictionary(
             {(a.database, a.code): a.id for a in biosphere_activities}
         )
+
+    def result_extras(self, node_name: str) -> dict:
+        return {"bw_activity_code": self.activityMap[node_name].bw_activity["code"]}
```

### Comparing `enbios-2.2.8/enbios/bw2/bw_models.py` & `enbios-2.2.9/enbios/bw2/bw_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,36 +2,35 @@
 from typing import Any, Optional, Callable, Sequence
 
 import bw2data
 from bw2data.backends import Activity
 from pydantic import BaseModel, ConfigDict, Field, model_validator, RootModel
 
 from enbios.generic.enbios2_logging import get_logger
-from enbios.models.experiment_base_models import NodeOutput
+from enbios.models.models import NodeOutput
 
 logger = get_logger(__name__)
 
 
 class ExperimentMethodPrepData(BaseModel):
     id: tuple[str, ...]
     bw_method_unit: str
 
 
 class RegionalizationConfig(BaseModel):
     model_config = ConfigDict(extra="forbid", validate_assignment=True, strict=True)
     run_regionalization: bool = Field(False)
-    select_regions: set = Field(None, description="regions to store the results for")
+    select_regions: set[str] = Field(None, description="regions to store the results for")
     set_node_regions: dict[str, Sequence[str]] = Field({}, description="Set node regions")
     clear_all_other_node_regions: Optional[bool] = Field(
         False, description="Delete all regions not in 'hierarchy' and 'set_node_regions'"
     )
 
     @model_validator(mode="before")
-    @classmethod
-    def validate(cls, data: Any) -> Any:
+    def validate(data: Any):
         if data.get("run_regionalization", False):
             if data.get("select_regions") is None:
                 raise ValueError(
                     "Select regions missing for BW regionalization (field: 'select_regions')"
                 )
         return data
 
@@ -50,16 +49,15 @@
     default_function: Callable[[float], float] = Field(None, init_var=False)
     get_defaults_from_original: Optional[bool] = Field(
         False,
         description="Method is already defined in BW and has characterization values. ",
     )
 
     @model_validator(mode="before")
-    @classmethod
-    def check_defaults(self, data: dict):
+    def check_defaults(data: dict):
         has_default_function = data.get("default_function")
         has_get_defaults_from_original = data.get("get_defaults_from_original", False)
         if has_default_function and has_get_defaults_from_original:
             logger.warning(
                 f"brightway nonlinear method config for method '{data['name']}' should only have one"
                 f"'default_function' or 'get_defaults_from_original'. Using 'default_function'"
             )
@@ -77,34 +75,23 @@
         has_module_path_function_name = data.get("module_path_function_name")
         if not has_functions and not has_module_path_function_name:
             raise ValueError(
                 "Either 'functions' or 'module_path_function_name' must be present."
             )
         return data
 
-    # @classmethod
-    # def model_json_schema(cls):
-    #     # Generate the default schema
-    #     schema = super().model_json_schema()
-    #
-    #     # Modify the schema for the 'functions' field
-    #     # For example, represent it as a dictionary of strings
-    #     schema['properties']['functions'] = {'type': 'object', 'additionalProperties': {'type': 'string'}}
-    #     return schema
-
 
 class NonLinearCharacterizationConfig(BaseModel):
     methods: dict[str, NonLinearMethodConfig] = Field(
         ...,
         description="Non linear characterization. "
         "Nested Dictionary: method_name > NonLinearMethodConfig",
     )
 
     @model_validator(mode="before")
-    @classmethod
     def add_method_names(cls, data):
         for method_name, method_config in data["methods"].items():
             method_config["name"] = method_name
         return data
 
 
 class BWAdapterConfig(BaseModel):
@@ -121,15 +108,15 @@
     )
     store_lca_object: bool = Field(
         False,
         description="If the LCA object should be stored. "
         "Will be stored in `lca_objects[scenario.name]`",
     )
     simple_regionalization: RegionalizationConfig = Field(
-        description="Generate regionalized LCA", default_factory=RegionalizationConfig
+        description="Generate regionalized LCA", default_factory=RegionalizationConfig  # type: ignore
     )
     nonlinear_characterization: Optional[NonLinearCharacterizationConfig] = Field(
         None, description="Nonlinear characterization"
     )
 
 
 class BrightwayActivityConfig(BaseModel):
@@ -149,14 +136,15 @@
     )
     # additional filter
     unit: str = Field(None, description="Search: unit filter of results")  # unit
     # internal-name
     default_output: NodeOutput = Field(
         None, description="Default output of the activity for all scenarios"
     )
+    methods: list[str] = Field(None, description="Subset of all methods")
 
 
 class BWMethodModel(BaseModel):
     name: str = Field(None, description="Name for identification")
     id: tuple[str, ...] = Field(None, description="Brightway method id")
 
 
@@ -164,18 +152,19 @@
     model_config = ConfigDict(
         title="Method definition",
         json_schema_extra={"description": "Simply a dict: name : BW method tuple"},
     )
     root: dict[str, Sequence[str]]
 
 
-@dataclass
-class BWActivityData:
+class BWActivityData(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True)
     bw_activity: Activity
     default_output: NodeOutput
+    scenario_outputs: dict[str, NodeOutput] = Field(default_factory=dict)
 
 
 @dataclass
 class BWCalculationSetup:
     name: str
     inv: list[dict[Activity, float]]
     ia: list[tuple[str, ...]]
```

### Comparing `enbios-2.2.8/enbios/bw2/check_bw_acts_normal.py` & `enbios-2.2.9/enbios/bw2/check_bw_acts_normal.py`

 * *Files identical despite different names*

### Comparing `enbios-2.2.8/enbios/bw2/import_ecoinvent.py` & `enbios-2.2.9/enbios/bw2/import_ecoinvent.py`

 * *Files identical despite different names*

### Comparing `enbios-2.2.8/enbios/bw2/regionalization.py` & `enbios-2.2.9/enbios/bw2/regionalization.py`

 * *Files identical despite different names*

### Comparing `enbios-2.2.8/enbios/bw2/resolve_lca_bioflows.py` & `enbios-2.2.9/enbios/bw2/resolve_lca_bioflows.py`

 * *Files identical despite different names*

### Comparing `enbios-2.2.8/enbios/bw2/util.py` & `enbios-2.2.9/enbios/bw2/util.py`

 * *Files identical despite different names*

### Comparing `enbios-2.2.8/enbios/dev/create_experiment_schema.py` & `enbios-2.2.9/enbios/dev/create_experiment_schema.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from pathlib import Path
 
 from enbios.generic.enbios2_logging import get_logger, get_module_name
-from enbios.models.experiment_base_models import ExperimentData
+from enbios.models.models import ExperimentData
 
 logger = get_logger(get_module_name(__file__))
 
 
 def create_experiment_schema():
     schema_file_path = Path(__file__).parent.parent.parent / "data/schema/experiment.schema.gen.json"
     schema_file_path.write_text(
```

### Comparing `enbios-2.2.8/enbios/generic/enbios2_logging.py` & `enbios-2.2.9/enbios/generic/enbios2_logging.py`

 * *Files identical despite different names*

### Comparing `enbios-2.2.8/enbios/generic/files.py` & `enbios-2.2.9/enbios/generic/files.py`

 * *Files identical despite different names*

### Comparing `enbios-2.2.8/enbios/generic/mermaid2hierarchy.py` & `enbios-2.2.9/enbios/generic/mermaid2hierarchy.py`

 * *Files identical despite different names*

### Comparing `enbios-2.2.8/enbios/generic/tree/basic_tree.py` & `enbios-2.2.9/enbios/generic/tree/basic_tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,24 +67,25 @@
                     child = BasicTreeNode.from_dict(
                         child, dataclass=dataclass, data_factory=data_factory
                     )
                 self.add_child(child)
         self.parent: Optional[BasicTreeNode[T]] = None
         self.temp_data: dict[str, Any] = temp_data if temp_data else {}
         self._id: bytes = self.generate_id()
+        self._data: Optional[Union[dict, T]]
         if data:
             if isinstance(data, dict):
                 if dataclass:
                     self._data = dataclass(**data)
                 else:
-                    self._data: dict = data
+                    self._data = data
             else:
-                self._data: T = data
+                self._data = data
         elif data_factory:
-            self._data: T = data_factory(temp_data)
+            self._data = data_factory(self.temp_data)
         else:
             self._data = None
 
     def generate_id(self) -> bytes:
         self._id = b64encode(uuid4().bytes)
         return self._id
 
@@ -222,15 +223,15 @@
         """
         Parse a dict and create a tree from it.
         :param data:
         :param dataclass:
         :param data_factory:
         :return: a node containing the whole tree
         """
-        name = data.get("name")
+        name = data.get("name", "")
         children = data.get("children")
         if dataclass:
             return BasicTreeNode(name, children, data=data, dataclass=dataclass)
         else:
             return BasicTreeNode(
                 name,
                 children,
@@ -467,87 +468,111 @@
         self,
         csv_file: PathLike,
         *,
         include_data: Optional[bool] = False,
         data_serializer: Optional[Callable[[T], dict]] = None,
         exclude_data_keys: Optional[list[str]] = None,
         level_names: Optional[list[str]] = None,
-        merge_first_sub_row: bool = False,
         repeat_parent_name: bool = False,
+        flat_hierarchy: Optional[bool] = False,
     ):
+        if not exclude_data_keys:
+            exclude_data_keys = []
         # Calculate max_depth based on root if not provided
         if include_data and not isinstance(self._data, dict) and not data_serializer:
             raise ValueError(
                 "If include_data is True, and data not a dict, "
                 "data_serializer must be provided"
             )
 
-        if include_data and merge_first_sub_row:
-            logger.warning(
-                "Merging first sub-row and including data is often not recommended, "
-                "as sub-row data will overwrite parent data"
-            )
-
-        include_data_keys = []
-        if include_data and self._data:
-            # todo, this will probably be enough to get diverse results...
-            if data_serializer:
-                include_data_keys = list(data_serializer(self._data).keys())
-            else:
-                if isinstance(self._data, dict):
-                    include_data_keys = list(self._data.keys())
-            if exclude_data_keys:
-                include_data_keys = list(set(include_data_keys) - set(exclude_data_keys))
+        if flat_hierarchy and level_names:
+            logger.warning("flat hierarchy do not make use of level_names")
+        if flat_hierarchy and repeat_parent_name:
+            logger.warning("flat hierarchy do not make use of repeat_parent_name")
         _total_level_names = level_names if level_names else []
 
         def level_name(level: int) -> str:
             if level >= len(_total_level_names):
                 _total_level_names.append(f"lvl_{level}")
             return _total_level_names[level]
 
         def rec_add_node_row(
             node: "BasicTreeNode[T]",
             include_data_: Optional[bool] = False,
             current_level: int = 0,
         ) -> list[dict[str, Union[str, float]]]:
             row = {}
             if include_data_ and node._data:
-                node_data: dict[str, Any] = {}
+                row: dict[str, Any] = {}
                 if data_serializer:
-                    node_data = data_serializer(node._data)
+                    row = data_serializer(node._data)
                 elif isinstance(node._data, dict):
-                    node_data = node._data
+                    row = node._data
                 else:
                     logger.warning(
                         "Data is not a dict and no data_serializer provided, "
                         "skipping data"
                     )
-                for data_key in include_data_keys:
-                    row[data_key] = node_data.get(data_key, "")
+                for delete in exclude_data_keys:
+                    row.pop(delete, None)
             row[level_name(current_level)] = node.name
+            row["level"] = node.level
             _sub_rows = []
             for child in node.children:
                 _sub_rows.extend(
                     rec_add_node_row(child, include_data_, current_level + 1)
                 )
             if _sub_rows:
-                if merge_first_sub_row:
-                    row = {**row, **_sub_rows[0]}
-                    _sub_rows = _sub_rows[1:]
                 if repeat_parent_name:
                     for sub_row in _sub_rows:
                         sub_row[level_name(current_level)] = node.name
             return [row] + _sub_rows
 
+        def rec_add_flat_node_row(
+            node: "BasicTreeNode[T]",
+            include_data_: Optional[bool] = False,
+            current_level: int = 0,
+        ) -> list[dict[str, Union[str, float]]]:
+            row = {}
+            if include_data_ and node._data:
+                if data_serializer:
+                    row = data_serializer(node._data)
+                elif isinstance(node._data, dict):
+                    row = node._data
+                else:
+                    logger.warning(
+                        "Data is not a dict and no data_serializer provided, "
+                        "skipping data"
+                    )
+            row["node_name"] = node.name
+            row["level"] = node.level
+            row["parent_name"] = node.parent.name if node.parent else ""
+            rows = [row]
+            for child in node.children:
+                rows.extend(
+                    rec_add_flat_node_row(child, include_data_, current_level + 1)
+                )
+            return rows
+
         # Write rows to csv
         if isinstance(csv_file, bytes):
             csv_file = csv_file.decode()
+
         with Path(csv_file).open("w", newline="") as csvfile:
-            rows = rec_add_node_row(self, include_data)
-            headers = _total_level_names + include_data_keys
+            if flat_hierarchy:
+                rows = rec_add_flat_node_row(self, include_data)
+                headers = ["node_name", "level", "parent_name"]
+            else:
+                rows = rec_add_node_row(self, include_data)
+                headers = ["level"] + _total_level_names
+
+            for row in rows:
+                for k in row:
+                    if k not in headers:
+                        headers.append(k)
             writer = csv.DictWriter(csvfile, headers)
             writer.writeheader()
             writer.writerows(rows)
 
     def to_sanky_tree(self, file_path: Path, value_key: str = "value"):
         """
         Write the hierarchy to a csv file.
```

### Comparing `enbios-2.2.8/enbios/generic/unit_util.py` & `enbios-2.2.9/enbios/generic/unit_util.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 from pint import Quantity
 
-from enbios import ureg
-from enbios.models.experiment_base_models import NodeOutput
+from enbios.base.unit_registry import ureg
+from enbios.models.models import NodeOutput
 
 
 def compact_all_to(quantities: list[Quantity], use_min: bool = True) -> list[Quantity]:
     """
     Convert all quantities to the same unit, and return the compacted values
     :param quantities:
     :param use_min: use the unit of the smallest quantity (otherwise use the largest)
     :return: a list of compacted quantities with the same unit
     """
     base_func = min if use_min else max
     base_value = base_func([q.to_compact() for q in quantities])
     return [q.to(base_value.units) for q in quantities]
 
 
+def unit_match(unit1: str, unit2: str) -> bool:
+    return ureg(unit1).is_compatible_with(unit2)
+
+
 def get_output_in_unit(output: NodeOutput, target_unit: str) -> float:
     """
     Convert the output to a magnitude the given unit
     :param output:
     :param target_unit:
     :return:
     """
-    return (
-        (ureg.parse_expression(output.unit) * output.magnitude).to(target_unit).magnitude
+    conversion_quant = (ureg.parse_expression(output.unit) * output.magnitude).to(
+        target_unit
     )
+    # experiment to avoid something like 1ML converted to 1000000.00000001
+    if (
+        ureg.parse_expression(output.unit) / ureg(target_unit)
+    ).to_base_units().magnitude > 1e6:
+        return round(conversion_quant.magnitude, 0)
+    else:
+        return conversion_quant.magnitude
```

### Comparing `enbios-2.2.8/enbios/generic/util.py` & `enbios-2.2.9/enbios/generic/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from pathlib import Path
 from time import time
 from types import ModuleType
 from typing import Union, Type, Any, Callable
 
 from enbios.const import BASE_DATA_PATH
 from enbios.generic.enbios2_logging import get_logger
+from enbios.generic.files import PathLike
 
 logger = get_logger(__name__)
 
 
 def generate_levensthein_name_map(
     names_a: list[str], names_b: list[str]
 ) -> dict[str, str]:
@@ -126,15 +127,15 @@
     start = time()
     try:
         yield
     finally:
         print(f"({time() - start:.2f}s)")
 
 
-def load_module(module_path: str) -> ModuleType:
+def load_module(module_path: Union[str, PathLike]) -> ModuleType:
     _path = Path(module_path)
     if not _path.exists():
         raise ValueError(f"Module path '{module_path}' does not exist")
     sys.path.insert(0, _path.parent.as_posix())
     return import_module(_path.stem)
```

### Comparing `enbios-2.2.8/enbios/models/experiment_base_models.py` & `enbios-2.2.9/enbios/models/models.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,108 +1,111 @@
+from dataclasses import field
 from typing import Optional, Union, Any
 
+from pint.facets.plain import PlainQuantity
 from pydantic import BaseModel, Field, model_validator, field_validator, ConfigDict
 
 from enbios.generic.files import PathLike
 
 StrictInputConfig = ConfigDict(extra="forbid", validate_assignment=True, strict=True)
 
 
 class ExperimentConfig(BaseModel):
     model_config = StrictInputConfig
     warn_default_demand: bool = True  # todo: bring this back
-    auto_aggregate: Optional[bool] = (
-        True  # aggregate, with same indicator, as all children, if given.
-    )
+    auto_aggregate: Optional[
+        bool
+    ] = True  # aggregate, with same indicator, as all children, if given.
     run_adapters_concurrently: bool = True
-    run_scenarios: Optional[list[str]] = (
-        None  # list of scenario-name to run, ALSO AS ENV-VAR
-    )
+    run_scenarios: Optional[
+        list[str]
+    ] = None  # list of scenario-name to run, ALSO AS ENV-VAR
     # only used by ExperimentDataIO
     # base_directory when loading files (activities, methods, ...)
     base_directory: Optional[Union[str, PathLike]] = None
     # those are only used for testing
     debug_test_is_valid: bool = True
-    debug_test_replace_bw_config: Union[bool, list[str]] = (
-        True  # standard replacement, or bw-project, bw-database
-    )
+    debug_test_replace_bw_config: Union[
+        bool, list[str]
+    ] = True  # standard replacement, or bw-project, bw-database
     debug_test_expected_error_code: Optional[int] = None
     debug_test_run: Optional[bool] = False
     note: Optional[str] = None
 
 
 class AdapterModel(BaseModel):
     model_config = ConfigDict(extra="allow")
     module_path: Optional[PathLike] = None
     adapter_name: Optional[str] = Field(
         None,
-        description="this this is to use inbuilt adapter "
-        "(e.g. 'simple-assignment-adapter'",
+        description="this this is to use inbuilt adapter " "(e.g. 'assignment-adapter'",
     )
     config: dict = Field(default_factory=dict)
     methods: dict[str, Any] = Field(default_factory=dict)
     note: Optional[str] = Field(None, description="A note for this adapter")
 
-    @model_validator(mode="before")
-    @classmethod
-    def module_specified(cls, data: Any) -> Any:
+    @model_validator(mode="before")  # type: ignore
+    def module_specified(data: Any):
         # either module_path or module_class must be specified
         if not ("module_path" in data or "adapter_name" in data):
             raise ValueError("Either module_path or adapter_name must be specified")
         return data
 
 
 class AggregationModel(BaseModel):
     module_path: Optional[PathLike] = None
     aggregator_name: str = Field(
         None,
         description="this this is to use inbuilt aggregator "
-        "(e.g. 'simple-assignment-adapter'",
+        "(e.g. 'assignment-adapter'",
     )
     config: Optional[dict] = Field(default_factory=dict)
     note: Optional[str] = None
 
     @model_validator(mode="before")
-    @classmethod
     def module_specified(cls, data: Any) -> Any:
         # either module_path or module_class must be specified
         if not ("module_path" in data or "aggregator_name" in data):
             raise ValueError("Either module_path or aggregator_name must be specified")
         return data
 
 
 class ExperimentHierarchyNodeData(BaseModel):
+    model_config = ConfigDict(extra="forbid")
     name: str
     aggregator: str = Field(..., description="name or node-indicator of the aggregator")
     config: Optional[Any] = Field(
-        None, description="setup data (id, outputs, ... arbitrary data"
+        default_factory=dict, description="setup data (id, outputs, ... arbitrary data"
     )
     children: Optional[
-        list[Union["ExperimentHierarchyNodeData", "ExperimentActivityData"]]
+        list[Union["ExperimentHierarchyNodeData", "HierarchyStructuralNodeData"]]
     ] = None
 
 
-class ExperimentActivityData(BaseModel):
+class HierarchyStructuralNodeData(BaseModel):
     """
     This is the dataclass for the activities in the experiment.
     """
 
+    model_config = ConfigDict(extra="forbid")
     name: str
-    config: Any = Field(..., description="setup data (id, outputs, ... arbitrary data")
+    config: Any = Field(
+        default_factory=dict, description="setup data (id, outputs, ... arbitrary data"
+    )
     adapter: str = Field(..., description="The adapter to be used")
 
 
 class HierarchyNodeReference(BaseModel):
     """
     This is a reference to a node in the hierarchy.
     """
 
     name: str
     config: Optional[Any] = Field(
-        None, description="setup data (id, outputs, ... arbitrary data"
+        default=None, description="setup data (id, outputs, ... arbitrary data"
     )
     aggregator: Optional[str] = None
     children: Optional[list["HierarchyNodeReference"]] = None
 
     @field_validator("children", mode="before")
     @classmethod
     def transform_simple_string_children(
@@ -111,40 +114,48 @@
         return [
             HierarchyNodeReference(name=child) if isinstance(child, str) else child
             for child in v
         ]
 
 
 class ScenarioConfig(BaseModel):
-    exclude_defaults: Optional[bool] = (
+    exclude_defaults: Optional[bool] = Field(
         False  # will only use on activities that are specified in the scenario
     )
 
 
 class NodeOutput(BaseModel):
     model_config = StrictInputConfig
     unit: str
     magnitude: float = 1.0
+    label: Optional[str] = None
 
     @model_validator(mode="before")
-    @classmethod
-    def transform_value(cls, v: Any) -> "dict":
+    def transform_value(cls, v: Any) -> dict:
         if isinstance(v, dict):
+            if v.get("label") == "":
+                v["label"] = None
             return v
         elif isinstance(v, tuple) or isinstance(v, list):
             return {"unit": v[0], "magnitude": v[1]}
+        return v
+
+    def from_quantity(self, q: PlainQuantity):
+        self.unit = str(q.units)
+        self.magnitude = q.magnitude
 
 
 class ExperimentScenarioData(BaseModel):
     model_config = StrictInputConfig
     name: Optional[str] = Field(None)
-    nodes: dict[str, NodeOutput] = Field(
-        None, description="name to output, null means default-output (check exists)"
+    nodes: dict[str, Any] = Field(
+        default_factory=dict,
+        description="name to output, null means default-output (check exists)",
     )
-    config: Optional[ScenarioConfig] = Field(default_factory=ScenarioConfig)
+    config: Optional[ScenarioConfig] = Field(default_factory=ScenarioConfig)  # type: ignore
 
     def name_factory(self, index: int):
         if not self.name:
             self.name = f"Scenario {index}"
 
 
 class ExperimentData(BaseModel):
@@ -187,7 +198,48 @@
     scenarios: Optional[list[ExperimentScenarioData]] = Field(
         None, description="The scenarios for this experiment"
     )
     config: ExperimentConfig = Field(
         default_factory=ExperimentConfig,
         description="The configuration of this experiment",
     )
+
+
+class TechTreeNodeData(BaseModel):
+    adapter: Optional[str] = None
+    aggregator: Optional[str] = None
+    config: Optional[Any] = Field(
+        None, description="The identifies (method to find) a node"
+    )
+
+    @model_validator(mode="before")
+    def check_model(cls, data: Any) -> Any:
+        if isinstance(data, dict):
+            leaf_node = "adapter" in data and "config" in data
+            non_leaf_node = "aggregator" in data
+            assert leaf_node or non_leaf_node, (
+                "Node must be either leaf ('id', 'adapter`) " "or non-leaf ('aggregator')"
+            )
+        return data
+
+
+class ResultValue(BaseModel):
+    model_config = StrictInputConfig
+    unit: str
+    magnitude: Optional[float] = None  # type: ignore
+    multi_magnitude: Optional[list[float]] = field(default_factory=list)
+
+
+class ScenarioResultNodeData(BaseModel):
+    model_config = StrictInputConfig
+    output: list[NodeOutput] = Field(default_factory=list)
+    results: dict[str, ResultValue] = Field(default_factory=dict)
+    adapter: Optional[str] = None
+    aggregator: Optional[str] = None
+    extras: Optional[dict[str, Any]] = None
+
+
+class EnbiosValidationException(Exception):
+    def __init__(self, message, exc_name=None, code: Optional[int] = None):
+        super().__init__(message)
+        self.exc_name = exc_name
+        self.code = code
```

### Comparing `enbios-2.2.8/enbios.egg-info/PKG-INFO` & `enbios-2.2.9/enbios.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enbios
-Version: 2.2.8
+Version: 2.2.9
 Summary: Enbios 2
 Author: Ramin Soleymani
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/LIVENlab/enbios
 Project-URL: Bug Tracker, https://github.com/LIVENlab/enbios/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -46,53 +46,65 @@
 Requires-Dist: fonttools==4.47.2
 Requires-Dist: frictionless==5.16.0
 Requires-Dist: fs==2.4.16
 Requires-Dist: idna==3.4
 Requires-Dist: importlib-resources==6.0.0
 Requires-Dist: kiwisolver==1.4.4
 Requires-Dist: lxml==4.9.3
-Requires-Dist: matplotlib==3.7.2
+Requires-Dist: matplotlib==3.8.3
+Requires-Dist: matplotlib-inline==0.1.6
 Requires-Dist: matrix-utils==0.2.5
 Requires-Dist: mrio-common-metadata==0.2.1
 Requires-Dist: numpy==1.26.4
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: packaging==23.1
 Requires-Dist: pandas==2.0.3
-Requires-Dist: peewee==3.17.0
-Requires-Dist: Pillow==10.2.0
-Requires-Dist: Pint==0.22
+Requires-Dist: peewee==3.17.1
+Requires-Dist: pillow==10.2.0
+Requires-Dist: Pint==0.23
+Requires-Dist: pkginfo==1.10.0
 Requires-Dist: platformdirs==3.9.1
-Requires-Dist: pydantic==2.5.2
-Requires-Dist: pyparsing
+Requires-Dist: pydantic==2.6.4
+Requires-Dist: pydantic-settings==2.2.1
+Requires-Dist: pydantic_core==2.16.3
+Requires-Dist: pydoc-markdown==4.8.2
+Requires-Dist: Pygments==2.17.2
+Requires-Dist: pyparsing==3.1.1
 Requires-Dist: PyPrind==2.11.3
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: python-mermaid==0.1.3
 Requires-Dist: pytz==2023.3
 Requires-Dist: pyxlsb==1.0.10
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: requests==2.31.0
-Requires-Dist: scipy==1.11.1
+Requires-Dist: scipy==1.12.0
 Requires-Dist: scikit-learn>=1.4.0
 Requires-Dist: six==1.16.0
 Requires-Dist: stats-arrays==0.6.5
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: tqdm==4.66.1
 Requires-Dist: tzdata==2023.3
 Requires-Dist: Unidecode==1.3.8
-Requires-Dist: urllib3==2.1.0
+Requires-Dist: urllib3==2.2.1
 Requires-Dist: voluptuous==0.13.1
 Requires-Dist: Whoosh==2.7.4
 Requires-Dist: wrapt==1.15.0
 Requires-Dist: xlrd==2.0.1
 Requires-Dist: XlsxWriter==3.1.9
 Requires-Dist: xmltodict==0.13.0
 Requires-Dist: zipp==3.16.2
 Provides-Extra: test
 Requires-Dist: pytest==7.3.2; extra == "test"
-Requires-Dist: Deprecated>=1.2.14; extra == "test"
+Provides-Extra: dev
+Requires-Dist: build==1.2.1; extra == "dev"
+Requires-Dist: twine==4.0.2; extra == "dev"
+Requires-Dist: jupyter==1.0.0; extra == "dev"
+Requires-Dist: ruff==0.3.3; extra == "dev"
+Requires-Dist: black==23.12.1; extra == "dev"
+Requires-Dist: tokenize-rt; extra == "dev"
 
 # ENBIOS2
 
 ## What is ENBIOS 2
 
 ENBIOS2 (Environmental and Bioeconomic System Analysis)  is a [python-based](https://pypi.org/project/enbios/)
 simulation tool for the assessment of environmental impacts and resource requirements of energy system
@@ -198,43 +210,65 @@
 - Environmental impact indicators from the most used LCIA methods (Recipe2016, CML, AWARE, etc.)
 - Environmental externalization rates
 - Forthcoming: Raw Material Recycling rates and Supply risk
 
 ### Features
 
 - Integration of LCA and MuSIASEM evaluation methods
-- Import of .spold LCA inventory data to a multi-level tree-like setting
 - Library of impact assessment methods based on LCIA
 - New impact assessment methods developed for raw materials and circularity
 - Consideration of externalized environmental impacts
 - Takes data from the friendly-data package (other formats under development)
 - High level methods to quickly obtain/refresh analyses
 
 ## Demos
 
 This repository contains a few notebooks (require jupyter notebook) in the demos folder, that can help you get started.
 We are updating and commenting these. Please bear with us while we do it and feel free to give us feedback on those (
 thanks).
 
+You can copy the demos into your project like this:
+
+```python
+from enbios import copy_demos
+
+copy_demos("<destination_path>")
+```
+
 [Getting started](https://github.com/LIVENlab/enbios/blob/main/demos/intro.ipynb)
 
 [Plotting results](https://github.com/LIVENlab/enbios/blob/main/demos/plot_results.ipynb)
 
 [Sorting the results in alternative hierarchies](https://github.com/LIVENlab/enbios/blob/main/demos/multiple_hierarchies.ipynb)
 
+Reevaluate the experiment with alternative hierarchies. For alternative hierarchies the structural nodes (none bottom
+nodes) can be changed/added.
+
+[Assignment Adapter](https://github.com/LIVENlab/enbios/blob/main/demos/assignment_adapter_demo.ipynb)
+
+The Simple Assignment Adapter does not any specific calculations.
+Instead, it allows the user to introduce fixed values, that should come from some external source into the enbios tree
+calculation. This includes not just the outputs of structural nodes, but in particular their impact results.
+These values can be either in the experiment configuration file or for convenience in a referenced csv file. The values
+can be specified in such a way, that scenario outputs and result values have consistent and valid units.
+
 [Splitting the configuration](https://github.com/LIVENlab/enbios/blob/main/demos/multiple_config_files.ipynb)
 
 [Working with trees](https://github.com/LIVENlab/enbios/blob/main/demos/trees.ipynb)
 
 [Experiment with uncertainties](https://github.com/LIVENlab/enbios/blob/main/demos/uncertainty_experiment.ipynb)
 
 [Convert mermaid diagrams to enbios hierarchy](https://github.com/LIVENlab/enbios/blob/main/demos/mermaid.ipynb)
 
 [A complete Brightway adaoter configuration object](https://github.com/LIVENlab/enbios/blob/main/demos/bw_adapter_config.ipynb)
 
+[Specifying the hierarchy in a csv file](https://github.com/LIVENlab/enbios/blob/main/demos/csv_hierarchy.ipynb)
+
+[Exporting to a csv file](https://github.com/LIVENlab/enbios/blob/main/demos/csv_export.ipynb)
+
 ## People
 
 * [Ramin Soleymani](https://es.linkedin.com/in/ramin-soleymani-4703b17). -[ICTA-UAB](https://www.uab.cat/icta/)
 * [Miquel Sierra Montoya](https://portalrecerca.uab.cat/en/persons/miquel-sierra-i-montoya). -[ICTA-UAB](https://www.uab.cat/icta/)
 * [Alexander de Tomás](https://www.linkedin.com/in/alexander-de-tom%C3%A1s-pascual-a85348185/). -[ICTA-UAB](https://www.uab.cat/icta/)
 * [Cristina Madrid-Lopez](https://portalrecerca.uab.cat/en/persons/cristina-madrid-lopez-3). - [ICTA-UAB](https://www.uab.cat/icta/)
```

### Comparing `enbios-2.2.8/enbios.egg-info/requires.txt` & `enbios-2.2.9/requirements.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 annotated-types==0.5.0
 appdirs==1.4.4
 asteval==0.9.31
 astunparse==1.6.3
 brightway25==1.0.6
 bw-migrations==0.2
-bw-processing<=0.9,>=0.8.3
+bw-processing>=0.8.3,<=0.9
 bw2analyzer==0.11.5
-bw2calc<=2.0.dev16,>=2.0.dev13
-bw2data<=4.0.dev33,>=4.0.dev19
-bw2io<=0.9.dev26,>=0.9.dev19
+bw2calc>=2.0.dev13,<=2.0.dev16
+bw2data>=4.0.dev19,<=4.0.dev33
+bw2io>=0.9.dev19, <=0.9.dev26
 bw2parameters==1.1.0
 certifi==2023.7.22
 charset-normalizer==3.2.0
 contourpy==1.1.0
 cycler==0.11.0
 et-xmlfile==1.1.0
 flatten-dict==0.4.2
 fonttools==4.47.2
 frictionless==5.16.0
 fs==2.4.16
 idna==3.4
 importlib-resources==6.0.0
 kiwisolver==1.4.4
 lxml==4.9.3
-matplotlib==3.7.2
+matplotlib==3.8.3
+matplotlib-inline==0.1.6
 matrix-utils==0.2.5
 mrio-common-metadata==0.2.1
 numpy==1.26.4
 openpyxl==3.1.2
 packaging==23.1
 pandas==2.0.3
-peewee==3.17.0
-Pillow==10.2.0
-Pint==0.22
+peewee==3.17.1
+pillow==10.2.0
+Pint==0.23
+pkginfo==1.10.0
 platformdirs==3.9.1
-pydantic==2.5.2
-pyparsing
+pydantic==2.6.4
+pydantic-settings==2.2.1
+pydantic_core==2.16.3
+pydoc-markdown==4.8.2
+Pygments==2.17.2
+pyparsing==3.1.1
 PyPrind==2.11.3
 python-dateutil==2.8.2
 python-mermaid==0.1.3
 pytz==2023.3
 pyxlsb==1.0.10
 PyYAML==6.0.1
 requests==2.31.0
-scipy==1.11.1
+scipy==1.12.0
 scikit-learn>=1.4.0
 six==1.16.0
 stats-arrays==0.6.5
 tabulate==0.9.0
 tqdm==4.66.1
 tzdata==2023.3
 Unidecode==1.3.8
-urllib3==2.1.0
+urllib3==2.2.1
 voluptuous==0.13.1
 Whoosh==2.7.4
 wrapt==1.15.0
 xlrd==2.0.1
 XlsxWriter==3.1.9
 xmltodict==0.13.0
 zipp==3.16.2
-
-[test]
-pytest==7.3.2
-Deprecated>=1.2.14
```

### Comparing `enbios-2.2.8/pyproject.toml` & `enbios-2.2.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "enbios"
-version = "2.2.8"
+version = "2.2.9"
 description = "Enbios 2"
 authors = [
     { name = "Ramin Soleymani" },
 ]
 dynamic = ["dependencies"]
 
 classifiers = [
@@ -35,17 +35,24 @@
 
 [project.urls]
 "Homepage" = "https://github.com/LIVENlab/enbios"
 "Bug Tracker" = "https://github.com/LIVENlab/enbios/issues"
 
 [project.optional-dependencies]
 test = [
-    "pytest==7.3.2", "Deprecated>=1.2.14"
+    "pytest==7.3.2"
 ]
 
+dev = [
+  "build==1.2.1", "twine==4.0.2","jupyter==1.0.0", "ruff==0.3.3","black==23.12.1", "tokenize-rt"
+]
+
+[tool.mypy]
+ignore_missing_imports = true
+
 
 [tool.setuptools]
 package-dir = { "enbios" = "enbios" }
 
 [tool.setuptools.dynamic]
 dependencies = {file="requirements.txt"}
```

### Comparing `enbios-2.2.8/requirements.txt` & `enbios-2.2.9/enbios.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,78 @@
 annotated-types==0.5.0
 appdirs==1.4.4
 asteval==0.9.31
 astunparse==1.6.3
 brightway25==1.0.6
 bw-migrations==0.2
-bw-processing>=0.8.3,<=0.9
+bw-processing<=0.9,>=0.8.3
 bw2analyzer==0.11.5
-bw2calc>=2.0.dev13,<=2.0.dev16
-bw2data>=4.0.dev19,<=4.0.dev33
-bw2io>=0.9.dev19, <=0.9.dev26
+bw2calc<=2.0.dev16,>=2.0.dev13
+bw2data<=4.0.dev33,>=4.0.dev19
+bw2io<=0.9.dev26,>=0.9.dev19
 bw2parameters==1.1.0
 certifi==2023.7.22
 charset-normalizer==3.2.0
 contourpy==1.1.0
 cycler==0.11.0
 et-xmlfile==1.1.0
 flatten-dict==0.4.2
 fonttools==4.47.2
 frictionless==5.16.0
 fs==2.4.16
 idna==3.4
 importlib-resources==6.0.0
 kiwisolver==1.4.4
 lxml==4.9.3
-matplotlib==3.7.2
+matplotlib==3.8.3
+matplotlib-inline==0.1.6
 matrix-utils==0.2.5
 mrio-common-metadata==0.2.1
 numpy==1.26.4
 openpyxl==3.1.2
 packaging==23.1
 pandas==2.0.3
-peewee==3.17.0
-Pillow==10.2.0
-Pint==0.22
+peewee==3.17.1
+pillow==10.2.0
+Pint==0.23
+pkginfo==1.10.0
 platformdirs==3.9.1
-pydantic==2.5.2
-pyparsing
+pydantic==2.6.4
+pydantic-settings==2.2.1
+pydantic_core==2.16.3
+pydoc-markdown==4.8.2
+Pygments==2.17.2
+pyparsing==3.1.1
 PyPrind==2.11.3
 python-dateutil==2.8.2
 python-mermaid==0.1.3
 pytz==2023.3
 pyxlsb==1.0.10
 PyYAML==6.0.1
 requests==2.31.0
-scipy==1.11.1
+scipy==1.12.0
 scikit-learn>=1.4.0
 six==1.16.0
 stats-arrays==0.6.5
 tabulate==0.9.0
 tqdm==4.66.1
 tzdata==2023.3
 Unidecode==1.3.8
-urllib3==2.1.0
+urllib3==2.2.1
 voluptuous==0.13.1
 Whoosh==2.7.4
 wrapt==1.15.0
 xlrd==2.0.1
 XlsxWriter==3.1.9
 xmltodict==0.13.0
 zipp==3.16.2
+
+[dev]
+build==1.2.1
+twine==4.0.2
+jupyter==1.0.0
+ruff==0.3.3
+black==23.12.1
+tokenize-rt
+
+[test]
+pytest==7.3.2
```

