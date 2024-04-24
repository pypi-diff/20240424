# Comparing `tmp/donetools-0.0.8.tar.gz` & `tmp/donetools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donetools-0.0.8.tar", last modified: Fri Apr 12 01:37:46 2024, max compression
+gzip compressed data, was "donetools-0.0.9.tar", last modified: Wed Apr 17 02:37:12 2024, max compression
```

## Comparing `donetools-0.0.8.tar` & `donetools-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 01:37:46.909027 donetools-0.0.8/
--rw-r--r--   0 root         (0) root         (0)     1068 2024-04-08 07:07:04.000000 donetools-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      311 2024-04-12 01:37:46.909027 donetools-0.0.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 01:37:46.909027 donetools-0.0.8/donetools/
--rw-r--r--   0 root         (0) root         (0)       54 2024-04-11 08:58:54.000000 donetools-0.0.8/donetools/__init__.py
--rw-r--r--   0 root         (0) root         (0)      684 2024-04-10 15:11:13.000000 donetools-0.0.8/donetools/info.py
--rw-r--r--   0 root         (0) root         (0)     2374 2024-04-12 01:37:20.000000 donetools-0.0.8/donetools/path.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 01:37:46.909027 donetools-0.0.8/donetools.egg-info/
--rw-r--r--   0 root         (0) root         (0)      311 2024-04-12 01:37:46.000000 donetools-0.0.8/donetools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      212 2024-04-12 01:37:46.000000 donetools-0.0.8/donetools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 01:37:46.000000 donetools-0.0.8/donetools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-12 01:37:46.000000 donetools-0.0.8/donetools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      457 2024-04-12 01:37:32.000000 donetools-0.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 01:37:46.909027 donetools-0.0.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 02:37:12.539460 donetools-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-04-08 07:07:04.000000 donetools-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      311 2024-04-17 02:37:12.539460 donetools-0.0.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 02:37:12.539460 donetools-0.0.9/donetools/
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-17 02:37:00.000000 donetools-0.0.9/donetools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      684 2024-04-10 15:11:13.000000 donetools-0.0.9/donetools/info.py
+-rw-r--r--   0 root         (0) root         (0)      351 2024-04-17 02:36:51.000000 donetools-0.0.9/donetools/json.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-04-17 02:31:27.000000 donetools-0.0.9/donetools/path.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 02:37:12.539460 donetools-0.0.9/donetools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      311 2024-04-17 02:37:12.000000 donetools-0.0.9/donetools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      230 2024-04-17 02:37:12.000000 donetools-0.0.9/donetools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 02:37:12.000000 donetools-0.0.9/donetools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-17 02:37:12.000000 donetools-0.0.9/donetools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      457 2024-04-17 02:36:58.000000 donetools-0.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 02:37:12.539460 donetools-0.0.9/setup.cfg
```

### Comparing `donetools-0.0.8/LICENSE` & `donetools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `donetools-0.0.8/donetools/info.py` & `donetools-0.0.9/donetools/info.py`

 * *Files identical despite different names*

### Comparing `donetools-0.0.8/donetools/path.py` & `donetools-0.0.9/donetools/path.py`

 * *Files identical despite different names*

