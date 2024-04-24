# Comparing `tmp/RiskLabAI-0.0.8.tar.gz` & `tmp/RiskLabAI-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RiskLabAI-0.0.8.tar", last modified: Wed May 17 15:40:07 2023, max compression
+gzip compressed data, was "RiskLabAI-0.0.9.tar", last modified: Mon Jul 31 10:59:47 2023, max compression
```

## Comparing `RiskLabAI-0.0.8.tar` & `RiskLabAI-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:40:07.272093 RiskLabAI-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-17 15:39:51.000000 RiskLabAI-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-17 15:40:07.272093 RiskLabAI-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-17 15:39:51.000000 RiskLabAI-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-17 15:39:51.000000 RiskLabAI-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-17 15:40:07.272093 RiskLabAI-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:40:07.268093 RiskLabAI-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:40:07.268093 RiskLabAI-0.0.8/src/RiskLabAI/
--rw-r--r--   0 runner    (1001) docker     (123)    12252 2023-05-17 15:39:51.000000 RiskLabAI-0.0.8/src/RiskLabAI/DataStructures.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-17 15:39:51.000000 RiskLabAI-0.0.8/src/RiskLabAI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:40:07.272093 RiskLabAI-0.0.8/src/RiskLabAI/data/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-17 15:39:51.000000 RiskLabAI-0.0.8/src/RiskLabAI/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:40:07.272093 RiskLabAI-0.0.8/src/RiskLabAI/data/structures/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-17 15:39:51.000000 RiskLabAI-0.0.8/src/RiskLabAI/data/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-17 15:39:51.000000 RiskLabAI-0.0.8/src/RiskLabAI/data/structures/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-17 15:39:51.000000 RiskLabAI-0.0.8/src/RiskLabAI/data/structures/hedging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-17 15:39:51.000000 RiskLabAI-0.0.8/src/RiskLabAI/data/structures/infomation_driven_bars.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-17 15:39:51.000000 RiskLabAI-0.0.8/src/RiskLabAI/data/structures/standard_bars.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-17 15:39:51.000000 RiskLabAI-0.0.8/src/RiskLabAI/data/structures/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:40:07.272093 RiskLabAI-0.0.8/src/RiskLabAI/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-17 15:39:51.000000 RiskLabAI-0.0.8/src/RiskLabAI/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-17 15:39:51.000000 RiskLabAI-0.0.8/src/RiskLabAI/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-17 15:39:51.000000 RiskLabAI-0.0.8/src/RiskLabAI/utils/smoothing_average.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:40:07.268093 RiskLabAI-0.0.8/src/RiskLabAI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-17 15:40:07.000000 RiskLabAI-0.0.8/src/RiskLabAI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-17 15:40:07.000000 RiskLabAI-0.0.8/src/RiskLabAI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:40:07.000000 RiskLabAI-0.0.8/src/RiskLabAI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-17 15:40:07.000000 RiskLabAI-0.0.8/src/RiskLabAI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 15:40:07.000000 RiskLabAI-0.0.8/src/RiskLabAI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:59:47.919233 RiskLabAI-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-31 10:59:47.919233 RiskLabAI-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:59:47.919233 RiskLabAI-0.0.9/RiskLabAI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:59:47.919233 RiskLabAI-0.0.9/RiskLabAI/RiskLabAI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-31 10:59:47.000000 RiskLabAI-0.0.9/RiskLabAI/RiskLabAI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-31 10:59:47.000000 RiskLabAI-0.0.9/RiskLabAI/RiskLabAI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 10:59:47.000000 RiskLabAI-0.0.9/RiskLabAI/RiskLabAI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-31 10:59:47.000000 RiskLabAI-0.0.9/RiskLabAI/RiskLabAI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-31 10:59:47.000000 RiskLabAI-0.0.9/RiskLabAI/RiskLabAI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:59:47.919233 RiskLabAI-0.0.9/RiskLabAI/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/RiskLabAI/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:59:47.919233 RiskLabAI-0.0.9/RiskLabAI/data/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/RiskLabAI/data/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/RiskLabAI/data/structures/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/RiskLabAI/data/structures/hedging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/RiskLabAI/data/structures/infomation_driven_bars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/RiskLabAI/data/structures/standard_bars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/RiskLabAI/data/structures/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:59:47.919233 RiskLabAI-0.0.9/RiskLabAI/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/RiskLabAI/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/RiskLabAI/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/RiskLabAI/utils/smoothing_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-31 10:59:33.000000 RiskLabAI-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-31 10:59:47.919233 RiskLabAI-0.0.9/setup.cfg
```

### Comparing `RiskLabAI-0.0.8/LICENSE` & `RiskLabAI-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `RiskLabAI-0.0.8/PKG-INFO` & `RiskLabAI-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RiskLabAI
-Version: 0.0.8
+Version: 0.0.9
 Summary: Financial AI using Python.
 Home-page: https://github.com/RiskLabAI/RiskLabAI.py
 Author: RiskLab
 Author-email: research@risklab.ai
 Project-URL: Bug Tracker, https://github.com/RiskLabAI/RiskLabAI.py/issues
 Project-URL: Changelog, https://github.com/RiskLabAI/RiskLabAI.py/releases
 Classifier: Programming Language :: Python :: 3
```

### Comparing `RiskLabAI-0.0.8/src/RiskLabAI/data/structures/filtering.py` & `RiskLabAI-0.0.9/RiskLabAI/data/structures/filtering.py`

 * *Files identical despite different names*

### Comparing `RiskLabAI-0.0.8/src/RiskLabAI/data/structures/hedging.py` & `RiskLabAI-0.0.9/RiskLabAI/data/structures/hedging.py`

 * *Files identical despite different names*

### Comparing `RiskLabAI-0.0.8/src/RiskLabAI/data/structures/infomation_driven_bars.py` & `RiskLabAI-0.0.9/RiskLabAI/data/structures/infomation_driven_bars.py`

 * *Files identical despite different names*

### Comparing `RiskLabAI-0.0.8/src/RiskLabAI/data/structures/standard_bars.py` & `RiskLabAI-0.0.9/RiskLabAI/data/structures/standard_bars.py`

 * *Files identical despite different names*

### Comparing `RiskLabAI-0.0.8/src/RiskLabAI/data/structures/utilities.py` & `RiskLabAI-0.0.9/RiskLabAI/data/structures/utilities.py`

 * *Files identical despite different names*

### Comparing `RiskLabAI-0.0.8/src/RiskLabAI/utils/progress.py` & `RiskLabAI-0.0.9/RiskLabAI/utils/progress.py`

 * *Files identical despite different names*

### Comparing `RiskLabAI-0.0.8/src/RiskLabAI/utils/smoothing_average.py` & `RiskLabAI-0.0.9/RiskLabAI/utils/smoothing_average.py`

 * *Files identical despite different names*

### Comparing `RiskLabAI-0.0.8/src/RiskLabAI.egg-info/PKG-INFO` & `RiskLabAI-0.0.9/RiskLabAI/RiskLabAI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RiskLabAI
-Version: 0.0.8
+Version: 0.0.9
 Summary: Financial AI using Python.
 Home-page: https://github.com/RiskLabAI/RiskLabAI.py
 Author: RiskLab
 Author-email: research@risklab.ai
 Project-URL: Bug Tracker, https://github.com/RiskLabAI/RiskLabAI.py/issues
 Project-URL: Changelog, https://github.com/RiskLabAI/RiskLabAI.py/releases
 Classifier: Programming Language :: Python :: 3
```

