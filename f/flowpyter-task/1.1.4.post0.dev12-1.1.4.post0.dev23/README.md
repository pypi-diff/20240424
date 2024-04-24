# Comparing `tmp/flowpyter-task-1.1.4.post0.dev12.tar.gz` & `tmp/flowpyter-task-1.1.4.post0.dev23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowpyter-task-1.1.4.post0.dev12.tar", last modified: Tue Apr 16 12:42:24 2024, max compression
+gzip compressed data, was "flowpyter-task-1.1.4.post0.dev23.tar", last modified: Wed Apr 24 16:38:05 2024, max compression
```

## Comparing `flowpyter-task-1.1.4.post0.dev12.tar` & `flowpyter-task-1.1.4.post0.dev23.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-16 12:42:24.099397 flowpyter-task-1.1.4.post0.dev12/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2024-04-16 12:37:59.000000 flowpyter-task-1.1.4.post0.dev12/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1691 2024-04-16 12:42:24.099397 flowpyter-task-1.1.4.post0.dev12/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2024-04-16 12:37:59.000000 flowpyter-task-1.1.4.post0.dev12/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-04-16 12:37:59.000000 flowpyter-task-1.1.4.post0.dev12/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      153 2024-04-16 12:42:24.099397 flowpyter-task-1.1.4.post0.dev12/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2306 2024-04-16 12:37:59.000000 flowpyter-task-1.1.4.post0.dev12/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-16 12:42:24.095397 flowpyter-task-1.1.4.post0.dev12/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-16 12:42:24.099397 flowpyter-task-1.1.4.post0.dev12/src/flowpyter_task.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1691 2024-04-16 12:42:24.000000 flowpyter-task-1.1.4.post0.dev12/src/flowpyter_task.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      590 2024-04-16 12:42:24.000000 flowpyter-task-1.1.4.post0.dev12/src/flowpyter_task.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-16 12:42:24.000000 flowpyter-task-1.1.4.post0.dev12/src/flowpyter_task.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2024-04-16 12:42:24.000000 flowpyter-task-1.1.4.post0.dev12/src/flowpyter_task.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2024-04-16 12:42:24.000000 flowpyter-task-1.1.4.post0.dev12/src/flowpyter_task.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-04-16 12:42:24.000000 flowpyter-task-1.1.4.post0.dev12/src/flowpyter_task.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-16 12:42:24.000000 flowpyter-task-1.1.4.post0.dev12/src/flowpyter_task.egg-info/zip-safe
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-16 12:42:24.095397 flowpyter-task-1.1.4.post0.dev12/src/flowpytertask/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      416 2024-04-16 12:37:59.000000 flowpyter-task-1.1.4.post0.dev12/src/flowpytertask/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      508 2024-04-16 12:42:24.099397 flowpyter-task-1.1.4.post0.dev12/src/flowpytertask/_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17940 2024-04-16 12:37:59.000000 flowpyter-task-1.1.4.post0.dev12/src/flowpytertask/flowpytertask.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-16 12:42:24.099397 flowpyter-task-1.1.4.post0.dev12/src/flowpytertask/plugins/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      242 2024-04-16 12:37:59.000000 flowpyter-task-1.1.4.post0.dev12/src/flowpytertask/plugins/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      237 2024-04-16 12:37:59.000000 flowpyter-task-1.1.4.post0.dev12/src/flowpytertask/plugins/base64_jinja.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-16 12:42:24.099397 flowpyter-task-1.1.4.post0.dev12/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16165 2024-04-16 12:37:59.000000 flowpyter-task-1.1.4.post0.dev12/tests/test_flowpyter_operator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7708 2024-04-16 12:37:59.000000 flowpyter-task-1.1.4.post0.dev12/tests/test_integration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    86677 2024-04-16 12:37:59.000000 flowpyter-task-1.1.4.post0.dev12/versioneer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 16:38:05.475788 flowpyter-task-1.1.4.post0.dev23/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2024-04-24 16:38:05.000000 flowpyter-task-1.1.4.post0.dev23/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1691 2024-04-24 16:38:05.475788 flowpyter-task-1.1.4.post0.dev23/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2024-04-24 16:38:05.000000 flowpyter-task-1.1.4.post0.dev23/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-04-24 16:38:05.000000 flowpyter-task-1.1.4.post0.dev23/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      181 2024-04-24 16:38:05.475788 flowpyter-task-1.1.4.post0.dev23/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2306 2024-04-24 16:38:05.000000 flowpyter-task-1.1.4.post0.dev23/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 16:38:05.471788 flowpyter-task-1.1.4.post0.dev23/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 16:38:05.475788 flowpyter-task-1.1.4.post0.dev23/src/flowpyter_task.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1691 2024-04-24 16:38:05.000000 flowpyter-task-1.1.4.post0.dev23/src/flowpyter_task.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      590 2024-04-24 16:38:05.000000 flowpyter-task-1.1.4.post0.dev23/src/flowpyter_task.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 16:38:05.000000 flowpyter-task-1.1.4.post0.dev23/src/flowpyter_task.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2024-04-24 16:38:05.000000 flowpyter-task-1.1.4.post0.dev23/src/flowpyter_task.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2024-04-24 16:38:05.000000 flowpyter-task-1.1.4.post0.dev23/src/flowpyter_task.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-04-24 16:38:05.000000 flowpyter-task-1.1.4.post0.dev23/src/flowpyter_task.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 16:38:05.000000 flowpyter-task-1.1.4.post0.dev23/src/flowpyter_task.egg-info/zip-safe
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 16:38:05.475788 flowpyter-task-1.1.4.post0.dev23/src/flowpytertask/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      416 2024-04-24 16:38:05.000000 flowpyter-task-1.1.4.post0.dev23/src/flowpytertask/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      508 2024-04-24 16:38:05.479788 flowpyter-task-1.1.4.post0.dev23/src/flowpytertask/_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17940 2024-04-24 16:38:05.000000 flowpyter-task-1.1.4.post0.dev23/src/flowpytertask/flowpytertask.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 16:38:05.475788 flowpyter-task-1.1.4.post0.dev23/src/flowpytertask/plugins/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      242 2024-04-24 16:38:05.000000 flowpyter-task-1.1.4.post0.dev23/src/flowpytertask/plugins/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      237 2024-04-24 16:38:05.000000 flowpyter-task-1.1.4.post0.dev23/src/flowpytertask/plugins/base64_jinja.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 16:38:05.475788 flowpyter-task-1.1.4.post0.dev23/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16165 2024-04-24 16:38:05.000000 flowpyter-task-1.1.4.post0.dev23/tests/test_flowpyter_operator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7708 2024-04-24 16:38:05.000000 flowpyter-task-1.1.4.post0.dev23/tests/test_integration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    86677 2024-04-24 16:38:05.000000 flowpyter-task-1.1.4.post0.dev23/versioneer.py
```

### Comparing `flowpyter-task-1.1.4.post0.dev12/LICENSE` & `flowpyter-task-1.1.4.post0.dev23/LICENSE`

 * *Files identical despite different names*

### Comparing `flowpyter-task-1.1.4.post0.dev12/PKG-INFO` & `flowpyter-task-1.1.4.post0.dev23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowpyter-task
-Version: 1.1.4.post0.dev12
+Version: 1.1.4.post0.dev23
 Home-page: https://github.com/Flowminder/flowpyter-task
 Author: Flowminder Foundation
 Author-email: flowkit@flowminder.org
 Keywords: mobile telecommunications analysis
 Platform: MacOS X
 Platform: Linux
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `flowpyter-task-1.1.4.post0.dev12/README.md` & `flowpyter-task-1.1.4.post0.dev23/README.md`

 * *Files identical despite different names*

### Comparing `flowpyter-task-1.1.4.post0.dev12/setup.py` & `flowpyter-task-1.1.4.post0.dev23/setup.py`

 * *Files identical despite different names*

### Comparing `flowpyter-task-1.1.4.post0.dev12/src/flowpyter_task.egg-info/PKG-INFO` & `flowpyter-task-1.1.4.post0.dev23/src/flowpyter_task.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowpyter-task
-Version: 1.1.4.post0.dev12
+Version: 1.1.4.post0.dev23
 Home-page: https://github.com/Flowminder/flowpyter-task
 Author: Flowminder Foundation
 Author-email: flowkit@flowminder.org
 Keywords: mobile telecommunications analysis
 Platform: MacOS X
 Platform: Linux
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `flowpyter-task-1.1.4.post0.dev12/src/flowpyter_task.egg-info/SOURCES.txt` & `flowpyter-task-1.1.4.post0.dev23/src/flowpyter_task.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flowpyter-task-1.1.4.post0.dev12/src/flowpytertask/flowpytertask.py` & `flowpyter-task-1.1.4.post0.dev23/src/flowpytertask/flowpytertask.py`

 * *Files identical despite different names*

### Comparing `flowpyter-task-1.1.4.post0.dev12/tests/test_flowpyter_operator.py` & `flowpyter-task-1.1.4.post0.dev23/tests/test_flowpyter_operator.py`

 * *Files identical despite different names*

### Comparing `flowpyter-task-1.1.4.post0.dev12/tests/test_integration.py` & `flowpyter-task-1.1.4.post0.dev23/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `flowpyter-task-1.1.4.post0.dev12/versioneer.py` & `flowpyter-task-1.1.4.post0.dev23/versioneer.py`

 * *Files identical despite different names*

