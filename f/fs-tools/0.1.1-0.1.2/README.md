# Comparing `tmp/fs_tools-0.1.1.tar.gz` & `tmp/fs_tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fs_tools-0.1.1.tar", last modified: Wed Apr 24 14:46:10 2024, max compression
+gzip compressed data, was "fs_tools-0.1.2.tar", last modified: Wed Apr 24 14:46:28 2024, max compression
```

## Comparing `fs_tools-0.1.1.tar` & `fs_tools-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 14:46:10.093954 fs_tools-0.1.1/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      355 2024-04-24 14:46:10.093954 fs_tools-0.1.1/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-04-24 13:03:55.000000 fs_tools-0.1.1/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      538 2024-04-24 14:46:07.000000 fs_tools-0.1.1/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-24 14:46:10.093954 fs_tools-0.1.1/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 14:46:10.093954 fs_tools-0.1.1/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 14:46:10.093954 fs_tools-0.1.1/src/fs_tools/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       62 2024-04-24 14:21:32.000000 fs_tools-0.1.1/src/fs_tools/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      290 2024-04-24 14:46:03.000000 fs_tools-0.1.1/src/fs_tools/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      928 2024-04-24 14:45:51.000000 fs_tools-0.1.1/src/fs_tools/compression.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1973 2024-04-24 14:19:34.000000 fs_tools-0.1.1/src/fs_tools/io.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      783 2024-04-24 14:21:15.000000 fs_tools-0.1.1/src/fs_tools/moving.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      597 2024-04-24 14:14:26.000000 fs_tools-0.1.1/src/fs_tools/paths.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 14:46:10.093954 fs_tools-0.1.1/src/fs_tools.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      355 2024-04-24 14:46:10.000000 fs_tools-0.1.1/src/fs_tools.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      346 2024-04-24 14:46:10.000000 fs_tools-0.1.1/src/fs_tools.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-24 14:46:10.000000 fs_tools-0.1.1/src/fs_tools.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-24 14:46:10.000000 fs_tools-0.1.1/src/fs_tools.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-04-24 14:46:10.000000 fs_tools-0.1.1/src/fs_tools.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 14:46:28.073953 fs_tools-0.1.2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      355 2024-04-24 14:46:28.073953 fs_tools-0.1.2/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-04-24 13:03:55.000000 fs_tools-0.1.2/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      538 2024-04-24 14:46:25.000000 fs_tools-0.1.2/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-24 14:46:28.073953 fs_tools-0.1.2/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 14:46:28.073953 fs_tools-0.1.2/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 14:46:28.073953 fs_tools-0.1.2/src/fs/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       62 2024-04-24 14:21:32.000000 fs_tools-0.1.2/src/fs/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      290 2024-04-24 14:46:03.000000 fs_tools-0.1.2/src/fs/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      928 2024-04-24 14:45:51.000000 fs_tools-0.1.2/src/fs/compression.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1973 2024-04-24 14:19:34.000000 fs_tools-0.1.2/src/fs/io.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      783 2024-04-24 14:21:15.000000 fs_tools-0.1.2/src/fs/moving.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      597 2024-04-24 14:14:26.000000 fs_tools-0.1.2/src/fs/paths.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-24 14:46:28.073953 fs_tools-0.1.2/src/fs_tools.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      355 2024-04-24 14:46:28.000000 fs_tools-0.1.2/src/fs_tools.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      310 2024-04-24 14:46:28.000000 fs_tools-0.1.2/src/fs_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-24 14:46:28.000000 fs_tools-0.1.2/src/fs_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-24 14:46:28.000000 fs_tools-0.1.2/src/fs_tools.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-24 14:46:28.000000 fs_tools-0.1.2/src/fs_tools.egg-info/top_level.txt
```

### Comparing `fs_tools-0.1.1/pyproject.toml` & `fs_tools-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fs-tools"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Simple, exception-free filesystem tools"
 dependencies = [
   "haskellian"
 ]
```

### Comparing `fs_tools-0.1.1/src/fs_tools/compression.py` & `fs_tools-0.1.2/src/fs/compression.py`

 * *Files identical despite different names*

### Comparing `fs_tools-0.1.1/src/fs_tools/io.py` & `fs_tools-0.1.2/src/fs/io.py`

 * *Files identical despite different names*

### Comparing `fs_tools-0.1.1/src/fs_tools/moving.py` & `fs_tools-0.1.2/src/fs/moving.py`

 * *Files identical despite different names*

### Comparing `fs_tools-0.1.1/src/fs_tools/paths.py` & `fs_tools-0.1.2/src/fs/paths.py`

 * *Files identical despite different names*

