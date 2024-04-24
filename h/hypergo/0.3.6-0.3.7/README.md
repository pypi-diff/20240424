# Comparing `tmp/hypergo-0.3.6.tar.gz` & `tmp/hypergo-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypergo-0.3.6.tar", last modified: Thu Mar 14 15:20:29 2024, max compression
+gzip compressed data, was "hypergo-0.3.7.tar", last modified: Wed Apr 24 17:50:43 2024, max compression
```

## Comparing `hypergo-0.3.6.tar` & `hypergo-0.3.7.tar`

### file list

```diff
@@ -1,75 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:20:29.335516 hypergo-0.3.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:20:29.323516 hypergo-0.3.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:20:29.323516 hypergo-0.3.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-14 15:20:18.000000 hypergo-0.3.6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-03-14 15:20:18.000000 hypergo-0.3.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-14 15:20:18.000000 hypergo-0.3.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-03-14 15:20:18.000000 hypergo-0.3.6/BACKLOG.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:20:18.000000 hypergo-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-14 15:20:29.335516 hypergo-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-14 15:20:18.000000 hypergo-0.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    12636 2024-03-14 15:20:18.000000 hypergo-0.3.6/RELEASE_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-14 15:20:18.000000 hypergo-0.3.6/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:20:29.327516 hypergo-0.3.6/hypergo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/azure_service_bus_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/azure_service_bus_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:20:29.331516 hypergo-0.3.6/hypergo/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/connectors/azure_application_insights.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/hypergo_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/hypergo_click.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/hypergo_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:20:29.331516 hypergo-0.3.6/hypergo/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/loggers/azure_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/loggers/base_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/loggers/hypergo_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:20:29.331516 hypergo-0.3.6/hypergo/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/metrics/base_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/metrics/custom_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/metrics/hypergo_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/service_bus_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/stdio_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-03-14 15:20:18.000000 hypergo-0.3.6/hypergo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:20:29.331516 hypergo-0.3.6/hypergo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-14 15:20:29.000000 hypergo-0.3.6/hypergo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-14 15:20:29.000000 hypergo-0.3.6/hypergo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 15:20:29.000000 hypergo-0.3.6/hypergo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-14 15:20:29.000000 hypergo-0.3.6/hypergo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-14 15:20:29.000000 hypergo-0.3.6/hypergo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-14 15:20:29.000000 hypergo-0.3.6/hypergo.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2851 2024-03-14 15:20:18.000000 hypergo-0.3.6/lint.sh
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-14 15:20:18.000000 hypergo-0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-14 15:20:29.335516 hypergo-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-14 15:20:18.000000 hypergo-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:20:29.331516 hypergo-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-03-14 15:20:18.000000 hypergo-0.3.6/tests/test.json
--rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-03-14 15:20:18.000000 hypergo-0.3.6/tests/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-14 15:20:18.000000 hypergo-0.3.6/tests/test_azure_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-03-14 15:20:18.000000 hypergo-0.3.6/tests/test_azure_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-03-14 15:20:18.000000 hypergo-0.3.6/tests/test_dynamic_input_bindings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-14 15:20:18.000000 hypergo-0.3.6/tests/test_dynamic_routing_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-14 15:20:18.000000 hypergo-0.3.6/tests/test_local_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-14 15:20:18.000000 hypergo-0.3.6/tests/test_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-03-14 15:20:18.000000 hypergo-0.3.6/tests/test_stdio_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-03-14 15:20:18.000000 hypergo-0.3.6/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-03-14 15:20:18.000000 hypergo-0.3.6/tests/test_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-03-14 15:20:18.000000 hypergo-0.3.6/tests/test_utility_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:50:43.152547 hypergo-0.3.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:50:43.136547 hypergo-0.3.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:50:43.140547 hypergo-0.3.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-24 17:50:38.000000 hypergo-0.3.7/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-24 17:50:38.000000 hypergo-0.3.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-24 17:50:38.000000 hypergo-0.3.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-04-24 17:50:38.000000 hypergo-0.3.7/BACKLOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:50:38.000000 hypergo-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-24 17:50:43.152547 hypergo-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-24 17:50:38.000000 hypergo-0.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12636 2024-04-24 17:50:38.000000 hypergo-0.3.7/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-24 17:50:38.000000 hypergo-0.3.7/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:50:43.144547 hypergo-0.3.7/hypergo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/azure_service_bus_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/azure_service_bus_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:50:43.144547 hypergo-0.3.7/hypergo/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/connectors/azure_application_insights.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/hypergo_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/hypergo_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/hypergo_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:50:43.144547 hypergo-0.3.7/hypergo/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/loggers/azure_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/loggers/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/loggers/hypergo_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:50:43.148547 hypergo-0.3.7/hypergo/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/metrics/base_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/metrics/custom_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/metrics/hypergo_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/service_bus_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/stdio_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-24 17:50:38.000000 hypergo-0.3.7/hypergo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:50:43.152547 hypergo-0.3.7/hypergo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-24 17:50:43.000000 hypergo-0.3.7/hypergo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-24 17:50:43.000000 hypergo-0.3.7/hypergo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 17:50:43.000000 hypergo-0.3.7/hypergo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-24 17:50:43.000000 hypergo-0.3.7/hypergo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-24 17:50:43.000000 hypergo-0.3.7/hypergo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 17:50:43.000000 hypergo-0.3.7/hypergo.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2851 2024-04-24 17:50:38.000000 hypergo-0.3.7/lint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-24 17:50:38.000000 hypergo-0.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-24 17:50:43.152547 hypergo-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-24 17:50:38.000000 hypergo-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:50:43.148547 hypergo-0.3.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:50:43.136547 hypergo-0.3.7/tests/integration_pipeline/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:50:43.148547 hypergo-0.3.7/tests/integration_pipeline/input_binder/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:50:43.148547 hypergo-0.3.7/tests/integration_pipeline/input_binder/input_binder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:50:38.000000 hypergo-0.3.7/tests/integration_pipeline/input_binder/input_binder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-24 17:50:38.000000 hypergo-0.3.7/tests/integration_pipeline/input_binder/input_binder/input_binder.json
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-24 17:50:38.000000 hypergo-0.3.7/tests/integration_pipeline/input_binder/input_binder/input_binder.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 17:50:38.000000 hypergo-0.3.7/tests/integration_pipeline/input_binder/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-24 17:50:38.000000 hypergo-0.3.7/tests/integration_pipeline/input_binder/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:50:43.148547 hypergo-0.3.7/tests/integration_pipeline/result_checker/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 17:50:38.000000 hypergo-0.3.7/tests/integration_pipeline/result_checker/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:50:43.152547 hypergo-0.3.7/tests/integration_pipeline/result_checker/result_checker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:50:38.000000 hypergo-0.3.7/tests/integration_pipeline/result_checker/result_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-24 17:50:38.000000 hypergo-0.3.7/tests/integration_pipeline/result_checker/result_checker/result_checker.json
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-24 17:50:38.000000 hypergo-0.3.7/tests/integration_pipeline/result_checker/result_checker/result_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-24 17:50:38.000000 hypergo-0.3.7/tests/integration_pipeline/result_checker/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-04-24 17:50:38.000000 hypergo-0.3.7/tests/test.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-04-24 17:50:38.000000 hypergo-0.3.7/tests/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-24 17:50:38.000000 hypergo-0.3.7/tests/test_azure_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-24 17:50:38.000000 hypergo-0.3.7/tests/test_azure_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-24 17:50:38.000000 hypergo-0.3.7/tests/test_dynamic_input_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-24 17:50:38.000000 hypergo-0.3.7/tests/test_dynamic_routing_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-24 17:50:38.000000 hypergo-0.3.7/tests/test_local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-24 17:50:38.000000 hypergo-0.3.7/tests/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-24 17:50:38.000000 hypergo-0.3.7/tests/test_stdio_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-24 17:50:38.000000 hypergo-0.3.7/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-24 17:50:38.000000 hypergo-0.3.7/tests/test_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-04-24 17:50:38.000000 hypergo-0.3.7/tests/test_utility_serialization.py
```

### Comparing `hypergo-0.3.6/.github/workflows/python-publish.yml` & `hypergo-0.3.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/.gitignore` & `hypergo-0.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/BACKLOG.md` & `hypergo-0.3.7/BACKLOG.md`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/PKG-INFO` & `hypergo-0.3.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypergo
-Version: 0.3.6
+Version: 0.3.7
 Summary: Project for service bus
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml
 Requires-Dist: glom
 Requires-Dist: pydash
 Requires-Dist: azure-servicebus
@@ -25,7 +25,8 @@
 Requires-Dist: opentelemetry-sdk
 Requires-Dist: opentelemetry-instrumentation
 Requires-Dist: opentelemetry-resource-detector-azure
 Requires-Dist: opentelemetry-semantic-conventions
 Requires-Dist: psutil
 Requires-Dist: mock
 Requires-Dist: freezegun
+Requires-Dist: line-profiler
```

### Comparing `hypergo-0.3.6/RELEASE_NOTES.md` & `hypergo-0.3.7/RELEASE_NOTES.md`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/hypergo/azure_service_bus_connection.py` & `hypergo-0.3.7/hypergo/azure_service_bus_connection.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/hypergo/config.py` & `hypergo-0.3.7/hypergo/config.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/hypergo/connection.py` & `hypergo-0.3.7/hypergo/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from hypergo.config import ConfigType
 from hypergo.executor import Executor
 from hypergo.message import MessageType
 from hypergo.monitor import collect_metrics
 
 
 class Connection(ABC):
+
     def general_consume(self, message: MessageType, **kwargs: Any) -> None:
         config: ConfigType = kwargs.pop("config")
         executor: Executor = Executor(config, **kwargs)
         self.__send_message(executor=executor, message=message, config=config)
 
     @collect_metrics
     def __send_message(self, executor: Executor, message: MessageType, config: ConfigType) -> None:
```

### Comparing `hypergo-0.3.6/hypergo/connectors/azure_application_insights.py` & `hypergo-0.3.7/hypergo/connectors/azure_application_insights.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/hypergo/executor.py` & `hypergo-0.3.7/hypergo/executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,35 +38,41 @@
 
 
 def do_substitution(value: Any, data: Dict[str, Any]) -> Any:
     @traverse_datastructures
     def substitute(string: str, data: Dict[str, Any]) -> Any:
         result = string
         if isinstance(string, str):
-            match: Optional[Match[str]] = re.match(r"^{([^}]+)}$", string)
+            matched_regex: Optional[Match[str]] = re.match(r"^{([^}]+)}$", string)
             result = (
                 Utility.deep_get(
                     data,
-                    do_question_mark(data, match.group(1)),
-                    match.group(0),
+                    do_question_mark(data, matched_regex.group(1)),
+                    matched_regex.group(0),
                 )
-                if match
+                # version 2.0.0 and above
+                if matched_regex
+                # backward compatibility
                 else re.sub(
                     r"{([^}]+)}",
                     lambda match: str(
                         Utility.deep_get(
                             data,
                             do_question_mark(data, match.group(1)),
                             match.group(0),
                         )
                     ),
                     string,
                 )
             )
 
+            # We were substituting message.* in the string with the actual payload
+            if re.match(r"^.*\{message\.[^\}]+\}.*$", string):
+                return result
+
         if result != string:
             result = substitute(result, data)
         return result
 
     return substitute(value, data)
 
 
@@ -129,39 +135,39 @@
         self._config = config
 
     def get_args(self, context: ContextType) -> List[Any]:
         return [
             val if argtype == inspect.Parameter.empty else Utility.safecast(argtype, val)
             for val, argtype in zip(
                 do_substitution(
-                    Utility.deep_get(self._config, "input_bindings"),
+                    Utility.deep_get(self.config, "input_bindings"),
                     cast(Dict[str, Any], context),
                 ),
                 self._arg_spec,
             )
         ]
 
     def get_output_routing_key(self, input_message_routing_key: str) -> str:
         routing_key_set: Set[str] = set(input_message_routing_key.split("."))
         tokens: List[str] = []
-        for input_key in self._config["input_keys"]:
+        for input_key in self.config["input_keys"]:
             # hypergo-144 dynamic routing key only for generic components
             # output key will contain context derived from the previous
             # producer routing key
             input_key_set: Set[str] = set(input_key.split("."))
             intersection_set: Set[str] = routing_key_set.intersection(input_key_set)
             # check if the routing key is in the input_key
             if intersection_set == input_key_set:
                 # set difference operation to remove the subset of the routing key captured by the component
                 # from its input_key and append it to tokens
                 tokens.append(".".join(routing_key_set.difference(intersection_set)))
         token: str = self.organize_tokens(tokens)
         output_tokens: List[str] = [
             re.sub(r"(?<=\.)\?(?=\.)|^\?|(?<=\.)\?$|^\?$", token, output_key)
-            for output_key in self._config["output_keys"]
+            for output_key in self.config["output_keys"]
         ]
         return self.organize_tokens(output_tokens)
 
     @configsubstitution
     @Transform.operation("pass_by_reference")
     @Transform.operation("compression")
     @Transform.operation("encryption")
@@ -190,23 +196,23 @@
                 "routingkey": output_routing_key,
                 "body": {},
                 "transaction": Utility.deep_get(context, "message.transaction"),
                 # "__txid__": Utility.deep_get(context, "message.__txid__"),
             }
             output_context: ContextType = {
                 "message": output_message,
-                "config": self._config,
+                "config": self.config,
             }
 
             def handle_tuple(dst: ContextType, src: Any) -> None:
-                for binding, tuple_elem in zip(self._config["output_bindings"], src):
+                for binding, tuple_elem in zip(self.config["output_bindings"], src):
                     Utility.deep_set(dst, binding, tuple_elem)
 
             def handle_default(dst: ContextType, src: Any) -> None:
-                for binding in self._config["output_bindings"]:
+                for binding in self.config["output_bindings"]:
                     Utility.deep_set(dst, binding, src)
 
             if isinstance(return_value, tuple):
                 handle_tuple(output_context, return_value)
             else:
                 handle_default(output_context, return_value)
```

### Comparing `hypergo-0.3.6/hypergo/graph.py` & `hypergo-0.3.7/hypergo/graph.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/hypergo/hypergo_cli.py` & `hypergo-0.3.7/hypergo/hypergo_cli.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/hypergo/hypergo_click.py` & `hypergo-0.3.7/hypergo/hypergo_click.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/hypergo/hypergo_cmd.py` & `hypergo-0.3.7/hypergo/hypergo_cmd.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/hypergo/local_storage.py` & `hypergo-0.3.7/hypergo/local_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/hypergo/logger.py` & `hypergo-0.3.7/hypergo/logger.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/hypergo/loggers/azure_logger.py` & `hypergo-0.3.7/hypergo/loggers/azure_logger.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/hypergo/loggers/base_logger.py` & `hypergo-0.3.7/hypergo/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/hypergo/loggers/hypergo_logger.py` & `hypergo-0.3.7/hypergo/loggers/hypergo_logger.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/hypergo/mapping.py` & `hypergo-0.3.7/hypergo/mapping.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/hypergo/message.py` & `hypergo-0.3.7/hypergo/message.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/hypergo/metrics/base_metrics.py` & `hypergo-0.3.7/hypergo/metrics/base_metrics.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/hypergo/metrics/custom_metrics.py` & `hypergo-0.3.7/hypergo/metrics/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/hypergo/metrics/hypergo_metrics.py` & `hypergo-0.3.7/hypergo/metrics/hypergo_metrics.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/hypergo/monitor.py` & `hypergo-0.3.7/hypergo/monitor.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/hypergo/stdio_connection.py` & `hypergo-0.3.7/hypergo/stdio_connection.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/hypergo/storage.py` & `hypergo-0.3.7/hypergo/storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/hypergo/transaction.py` & `hypergo-0.3.7/hypergo/transaction.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/hypergo/transform.py` & `hypergo-0.3.7/hypergo/transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from functools import wraps
-from typing import Any, Callable, Dict, Generator, List, Tuple, TypeVar, cast
+from typing import (Any, Callable, Dict, Generator, List, Tuple, TypeVar,
+                    Union, cast)
 
-from hypergo.custom_types import JsonDict
+from hypergo.custom_types import JsonDict, TypedDictType
 from hypergo.storage import Storage
 from hypergo.transaction import Transaction
 from hypergo.utility import Utility, root_node
 
 T = TypeVar("T")
 
 ENCRYPTIONKEY = "KRAgZMBXbP1OQQEJPvMTa6nfkVq63sgL2ULJIaMgfLA="
@@ -142,25 +143,29 @@
     @staticmethod
     def remove_context(data: Any, key: str) -> Any:
         return data
 
     @staticmethod
     @root_node
     @config_v0_v1_passbyreference_backward_compatible
-    def storebyreference(data: Any, key: str, base_storage: Storage) -> Any:
+    def storebyreference(
+        data: Union[TypedDictType, Dict[str, Any]], key: str, base_storage: Storage
+    ) -> Union[TypedDictType, Dict[str, Any]]:
         storage: Storage = base_storage.use_sub_path("passbyreference")
         str_result = Utility.stringify(Utility.deep_get(data, key))
         out_storage_key = f"storagekey_{Utility.hash(str_result)}"
         storage.save(out_storage_key, str_result)
         Utility.deep_set(data, key, out_storage_key)
         return data
 
     @staticmethod
     @root_node
     @config_v0_v1_passbyreference_backward_compatible
-    def fetchbyreference(data: Any, key: str, base_storage: Storage) -> Any:
+    def fetchbyreference(
+        data: Union[TypedDictType, Dict[str, Any]], key: str, base_storage: Storage
+    ) -> Union[TypedDictType, Dict[str, Any]]:
         storage = base_storage.use_sub_path("passbyreference")
         storage_key = Utility.deep_get(cast(JsonDict, data), key)
         loaded = storage.load(storage_key)
         the_data = Utility.objectify(loaded)
         Utility.deep_set(data, key, the_data)
         return data
```

### Comparing `hypergo-0.3.6/hypergo/utility.py` & `hypergo-0.3.7/hypergo/utility.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,108 @@
+from __future__ import print_function
+
 import base64
 import binascii
+import cProfile
 import hashlib
 import inspect
 import json
 import lzma
 import os
 import uuid
+from collections import deque
 from datetime import datetime
 from functools import wraps
 from importlib import import_module
+from itertools import chain
+from sys import getsizeof, stderr
 from types import ModuleType
 from typing import (Any, Callable, Dict, Mapping, Optional, Tuple, Union, cast,
                     get_origin)
 
 import dill
-import glom
+#import glom
 import pydash
 import yaml
 from cryptography.fernet import Fernet
+from line_profiler import LineProfiler
 
 from hypergo.custom_types import JsonType, TypedDictType
 
 
+# ref https://code.activestate.com/recipes/577504/
+def total_size(o: object, verbose: bool = False) -> int:
+    """Returns the approximate memory footprint an object and all of its contents.
+
+    Automatically finds the contents of the following builtin containers and
+    their subclasses:  tuple, list, deque, dict, set and frozenset.
+
+    """
+
+    def dict_handler(d: Dict[Any, Any]) -> Any:
+        return chain.from_iterable(d.items())
+
+    all_handlers: Dict[Any, Any] = {
+        tuple: iter,
+        list: iter,
+        deque: iter,
+        dict: dict_handler,
+        set: iter,
+        frozenset: iter,
+    }
+
+    seen = set()  # track which object id's have already been seen
+    # estimate sizeof object without __sizeof__
+    default_size = getsizeof(0)
+
+    def sizeof(o: object) -> int:
+        if id(o) in seen:  # do not double count the same object
+            return 0
+        seen.add(id(o))
+        s = getsizeof(o, default_size)
+
+        if verbose:
+            print(s, type(o), repr(o), file=stderr)
+
+        for typ, handler in all_handlers.items():
+            if isinstance(o, typ):
+                s += sum(map(sizeof, handler(o)))
+                break
+        return s
+
+    return sizeof(o)
+
+
+def do_cprofile(func: Callable[..., Any]) -> Callable[..., Any]:
+    def profiled_func(*args: Tuple[Any, ...], **kwargs: Any) -> Any:
+        profile = cProfile.Profile(builtins=False)
+        try:
+            profile.enable()
+            result = func(*args, **kwargs)
+            profile.disable()
+            return result
+        finally:
+            profile.print_stats("cumtime")
+
+    return profiled_func
+
+
+def do_line_profile(func: Callable[..., Any]) -> Callable[..., Any]:
+    def profiled_func(*args: Tuple[Any, ...], **kwargs: Any) -> Any:
+        try:
+            profiler = LineProfiler()
+            profiler.add_function(func)
+            profiler.enable_by_count()
+            return func(*args, **kwargs)
+        finally:
+            profiler.print_stats()
+
+    return profiled_func
+
+
 def traverse_datastructures(func: Callable[..., Any]) -> Callable[..., Any]:
     @wraps(func)
     def wrapper(value: Any, *args: Tuple[Any, ...]) -> Any:
         handlers: Dict[type, Callable[[Any], Any]] = {
             dict: lambda _dict, *args: {wrapper(key, *args): wrapper(val, *args) for key, val in _dict.items()},
             list: lambda _list, *args: [wrapper(item, *args) for item in _list],
             tuple: lambda _tuple, *args: tuple(wrapper(item, *args) for item in _tuple),
@@ -86,15 +163,16 @@
     ) -> Any:
         if not pydash.has(dic, key) and default_sentinel == object:
             raise KeyError(f"Spec \"{key}\" not found in the dictionary {json.dumps(Utility.serialize(dic, None))}")
         return pydash.get(dic, key, default_sentinel)
 
     @staticmethod
     def deep_set(dic: Union[TypedDictType, Dict[str, Any]], key: str, val: Any) -> None:
-        glom.assign(dic, key, val, missing=dict)
+        #glom.assign(dic, key, val, missing=dict)
+        pydash.set_(dic, key, val)
 
     @staticmethod
     def yaml_read(file_name: str) -> Mapping[str, Any]:
         with open(file_name, "r", encoding="utf-8") as file_handle:
             return cast(Mapping[str, Any], yaml.safe_load(file_handle))
 
     @staticmethod
```

### Comparing `hypergo-0.3.6/hypergo/version.py` & `hypergo-0.3.7/hypergo/version.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/hypergo.egg-info/PKG-INFO` & `hypergo-0.3.7/hypergo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypergo
-Version: 0.3.6
+Version: 0.3.7
 Summary: Project for service bus
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml
 Requires-Dist: glom
 Requires-Dist: pydash
 Requires-Dist: azure-servicebus
@@ -25,7 +25,8 @@
 Requires-Dist: opentelemetry-sdk
 Requires-Dist: opentelemetry-instrumentation
 Requires-Dist: opentelemetry-resource-detector-azure
 Requires-Dist: opentelemetry-semantic-conventions
 Requires-Dist: psutil
 Requires-Dist: mock
 Requires-Dist: freezegun
+Requires-Dist: line-profiler
```

### Comparing `hypergo-0.3.6/lint.sh` & `hypergo-0.3.7/lint.sh`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/setup.cfg` & `hypergo-0.3.7/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hypergo
-version = 0.3.6
+version = 0.3.7
 description = Project for service bus
 long_description_content_type = text/markdown
 
 [options]
 packages = find:
 install_requires = 
 	pyyaml
@@ -29,12 +29,13 @@
 	opentelemetry-sdk
 	opentelemetry-instrumentation
 	opentelemetry-resource-detector-azure
 	opentelemetry-semantic-conventions
 	psutil
 	mock
 	freezegun
+	line-profiler
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `hypergo-0.3.6/setup.py` & `hypergo-0.3.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 
 
 # Define the setup parameters
 setup(
     name='hypergo',
-    version='0.3.6',  # Enclose the version number in quotes
+    version='0.3.7',  # Enclose the version number in quotes
     description='Project for service bus',
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         "pyyaml",
 	    "glom",
 	    "pydash",
@@ -30,15 +30,16 @@
         "opentelemetry-instrumentation",
         "opentelemetry-sdk",
         "opentelemetry-instrumentation",
         "opentelemetry-resource-detector-azure",
         "opentelemetry-semantic-conventions",
         "psutil",
         "mock",
-        "freezegun"
+        "freezegun",
+        "line-profiler"
     ],
     entry_points={
         "console_scripts": [
             "hypergo=hypergo.hypergo_click:main"
         ]
     },
```

### Comparing `hypergo-0.3.6/tests/test.json` & `hypergo-0.3.7/tests/test.json`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/tests/test.yaml` & `hypergo-0.3.7/tests/test.yaml`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/tests/test_azure_logger.py` & `hypergo-0.3.7/tests/test_azure_logger.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/tests/test_azure_monitor.py` & `hypergo-0.3.7/tests/test_azure_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,19 @@
         self.message: MessageType = {
             "routingkey": "workday.scheduled"
         }
         return super().setUp()
 
     @collect_metrics
     def __mock_send_message(self, executor: Executor, message: MessageType, config: ConfigType):
-        for _ in executor.execute(message):
-            _
+        try:
+            for _ in executor.execute(message):
+                _
+        except Exception:
+            pass
 
     @patch.dict(os.environ, {"APPLICATIONINSIGHTS-CONNECTION-STRING": f"InstrumentationKey={uuid4()};IngestionEndpoint=https://eastus2-3.in.applicationinsights.azure.com/;LiveEndpoint=https://eastus2.livediagnostics.monitor.azure.com/"})
     @patch("opentelemetry.sdk.metrics.export.MetricReader.collect")
     @patch("hypergo.metrics.hypergo_metrics.HypergoMetric.send")
     @patch("hypergo.secrets.LocalSecrets")
     def test_azure_monitor(self, mock_secrets, mock_send, mock_collect):
         cfg: ConfigType = {
```

### Comparing `hypergo-0.3.6/tests/test_dynamic_input_bindings.py` & `hypergo-0.3.7/tests/test_dynamic_input_bindings.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/tests/test_dynamic_routing_key.py` & `hypergo-0.3.7/tests/test_dynamic_routing_key.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/tests/test_local_storage.py` & `hypergo-0.3.7/tests/test_local_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/tests/test_message.py` & `hypergo-0.3.7/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/tests/test_stdio_monitor.py` & `hypergo-0.3.7/tests/test_stdio_monitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,19 @@
         self.message: MessageType = {
             "routingkey": "workday.scheduled"
         }
         return super().setUp()
 
     @collect_metrics
     def __mock_send_message(self, executor: Executor, message: MessageType, config: ConfigType):
-        for _ in executor.execute(message):
-            _
+        try:
+            for _ in executor.execute(message):
+                _
+        except Exception:
+            pass
 
     @patch("hypergo.metrics.hypergo_metrics.HypergoMetric.send")
     @patch("opentelemetry.sdk.metrics.export.PeriodicExportingMetricReader.collect")
     def test_stdio_monitor(self, mock_collect, mock_send):
         cfg: ConfigType = {
                                 "version": "2.0.0",
                                 "namespace": "datalink",
```

### Comparing `hypergo-0.3.6/tests/test_storage.py` & `hypergo-0.3.7/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/tests/test_utility.py` & `hypergo-0.3.7/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.6/tests/test_utility_serialization.py` & `hypergo-0.3.7/tests/test_utility_serialization.py`

 * *Files identical despite different names*

