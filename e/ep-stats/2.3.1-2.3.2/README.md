# Comparing `tmp/ep-stats-2.3.1.tar.gz` & `tmp/ep-stats-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ep-stats-2.3.1.tar", last modified: Thu Mar  7 13:57:30 2024, max compression
+gzip compressed data, was "ep-stats-2.3.2.tar", last modified: Wed Apr 24 12:57:27 2024, max compression
```

## Comparing `ep-stats-2.3.1.tar` & `ep-stats-2.3.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:57:30.642066 ep-stats-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-07 13:57:21.000000 ep-stats-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-03-07 13:57:30.642066 ep-stats-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-03-07 13:57:21.000000 ep-stats-2.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-07 13:57:21.000000 ep-stats-2.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-03-07 13:57:30.642066 ep-stats-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-07 13:57:21.000000 ep-stats-2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:57:30.634066 ep-stats-2.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:57:30.638066 ep-stats-2.3.1/src/ep_stats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-03-07 13:57:30.000000 ep-stats-2.3.1/src/ep_stats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-07 13:57:30.000000 ep-stats-2.3.1/src/ep_stats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 13:57:30.000000 ep-stats-2.3.1/src/ep_stats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-07 13:57:30.000000 ep-stats-2.3.1/src/ep_stats.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-07 13:57:30.000000 ep-stats-2.3.1/src/ep_stats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-07 13:57:30.000000 ep-stats-2.3.1/src/ep_stats.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:57:30.638066 ep-stats-2.3.1/src/epstats/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/locust.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:57:30.638066 ep-stats-2.3.1/src/epstats/server/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/server/api_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/server/api_sample_size_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/server/api_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/server/json_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15127 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/server/req.py
--rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/server/res.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:57:30.642066 ep-stats-2.3.1/src/epstats/toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/toolkit/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/toolkit/dao.py
--rw-r--r--   0 runner    (1001) docker     (127)    32779 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/toolkit/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/toolkit/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    14097 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/toolkit/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/toolkit/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    17549 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/toolkit/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:57:30.642066 ep-stats-2.3.1/src/epstats/toolkit/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/toolkit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:57:30.642066 ep-stats-2.3.1/src/epstats/toolkit/testing/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/toolkit/testing/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/toolkit/testing/resources/evaluations_checks.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/toolkit/testing/resources/evaluations_exposures.csv
--rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/toolkit/testing/resources/evaluations_metrics.csv
--rw-r--r--   0 runner    (1001) docker     (127)    14376 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/toolkit/testing/resources/goals_agg.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/toolkit/testing/resources/goals_by_unit.csv
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/toolkit/testing/resources/goals_simple_agg.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/toolkit/testing/test_dao.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/toolkit/testing/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/toolkit/testing/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-03-07 13:57:21.000000 ep-stats-2.3.1/src/epstats/toolkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:27.017111 ep-stats-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 12:57:04.000000 ep-stats-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-24 12:57:27.021111 ep-stats-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-24 12:57:04.000000 ep-stats-2.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-24 12:57:04.000000 ep-stats-2.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-24 12:57:27.021111 ep-stats-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-24 12:57:04.000000 ep-stats-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:27.013111 ep-stats-2.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:27.013111 ep-stats-2.3.2/src/ep_stats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-24 12:57:26.000000 ep-stats-2.3.2/src/ep_stats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-24 12:57:26.000000 ep-stats-2.3.2/src/ep_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:57:26.000000 ep-stats-2.3.2/src/ep_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 12:57:26.000000 ep-stats-2.3.2/src/ep_stats.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-24 12:57:26.000000 ep-stats-2.3.2/src/ep_stats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 12:57:26.000000 ep-stats-2.3.2/src/ep_stats.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:27.017111 ep-stats-2.3.2/src/epstats/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/locust.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:27.017111 ep-stats-2.3.2/src/epstats/server/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/server/api_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/server/api_sample_size_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/server/api_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/server/json_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15127 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/server/req.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/server/res.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:27.017111 ep-stats-2.3.2/src/epstats/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/dao.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32779 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14097 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17549 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:27.017111 ep-stats-2.3.2/src/epstats/toolkit/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:27.017111 ep-stats-2.3.2/src/epstats/toolkit/testing/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/testing/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/testing/resources/evaluations_checks.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/testing/resources/evaluations_exposures.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    15134 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/testing/resources/evaluations_metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    14946 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/testing/resources/goals_agg.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/testing/resources/goals_by_unit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/testing/resources/goals_simple_agg.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/testing/test_dao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/testing/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/testing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-24 12:57:04.000000 ep-stats-2.3.2/src/epstats/toolkit/utils.py
```

### Comparing `ep-stats-2.3.1/LICENSE` & `ep-stats-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.1/PKG-INFO` & `ep-stats-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ep-stats
-Version: 2.3.1
+Version: 2.3.2
 Summary: Statistical package to evaluate ab tests in experimentation platform.
 Home-page: https://github.com/avast/ep-stats
 Author: Ondrej Zahradnik
 Author-email: ondrej.zahradnik@avast.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ep-stats-2.3.1/README.md` & `ep-stats-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.1/setup.cfg` & `ep-stats-2.3.2/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ep-stats
-version = 2.3.1
+version = 2.3.2
 description = Statistical package to evaluate ab tests in experimentation platform.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Ondrej Zahradnik
 author_email = ondrej.zahradnik@avast.com
 url = https://github.com/avast/ep-stats
 classifiers =
```

### Comparing `ep-stats-2.3.1/src/ep_stats.egg-info/PKG-INFO` & `ep-stats-2.3.2/src/ep_stats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ep-stats
-Version: 2.3.1
+Version: 2.3.2
 Summary: Statistical package to evaluate ab tests in experimentation platform.
 Home-page: https://github.com/avast/ep-stats
 Author: Ondrej Zahradnik
 Author-email: ondrej.zahradnik@avast.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ep-stats-2.3.1/src/ep_stats.egg-info/SOURCES.txt` & `ep-stats-2.3.2/src/ep_stats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.1/src/epstats/config.py` & `ep-stats-2.3.2/src/epstats/config.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.1/src/epstats/locust.py` & `ep-stats-2.3.2/src/epstats/locust.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.1/src/epstats/main.py` & `ep-stats-2.3.2/src/epstats/main.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.1/src/epstats/prometheus.py` & `ep-stats-2.3.2/src/epstats/prometheus.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.1/src/epstats/server/api.py` & `ep-stats-2.3.2/src/epstats/server/api.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.1/src/epstats/server/api_evaluate.py` & `ep-stats-2.3.2/src/epstats/server/api_evaluate.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.1/src/epstats/server/api_sample_size_calculation.py` & `ep-stats-2.3.2/src/epstats/server/api_sample_size_calculation.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.1/src/epstats/server/req.py` & `ep-stats-2.3.2/src/epstats/server/req.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.1/src/epstats/server/res.py` & `ep-stats-2.3.2/src/epstats/server/res.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.1/src/epstats/toolkit/check.py` & `ep-stats-2.3.2/src/epstats/toolkit/check.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.1/src/epstats/toolkit/dao.py` & `ep-stats-2.3.2/src/epstats/toolkit/dao.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.1/src/epstats/toolkit/experiment.py` & `ep-stats-2.3.2/src/epstats/toolkit/experiment.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.1/src/epstats/toolkit/metric.py` & `ep-stats-2.3.2/src/epstats/toolkit/metric.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.1/src/epstats/toolkit/parser.py` & `ep-stats-2.3.2/src/epstats/toolkit/parser.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -46,16 +46,16 @@
         tildaop = oneOf("~")
 
         expr = infixNotation(
             operand,
             [
                 (multop, 2, opAssoc.LEFT, MultBinOp),
                 (divop, 2, opAssoc.LEFT, DivBinOp),
-                (plusop, 2, opAssoc.LEFT, PlusBinOp),
                 (subop, 2, opAssoc.LEFT, SubBinOp),
+                (plusop, 2, opAssoc.LEFT, PlusBinOp),
                 (tildaop, 2, opAssoc.LEFT, TildaBinOp),
             ],
         )
 
         self._nominator_expr = expr.parseString(nominator)[0]
         self._denominator_expr = expr.parseString(denominator)[0]
         self._update_dimension_to_value()
```

### Comparing `ep-stats-2.3.1/src/epstats/toolkit/results.py` & `ep-stats-2.3.2/src/epstats/toolkit/results.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.1/src/epstats/toolkit/statistics.py` & `ep-stats-2.3.2/src/epstats/toolkit/statistics.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.1/src/epstats/toolkit/testing/resources/evaluations_checks.csv` & `ep-stats-2.3.2/src/epstats/toolkit/testing/resources/evaluations_checks.csv`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.1/src/epstats/toolkit/testing/resources/evaluations_exposures.csv` & `ep-stats-2.3.2/src/epstats/toolkit/testing/resources/evaluations_exposures.csv`

 * *Files 4% similar despite different names*

```diff
@@ -62,7 +62,9 @@
 test-multi-check	b	test_unit_type	global	exposure	5100
 test-multi-check	c	test_unit_type	global	exposure	5200
 test-conversion-with-minimum-effect	a	test_unit_type	global	exposure	21
 test-conversion-with-minimum-effect	b	test_unit_type	global	exposure	26
 test-conversion-with-minimum-effect	c	test_unit_type	global	exposure	30
 test-dim-operators	a	test_unit_type	global	exposure	1000
 test-dim-operators	b	test_unit_type	global	exposure	1001
+test-operator-precedence	a	test_unit_type	global	exposure	80
+test-operator-precedence	b	test_unit_type	global	exposure	70
```

### Comparing `ep-stats-2.3.1/src/epstats/toolkit/testing/resources/evaluations_metrics.csv` & `ep-stats-2.3.2/src/epstats/toolkit/testing/resources/evaluations_metrics.csv`

 * *Files 3% similar despite different names*

```diff
@@ -70,7 +70,9 @@
 test-conversion-with-minimum-effect	a	1	Click-through Rate	21	5	5	0.2380952381	0.0	0.0	0.4364357805	0.0181405896	0.5656854249	0.0	40.0	1.0	1.0	1.0	0.95	1.0	1.143292891	0.95	N/A	21	N/A	N/A
 test-conversion-with-minimum-effect	b	1	Click-through Rate	26	7	7	0.2692307692	0.0311355311	0.1307692308	0.4523443209	0.0169401173	0.5860084617	0.2231524616	43.540122204	0.8244735669	1.0	0.8244735669	0.9587763217	0.8120572626	1.2332152488	0.95	0.1	26	6624.0	0.020268
 test-conversion-with-minimum-effect	c	1	Click-through Rate	30	9	9	0.3	0.0619047619	0.26	0.4660915997	0.0163116741	0.6178623884	0.4208056759	44.93143953	0.6759453226	1.0	0.6759453226	0.9662027339	0.6302424265	1.3536951139	0.95	0.1	30	6836.0	0.020817
 test-dim-operators	a	1	^button-1, product>1	1000	200	200	0.2	0.0	0.0	0.4002001501	0.0003203203	0.089487474	0.0	1998.0	1.0	1.0	1.0	0.95	N/A	0.17549854	0.95	N/A	1000	N/A	N/A
 test-dim-operators	b	1	^button-1, product>1	1001	220	220	0.2197802198	0.0197802198	0.0989010989	0.4143046604	0.000331637	0.0955096411	1.0355090625	1996.7425963597	0.3005566728	0.3005566728	1.0	0.95	N/A	0.1873090388	0.95	N/A	1001	N/A	N/A
 test-dim-operators	a	2	^button-1, product!=1	1000	300	300	0.3	0.0	0.0	0.4584868703	0.0004204204	0.0683471872	0.0	1998.0	1.0	1.0	1.0	0.95	N/A	0.134039224	0.95	N/A	1000	N/A	N/A
 test-dim-operators	b	2	^button-1, product!=1	1001	400	400	0.3996003996	0.0996003996	0.332001332	0.4900610576	0.0004501301	0.0825214225	4.0232138728	1990.4598431179	5.95556e-05	5.95556e-05	1.0	0.95	N/A	0.1618374485	0.95	N/A	1001	N/A	N/A
+test-operator-precedence	a	1	Clicks	80	57	N/A	0.712500	N/A	0.0	N/A	N/A	N/A	N/A	N/A	1.0	1.0	N/A	N/A	N/A	0.199625	0.95	N/A	80	N/A	N/A
+test-operator-precedence	b	1	Clicks	70	47	N/A	0.671429	N/A	-0.057644	N/A	N/A	N/A	N/A	N/A	0.580573	0.580573	N/A	N/A	N/A	0.205746	0.95	N/A	70	N/A	N/A
```

### Comparing `ep-stats-2.3.1/src/epstats/toolkit/testing/resources/goals_agg.csv` & `ep-stats-2.3.2/src/epstats/toolkit/testing/resources/goals_agg.csv`

 * *Files 2% similar despite different names*

```diff
@@ -179,7 +179,15 @@
 test-conversion-with-minimum-effect		c	test_unit_type	global	exposure			30	30	30	30	30
 test-dim-operators		a	test_unit_type	global	exposure			1000	1000	1000	1000	1000
 test-dim-operators		b	test_unit_type	global	exposure			1001	1001	1001	1001	1001
 test-dim-operators		a	test_unit_type	unit	view	^button-1	>1	200	200	200	200	200
 test-dim-operators		b	test_unit_type	unit	view	^button-1	>1	220	220	220	220	220
 test-dim-operators		a	test_unit_type	unit	view	^button-1	!=1	300	300	300	300	300
 test-dim-operators		b	test_unit_type	unit	view	^button-1	!=1	400	400	400	400	400
+test-operator-precedence		a	test_unit_type	unit	click_1			55	55	55	55	55
+test-operator-precedence		a	test_unit_type	unit	click_2			7	7	7	7	7
+test-operator-precedence		a	test_unit_type	unit	click_3			9	9	9	9	9
+test-operator-precedence		b	test_unit_type	unit	click_1			45	45	45	45	45
+test-operator-precedence		b	test_unit_type	unit	click_2			7	7	7	7	7
+test-operator-precedence		b	test_unit_type	unit	click_3			9	9	9	9	9
+test-operator-precedence		a	test_unit_type	global	exposure			80	80	80	80	80
+test-operator-precedence		b	test_unit_type	global	exposure			70	70	70	70	70
```

### Comparing `ep-stats-2.3.1/src/epstats/toolkit/testing/resources/goals_by_unit.csv` & `ep-stats-2.3.2/src/epstats/toolkit/testing/resources/goals_by_unit.csv`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.1/src/epstats/toolkit/testing/test_dao.py` & `ep-stats-2.3.2/src/epstats/toolkit/testing/test_dao.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.1/src/epstats/toolkit/testing/test_data.py` & `ep-stats-2.3.2/src/epstats/toolkit/testing/test_data.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.1/src/epstats/toolkit/testing/utils.py` & `ep-stats-2.3.2/src/epstats/toolkit/testing/utils.py`

 * *Files identical despite different names*

### Comparing `ep-stats-2.3.1/src/epstats/toolkit/utils.py` & `ep-stats-2.3.2/src/epstats/toolkit/utils.py`

 * *Files identical despite different names*

