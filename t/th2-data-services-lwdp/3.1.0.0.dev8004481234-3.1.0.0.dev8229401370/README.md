# Comparing `tmp/th2_data_services_lwdp-3.1.0.0.dev8004481234.tar.gz` & `tmp/th2_data_services_lwdp-3.1.0.0.dev8229401370.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services_lwdp-3.1.0.0.dev8004481234.tar", last modified: Thu Feb 22 12:31:31 2024, max compression
+gzip compressed data, was "dist/th2_data_services_lwdp-3.1.0.0.dev8229401370.tar", last modified: Mon Mar 11 07:59:43 2024, max compression
```

## Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234.tar` & `th2_data_services_lwdp-3.1.0.0.dev8229401370.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:31:31.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12960 2024-02-22 12:31:31.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10382 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-22 12:31:14.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/package_info.json
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 12:31:31.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:31:31.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:31:31.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:31:31.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:31:31.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:31:31.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    68705 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/commands/http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:31:31.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/data_source/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/data_source/http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:31:31.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/event_tree/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:31:31.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/filters/event_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/filters/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/init_resolvers_by_import.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:31:31.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/interfaces/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/message_response_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:31:31.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/source_api/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/source_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/source_api/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:31:31.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/utils/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/utils/_response_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-02-22 12:30:05.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/utils/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 12:31:31.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services_lwdp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12960 2024-02-22 12:31:30.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services_lwdp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-02-22 12:31:31.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services_lwdp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 12:31:30.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services_lwdp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-22 12:31:30.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services_lwdp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-22 12:31:30.000000 th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services_lwdp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 07:59:43.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12960 2024-03-11 07:59:43.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10382 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-11 07:59:27.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 07:59:43.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 07:59:43.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 07:59:43.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 07:59:43.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 07:59:43.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 07:59:43.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75754 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/commands/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 07:59:43.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/data_source/
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/data_source/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 07:59:43.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 07:59:43.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/filters/event_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/filters/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/init_resolvers_by_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 07:59:43.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/interfaces/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/message_response_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 07:59:43.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/source_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/source_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/source_api/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 07:59:43.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/utils/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/utils/_response_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-03-11 07:58:19.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/utils/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 07:59:43.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services_lwdp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12960 2024-03-11 07:59:42.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services_lwdp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-11 07:59:43.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services_lwdp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 07:59:42.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services_lwdp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-11 07:59:42.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services_lwdp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-11 07:59:42.000000 th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services_lwdp.egg-info/top_level.txt
```

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/PKG-INFO` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_data_services_lwdp
-Version: 3.1.0.0.dev8004481234
+Version: 3.1.0.0.dev8229401370
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 3).
         # Introduction
```

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/README.md` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/setup.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/__init__.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/adapters/__init__.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/adapters/adapter_sse.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/adapters/adapter_sse.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/commands/__init__.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/commands/http.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/commands/http.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,30 +21,35 @@
 import http as aiohttp
 from deprecated.classic import deprecated
 import json
 
 import requests
 from th2_data_services.data import Data
 from th2_data_services.exceptions import EventNotFound, MessageNotFound
-from th2_data_services.utils.converters import DatetimeConverter, ProtobufTimestampConverter
+from th2_data_services.utils.converters import (
+    UniversalDatetimeStringConverter,
+    UnixTimestampConverter,
+    DatetimeConverter,
+    ProtobufTimestampConverter,
+)
 
 from th2_data_services.data_source.lwdp import Page
 from th2_data_services.data_source.lwdp.interfaces.command import IHTTPCommand
 from th2_data_services.data_source.lwdp.data_source.http import DataSource
 from th2_data_services.data_source.lwdp.source_api.http import API
 from th2_data_services.data_source.lwdp.streams import Streams, Stream
 from th2_data_services.utils.sse_client import SSEClient
 from th2_data_services.data_source.lwdp.adapters.adapter_sse import (
     SSEAdapter,
     DEFAULT_BUFFER_LIMIT,
 )
 from th2_data_services.utils.decode_error_handler import UNICODE_REPLACE_HANDLER
 from th2_data_services.data_source.lwdp.filters.event_filters import EventFilter
 from th2_data_services.data_source.lwdp.utils import (
-    _check_datetime,
+    _check_timestamp,
     _check_list_or_tuple,
     _check_response_formats,
 )
 from th2_data_services.data_source.lwdp.utils._misc import (
     get_utc_datetime_now,
     _get_response_format,
 )
@@ -173,29 +178,29 @@
     Returns:
         dict: List[str].
     """
 
     def __init__(
         self,
         book_id: str,
-        start_timestamp: datetime = None,
-        end_timestamp: datetime = None,
+        start_timestamp: Union[datetime, str, int] = None,
+        end_timestamp: Union[datetime, str, int] = None,
         cache: bool = False,
         char_enc: str = "utf-8",
         decode_error_handler: str = UNICODE_REPLACE_HANDLER,
         buffer_limit: int = DEFAULT_BUFFER_LIMIT,
     ) -> None:
         """GetEventScopes Constructor.
 
         If start_timestamp and end_timestamp are not provided, it returns all aliases.
 
         Args:
             book_id (str): Book ID.
-            start_timestamp (datetime): Start Timestamp.
-            end_timestamp (datetime): End Timestamp.
+            start_timestamp (datetime): Start Timestamp. Can be datetime object, datetime string or unix timestamp integer.
+            end_timestamp (datetime): End Timestamp. Can be datetime object, datetime string or unix timestamp integer.
             cache: If True, all requested data from lw-data-provider will be saved to cache.
             char_enc: Encoding for the byte stream.
             decode_error_handler: Registered decode error handler.
             max_url_length: API request url max length.
             buffer_limit: SSEAdapter BufferedJSONProcessor buffer limit.
         """
         super().__init__(
@@ -203,18 +208,30 @@
             buffer_limit=buffer_limit,
             char_enc=char_enc,
             decode_error_handler=decode_error_handler,
         )
         if all(timestamp is None for timestamp in (start_timestamp, end_timestamp)):
             self._all_results = True
         else:
-            _check_datetime(start_timestamp)
-            _check_datetime(end_timestamp)
-            self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
-            self._end_timestamp = DatetimeConverter.to_nanoseconds(end_timestamp)
+            _check_timestamp(start_timestamp)
+            _check_timestamp(end_timestamp)
+            if isinstance(start_timestamp, datetime):
+                self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
+            if isinstance(start_timestamp, str):
+                self._start_timestamp = UniversalDatetimeStringConverter.to_nanoseconds(
+                    start_timestamp
+                )
+            if isinstance(start_timestamp, int):
+                self._start_timestamp = UnixTimestampConverter.to_nanoseconds(start_timestamp)
+            if isinstance(end_timestamp, datetime):
+                self._end_timestamp = DatetimeConverter.to_nanoseconds(end_timestamp)
+            if isinstance(end_timestamp, str):
+                self._end_timestamp = UniversalDatetimeStringConverter.to_nanoseconds(end_timestamp)
+            if isinstance(end_timestamp, int):
+                self._end_timestamp = UnixTimestampConverter.to_nanoseconds(end_timestamp)
             self._all_results = False
         self._book_id = book_id
 
     def _get_urls(self, data_source: DataSource):
         api = data_source.source_api
         if self._all_results:
             return [api.get_url_get_scopes(book_id=self._book_id)]
@@ -246,29 +263,29 @@
     Returns:
         dict: List[str].
     """
 
     def __init__(
         self,
         book_id: str,
-        start_timestamp: datetime = None,
-        end_timestamp: datetime = None,
+        start_timestamp: Union[datetime, str, int] = None,
+        end_timestamp: Union[datetime, str, int] = None,
         cache: bool = False,
         char_enc: str = "utf-8",
         decode_error_handler: str = UNICODE_REPLACE_HANDLER,
         buffer_limit: int = DEFAULT_BUFFER_LIMIT,
     ) -> None:
         """GetMessageAliases Constructor.
 
         If start_timestamp and end_timestamp are not provided, it returns all aliases.
 
         Args:
             book_id (str): Book ID.
-            start_timestamp (datetime): Start Timestamp.
-            end_timestamp (datetime): End Timestamp.
+            start_timestamp (datetime): Start Timestamp. Can be datetime object, datetime string or unix timestamp integer.
+            end_timestamp (datetime): End Timestamp. Can be datetime object, datetime string or unix timestamp integer.
             cache: If True, all requested data from lw-data-provider will be saved to cache.
             char_enc: Encoding for the byte stream.
             decode_error_handler: Registered decode error handler.
             max_url_length: API request url max length.
             buffer_limit: SSEAdapter BufferedJSONProcessor buffer limit.
         """
         super().__init__(
@@ -276,18 +293,30 @@
             buffer_limit=buffer_limit,
             char_enc=char_enc,
             decode_error_handler=decode_error_handler,
         )
         if all(timestamp is None for timestamp in (start_timestamp, end_timestamp)):
             self._all_results = True
         else:
-            _check_datetime(start_timestamp)
-            _check_datetime(end_timestamp)
-            self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
-            self._end_timestamp = DatetimeConverter.to_nanoseconds(end_timestamp)
+            _check_timestamp(start_timestamp)
+            _check_timestamp(end_timestamp)
+            if isinstance(start_timestamp, datetime):
+                self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
+            if isinstance(start_timestamp, str):
+                self._start_timestamp = UniversalDatetimeStringConverter.to_nanoseconds(
+                    start_timestamp
+                )
+            if isinstance(start_timestamp, int):
+                self._start_timestamp = UnixTimestampConverter.to_nanoseconds(start_timestamp)
+            if isinstance(end_timestamp, datetime):
+                self._end_timestamp = DatetimeConverter.to_nanoseconds(end_timestamp)
+            if isinstance(end_timestamp, str):
+                self._end_timestamp = UniversalDatetimeStringConverter.to_nanoseconds(end_timestamp)
+            if isinstance(end_timestamp, int):
+                self._end_timestamp = UnixTimestampConverter.to_nanoseconds(end_timestamp)
             self._all_results = False
         self._book_id = book_id
 
     def _get_urls(self, data_source: DataSource):
         api = data_source.source_api
         if self._all_results:
             return [api.get_url_get_message_aliases(book_id=self._book_id)]
@@ -321,29 +350,29 @@
     Returns:
         dict: List[str].
     """
 
     def __init__(
         self,
         book_id: str,
-        start_timestamp: datetime = None,
-        end_timestamp: datetime = None,
+        start_timestamp: Union[datetime, str, int] = None,
+        end_timestamp: Union[datetime, str, int] = None,
         cache: bool = False,
         char_enc: str = "utf-8",
         decode_error_handler: str = UNICODE_REPLACE_HANDLER,
         buffer_limit: int = DEFAULT_BUFFER_LIMIT,
     ) -> None:
         """GetMessageGroups Constructor.
 
         If start_timestamp and end_timestamp are not provided, it returns all aliases.
 
         Args:
             book_id (str): Book ID.
-            start_timestamp (datetime): Start Timestamp.
-            end_timestamp (datetime): End Timestamp.
+            start_timestamp (datetime): Start Timestamp. Can be datetime object, datetime string or unix timestamp integer.
+            end_timestamp (datetime): End Timestamp. Can be datetime object, datetime string or unix timestamp integer.
             cache: If True, all requested data from lw-data-provider will be saved to cache.
             char_enc: Encoding for the byte stream.
             decode_error_handler: Registered decode error handler.
             max_url_length: API request url max length.
             buffer_limit: SSEAdapter BufferedJSONProcessor buffer limit.
         """
         super().__init__(
@@ -351,18 +380,30 @@
             buffer_limit=buffer_limit,
             char_enc=char_enc,
             decode_error_handler=decode_error_handler,
         )
         if all(timestamp is None for timestamp in (start_timestamp, end_timestamp)):
             self._all_results = True
         else:
-            _check_datetime(start_timestamp)
-            _check_datetime(end_timestamp)
-            self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
-            self._end_timestamp = DatetimeConverter.to_nanoseconds(end_timestamp)
+            _check_timestamp(start_timestamp)
+            _check_timestamp(end_timestamp)
+            if isinstance(start_timestamp, datetime):
+                self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
+            if isinstance(start_timestamp, str):
+                self._start_timestamp = UniversalDatetimeStringConverter.to_nanoseconds(
+                    start_timestamp
+                )
+            if isinstance(start_timestamp, int):
+                self._start_timestamp = UnixTimestampConverter.to_nanoseconds(start_timestamp)
+            if isinstance(end_timestamp, datetime):
+                self._end_timestamp = DatetimeConverter.to_nanoseconds(end_timestamp)
+            if isinstance(end_timestamp, str):
+                self._end_timestamp = UniversalDatetimeStringConverter.to_nanoseconds(end_timestamp)
+            if isinstance(end_timestamp, int):
+                self._end_timestamp = UnixTimestampConverter.to_nanoseconds(end_timestamp)
             self._all_results = False
         self._book_id = book_id
 
     def _get_urls(self, data_source: DataSource):
         api = data_source.source_api
         if self._all_results:
             return [api.get_url_get_message_groups(book_id=self._book_id)]
@@ -443,44 +484,56 @@
             raise PageNotFound(self._page_name, self._book_id)
 
 
 class GetPages(SSEHandlerClassBase):
     def __init__(
         self,
         book_id: str,
-        start_timestamp: datetime = None,
-        end_timestamp: datetime = None,
+        start_timestamp: Union[datetime, str, int] = None,
+        end_timestamp: Union[datetime, str, int] = None,
         result_limit: int = None,
         cache: bool = False,
         char_enc: str = "utf-8",
         decode_error_handler: str = UNICODE_REPLACE_HANDLER,
         buffer_limit: int = DEFAULT_BUFFER_LIMIT,
     ) -> None:
         """GetPages Constructor.
 
         If start_timestamp and end_timestamp are not provided, it returns all Pages.
 
         Args:
             book_id (str): Book ID.
-            start_timestamp (datetime): Start Timestamp.
-            end_timestamp (datetime): End Timestamp.
+            start_timestamp (datetime): Start Timestamp. Can be datetime object, datetime string or unix timestamp integer.
+            end_timestamp (datetime): End Timestamp. Can be datetime object, datetime string or unix timestamp integer.
             result_limit (Optional, int): Return Result Limit.
             cache: If True, all requested data from lw-data-provider will be saved to cache.
             char_enc: Encoding for the byte stream.
             decode_error_handler: Registered decode error handler.
             max_url_length: API request url max length.
             buffer_limit: SSEAdapter BufferedJSONProcessor buffer limit.
         """
         if all(timestamp is None for timestamp in (start_timestamp, end_timestamp)):
             self._all_results = True
         else:
-            _check_datetime(start_timestamp)
-            _check_datetime(end_timestamp)
-            self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
-            self._end_timestamp = DatetimeConverter.to_nanoseconds(end_timestamp)
+            _check_timestamp(start_timestamp)
+            _check_timestamp(end_timestamp)
+            if isinstance(start_timestamp, datetime):
+                self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
+            if isinstance(start_timestamp, str):
+                self._start_timestamp = UniversalDatetimeStringConverter.to_nanoseconds(
+                    start_timestamp
+                )
+            if isinstance(start_timestamp, int):
+                self._start_timestamp = UnixTimestampConverter.to_nanoseconds(start_timestamp)
+            if isinstance(end_timestamp, datetime):
+                self._end_timestamp = DatetimeConverter.to_nanoseconds(end_timestamp)
+            if isinstance(end_timestamp, str):
+                self._end_timestamp = UniversalDatetimeStringConverter.to_nanoseconds(end_timestamp)
+            if isinstance(end_timestamp, int):
+                self._end_timestamp = UnixTimestampConverter.to_nanoseconds(end_timestamp)
             self._all_results = False
         super().__init__(
             cache=cache,
             buffer_limit=buffer_limit,
             char_enc=char_enc,
             decode_error_handler=decode_error_handler,
         )
@@ -722,18 +775,18 @@
 
     Returns:
         Iterable[dict]: Stream of Th2 events.
     """
 
     def __init__(
         self,
-        start_timestamp: datetime,
+        start_timestamp: Union[datetime, str, int],
         book_id: str,
         scopes: List[str],
-        end_timestamp: Optional[datetime] = None,
+        end_timestamp: Optional[Union[datetime, str, int]] = None,
         parent_event: str = None,
         search_direction: str = "next",
         result_count_limit: int = None,
         filters: Union[EventFilter, List[EventFilter]] = None,
         # Non-data source args.
         # +TODO - add `max_url_length: int = 2048,`
         #   It'll be required when you implement `__split_requests` in source_api/http.py
@@ -741,45 +794,56 @@
         char_enc: str = "utf-8",
         decode_error_handler: str = UNICODE_REPLACE_HANDLER,
         buffer_limit: int = DEFAULT_BUFFER_LIMIT,
     ):
         """GetEventsByBookByScopes constructor.
 
         Args:
-            start_timestamp: Start timestamp of search.
+            start_timestamp: Start timestamp of search. Can be datetime object, datetime string or unix timestamp integer.
             book_id: Book ID for messages.
             scopes: Scope names for events.
-            end_timestamp: End timestamp of search.
+            end_timestamp: End timestamp of search. Can be datetime object, datetime string or unix timestamp integer.
             parent_event: Match events to the specified parent.
             search_direction: Search direction.
             result_count_limit: Result count limit.
             filters: Filters using in search for messages.
             cache: If True, all requested data from lw-data-provider will be saved to cache.
             char_enc: Encoding for the byte stream.
             decode_error_handler: Registered decode error handler.
             max_url_length: API request url max length.
             buffer_limit: SSEAdapter BufferedJSONProcessor buffer limit.
         """
-        _check_datetime(start_timestamp)
+        _check_timestamp(start_timestamp)
         if end_timestamp:
-            _check_datetime(end_timestamp)
+            _check_timestamp(end_timestamp)
         super().__init__(
             cache=cache,
             buffer_limit=buffer_limit,
             char_enc=char_enc,
             decode_error_handler=decode_error_handler,
         )
 
         self._cache = cache
         # +TODO - we can make timestamps optional datetime or int. We have to check that it's in ms.
 
-        self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
-        self._end_timestamp = (
-            DatetimeConverter.to_nanoseconds(end_timestamp) if end_timestamp else None
-        )
+        if isinstance(start_timestamp, datetime):
+            self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
+        if isinstance(start_timestamp, str):
+            self._start_timestamp = UniversalDatetimeStringConverter.to_nanoseconds(start_timestamp)
+        if isinstance(start_timestamp, int):
+            self._start_timestamp = UnixTimestampConverter.to_nanoseconds(start_timestamp)
+        if end_timestamp:
+            if isinstance(end_timestamp, datetime):
+                self._end_timestamp = DatetimeConverter.to_nanoseconds(end_timestamp)
+            if isinstance(end_timestamp, str):
+                self._end_timestamp = UniversalDatetimeStringConverter.to_nanoseconds(end_timestamp)
+            if isinstance(end_timestamp, int):
+                self._end_timestamp = UnixTimestampConverter.to_nanoseconds(end_timestamp)
+        else:
+            self._end_timestamp = None
         self._parent_event = parent_event
         self._search_direction = search_direction
         self._result_count_limit = result_count_limit
         self._filters = filters
         self._book_id = book_id
         self._scopes = scopes
         if isinstance(filters, EventFilter):
@@ -1046,56 +1110,56 @@
 
     Returns:
         Iterable[dict]: Stream of Th2 messages.
     """
 
     def __init__(
         self,
-        start_timestamp: datetime,
+        start_timestamp: Union[datetime, str, int],
         book_id: str,
         streams: Union[List[Union[str, Streams, Stream]], Streams],
         message_ids: List[str] = None,
         search_direction: str = "next",
         result_count_limit: int = None,
-        end_timestamp: datetime = None,
+        end_timestamp: Union[datetime, str, int] = None,
         response_formats: Union[List[str], str] = None,
         keep_open: bool = False,
         # Non-data source args.
         # +TODO - we often repeat these args. Perhaps it's better to move them to some class.
         max_url_length: int = 2048,
         char_enc: str = "utf-8",
         decode_error_handler: str = UNICODE_REPLACE_HANDLER,
         cache: bool = False,
         buffer_limit: int = DEFAULT_BUFFER_LIMIT,
     ):
         """GetMessagesByBookByStreams constructor.
 
         Args:
-            start_timestamp: Start timestamp of search.
+            start_timestamp: Start timestamp of search. Can be datetime object, datetime string or unix timestamp integer.
             book_id: Book ID for messages
             streams: List of aliases to request. If direction is not specified all directions will be requested for stream.
             message_ids: List of message IDs to restore search. If given, it has
                 the highest priority and ignores streams (uses streams from ids), startTimestamp and resumeFromId.
             search_direction: Search direction.
             result_count_limit: Result count limit.
-            end_timestamp: End timestamp of search.
+            end_timestamp: End timestamp of search. Can be datetime object, datetime string or unix timestamp integer.
             response_formats: The format of the response
             keep_open: If the search has reached the current moment.
                 It needs to wait further for the appearance of new data.
             char_enc: Encoding for the byte stream.
             decode_error_handler: Registered decode error handler.
             cache: If True, all requested data from lw-data-provider will be saved to cache.
             max_url_length: API request url max length.
             buffer_limit: SSEAdapter BufferedJSONProcessor buffer limit.
         """
         response_formats = _get_response_format(response_formats)
         _check_response_formats(response_formats)
-        _check_datetime(start_timestamp)
+        _check_timestamp(start_timestamp)
         if end_timestamp:
-            _check_datetime(end_timestamp)
+            _check_timestamp(end_timestamp)
         super().__init__(
             cache=cache,
             buffer_limit=buffer_limit,
             char_enc=char_enc,
             decode_error_handler=decode_error_handler,
         )
 
@@ -1107,19 +1171,29 @@
         self._message_ids = message_ids
         self._book_id = book_id
         self._max_url_length = max_url_length
         self._char_enc = char_enc
         self._decode_error_handler = decode_error_handler
         self._cache = cache
 
-        # + TODO - we can make timestamps optional datetime or int
-        self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
-        self._end_timestamp = (
-            DatetimeConverter.to_nanoseconds(end_timestamp) if end_timestamp else None
-        )
+        if isinstance(start_timestamp, datetime):
+            self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
+        if isinstance(start_timestamp, str):
+            self._start_timestamp = UniversalDatetimeStringConverter.to_nanoseconds(start_timestamp)
+        if isinstance(start_timestamp, int):
+            self._start_timestamp = UnixTimestampConverter.to_nanoseconds(start_timestamp)
+        if end_timestamp:
+            if isinstance(end_timestamp, datetime):
+                self._end_timestamp = DatetimeConverter.to_nanoseconds(end_timestamp)
+            if isinstance(end_timestamp, str):
+                self._end_timestamp = UniversalDatetimeStringConverter.to_nanoseconds(end_timestamp)
+            if isinstance(end_timestamp, int):
+                self._end_timestamp = UnixTimestampConverter.to_nanoseconds(end_timestamp)
+        else:
+            self._end_timestamp = None
 
         if self._start_timestamp is None and not self._message_ids:
             raise TypeError("One of start_timestamp or message_id arguments must not be empty")
 
         if isinstance(streams, Streams):
             self._streams = streams.as_list()
         elif isinstance(streams, (tuple, list, Streams)):
@@ -1276,15 +1350,14 @@
 
             except requests.exceptions.HTTPError as e:
                 raise Exception(e)
 
             finally:
                 if task_id:
                     api.execute_delete(task_request_url)
-                    pass
 
     return do_req_and_store(f"{filename}.gz", headers, url, raw_body)
 
 
 class DownloadMessagesByPageByGroupsGzip(IHTTPCommand):
     """A Class-Command for request to lw-data-provider.
 
@@ -1325,17 +1398,17 @@
             streams: List of streams to search messages from the specified groups.
                 You will receive only the specified streams and directions for them.
                 You can specify direction for your streams.
                 e.g. ['stream_abc:1']. 1 - IN, 2 - OUT.
             fast_fail: If true, stops task execution right after first error.
         """
         response_formats = _get_response_format(response_formats)
-        _check_response_formats(response_formats) 
+        _check_response_formats(response_formats)
         self._filename = filename
-        if self._filename.endswith('.gz'):
+        if self._filename.endswith(".gz"):
             self._filename = self._filename[:-3]
         self._page = page
         self._book_id = book_id
         self._groups = groups
         self._streams = streams
         self._sort = sort
         self._response_formats = response_formats
@@ -1366,15 +1439,17 @@
             fast_fail=self._fast_fail,
         )
 
         headers = {"Accept": "application/stream+json", "Accept-Encoding": "gzip, deflate"}
 
         status = _download_messages(api, url, body, headers, self._filename)
 
-        return Data.from_json(f'{self._filename}.gz', gzip=True).update_metadata({"Task status": status})
+        return Data.from_json(f"{self._filename}.gz", gzip=True).update_metadata(
+            {"Task status": status}
+        )
 
 
 class DownloadMessagesByBookByGroupsGzip(IHTTPCommand):
     """A Class-Command for request to lw-data-provider.
 
     It searches messages stream by page & groups and downloads them.
     Beware that if you request this command with long list of groups,
@@ -1389,29 +1464,29 @@
     Returns:
         Nothing.
     """
 
     def __init__(
         self,
         filename: str,
-        start_timestamp: datetime,
-        end_timestamp: datetime,
+        start_timestamp: Union[datetime, str, int],
+        end_timestamp: Union[datetime, str, int],
         book_id: str,
         groups: List[str],
         sort: bool = None,
         response_formats: Union[List[str], str] = None,
         streams: List[str] = [],
         fast_fail: bool = True,
     ):
         """DownloadMessagesByBookByGroupsGzip Constructor.
 
         Args:
             filename: Filename of downloaded files.
-            start_timestamp: Sets the search starting point.
-            end_timestamp: Sets the timestamp to which the search will be performed, starting with 'start_timestamp'.
+            start_timestamp: Sets the search starting point. Can be datetime object, datetime string or unix timestamp integer.
+            end_timestamp: Sets the timestamp to which the search will be performed, starting with 'start_timestamp'. Can be datetime object, datetime string or unix timestamp integer.
 
             book_id: book ID for requested groups.
             groups: List of groups to search messages from.
             sort: Enables message sorting within a group. It is not sorted between groups.
                   (You cannot specify a direction in groups unlike streams.
                   It's possible to add it to the CradleAPI by request to dev team.)
             response_formats: The format of the response
@@ -1419,21 +1494,31 @@
                 You will receive only the specified streams and directions for them.
                 You can specify direction for your streams.
                 e.g. ['stream_abc:1']. 1 - IN, 2 - OUT.
             fast_fail: If true, stops task execution right after first error.
         """
         response_formats = _get_response_format(response_formats)
         _check_response_formats(response_formats)
-        _check_datetime(start_timestamp)
-        _check_datetime(end_timestamp)
+        _check_timestamp(start_timestamp)
+        _check_timestamp(end_timestamp)
         self._filename = filename
-        if self._filename.endswith('.gz'):
+        if self._filename.endswith(".gz"):
             self._filename = self._filename[:-3]
-        self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
-        self._end_timestamp = DatetimeConverter.to_nanoseconds(end_timestamp)
+        if isinstance(start_timestamp, datetime):
+            self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
+        if isinstance(start_timestamp, str):
+            self._start_timestamp = UniversalDatetimeStringConverter.to_nanoseconds(start_timestamp)
+        if isinstance(start_timestamp, int):
+            self._start_timestamp = UnixTimestampConverter.to_nanoseconds(start_timestamp)
+        if isinstance(end_timestamp, datetime):
+            self._end_timestamp = DatetimeConverter.to_nanoseconds(end_timestamp)
+        if isinstance(end_timestamp, str):
+            self._end_timestamp = UniversalDatetimeStringConverter.to_nanoseconds(end_timestamp)
+        if isinstance(end_timestamp, int):
+            self._end_timestamp = UnixTimestampConverter.to_nanoseconds(end_timestamp)
         self._groups = groups
         self._streams = streams
         self._sort = sort
         self._response_formats = response_formats
         self._book_id = book_id
         self._fast_fail = fast_fail
 
@@ -1453,30 +1538,30 @@
             response_formats=self._response_formats,
             fast_fail=self._fast_fail,
         )
         headers = {"Accept": "application/stream+json", "Accept-Encoding": "gzip, deflate"}
 
         status = _download_messages(api, url, body, headers, self._filename)
 
-        return Data.from_json(f'{self._filename}.gz', gzip=True).update_metadata(status)
+        return Data.from_json(f"{self._filename}.gz", gzip=True).update_metadata(status)
 
 
 class GetMessagesByBookByGroups(SSEHandlerClassBase):
     """A Class-Command for request to lw-data-provider.
 
     It searches messages stream by groups.
 
     Returns:
         Iterable[dict]: Stream of Th2 messages.
     """
 
     def __init__(
         self,
-        start_timestamp: datetime,
-        end_timestamp: datetime,
+        start_timestamp: Union[datetime, str, int],
+        end_timestamp: Union[datetime, str, int],
         book_id: str,
         groups: List[str],
         sort: bool = None,
         response_formats: Union[List[str], str] = None,
         keep_open: bool = None,
         streams: List[str] = None,
         # Non-data source args.
@@ -1485,16 +1570,16 @@
         decode_error_handler: str = UNICODE_REPLACE_HANDLER,
         cache: bool = False,
         buffer_limit=DEFAULT_BUFFER_LIMIT,
     ):
         """GetMessagesByBookByGroups Constructor.
 
         Args:
-            start_timestamp: Sets the search starting point.
-            end_timestamp: Sets the timestamp to which the search will be performed, starting with 'start_timestamp'.
+            start_timestamp: Sets the search starting point. Can be datetime object, datetime string or unix timestamp integer.
+            end_timestamp: Sets the timestamp to which the search will be performed, starting with 'start_timestamp'. Can be datetime object, datetime string or unix timestamp integer.
 
             book_id: book ID for requested groups.
             groups: List of groups to search messages from.
             sort: Enables message sorting within a group. It is not sorted between groups.
                   (You cannot specify a direction in groups unlike streams.
                   It's possible to add it to the CradleAPI by request to dev team.)
             response_formats: The format of the response
@@ -1507,28 +1592,38 @@
             decode_error_handler: Registered decode error handler.
             cache: If True, all requested data from lw-data-provider will be saved to cache.
             max_url_length: API request url max length.
             buffer_limit: SSEAdapter BufferedJSONProcessor buffer limit.
         """
         response_formats = _get_response_format(response_formats)
         _check_response_formats(response_formats)
-        _check_datetime(start_timestamp)
-        _check_datetime(end_timestamp)
+        _check_timestamp(start_timestamp)
+        _check_timestamp(end_timestamp)
         super().__init__(
             cache=cache,
             buffer_limit=buffer_limit,
             char_enc=char_enc,
             decode_error_handler=decode_error_handler,
         )
 
         self._char_enc = char_enc
         self._decode_error_handler = decode_error_handler
         self._cache = cache
-        self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
-        self._end_timestamp = DatetimeConverter.to_nanoseconds(end_timestamp)
+        if isinstance(start_timestamp, datetime):
+            self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
+        if isinstance(start_timestamp, str):
+            self._start_timestamp = UniversalDatetimeStringConverter.to_nanoseconds(start_timestamp)
+        if isinstance(start_timestamp, int):
+            self._start_timestamp = UnixTimestampConverter.to_nanoseconds(start_timestamp)
+        if isinstance(end_timestamp, datetime):
+            self._end_timestamp = DatetimeConverter.to_nanoseconds(end_timestamp)
+        if isinstance(end_timestamp, str):
+            self._end_timestamp = UniversalDatetimeStringConverter.to_nanoseconds(end_timestamp)
+        if isinstance(end_timestamp, int):
+            self._end_timestamp = UnixTimestampConverter.to_nanoseconds(end_timestamp)
         self._groups = groups
         self._streams = streams
         self._sort = sort
         self._response_formats = response_formats
         self._keep_open = keep_open
         self._book_id = book_id
         self._max_url_length = max_url_length
```

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/data_source/__init__.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/data_source/http.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/data_source/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/event_tree/__init__.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/filters/__init__.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/filters/event_filters.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/filters/event_filters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/filters/filter.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/filters/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/init_resolvers_by_import.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/init_resolvers_by_import.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/interfaces/__init__.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/interfaces/command.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/interfaces/data_source.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/interfaces/filter.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/interfaces/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/interfaces/source_api.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/message_response_format.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/message_response_format.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/page.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/page.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/resolver.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/source_api/__init__.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/source_api/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/source_api/http.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/source_api/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/streams.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/streams.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/struct.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/stub_builder.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/utils/__init__.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from ._misc import _check_list_or_tuple, _check_datetime, _check_response_formats
+from ._misc import _check_list_or_tuple, _check_timestamp, _check_response_formats
```

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/utils/_misc.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/utils/_misc.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,28 +8,30 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from datetime import datetime, timezone
-from typing import List
+from typing import List, Union
 
 from th2_data_services.data_source.lwdp import ResponseFormat
 from th2_data_services.data_source.lwdp.utils._response_formats import ResponseFormatsChecker
 
 
 def _check_list_or_tuple(variable, var_name):  # noqa
     if not (isinstance(variable, tuple) or isinstance(variable, list)):
         raise TypeError(f"{var_name} argument has to be list or tuple type. Got {type(variable)}")
 
 
-def _check_datetime(dt: datetime):
-    if not isinstance(dt, datetime):
-        raise TypeError("Provided timestamp should be `datetime` object in UTC time")
+def _check_timestamp(dt: Union[datetime, str, int]):
+    if not isinstance(dt, datetime) and not isinstance(dt, str) and not isinstance(dt, int):
+        raise TypeError(
+            "Provided timestamp should be `datetime`, `str` or `int` object in UTC time"
+        )
 
 
 def _check_response_formats(formats: List[str]):
     rf = ResponseFormatsChecker()
     if not rf.is_valid_response_format(formats):
         raise Exception("Invalid response format")
```

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/utils/_response_formats.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/utils/_response_formats.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services/data_source/lwdp/utils/json.py` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services/data_source/lwdp/utils/json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services_lwdp.egg-info/PKG-INFO` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services_lwdp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-data-services-lwdp
-Version: 3.1.0.0.dev8004481234
+Version: 3.1.0.0.dev8229401370
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 3).
         # Introduction
```

### Comparing `th2_data_services_lwdp-3.1.0.0.dev8004481234/th2_data_services_lwdp.egg-info/SOURCES.txt` & `th2_data_services_lwdp-3.1.0.0.dev8229401370/th2_data_services_lwdp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

