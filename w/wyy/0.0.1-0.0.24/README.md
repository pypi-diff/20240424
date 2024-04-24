# Comparing `tmp/wyy-0.0.1.tar.gz` & `tmp/wyy-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wyy-0.0.1.tar", last modified: Wed Apr 24 04:24:05 2024, max compression
+gzip compressed data, was "wyy-0.0.24.tar", last modified: Wed Apr 24 04:23:54 2024, max compression
```

## Comparing `wyy-0.0.1.tar` & `wyy-0.0.24.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 04:24:05.215474 wyy-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1068 2024-04-08 07:07:04.000000 wyy-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      305 2024-04-24 04:24:05.215474 wyy-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      445 2024-04-24 04:24:01.000000 wyy-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 04:24:05.215474 wyy-0.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 04:24:05.215474 wyy-0.0.1/wyy/
--rw-r--r--   0 root         (0) root         (0)       59 2024-04-24 04:16:33.000000 wyy-0.0.1/wyy/__init__.py
--rw-r--r--   0 root         (0) root         (0)      886 2024-04-19 14:00:41.000000 wyy-0.0.1/wyy/info.py
--rw-r--r--   0 root         (0) root         (0)      424 2024-04-24 04:16:30.000000 wyy-0.0.1/wyy/json.py
--rw-r--r--   0 root         (0) root         (0)     3549 2024-04-24 04:23:51.000000 wyy-0.0.1/wyy/path.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 04:24:05.215474 wyy-0.0.1/wyy.egg-info/
--rw-r--r--   0 root         (0) root         (0)      305 2024-04-24 04:24:05.000000 wyy-0.0.1/wyy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2024-04-24 04:24:05.000000 wyy-0.0.1/wyy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 04:24:05.000000 wyy-0.0.1/wyy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2024-04-24 04:24:05.000000 wyy-0.0.1/wyy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 04:23:54.698862 wyy-0.0.24/
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-04-08 07:07:04.000000 wyy-0.0.24/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      306 2024-04-24 04:23:54.698862 wyy-0.0.24/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      446 2024-04-24 04:23:40.000000 wyy-0.0.24/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 04:23:54.698862 wyy-0.0.24/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 04:23:54.698862 wyy-0.0.24/wyy/
+-rw-r--r--   0 root         (0) root         (0)       59 2024-04-24 04:16:33.000000 wyy-0.0.24/wyy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      886 2024-04-19 14:00:41.000000 wyy-0.0.24/wyy/info.py
+-rw-r--r--   0 root         (0) root         (0)      424 2024-04-24 04:16:30.000000 wyy-0.0.24/wyy/json.py
+-rw-r--r--   0 root         (0) root         (0)     3549 2024-04-24 04:23:51.000000 wyy-0.0.24/wyy/path.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 04:23:54.698862 wyy-0.0.24/wyy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      306 2024-04-24 04:23:54.000000 wyy-0.0.24/wyy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2024-04-24 04:23:54.000000 wyy-0.0.24/wyy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 04:23:54.000000 wyy-0.0.24/wyy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-04-24 04:23:54.000000 wyy-0.0.24/wyy.egg-info/top_level.txt
```

### Comparing `wyy-0.0.1/LICENSE` & `wyy-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `wyy-0.0.1/wyy/info.py` & `wyy-0.0.24/wyy/info.py`

 * *Files identical despite different names*

### Comparing `wyy-0.0.1/wyy/path.py` & `wyy-0.0.24/wyy/path.py`

 * *Files identical despite different names*

