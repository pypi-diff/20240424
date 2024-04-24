# Comparing `tmp/stabilizer_timelime-0.2.0.tar.gz` & `tmp/stabilizer_timelime-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stabilizer_timelime-0.2.0.tar", max compression
+gzip compressed data, was "stabilizer_timelime-0.2.1.tar", max compression
```

## Comparing `stabilizer_timelime-0.2.0.tar` & `stabilizer_timelime-0.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1492 2024-04-16 18:48:45.808071 stabilizer_timelime-0.2.0/LICENSE
--rw-r--r--   0        0        0      776 2024-04-16 20:19:56.407964 stabilizer_timelime-0.2.0/README.md
--rw-r--r--   0        0        0      774 2024-04-23 16:23:01.427188 stabilizer_timelime-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-15 00:03:23.296661 stabilizer_timelime-0.2.0/stabilizer_timelime/src/__init__.py
--rw-r--r--   0        0        0       24 2024-04-15 19:42:45.228609 stabilizer_timelime-0.2.0/stabilizer_timelime/src/dataslurper/__init__.py
--rw-r--r--   0        0        0     4801 2024-04-19 18:20:35.183976 stabilizer_timelime-0.2.0/stabilizer_timelime/src/dataslurper/prudenceChecker.py
--rw-r--r--   0        0        0     8171 2024-04-19 18:20:58.398569 stabilizer_timelime-0.2.0/stabilizer_timelime/src/dataslurper/slurpdata.py
--rw-r--r--   0        0        0      517 2024-04-21 16:22:21.965311 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/__init__.py
--rw-r--r--   0        0        0     1003 2024-04-15 19:46:28.151618 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/config.py
--rw-r--r--   0        0        0     6148 2024-04-21 14:52:45.759246 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/.DS_Store
--rwxr-xr-x   0        0        0    10689 2024-04-14 16:32:20.312051 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/CFS.py
--rwxr-xr-x   0        0        0    11922 2024-04-14 16:32:21.643298 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/CFS_regression.py
--rw-r--r--   0        0        0     7270 2024-04-15 19:28:57.554189 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/DE.py
--rw-r--r--   0        0        0     9862 2024-04-15 19:29:45.282751 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/Find_bellwethers.py
--rw-r--r--   0        0        0    10716 2024-04-15 23:28:50.247476 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/Performance_Calculator.py
--rw-r--r--   0        0        0     2531 2024-04-15 19:35:14.983457 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/Stats_files.py
--rw-r--r--   0        0        0        0 2024-04-14 16:32:19.433820 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/__init__.py
--rw-r--r--   0        0        0     3128 2024-04-15 20:03:02.460402 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/attribute_selector.py
--rwxr-xr-x   0        0        0     8784 2024-04-15 22:32:53.920281 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/birch.py
--rw-r--r--   0        0        0    11445 2024-04-15 22:40:20.361407 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/birch_bellwether_p_CFS.py
--rw-r--r--   0        0        0     4221 2024-04-15 19:28:50.926587 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/collect_bellwethers.py
--rw-r--r--   0        0        0     9306 2024-04-15 23:03:18.017939 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/default_bellwether.py
--rw-r--r--   0        0        0     2408 2024-04-23 16:19:09.557286 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/generate_results.py
--rw-r--r--   0        0        0     4149 2024-04-19 19:52:55.063561 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/init_datafiles.py
--rw-r--r--   0        0        0     8124 2024-04-15 19:30:24.992210 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/learners.py
--rw-r--r--   0        0        0     5317 2024-04-15 19:34:25.519136 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/optimizer.py
--rw-r--r--   0        0        0    13670 2024-04-15 19:39:18.188946 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/predictor_advance_v1.py
--rw-r--r--   0        0        0     5568 2024-04-15 19:32:22.898327 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/predictor_baseline.py
--rw-r--r--   0        0        0     9951 2024-04-23 16:20:41.196495 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/scott_knott.py
--rw-r--r--   0        0        0     7377 2024-04-15 21:47:14.987970 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/utils.py
--rw-r--r--   0        0        0        0 2024-04-23 16:22:21.372525 stabilizer_timelime-0.2.0/stabilizer_timelime/src/timeLIME/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 16:22:21.372785 stabilizer_timelime-0.2.0/stabilizer_timelime/src/timeLIME/src/__init__.py
--rw-r--r--   0        0        0    11030 2024-04-23 16:22:21.373200 stabilizer_timelime-0.2.0/stabilizer_timelime/src/timeLIME/src/othertools.py
--rw-r--r--   0        0        0    10035 2024-04-23 16:22:21.373488 stabilizer_timelime-0.2.0/stabilizer_timelime/src/timeLIME/src/planner.py
--rw-r--r--   0        0        0     2012 2024-04-23 16:22:21.373671 stabilizer_timelime-0.2.0/stabilizer_timelime/src/timeLIME/src/runexp.py
--rw-r--r--   0        0        0     1891 2024-04-23 16:22:21.373856 stabilizer_timelime-0.2.0/stabilizer_timelime/src/timeLIME/src/split_dataset.py
--rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 stabilizer_timelime-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1492 2024-04-16 18:48:45.808071 stabilizer_timelime-0.2.1/LICENSE
+-rw-r--r--   0        0        0      776 2024-04-16 20:19:56.407964 stabilizer_timelime-0.2.1/README.md
+-rw-r--r--   0        0        0      774 2024-04-24 17:57:51.396946 stabilizer_timelime-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 00:03:23.296661 stabilizer_timelime-0.2.1/stabilizer_timelime/src/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-15 19:42:45.228609 stabilizer_timelime-0.2.1/stabilizer_timelime/src/dataslurper/__init__.py
+-rw-r--r--   0        0        0     4801 2024-04-19 18:20:35.183976 stabilizer_timelime-0.2.1/stabilizer_timelime/src/dataslurper/prudenceChecker.py
+-rw-r--r--   0        0        0     8171 2024-04-19 18:20:58.398569 stabilizer_timelime-0.2.1/stabilizer_timelime/src/dataslurper/slurpdata.py
+-rw-r--r--   0        0        0      517 2024-04-21 16:22:21.965311 stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/__init__.py
+-rw-r--r--   0        0        0     1003 2024-04-15 19:46:28.151618 stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/config.py
+-rw-r--r--   0        0        0     6148 2024-04-21 14:52:45.759246 stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/.DS_Store
+-rwxr-xr-x   0        0        0    10689 2024-04-14 16:32:20.312051 stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/CFS.py
+-rwxr-xr-x   0        0        0    11922 2024-04-14 16:32:21.643298 stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/CFS_regression.py
+-rw-r--r--   0        0        0     7270 2024-04-15 19:28:57.554189 stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/DE.py
+-rw-r--r--   0        0        0     9862 2024-04-15 19:29:45.282751 stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/Find_bellwethers.py
+-rw-r--r--   0        0        0    10716 2024-04-15 23:28:50.247476 stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/Performance_Calculator.py
+-rw-r--r--   0        0        0     2531 2024-04-15 19:35:14.983457 stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/Stats_files.py
+-rw-r--r--   0        0        0        0 2024-04-14 16:32:19.433820 stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/__init__.py
+-rw-r--r--   0        0        0     3128 2024-04-15 20:03:02.460402 stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/attribute_selector.py
+-rwxr-xr-x   0        0        0     8784 2024-04-15 22:32:53.920281 stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/birch.py
+-rw-r--r--   0        0        0    11445 2024-04-15 22:40:20.361407 stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/birch_bellwether_p_CFS.py
+-rw-r--r--   0        0        0     4164 2024-04-24 16:59:27.303734 stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/collect_bellwethers.py
+-rw-r--r--   0        0        0     9306 2024-04-15 23:03:18.017939 stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/default_bellwether.py
+-rw-r--r--   0        0        0     2408 2024-04-23 16:19:09.557286 stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/generate_results.py
+-rw-r--r--   0        0        0     4081 2024-04-24 16:43:56.220533 stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/init_datafiles.py
+-rw-r--r--   0        0        0     8124 2024-04-15 19:30:24.992210 stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/learners.py
+-rw-r--r--   0        0        0     5317 2024-04-15 19:34:25.519136 stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/optimizer.py
+-rw-r--r--   0        0        0    13670 2024-04-15 19:39:18.188946 stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/predictor_advance_v1.py
+-rw-r--r--   0        0        0     5568 2024-04-15 19:32:22.898327 stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/predictor_baseline.py
+-rw-r--r--   0        0        0     9951 2024-04-23 16:20:41.196495 stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/scott_knott.py
+-rw-r--r--   0        0        0     7377 2024-04-15 21:47:14.987970 stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/utils.py
+-rw-r--r--   0        0        0        0 2024-04-23 16:22:21.372525 stabilizer_timelime-0.2.1/stabilizer_timelime/src/timeLIME/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 16:22:21.372785 stabilizer_timelime-0.2.1/stabilizer_timelime/src/timeLIME/src/__init__.py
+-rw-r--r--   0        0        0    11030 2024-04-23 16:22:21.373200 stabilizer_timelime-0.2.1/stabilizer_timelime/src/timeLIME/src/othertools.py
+-rw-r--r--   0        0        0    10035 2024-04-23 16:22:21.373488 stabilizer_timelime-0.2.1/stabilizer_timelime/src/timeLIME/src/planner.py
+-rw-r--r--   0        0        0     2012 2024-04-23 16:22:21.373671 stabilizer_timelime-0.2.1/stabilizer_timelime/src/timeLIME/src/runexp.py
+-rw-r--r--   0        0        0     1891 2024-04-23 16:22:21.373856 stabilizer_timelime-0.2.1/stabilizer_timelime/src/timeLIME/src/split_dataset.py
+-rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 stabilizer_timelime-0.2.1/PKG-INFO
```

### Comparing `stabilizer_timelime-0.2.0/LICENSE` & `stabilizer_timelime-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/README.md` & `stabilizer_timelime-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/pyproject.toml` & `stabilizer_timelime-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "stabilizer_timelime"
-version = "0.2.0"
+version = "0.2.1"
 authors = ["Sukhad Joshi <sjoshi32@ncsu.edu>"]
 description = "Packaged project that contains code to scrape GitHub data, build and run stabilizer and timeline"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/dataslurper/prudenceChecker.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/dataslurper/prudenceChecker.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/dataslurper/slurpdata.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/dataslurper/slurpdata.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/__init__.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/__init__.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/config.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/config.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/.DS_Store` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/CFS.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/CFS.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/CFS_regression.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/CFS_regression.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/DE.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/DE.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/Find_bellwethers.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/Find_bellwethers.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/Performance_Calculator.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/Performance_Calculator.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/Stats_files.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/Stats_files.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/attribute_selector.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/attribute_selector.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/birch.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/birch.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/birch_bellwether_p_CFS.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/birch_bellwether_p_CFS.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/collect_bellwethers.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/collect_bellwethers.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,36 +3,32 @@
 
 from . import utils
 
 from ..config import Config
 
 DEFAULT_CONFIG = Config()
 
-def collect_bellwether(config=DEFAULT_CONFIG):
-    month = config.month
-    no_goals= config.no_goals
-    seed = config.seed
-
+def collect_bellwether(seeds: list, month: int, goals: list):
     output_folder = "bellwethers/"
 
-    for i in range(no_goals):
-        goal = utils.get_goal(i, config)
+    for goal in goals:
 
         res_df_0 = pd.DataFrame()
         res_df_1 = pd.DataFrame()
 
-        result_source = 'results/with_CFS_DE/'+str(seed)+'/month_' + str(month) + '_models/' + goal + '/'
-        bellwether_0 = pd.read_csv(os.path.join(result_source, "bellwether_level_0.csv"))
-        bellwether_1 = pd.read_csv(os.path.join(result_source, "bellwether_level_1.csv"))
+        for seed in seeds:
+            result_source = 'results/with_CFS_DE/'+str(seed)+'/month_' + str(month) + '_models/' + goal + '/'
+            bellwether_0 = pd.read_csv(os.path.join(result_source, "bellwether_level_0.csv"))
+            bellwether_1 = pd.read_csv(os.path.join(result_source, "bellwether_level_1.csv"))
 
-        bellwether_0["seed"] = seed
-        bellwether_1["seed"] = seed
+            bellwether_0["seed"] = seed
+            bellwether_1["seed"] = seed
 
-        res_df_0 = res_df_0.append(bellwether_0, ignore_index=True)
-        res_df_1 = res_df_1.append(bellwether_1, ignore_index=True)
+            res_df_0 = res_df_0.append(bellwether_0, ignore_index=True)
+            res_df_1 = res_df_1.append(bellwether_1, ignore_index=True)
         
         if not os.path.exists("meta_data/old_new_names_mapping.csv"):
             print("Old names - New names mapping missing. Exiting ...")
             exit(0)
 
         mapping_df = pd.read_csv("meta_data/old_new_names_mapping.csv")
```

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/default_bellwether.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/default_bellwether.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/generate_results.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/generate_results.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/init_datafiles.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/init_datafiles.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,51 +3,47 @@
 
 import os
 import csv
 import sys
 
 import pandas as pd
 
-from ..config import Config
-
-DEFAULT_CONFIG = Config()
-
-def create_folders(config=DEFAULT_CONFIG):
+def create_folders(seeds: list, month: int, goals: list):
     folders_to_create = ["data/data_use/","results/attribute/", "results/with_CFS_DE/", "meta_data/", "bellwethers/"]
 
     for folder in folders_to_create:
         shutil.rmtree(folder, ignore_errors=True)
         Path(folder).mkdir(parents=True, exist_ok=True)
     
-    shutil.rmtree("data/data_use_{0}_months/".format(config.month), ignore_errors=True)
-    Path("data/data_use_{0}_months/".format(config.month)).mkdir(parents=True, exist_ok=True)
+    shutil.rmtree("data/data_use_{0}_months/".format(month), ignore_errors=True)
+    Path("data/data_use_{0}_months/".format(month)).mkdir(parents=True, exist_ok=True)
 
-    attr_seed = os.path.join("results/attribute/", str(config.seed))
-    Path(attr_seed).mkdir(parents=True, exist_ok=True)
+    for seed in seeds:
+        attr_seed = os.path.join("results/attribute/", str(seed))
+        Path(attr_seed).mkdir(parents=True, exist_ok=True)
 
-    cfs_seed = os.path.join("results/with_CFS_DE/", str(config.seed))
-    Path(cfs_seed).mkdir(parents=True, exist_ok=True)
+        cfs_seed = os.path.join("results/with_CFS_DE/", str(seed))
+        Path(cfs_seed).mkdir(parents=True, exist_ok=True)
 
-    subfolders = ['Stats_new', 'month_{0}_models'.format(config.month)]
+    subfolders = ['Stats_new', 'month_{0}_models'.format(month)]
 
     for subfolder in subfolders:
         subfolder_path = os.path.join(cfs_seed, subfolder)
         if subfolder!='Stats_new':
-            goals=config.goals
             for goal in goals:
                 updated_goal_path=os.path.join(subfolder_path, goal)
                 os.makedirs(updated_goal_path, exist_ok=True)
         else:
             os.makedirs(subfolder_path, exist_ok=True)
 
     Path("results/with_CFS_DE/Stats_new").mkdir(parents=True, exist_ok=True)
 
 
-def copy_source_2_data_use(config=DEFAULT_CONFIG):
-    source_dir = config.data_path
+def copy_source_2_data_use(data_path: str):
+    source_dir = data_path
     dest_dir = "data/data_use/"
 
     for file_name in os.listdir(source_dir):
         file_path = os.path.join(source_dir, file_name)
         if file_name.endswith('.csv'):
             shutil.copy(file_path, os.path.join(dest_dir, file_name))
 
@@ -72,38 +68,38 @@
         num += 1
         di = {"old":os.path.splitext(file)[0], "new":new_name}
         record.append(di)
     
     pd.DataFrame.from_dict(record).to_csv("meta_data/old_new_names_mapping.csv", index=False)
 
 
-def move_x_months_data(config=DEFAULT_CONFIG):
+def move_x_months_data(month: int):
     source_folder = "data/data_use"
-    destination_folder = "data/data_use_{0}_months/".format(config.month)
+    destination_folder = "data/data_use_{0}_months/".format(month)
 
     for filename in os.listdir(source_folder):
         if filename.endswith(".csv"):
             filepath = os.path.join(source_folder, filename)
             df = pd.read_csv(filepath)
 
             num_rows = df.shape[0]
 
-            if num_rows>config.month:
+            if num_rows>month:
                 shutil.copy(filepath, os.path.join(destination_folder, filename))
 
-def move_back_2_data_use(config=DEFAULT_CONFIG):
-    source_dir = "data/data_use_{0}_months/".format(config.month)
+def move_back_2_data_use(month: int, goals: list):
+    source_dir = "data/data_use_{0}_months/".format(month)
     dest_dir = "data/data_use/"
 
     for file_name in os.listdir(dest_dir):
         file_path = os.path.join(dest_dir, file_name)
 
         os.remove(file_path)
 
-    cols = ["dates"] + config.goals
+    cols = ["dates"] + goals
 
     # Loop through all files in the source directory
     for file_name in os.listdir(source_dir):
         file_path = os.path.join(source_dir, file_name)
         
         # Check if the file is a CSV file
         if file_name.endswith('.csv'):
@@ -113,22 +109,22 @@
             df = df.reindex(sorted(df.columns), axis=1)
 
             df.to_csv(file_path, index=False)
             
             shutil.copy(file_path, os.path.join(dest_dir, file_name))
 
 
-def init_datafiles(config=DEFAULT_CONFIG):
+def init_datafiles(data_path:str, seeds: list, month: int, goals: list):
     # Create necessary folders
-    create_folders(config)
+    create_folders(seeds, month, goals)
 
     # Copy data files to data_use/
-    copy_source_2_data_use(config)
+    copy_source_2_data_use(data_path)
 
     # Rename data files
     rename_data_files()
 
     # Only take data for x months
-    move_x_months_data(config)
+    move_x_months_data(month)
 
     # Move data back to data_use/ with some cleaning
-    move_back_2_data_use(config)
+    move_back_2_data_use(month, goals)
```

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/learners.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/learners.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/optimizer.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/optimizer.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/predictor_advance_v1.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/predictor_advance_v1.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/predictor_baseline.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/predictor_baseline.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/scott_knott.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/scott_knott.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/utils.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/stabilizer/src/utils.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/timeLIME/src/othertools.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/timeLIME/src/othertools.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/timeLIME/src/planner.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/timeLIME/src/planner.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/timeLIME/src/runexp.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/timeLIME/src/runexp.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/stabilizer_timelime/src/timeLIME/src/split_dataset.py` & `stabilizer_timelime-0.2.1/stabilizer_timelime/src/timeLIME/src/split_dataset.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.2.0/PKG-INFO` & `stabilizer_timelime-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stabilizer_timelime
-Version: 0.2.0
+Version: 0.2.1
 Summary: Packaged project that contains code to scrape GitHub data, build and run stabilizer and timeline
 Author: Sukhad Joshi
 Author-email: sjoshi32@ncsu.edu
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

