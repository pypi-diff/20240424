# Comparing `tmp/mctech_core-1.0.1.tar.gz` & `tmp/mctech_core-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mctech_core-1.0.1.tar", last modified: Mon Apr  1 02:10:01 2024, max compression
+gzip compressed data, was "mctech_core-1.0.2.tar", last modified: Wed Apr 24 08:22:14 2024, max compression
```

## Comparing `mctech_core-1.0.1.tar` & `mctech_core-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 02:10:01.672133 mctech_core-1.0.1/
--rw-rw-rw-   0        0        0      146 2024-04-01 02:10:01.672133 mctech_core-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      555 2024-04-01 02:09:31.000000 mctech_core-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 02:10:01.629675 mctech_core-1.0.1/mctech_core/
--rw-rw-rw-   0        0        0      131 2024-04-01 02:03:19.000000 mctech_core-1.0.1/mctech_core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 02:10:01.670012 mctech_core-1.0.1/mctech_core/config/
--rw-rw-rw-   0        0        0      977 2024-04-01 02:00:51.000000 mctech_core-1.0.1/mctech_core/config/__init__.py
--rw-rw-rw-   0        0        0     8300 2023-09-20 02:30:17.000000 mctech_core-1.0.1/mctech_core/config/_configure.py
--rw-rw-rw-   0        0        0     8384 2023-08-26 09:57:47.000000 mctech_core-1.0.1/mctech_core/config/config_merger.py
--rw-rw-rw-   0        0        0     1922 2022-10-08 03:15:48.000000 mctech_core-1.0.1/mctech_core/config/config_value.py
--rw-rw-rw-   0        0        0     1464 2023-05-12 06:58:39.000000 mctech_core-1.0.1/mctech_core/config/yaml_loader.py
-drwxrwxrwx   0        0        0        0 2024-04-01 02:10:01.651275 mctech_core-1.0.1/mctech_core.egg-info/
--rw-rw-rw-   0        0        0      146 2024-04-01 02:10:01.000000 mctech_core-1.0.1/mctech_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2024-04-01 02:10:01.000000 mctech_core-1.0.1/mctech_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 02:10:01.000000 mctech_core-1.0.1/mctech_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-01 02:10:01.000000 mctech_core-1.0.1/mctech_core.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-01 02:10:01.000000 mctech_core-1.0.1/mctech_core.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      258 2024-04-01 02:09:01.000000 mctech_core-1.0.1/mctech_core_setup.py
--rw-rw-rw-   0        0        0       42 2024-04-01 02:10:01.676555 mctech_core-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 08:22:14.665592 mctech_core-1.0.2/
+-rw-rw-rw-   0        0        0      146 2024-04-24 08:22:14.663593 mctech_core-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      555 2024-04-01 06:27:50.000000 mctech_core-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 08:22:14.608584 mctech_core-1.0.2/mctech_core/
+-rw-rw-rw-   0        0        0      161 2024-04-24 02:25:59.000000 mctech_core-1.0.2/mctech_core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:22:14.642584 mctech_core-1.0.2/mctech_core/config/
+-rw-rw-rw-   0        0        0      977 2024-04-01 06:27:50.000000 mctech_core-1.0.2/mctech_core/config/__init__.py
+-rw-rw-rw-   0        0        0     8300 2024-04-01 06:27:50.000000 mctech_core-1.0.2/mctech_core/config/_configure.py
+-rw-rw-rw-   0        0        0     8384 2024-04-01 06:27:50.000000 mctech_core-1.0.2/mctech_core/config/config_merger.py
+-rw-rw-rw-   0        0        0     1922 2024-04-01 06:27:50.000000 mctech_core-1.0.2/mctech_core/config/config_value.py
+-rw-rw-rw-   0        0        0     1464 2024-04-01 06:27:50.000000 mctech_core-1.0.2/mctech_core/config/yaml_loader.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:22:14.652594 mctech_core-1.0.2/mctech_core/context/
+-rw-rw-rw-   0        0        0      107 2024-04-24 02:37:12.000000 mctech_core-1.0.2/mctech_core/context/__init__.py
+-rw-rw-rw-   0        0        0     2426 2024-04-24 07:30:35.000000 mctech_core-1.0.2/mctech_core/context/async_context.py
+-rw-rw-rw-   0        0        0     1113 2024-04-24 07:41:08.000000 mctech_core-1.0.2/mctech_core/context/header_filter.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:22:14.658593 mctech_core-1.0.2/mctech_core/tracing/
+-rw-rw-rw-   0        0        0      402 2024-04-24 07:53:32.000000 mctech_core-1.0.2/mctech_core/tracing/__init__.py
+-rw-rw-rw-   0        0        0      846 2024-04-24 07:53:19.000000 mctech_core-1.0.2/mctech_core/tracing/tracing_context_middleware.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:22:14.626582 mctech_core-1.0.2/mctech_core.egg-info/
+-rw-rw-rw-   0        0        0      146 2024-04-24 08:22:14.000000 mctech_core-1.0.2/mctech_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      585 2024-04-24 08:22:14.000000 mctech_core-1.0.2/mctech_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 08:22:14.000000 mctech_core-1.0.2/mctech_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-24 08:22:14.000000 mctech_core-1.0.2/mctech_core.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-24 08:22:14.000000 mctech_core-1.0.2/mctech_core.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      258 2024-04-24 03:48:34.000000 mctech_core-1.0.2/mctech_core_setup.py
+-rw-rw-rw-   0        0        0       42 2024-04-24 08:22:14.665592 mctech_core-1.0.2/setup.cfg
```

### Comparing `mctech_core-1.0.1/README.md` & `mctech_core-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mctech_core-1.0.1/mctech_core/config/__init__.py` & `mctech_core-1.0.2/mctech_core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `mctech_core-1.0.1/mctech_core/config/_configure.py` & `mctech_core-1.0.2/mctech_core/config/_configure.py`

 * *Files identical despite different names*

### Comparing `mctech_core-1.0.1/mctech_core/config/config_merger.py` & `mctech_core-1.0.2/mctech_core/config/config_merger.py`

 * *Files identical despite different names*

### Comparing `mctech_core-1.0.1/mctech_core/config/config_value.py` & `mctech_core-1.0.2/mctech_core/config/config_value.py`

 * *Files identical despite different names*

### Comparing `mctech_core-1.0.1/mctech_core/config/yaml_loader.py` & `mctech_core-1.0.2/mctech_core/config/yaml_loader.py`

 * *Files identical despite different names*

