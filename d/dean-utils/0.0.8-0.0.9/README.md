# Comparing `tmp/dean_utils-0.0.8.tar.gz` & `tmp/dean_utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dean_utils-0.0.8.tar", last modified: Wed Dec 20 15:39:29 2023, max compression
+gzip compressed data, was "dean_utils-0.0.9.tar", last modified: Wed Dec 20 16:16:47 2023, max compression
```

## Comparing `dean_utils-0.0.8.tar` & `dean_utils-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:39:29.582464 dean_utils-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-12-20 15:38:59.000000 dean_utils-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      729 2023-12-20 15:39:29.582464 dean_utils-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      287 2023-12-20 15:38:59.000000 dean_utils-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-12-20 15:38:59.000000 dean_utils-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-20 15:39:29.582464 dean_utils-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:39:29.578464 dean_utils-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:39:29.582464 dean_utils-0.0.8/src/dean_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2023-12-20 15:38:59.000000 dean_utils-0.0.8/src/dean_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6641 2023-12-20 15:38:59.000000 dean_utils-0.0.8/src/dean_utils/polars_extras.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:39:29.582464 dean_utils-0.0.8/src/dean_utils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     8726 2023-12-20 15:38:59.000000 dean_utils-0.0.8/src/dean_utils/utils/az_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2023-12-20 15:38:59.000000 dean_utils-0.0.8/src/dean_utils/utils/email_utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 15:39:29.582464 dean_utils-0.0.8/src/dean_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2023-12-20 15:39:29.000000 dean_utils-0.0.8/src/dean_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      351 2023-12-20 15:39:29.000000 dean_utils-0.0.8/src/dean_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 15:39:29.000000 dean_utils-0.0.8/src/dean_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-20 15:39:29.000000 dean_utils-0.0.8/src/dean_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-20 15:39:29.000000 dean_utils-0.0.8/src/dean_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 16:16:47.021188 dean_utils-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-12-20 16:16:17.000000 dean_utils-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2023-12-20 16:16:47.021188 dean_utils-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2023-12-20 16:16:17.000000 dean_utils-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2023-12-20 16:16:17.000000 dean_utils-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-20 16:16:47.021188 dean_utils-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 16:16:47.017188 dean_utils-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 16:16:47.017188 dean_utils-0.0.9/src/dean_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2023-12-20 16:16:17.000000 dean_utils-0.0.9/src/dean_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6641 2023-12-20 16:16:17.000000 dean_utils-0.0.9/src/dean_utils/polars_extras.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 16:16:47.021188 dean_utils-0.0.9/src/dean_utils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     8726 2023-12-20 16:16:17.000000 dean_utils-0.0.9/src/dean_utils/utils/az_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2023-12-20 16:16:17.000000 dean_utils-0.0.9/src/dean_utils/utils/email_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 16:16:47.021188 dean_utils-0.0.9/src/dean_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2023-12-20 16:16:47.000000 dean_utils-0.0.9/src/dean_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2023-12-20 16:16:47.000000 dean_utils-0.0.9/src/dean_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 16:16:47.000000 dean_utils-0.0.9/src/dean_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-20 16:16:47.000000 dean_utils-0.0.9/src/dean_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-20 16:16:47.000000 dean_utils-0.0.9/src/dean_utils.egg-info/top_level.txt
```

### Comparing `dean_utils-0.0.8/LICENSE` & `dean_utils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dean_utils-0.0.8/PKG-INFO` & `dean_utils-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dean_utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: various utils, functions, patches that I like
 Author-email: Dean MacGregor <powertrading121@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: polars
 Requires-Dist: pyarrow
```

### Comparing `dean_utils-0.0.8/src/dean_utils/polars_extras.py` & `dean_utils-0.0.9/src/dean_utils/polars_extras.py`

 * *Files identical despite different names*

### Comparing `dean_utils-0.0.8/src/dean_utils/utils/az_utils.py` & `dean_utils-0.0.9/src/dean_utils/utils/az_utils.py`

 * *Files identical despite different names*

### Comparing `dean_utils-0.0.8/src/dean_utils/utils/email_utility.py` & `dean_utils-0.0.9/src/dean_utils/utils/email_utility.py`

 * *Files identical despite different names*

### Comparing `dean_utils-0.0.8/src/dean_utils.egg-info/PKG-INFO` & `dean_utils-0.0.9/src/dean_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dean-utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: various utils, functions, patches that I like
 Author-email: Dean MacGregor <powertrading121@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: polars
 Requires-Dist: pyarrow
```

