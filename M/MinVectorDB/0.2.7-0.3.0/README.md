# Comparing `tmp/minvectordb-0.2.7.tar.gz` & `tmp/minvectordb-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minvectordb-0.2.7.tar", last modified: Wed Apr 17 08:50:41 2024, max compression
+gzip compressed data, was "minvectordb-0.3.0.tar", last modified: Tue Apr 23 13:49:11 2024, max compression
```

## Comparing `minvectordb-0.2.7.tar` & `minvectordb-0.3.0.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-17 08:50:41.823442 minvectordb-0.2.7/
--rw-r--r--   0 guobingming   (501) staff       (20)    11357 2023-09-19 11:00:45.000000 minvectordb-0.2.7/LICENSE
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-17 08:50:41.822956 minvectordb-0.2.7/MinVectorDB.egg-info/
--rw-r--r--   0 guobingming   (501) staff       (20)    17247 2024-04-17 08:50:41.000000 minvectordb-0.2.7/MinVectorDB.egg-info/PKG-INFO
--rw-r--r--   0 guobingming   (501) staff       (20)     1102 2024-04-17 08:50:41.000000 minvectordb-0.2.7/MinVectorDB.egg-info/SOURCES.txt
--rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-04-17 08:50:41.000000 minvectordb-0.2.7/MinVectorDB.egg-info/dependency_links.txt
--rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-03-07 03:06:27.000000 minvectordb-0.2.7/MinVectorDB.egg-info/not-zip-safe
--rw-r--r--   0 guobingming   (501) staff       (20)      173 2024-04-17 08:50:41.000000 minvectordb-0.2.7/MinVectorDB.egg-info/requires.txt
--rw-r--r--   0 guobingming   (501) staff       (20)       13 2024-04-17 08:50:41.000000 minvectordb-0.2.7/MinVectorDB.egg-info/top_level.txt
--rw-r--r--   0 guobingming   (501) staff       (20)    17247 2024-04-17 08:50:41.823199 minvectordb-0.2.7/PKG-INFO
--rw-r--r--   0 guobingming   (501) staff       (20)    15931 2024-04-17 05:54:49.000000 minvectordb-0.2.7/README.md
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-17 08:50:41.818629 minvectordb-0.2.7/min_vec/
--rw-r--r--   0 guobingming   (501) staff       (20)      115 2024-04-16 07:36:11.000000 minvectordb-0.2.7/min_vec/__init__.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-17 08:50:41.818872 minvectordb-0.2.7/min_vec/api/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:42.000000 minvectordb-0.2.7/min_vec/api/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)    13736 2024-04-17 08:23:55.000000 minvectordb-0.2.7/min_vec/api/api.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-17 08:50:41.819102 minvectordb-0.2.7/min_vec/computational_layer/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:06:12.000000 minvectordb-0.2.7/min_vec/computational_layer/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)      890 2024-04-17 08:04:09.000000 minvectordb-0.2.7/min_vec/computational_layer/engines.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-17 08:50:41.819443 minvectordb-0.2.7/min_vec/configs/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:24.000000 minvectordb-0.2.7/min_vec/configs/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2553 2024-04-17 05:52:07.000000 minvectordb-0.2.7/min_vec/configs/config.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3611 2024-04-17 06:40:43.000000 minvectordb-0.2.7/min_vec/configs/parameters_validator.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-17 08:50:41.820762 minvectordb-0.2.7/min_vec/data_structures/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:07:22.000000 minvectordb-0.2.7/min_vec/data_structures/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2316 2024-04-03 03:58:31.000000 minvectordb-0.2.7/min_vec/data_structures/fields_mapper.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1036 2024-03-06 14:55:44.000000 minvectordb-0.2.7/min_vec/data_structures/filter.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1545 2024-04-12 07:35:09.000000 minvectordb-0.2.7/min_vec/data_structures/kmeans.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1282 2024-04-13 15:42:07.000000 minvectordb-0.2.7/min_vec/data_structures/limited_dict.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2977 2024-04-17 08:45:02.000000 minvectordb-0.2.7/min_vec/data_structures/limited_sort.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3811 2024-04-12 09:25:04.000000 minvectordb-0.2.7/min_vec/data_structures/scaler.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-17 08:50:41.821481 minvectordb-0.2.7/min_vec/execution_layer/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:09:45.000000 minvectordb-0.2.7/min_vec/execution_layer/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2316 2024-04-16 09:40:39.000000 minvectordb-0.2.7/min_vec/execution_layer/cluster_worker.py
--rw-r--r--   0 guobingming   (501) staff       (20)    19379 2024-04-16 10:23:42.000000 minvectordb-0.2.7/min_vec/execution_layer/matrix_serializer.py
--rw-r--r--   0 guobingming   (501) staff       (20)     7818 2024-04-17 08:40:57.000000 minvectordb-0.2.7/min_vec/execution_layer/query.py
--rw-r--r--   0 guobingming   (501) staff       (20)      362 2024-02-26 09:43:31.000000 minvectordb-0.2.7/min_vec/execution_layer/session.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-17 08:50:41.821821 minvectordb-0.2.7/min_vec/storage_layer/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:04:15.000000 minvectordb-0.2.7/min_vec/storage_layer/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)    16764 2024-04-16 10:15:07.000000 minvectordb-0.2.7/min_vec/storage_layer/storage.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-17 08:50:41.822055 minvectordb-0.2.7/min_vec/utils/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:09.000000 minvectordb-0.2.7/min_vec/utils/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3389 2024-04-15 04:05:21.000000 minvectordb-0.2.7/min_vec/utils/utils.py
--rw-r--r--   0 guobingming   (501) staff       (20)       38 2024-04-17 08:50:41.823498 minvectordb-0.2.7/setup.cfg
--rw-r--r--   0 guobingming   (501) staff       (20)     1471 2024-04-16 07:36:11.000000 minvectordb-0.2.7/setup.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-17 08:50:41.822661 minvectordb-0.2.7/test/
--rw-r--r--   0 guobingming   (501) staff       (20)       31 2024-01-31 10:38:44.000000 minvectordb-0.2.7/test/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1834 2024-04-15 04:04:57.000000 minvectordb-0.2.7/test/test_initial.py
--rw-r--r--   0 guobingming   (501) staff       (20)    11844 2024-04-12 07:35:09.000000 minvectordb-0.2.7/test/test_save_and_query.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-23 13:49:11.941129 minvectordb-0.3.0/
+-rw-r--r--   0 guobingming   (501) staff       (20)    11357 2023-09-19 11:00:45.000000 minvectordb-0.3.0/LICENSE
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-23 13:49:11.940550 minvectordb-0.3.0/MinVectorDB.egg-info/
+-rw-r--r--   0 guobingming   (501) staff       (20)    11365 2024-04-23 13:49:11.000000 minvectordb-0.3.0/MinVectorDB.egg-info/PKG-INFO
+-rw-r--r--   0 guobingming   (501) staff       (20)     1171 2024-04-23 13:49:11.000000 minvectordb-0.3.0/MinVectorDB.egg-info/SOURCES.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-04-23 13:49:11.000000 minvectordb-0.3.0/MinVectorDB.egg-info/dependency_links.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-03-07 03:06:27.000000 minvectordb-0.3.0/MinVectorDB.egg-info/not-zip-safe
+-rw-r--r--   0 guobingming   (501) staff       (20)      173 2024-04-23 13:49:11.000000 minvectordb-0.3.0/MinVectorDB.egg-info/requires.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)       13 2024-04-23 13:49:11.000000 minvectordb-0.3.0/MinVectorDB.egg-info/top_level.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)    11365 2024-04-23 13:49:11.940836 minvectordb-0.3.0/PKG-INFO
+-rw-r--r--   0 guobingming   (501) staff       (20)    10049 2024-04-23 13:48:08.000000 minvectordb-0.3.0/README.md
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-23 13:49:11.935109 minvectordb-0.3.0/min_vec/
+-rw-r--r--   0 guobingming   (501) staff       (20)      122 2024-04-22 03:08:06.000000 minvectordb-0.3.0/min_vec/__init__.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-23 13:49:11.935898 minvectordb-0.3.0/min_vec/api/
+-rw-r--r--   0 guobingming   (501) staff       (20)      273 2024-04-23 05:39:11.000000 minvectordb-0.3.0/min_vec/api/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    10308 2024-04-22 10:03:25.000000 minvectordb-0.3.0/min_vec/api/high_level.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    14711 2024-04-23 11:06:39.000000 minvectordb-0.3.0/min_vec/api/low_level.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-23 13:49:11.936156 minvectordb-0.3.0/min_vec/computational_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:06:12.000000 minvectordb-0.3.0/min_vec/computational_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      890 2024-04-17 08:04:09.000000 minvectordb-0.3.0/min_vec/computational_layer/engines.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-23 13:49:11.936671 minvectordb-0.3.0/min_vec/configs/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:24.000000 minvectordb-0.3.0/min_vec/configs/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2553 2024-04-23 13:22:47.000000 minvectordb-0.3.0/min_vec/configs/config.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3548 2024-04-19 15:33:58.000000 minvectordb-0.3.0/min_vec/configs/parameters_validator.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-23 13:49:11.937651 minvectordb-0.3.0/min_vec/execution_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:09:45.000000 minvectordb-0.3.0/min_vec/execution_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2328 2024-04-23 10:00:41.000000 minvectordb-0.3.0/min_vec/execution_layer/cluster_worker.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    18058 2024-04-23 13:36:51.000000 minvectordb-0.3.0/min_vec/execution_layer/matrix_serializer.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     7236 2024-04-23 13:11:40.000000 minvectordb-0.3.0/min_vec/execution_layer/query.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      362 2024-02-26 09:43:31.000000 minvectordb-0.3.0/min_vec/execution_layer/session.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-23 13:49:11.938093 minvectordb-0.3.0/min_vec/storage_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:04:15.000000 minvectordb-0.3.0/min_vec/storage_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    14526 2024-04-23 09:08:02.000000 minvectordb-0.3.0/min_vec/storage_layer/storage.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-23 13:49:11.939513 minvectordb-0.3.0/min_vec/structures/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:07:22.000000 minvectordb-0.3.0/min_vec/structures/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     6256 2024-04-23 13:26:51.000000 minvectordb-0.3.0/min_vec/structures/fields_filter.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     4656 2024-04-23 11:07:42.000000 minvectordb-0.3.0/min_vec/structures/filter.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1037 2024-04-23 08:37:07.000000 minvectordb-0.3.0/min_vec/structures/id_checker.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1545 2024-04-12 07:35:09.000000 minvectordb-0.3.0/min_vec/structures/kmeans.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1449 2024-04-18 02:30:25.000000 minvectordb-0.3.0/min_vec/structures/limited_dict.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3150 2024-04-23 05:39:11.000000 minvectordb-0.3.0/min_vec/structures/limited_sort.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3810 2024-04-18 03:39:58.000000 minvectordb-0.3.0/min_vec/structures/scaler.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-23 13:49:11.939788 minvectordb-0.3.0/min_vec/utils/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:09.000000 minvectordb-0.3.0/min_vec/utils/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     4021 2024-04-23 09:26:54.000000 minvectordb-0.3.0/min_vec/utils/utils.py
+-rw-r--r--   0 guobingming   (501) staff       (20)       38 2024-04-23 13:49:11.941173 minvectordb-0.3.0/setup.cfg
+-rw-r--r--   0 guobingming   (501) staff       (20)     1468 2024-04-23 05:39:11.000000 minvectordb-0.3.0/setup.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-23 13:49:11.940338 minvectordb-0.3.0/test/
+-rw-r--r--   0 guobingming   (501) staff       (20)      198 2024-04-23 11:11:07.000000 minvectordb-0.3.0/test/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1557 2024-04-23 11:18:25.000000 minvectordb-0.3.0/test/test_hmvdb_initial.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1591 2024-04-23 10:40:50.000000 minvectordb-0.3.0/test/test_smvdb_initial.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    13195 2024-04-23 11:10:18.000000 minvectordb-0.3.0/test/test_smvdb_save_and_query.py
```

### Comparing `minvectordb-0.2.7/LICENSE` & `minvectordb-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.7/MinVectorDB.egg-info/SOURCES.txt` & `minvectordb-0.3.0/MinVectorDB.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -5,32 +5,35 @@
 MinVectorDB.egg-info/SOURCES.txt
 MinVectorDB.egg-info/dependency_links.txt
 MinVectorDB.egg-info/not-zip-safe
 MinVectorDB.egg-info/requires.txt
 MinVectorDB.egg-info/top_level.txt
 min_vec/__init__.py
 min_vec/api/__init__.py
-min_vec/api/api.py
+min_vec/api/high_level.py
+min_vec/api/low_level.py
 min_vec/computational_layer/__init__.py
 min_vec/computational_layer/engines.py
 min_vec/configs/__init__.py
 min_vec/configs/config.py
 min_vec/configs/parameters_validator.py
-min_vec/data_structures/__init__.py
-min_vec/data_structures/fields_mapper.py
-min_vec/data_structures/filter.py
-min_vec/data_structures/kmeans.py
-min_vec/data_structures/limited_dict.py
-min_vec/data_structures/limited_sort.py
-min_vec/data_structures/scaler.py
 min_vec/execution_layer/__init__.py
 min_vec/execution_layer/cluster_worker.py
 min_vec/execution_layer/matrix_serializer.py
 min_vec/execution_layer/query.py
 min_vec/execution_layer/session.py
 min_vec/storage_layer/__init__.py
 min_vec/storage_layer/storage.py
+min_vec/structures/__init__.py
+min_vec/structures/fields_filter.py
+min_vec/structures/filter.py
+min_vec/structures/id_checker.py
+min_vec/structures/kmeans.py
+min_vec/structures/limited_dict.py
+min_vec/structures/limited_sort.py
+min_vec/structures/scaler.py
 min_vec/utils/__init__.py
 min_vec/utils/utils.py
 test/__init__.py
-test/test_initial.py
-test/test_save_and_query.py
+test/test_hmvdb_initial.py
+test/test_smvdb_initial.py
+test/test_smvdb_save_and_query.py
```

### Comparing `minvectordb-0.2.7/min_vec/api/api.py` & `minvectordb-0.3.0/min_vec/api/low_level.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,25 @@
-"""api.py - The MinVectorDB API."""
+"""low_level.py - The MinVectorDB API."""
 import os
+from pathlib import Path
 from typing import Union, List, Tuple
 
 import numpy as np
 from spinesUtils.asserts import raise_if, ParameterTypeAssert
-from spinesUtils.logging import Logger
 from spinesUtils.timer import Timer
 
-from min_vec.configs.config import config
 from min_vec.configs.parameters_validator import ParametersValidator
 from min_vec.execution_layer.query import Query
 from min_vec.execution_layer.matrix_serializer import MatrixSerializer
 from min_vec.utils.utils import unavailable_if_deleted
+from min_vec.api import logger
+from min_vec.structures.filter import Filter
 
-logger = Logger(
-    fp=config.MVDB_LOG_PATH,
-    name='MinVectorDB',
-    truncate_file=config.MVDB_TRUNCATE_LOG,
-    with_time=config.MVDB_LOG_WITH_TIME,
-    level=config.MVDB_LOG_LEVEL
-)
 
-
-class MinVectorDB:
+class StandaloneMinVectorDB:
     """
     A class for managing a vector database stored in .mvdb files and computing vectors similarity.
     """
 
     @ParametersValidator(
         update_configs=['dim', 'n_clusters', 'chunk_size', 'index_mode', 'dtypes', 'scaler_bits'],
         logger=logger
@@ -38,28 +31,29 @@
         'chunk_size': int,
         'distance': str,
         'index_mode': str,
         'dtypes': str,
         'use_cache': bool,
         'scaler_bits': (None, int),
         'n_threads': (None, int),
-        'warm_up': bool
-    }, func_name='MinVectorDB')
+        'warm_up': bool,
+        'initialize_as_collection': bool
+    }, func_name='StandaloneMinVectorDB')
     def __init__(
-            self, dim: int, database_path: str, n_clusters: int = 16, chunk_size: int = 100_000,
+            self, dim: int, database_path: Union[str, Path], n_clusters: int = 16, chunk_size: int = 100_000,
             distance: str = 'cosine', index_mode: str = 'IVF-FLAT', dtypes: str = 'float32',
             use_cache: bool = True, scaler_bits: Union[int, None] = 8, n_threads: Union[int, None] = 10,
-            warm_up: bool = False
+            warm_up: bool = False, initialize_as_collection: bool = False
     ) -> None:
         """
         Initialize the vector database.
 
         Parameters:
             dim (int): Dimension of the vectors.
-            database_path (str): Path to the database file.
+            database_path (str or Path): The path to the database file.
             n_clusters (int): The number of clusters for the IVF-FLAT index. Default is 8.
             chunk_size (int): The size of each data chunk. Default is 100_000.
             distance (str): Method for calculating vector distance.
                 Options are 'cosine' or 'L2' for Euclidean distance. Default is 'cosine'.
             index_mode (str): The storage mode of the database.
                 Options are 'FLAT' or 'IVF-FLAT'. Default is 'IVF-FLAT'.
             dtypes (str): The data type of the vectors. Default is 'float32'.
@@ -67,51 +61,56 @@
             use_cache (bool): Whether to use cache for query. Default is True.
             scaler_bits (int): The number of bits for scalar quantization.
                 Options are 8, 16, or 32. The default is None, which means no scalar quantization.
                 The 8 for 8-bit, 16 for 16-bit, and 32 for 32-bit.
             n_threads (int): The number of threads to use for parallel processing. Default is 10.
             warm_up (bool): Whether to warm up the database. Default is False.
                 .. versionadded:: 0.2.6
+            initialize_as_collection (bool): Whether to initialize the database as a collection.
+                .. versionadded:: 0.3.0
 
         Raises:
             ValueError: If `chunk_size` is less than or equal to 1.
         """
-        raise_if(ValueError, not str(database_path).endswith('mvdb'), 'database_path must end with .mvdb')
         raise_if(ValueError, chunk_size <= 1, 'chunk_size must greater than 1')
         raise_if(ValueError, distance not in ('cosine', 'L2'), 'distance must be "cosine" or "L2"')
         raise_if(ValueError, index_mode not in ('FLAT', 'IVF-FLAT'), 'index_mode must be "FLAT" or "IVF-FLAT"')
         raise_if(ValueError, dtypes not in ('float16', 'float32', 'float64'),
                  'dtypes must be "float16", "float32" or "float64')
         raise_if(ValueError, not isinstance(n_clusters, int) or n_clusters <= 0,
                  'n_clusters must be int and greater than 0')
         raise_if(ValueError, scaler_bits not in (8, 16, 32, None), 'sq_bits must be 8, 16, 32 or None')
 
-        logger.info("Initializing MinVectorDB with: \n "
-                    f"\r//    dim={dim}, database_path='{database_path}', \n"
-                    f"\r//    n_clusters={n_clusters}, chunk_size={chunk_size},\n"
-                    f"\r//    distance='{distance}', index_mode='{index_mode}', \n"
-                    f"\r//    dtypes='{dtypes}', use_cache={use_cache}, \n"
-                    f"\r//    scaler_bits={scaler_bits}\n"
-                    )
+        if not initialize_as_collection:
+            logger.info("Initializing MinVectorDB with: \n "
+                        f"\r//    dim={dim}, database_path='{database_path}', \n"
+                        f"\r//    n_clusters={n_clusters}, chunk_size={chunk_size},\n"
+                        f"\r//    distance='{distance}', index_mode='{index_mode}', \n"
+                        f"\r//    dtypes='{dtypes}', use_cache={use_cache}, \n"
+                        f"\r//    scaler_bits={scaler_bits}, n_threads={n_threads}, \n"
+                        f"\r//    warm_up={warm_up}, initialize_as_collection={initialize_as_collection}"
+                        )
 
         if chunk_size <= 1:
             raise ValueError('chunk_size must be greater than 1')
 
+        self._database_path = database_path
+
         self._matrix_serializer = MatrixSerializer(
             dim=dim,
-            database_path=database_path,
+            collection_path=self._database_path,
             n_clusters=n_clusters,
             chunk_size=chunk_size,
             index_mode=index_mode,
             logger=logger,
             dtypes=dtypes,
             scaler_bits=scaler_bits,
             warm_up=warm_up
         )
-        self._data_loader = self._matrix_serializer.iterable_dataloader
+        self._data_loader = self._matrix_serializer.dataloader
         self._id_filter = self._matrix_serializer.id_filter
 
         self._timer = Timer()
         self._use_cache = use_cache
         self._distance = distance
 
         raise_if(TypeError, n_threads is not None and not isinstance(n_threads, int), "n_threads must be an integer.")
@@ -121,38 +120,57 @@
             matrix_serializer=self._matrix_serializer,
             n_threads=n_threads if n_threads else min(32, os.cpu_count() + 4),
             distance=distance
         )
 
         self._query.query.clear_cache()
 
-        self._most_recent_query_report = {}
+        self.most_recent_query_report = {}
+
+        self._initialize_as_collection = initialize_as_collection
+
+        if warm_up and self._matrix_serializer.shape[0] > 0:
+            # Pre query once to cache the jax function
+            self.query(np.ones(dim), k=1)
+
+            self.most_recent_query_report = {}
+
+    def get_max_id(self):
+        """
+        Get the maximum ID in the database.
+
+        Returns:
+            int: The maximum ID in the database.
+        """
+        if self._matrix_serializer.IS_DELETED or self._matrix_serializer.id_filter is None:
+            return
+        return self._matrix_serializer.id_filter.find_max_value()
 
     @unavailable_if_deleted
-    def add_item(self, vector: np.ndarray, *, index: int = None, field: str = None) -> int:
+    def add_item(self, vector: Union[np.ndarray, list], *, id: int = None, field: dict = None) -> int:
         """
         Add a single vector to the database.
 
         Parameters:
-            vector (np.ndarray): The vector to be added.
-            index (int, optional, keyword-only): The ID of the vector. If None, a new ID will be generated.
-            field (str, optional, keyword-only): The field of the vector. Default is None. If None, the field will be
+            vector (np.ndarray or list): The vector to be added.
+            id (int, optional, keyword-only): The ID of the vector. If None, a new ID will be generated.
+            field (dict, optional, keyword-only): The field of the vector. Default is None. If None, the field will be
                 set to an empty string.
 
         Returns:
             int: The ID of the added vector.
 
         Raises:
             ValueError: If the vector dimensions don't match or the ID already exists.
         """
-        return self._matrix_serializer.add_item(vector, index=index, field=field)
+        return self._matrix_serializer.add_item(vector, index=id, field=field)
 
     @unavailable_if_deleted
     def bulk_add_items(
-            self, vectors: Union[List[Tuple[np.ndarray, int, str]], List[Tuple[np.ndarray, int]], List[np.ndarray]]
+            self, vectors: Union[List[Tuple[np.ndarray, int, dict]], List[Tuple[np.ndarray, int]], List[Tuple[np.ndarray]]]
     ):
         """
         Bulk add vectors to the database in batches.
 
         Parameters: vectors (list or tuple): A list or tuple of vectors to be saved. Each vector can be a tuple of (
             vector, id, field).
 
@@ -166,89 +184,86 @@
         """
         Save the database, ensuring that all data is written to disk.
         This method is required to be called after saving vectors to query them.
         """
         self._matrix_serializer.commit()
 
     @unavailable_if_deleted
-    def query(self, vector: np.ndarray, k: int = 12, *,
-              fields: Union[List, None] = None,
-              subset_indices: Union[List, None] = None,
+    def query(self, vector: Union[np.ndarray, list], k: int = 12, *,
+              query_filter: Filter = None,
               distance: Union[str, None] = None,
               return_similarity: bool = True):
         """
         Query the database for the vectors most similar to the given vector in batches.
 
         Parameters:
-            vector (np.ndarray): The query vector.
+            vector (np.ndarray or list): The query vector.
             k (int): The number of nearest vectors to return.
-            fields (list, optional): The target of the vector.
-            subset_indices (list, optional): The subset of indices to query.
+            query_filter (Filter, optional): The field filter to apply to the query.
             distance (str): The distance metric to use for the query.
                 .. versionadded:: 0.2.7
             return_similarity (bool): Whether to return the similarity scores.Default is True.
                 .. versionadded:: 0.2.5
 
         Returns:
             Tuple: The indices and similarity scores of the top k nearest vectors.
 
         Raises:
             ValueError: If the database is empty.
         """
+        raise_if(ValueError, not isinstance(vector, (np.ndarray, list)), 'vector must be np.ndarray or list.')
+
         import datetime
 
-        logger.debug(f'Query vector: {vector.tolist()}')
+        logger.debug(f'Query vector: {vector.tolist() if isinstance(vector, np.ndarray) else vector}')
         logger.debug(f'Query k: {k}')
-        logger.debug(f'Query fields: {fields}')
-        logger.debug(f'Query subset_indices: {subset_indices}')
+        logger.debug(f'Query distance: {self._distance if distance is None else distance}')
+        logger.debug(f'Query return_similarity: {return_similarity}')
 
         raise_if(TypeError, not isinstance(k, int) and not (isinstance(k, str) and k != 'all'),
                  'k must be int or "all".')
         raise_if(ValueError, k <= 0, 'k must be greater than 0.')
-        raise_if(ValueError, not isinstance(fields, list) and fields is not None,
-                 'fields must be list or None.')
-        raise_if(ValueError, not isinstance(subset_indices, list) and subset_indices is not None,
-                 'subset_indices must be list or None.')
-        raise_if(ValueError, vector is None, 'vector must be not None.')
+        raise_if(ValueError, not isinstance(query_filter, (Filter, type(None))), 'query_filter must be Filter or None.')
+
         raise_if(ValueError, len(vector) != self._matrix_serializer.shape[1],
                  'vector must be same dim with database.')
-        raise_if(ValueError, not isinstance(vector, np.ndarray), 'vector must be np.ndarray.')
-        raise_if(ValueError, vector.ndim != 1, 'vector must be 1d array.')
+
         raise_if(ValueError, not isinstance(return_similarity, bool), 'return_similarity must be bool.')
         raise_if(ValueError, distance is not None and distance not in ['cosine', 'L2'],
                  'distance must be "cosine" or "L2" or None.')
 
         if self._matrix_serializer.shape[0] == 0:
             raise ValueError('database is empty.')
 
         if k > self._matrix_serializer.shape[0]:
             k = self._matrix_serializer.shape[0]
 
-        self._most_recent_query_report = {}
+        self.most_recent_query_report = {}
 
         self._timer.start()
         if self._use_cache:
-            res = self._query.query(vector=vector, k=k, fields=fields,
-                                    subset_indices=subset_indices, index_mode=self._matrix_serializer.index_mode,
+            res = self._query.query(vector=vector, k=k, query_filter=query_filter, index_mode=self._matrix_serializer.index_mode,
                                     distance=distance, return_similarity=return_similarity)
         else:
-            res = self._query.query(vector=vector, k=k, fields=fields,
-                                    subset_indices=subset_indices, index_mode=self._matrix_serializer.index_mode,
+            res = self._query.query(vector=vector, k=k, query_filter=query_filter,
+                                    index_mode=self._matrix_serializer.index_mode,
                                     now_time=datetime.datetime.now().strftime('%Y%m%d%H%M%S%f'),
                                     distance=distance,
                                     return_similarity=return_similarity)
 
         time_cost = self._timer.last_timestamp_diff()
-        self._most_recent_query_report['Database Shape'] = self.shape
-        self._most_recent_query_report['Query Time'] = f"{time_cost :>.5f} s"
-        self._most_recent_query_report['Query Distance'] = self._distance if distance is None else distance
-        self._most_recent_query_report['Query K'] = k
-        self._most_recent_query_report[f'Top {k} Results Index'] = res[0]
-        if return_similarity:
-            self._most_recent_query_report[f'Top {k} Results Similarity'] = np.array([round(i, 6) for i in res[1]])
+        self.most_recent_query_report['Database Shape'] = self.shape
+        self.most_recent_query_report['Query Time'] = f"{time_cost :>.5f} s"
+        self.most_recent_query_report['Query Distance'] = self._distance if distance is None else distance
+        self.most_recent_query_report['Query K'] = k
+
+        if res[0] is not None:
+            self.most_recent_query_report[f'Top {k} Results ID'] = res[0]
+            if return_similarity:
+                self.most_recent_query_report[f'Top {k} Results Similarity'] = np.array([round(i, 6) for i in res[1]])
 
         return res
 
     @property
     def shape(self):
         """
         Return the shape of the entire database.
@@ -263,19 +278,21 @@
         """
         Create a session to insert data, which will automatically commit the data when the session ends.
         """
         from min_vec.execution_layer.session import DatabaseSession
 
         return DatabaseSession(self)
 
-    @unavailable_if_deleted
     def delete(self):
         """
         Delete the database.
         """
+        if self._matrix_serializer.IS_DELETED:
+            return
+
         import gc
 
         self._matrix_serializer.delete()
         self._query.query.clear_cache()
         self._query.delete()
 
         gc.collect()
@@ -284,15 +301,15 @@
     def query_report_(self):
         """
         Return the most recent query report.
         """
         # print as a pretty string
         # title use bold font
         report = '\n* - MOST RECENT QUERY REPORT -\n'
-        for key, value in self._most_recent_query_report.items():
+        for key, value in self.most_recent_query_report.items():
             report += f'| - {key}: {value}\n'
 
         report += '* - END OF REPORT -\n'
 
         return report
 
     @property
@@ -309,15 +326,25 @@
             'Database use_cache': self._use_cache,
             'Database status': 'DELETED' if self._matrix_serializer.IS_DELETED else 'ACTIVE'
         }}
 
         return db_report
 
     def __repr__(self):
-        title = "Deleted MinVectorDB object with status: \n"
+        if self._matrix_serializer.IS_DELETED:
+            if self._initialize_as_collection:
+                title = "Deleted MinVectorDB collection with status: \n"
+            else:
+                title = "Deleted MinVectorDB object with status: \n"
+        else:
+            if self._initialize_as_collection:
+                title = "MinVectorDB collection with status: \n"
+            else:
+                title = "MinVectorDB object with status: \n"
+
         report = '\n* - DATABASE STATUS REPORT -\n'
         for key, value in self.status_report_['DATABASE STATUS REPORT'].items():
             report += f'| - {key}: {value}\n'
 
         return title + report
 
     def __str__(self):
```

### Comparing `minvectordb-0.2.7/min_vec/computational_layer/engines.py` & `minvectordb-0.3.0/min_vec/computational_layer/engines.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.7/min_vec/configs/config.py` & `minvectordb-0.3.0/min_vec/configs/config.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.7/min_vec/configs/parameters_validator.py` & `minvectordb-0.3.0/min_vec/configs/parameters_validator.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,16 +66,15 @@
 
             dir_path = Path(kwargs.get("database_path"))
 
             update_configs_dict = {}
             for key in self.update_configs_list:
                 update_configs_dict[key] = kwargs.get(key)
 
-            self.database_path_parent = Path(dir_path).parent.absolute() / Path(
-                '.mvdb'.join(Path(dir_path).absolute().name.split('.mvdb')[:-1]))
+            self.database_path_parent = Path(dir_path).parent.absolute() / dir_path.absolute().name
 
             if not self.database_path_parent.exists():
                 self.database_path_parent.mkdir(parents=True)
                 first_create = True
             else:
                 first_create = False
```

### Comparing `minvectordb-0.2.7/min_vec/data_structures/filter.py` & `minvectordb-0.3.0/min_vec/structures/id_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pyroaring import BitMap
 
 
-class IDFilter:
+class IDChecker:
     def __init__(self):
         self.ids = BitMap()
 
     def add(self, items):
         if isinstance(items, int):  # 如果items是单个整数
             self.ids.add(items)
         else:  # 如果items是可迭代的整数集合
```

### Comparing `minvectordb-0.2.7/min_vec/data_structures/kmeans.py` & `minvectordb-0.3.0/min_vec/structures/kmeans.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.7/min_vec/data_structures/limited_dict.py` & `minvectordb-0.3.0/min_vec/structures/limited_dict.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,56 @@
 from collections import OrderedDict
+import threading
 
 
 class LimitedDict:
     def __init__(self, max_size):
         self.max_size = max_size
         self.cache = OrderedDict()
+        self.lock = threading.RLock()
 
     def __setitem__(self, key, value):
-        # 先检查键是否已存在，如果是，则先删除旧键
-        if key in self.cache:
-            del self.cache[key]
-        self.cache[key] = value
-        # 如果缓存超出最大大小，移除最老的项
-        if len(self.cache) > self.max_size:
-            self.cache.popitem(last=False)
+        with self.lock:
+            if key in self.cache:
+                del self.cache[key]
+            self.cache[key] = value
+            if len(self.cache) > self.max_size:
+                self.cache.popitem(last=False)
 
     def __getitem__(self, key):
-        try:
-            # 移动到末尾，表示最近使用
-            value = self.cache.pop(key)
-            self.cache[key] = value
-            return value
-        except KeyError:
-            raise KeyError('Key not found')
+        with self.lock:
+            try:
+                value = self.cache.pop(key)
+                self.cache[key] = value
+                return value
+            except KeyError:
+                raise KeyError('Key not found')
 
     def get(self, key, default=None):
-        if key not in self.cache:
-            return default
-        return self.__getitem__(key)
+        with self.lock:
+            if key not in self.cache:
+                return default
+            return self.__getitem__(key)
 
     def clear(self):
-        self.cache.clear()
+        with self.lock:
+            self.cache.clear()
 
     def keys(self):
-        return self.cache.keys()
+        with self.lock:
+            return self.cache.keys()
 
     def pop(self, key, default=None):
-        return self.cache.pop(key, default)
+        with self.lock:
+            return self.cache.pop(key, default)
 
     def __contains__(self, key):
-        return key in self.cache
+        with self.lock:
+            return key in self.cache
 
     def __len__(self):
-        return len(self.cache)
+        with self.lock:
+            return len(self.cache)
 
     def __repr__(self):
-        return repr(self.cache)
+        with self.lock:
+            return repr(self.cache)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `minvectordb-0.2.7/min_vec/data_structures/limited_sort.py` & `minvectordb-0.3.0/min_vec/structures/limited_sort.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 import threading
 import numpy as np
 
 from min_vec.computational_layer.engines import cosine_distance, argsort_topk, euclidean_distance
 
 
 class LimitedSorted:
-    def __init__(self, vector: np.ndarray, n: int, scaler, chunk_size, distance='cosine'):
+    def __init__(self, dim, dtype, scaler, chunk_size):
         """A class to store the top n most similar vectors to a given vector.
 
         .. versionadded:: 0.2.5
 
         Parameters:
-            vector (np.ndarray): The vector to compare against.
-            n (int): The number of most similar vectors to store.
+            dim (int): The dimension of the vectors.
+            dtype (type): The data type of the vectors.
             scaler (Scaler, optional): The scaler to decode the vectors.
             chunk_size (int): The maximum number of vectors to store.
                 .. versionadded:: 0.2.7
-            distance (str): The distance metric to use for the query.
-                .. versionadded:: 0.2.7
         """
         self.lock = threading.RLock()
-        self.vector = vector
-        self.n = n
-        self.distance = distance
-        self.distance_func = cosine_distance if distance == 'cosine' else euclidean_distance
+        self.dim = dim
+        self.n = None
         self.scaler = scaler
         self.max_length = chunk_size
         self.current_length = 0
-        self.similarities = np.empty(self.max_length, dtype=vector.dtype)
+        self.similarities = np.empty(self.max_length, dtype=dtype)
         self.indices = np.empty(self.max_length, dtype=int)
-        self.matrix_subset = np.empty((self.max_length, vector.size), dtype=vector.dtype)
+        self.matrix_subset = np.empty((self.max_length, dim), dtype=dtype)
+
+    def set_n(self, n):
+        self.n = n
 
     def add(self, sim: np.ndarray, indices: np.ndarray, matrix: np.ndarray):
         num_new_items = len(sim)
         with self.lock:
             end_pos = self.current_length + num_new_items
             if end_pos > self.max_length:
                 self.max_length = max(self.max_length * 2, end_pos)
                 self.similarities = np.resize(self.similarities, self.max_length)
                 self.indices = np.resize(self.indices, self.max_length)
-                self.matrix_subset = np.resize(self.matrix_subset, (self.max_length, self.vector.size))
+                self.matrix_subset = np.resize(self.matrix_subset, (self.max_length, self.dim))
 
             self.similarities[self.current_length:end_pos] = sim
             self.indices[self.current_length:end_pos] = indices
             self.matrix_subset[self.current_length:end_pos] = matrix
 
             self.current_length = end_pos
 
@@ -51,17 +50,28 @@
 
             idx_len = len(idx)
             self.similarities[:idx_len] = self.similarities[idx]
             self.indices[:idx_len] = self.indices[idx]
             self.matrix_subset[:idx_len] = self.matrix_subset[idx]
             self.current_length = idx_len
 
-    def get_top_n(self):
+    def get_top_n(self, vector: np.ndarray, distance='cosine'):
+        if distance == 'cosine':
+            distance_func = cosine_distance
+        else:
+            distance_func = euclidean_distance
+
         if self.scaler is None:
-            sim = self.distance_func(self.vector, self.matrix_subset[:self.current_length])
+            sim = distance_func(vector, self.matrix_subset[:self.current_length])
         else:
             decoded_vectors = self.scaler.decode(self.matrix_subset[:self.current_length])
-            sim = self.distance_func(self.vector, decoded_vectors)
+            sim = distance_func(vector, decoded_vectors)
 
-        sorted_idx = np.argsort(-sim) if self.distance_func == cosine_distance else np.argsort(sim)
+        sorted_idx = np.argsort(-sim) if distance == 'cosine' else np.argsort(sim)
 
         return self.indices[sorted_idx], sim[sorted_idx]
+
+    def clear(self):
+        self.current_length = 0
+        self.similarities = np.empty(self.max_length, dtype=self.similarities.dtype)
+        self.indices = np.empty(self.max_length, dtype=self.indices.dtype)
+        self.matrix_subset = np.empty((self.max_length, self.dim), dtype=self.matrix_subset.dtype)
```

### Comparing `minvectordb-0.2.7/min_vec/data_structures/scaler.py` & `minvectordb-0.3.0/min_vec/structures/scaler.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,21 +50,21 @@
         self.fitted = True
 
     def encode(self, vectors):
         raise_if(ValueError, not self.fitted, 'The model must be fitted before encoding.')
 
         epsilon = 1e-9
         n_levels_minus_1 = self.n_levels - 1
+        range_vals = self.range_vals
         min_vals = self.min_vals
-        max_vals = self.max_vals
 
         quantized = ne.evaluate(
-            "((vectors - min_vals) / (max_vals - min_vals + epsilon)) * n_levels_minus_1", optimization='moderate',
-            local_dict={'vectors': vectors, 'min_vals': min_vals, 'max_vals': max_vals,
-                        'n_levels_minus_1': n_levels_minus_1, 'epsilon': epsilon}
+            "((vectors - min_vals) / (range_vals + epsilon)) * n_levels_minus_1", optimization='moderate',
+            local_dict={'vectors': vectors, 'min_vals': min_vals, 'n_levels_minus_1': n_levels_minus_1,
+                        'epsilon': epsilon, 'range_vals': range_vals}
         )
         quantized = np.clip(quantized, 0, n_levels_minus_1).astype(self.bits)
 
         return quantized
 
     def fit_transform(self, vectors):
         self.partial_fit(vectors)
```

### Comparing `minvectordb-0.2.7/min_vec/execution_layer/cluster_worker.py` & `minvectordb-0.3.0/min_vec/execution_layer/cluster_worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Callable
 
 from spinesUtils.logging import Logger
 
 from min_vec.storage_layer.storage import StorageWorker
-from min_vec.data_structures.kmeans import BatchKMeans
+from min_vec.structures.kmeans import BatchKMeans
 
 
 class ClusterWorker:
     def __init__(
             self,
             logger: Logger,
             iterable_dataloader: Callable,
@@ -31,35 +31,36 @@
 
     def build_index(self, scaler=None):
         """
         Build the IVF index more efficiently.
         """
         max_len = 0
         # 初始化每个聚类的存储列表
-        temp_clusters = {i: ([], [], []) for i in range(self.n_clusters)}
+        temp_clusters = {i: ([], []) for i in range(self.n_clusters)}
 
-        for data, indices, fields in self.iterable_dataloader(read_chunk_only=True, mode='lazy'):
+        filenames = self.storage_worker.get_all_files(read_type='chunk')
+        for filename in filenames:
+            data, indices = self.iterable_dataloader(filename, mode='lazy')
             labels = self._kmeans_clustering(data)
 
             # 直接按标签将数据分配到相应的聚类
-            for d, idx, f, label in zip(data, indices, fields, labels):
+            for d, idx, label in zip(data, indices, labels):
                 temp_clusters[label][0].append(d)
                 temp_clusters[label][1].append(idx)
-                temp_clusters[label][2].append(f)
                 max_len += 1
 
             if max_len >= 10000:
                 # 遍历每个聚类，保存数据
-                for cluster_id, (d, idx, f) in temp_clusters.items():
+                for cluster_id, (d, idx) in temp_clusters.items():
                     if d:  # 检查是否有数据，避免保存空聚类
-                        self.save_data(d, idx, f, write_chunk=False, cluster_id=cluster_id)
+                        self.save_data(d, idx, None, write_chunk=False, cluster_id=cluster_id)
 
                 # 初始化每个聚类的存储列表
-                temp_clusters = {i: ([], [], []) for i in range(self.n_clusters)}
+                temp_clusters = {i: ([], []) for i in range(self.n_clusters)}
                 max_len = 0
 
         if max_len > 0:
-            for cluster_id, (d, idx, f) in temp_clusters.items():
+            for cluster_id, (d, idx) in temp_clusters.items():
                 if d:
-                    self.save_data(d, idx, f, write_chunk=False, cluster_id=cluster_id)
+                    self.save_data(d, idx, None, write_chunk=False, cluster_id=cluster_id)
 
         self.storage_worker.delete_chunk()
```

### Comparing `minvectordb-0.2.7/min_vec/execution_layer/matrix_serializer.py` & `minvectordb-0.3.0/min_vec/execution_layer/matrix_serializer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,346 +1,312 @@
 from datetime import datetime
 from pathlib import Path
 import shutil
+from typing import Union
 
 import numpy as np
 from spinesUtils.asserts import raise_if
 from spinesUtils.logging import Logger
 
-from min_vec.data_structures.filter import IDFilter
+from min_vec.structures.id_checker import IDChecker
 from min_vec.utils.utils import io_checker
 from min_vec.configs.config import config
-from min_vec.data_structures.kmeans import BatchKMeans
-from min_vec.data_structures.scaler import ScalarQuantization
-from min_vec.data_structures.fields_mapper import FieldsMapper
+from min_vec.structures.kmeans import BatchKMeans
+from min_vec.structures.scaler import ScalarQuantization
+from min_vec.structures.fields_filter import FieldIndex
 from min_vec.storage_layer.storage import StorageWorker
 from min_vec.execution_layer.cluster_worker import ClusterWorker
 
 
 class MatrixSerializer:
     """
     The MatrixSerializer class is used to serialize and deserialize the matrix data.
     """
     def __init__(
             self,
             dim: int,
-            database_path: str,
+            collection_path: Union[str, Path],
             logger: Logger,
             n_clusters: int = 16,
             chunk_size: int = 1_000_000,
             index_mode: str = 'IVF-FLAT',
             dtypes: str = 'float32',
             scaler_bits=None,
             warm_up: bool = False
     ) -> None:
         """
-        Initialize the vector database.
+        Initialize the vector collection.
 
         Parameters:
             dim (int): Dimension of the vectors.
-            database_path (str): Path to the database file.
+            collection_path (str): Path to the collections file.
             logger (Logger): The logger object.
             n_clusters (int): The number of clusters for the IVF-FLAT index. Default is 16.
             chunk_size (int): The size of each data chunk. Default is 1_000_000.
-            index_mode (str): The index mode of the database.
+            index_mode (str): The index mode of the collection.
                 Options are 'FLAT' or 'IVF-FLAT'. Default is 'IVF-FLAT'.
             dtypes (str): The data type of the vectors. Default is 'float32'.
                 Options are 'float16', 'float32' or 'float64'.
             scaler_bits (int): The number of bits for scalar quantization. Default is None.
                 Options are 8, 16, 32. If None, scalar quantization will not be used.
                 The 8 bits for uint8, 16 bits for uint16, 32 bits for uint32.
-            warm_up (bool): Whether to warm up the database. Default is False.
+            warm_up (bool): Whether to warm up the collection. Default is False.
 
         Raises:
             ValueError: If `chunk_size` is less than or equal to 1.
         """
         self.last_commit_time = None
-        # set commit flag, if the flag is True, the database will not be saved
+        # set commit flag, if the flag is True, the collection will not be saved
         self.COMMIT_FLAG = True
-        # set flag for scalar quantization, if the flag is True, the database will be rescanned for scalar quantization
-        self.RESCAN_FOR_SQ_FLAG = False
-
         self.IS_DELETED = False
 
         self.logger = logger
 
         # set parent path
-        self._initialize_parent_path(database_path)
+        self._initialize_parent_path(collection_path)
 
         self._dtypes_map = {'float16': np.float16, 'float32': np.float32, 'float64': np.float64}
 
         # set dtypes
         self.dtypes = self._dtypes_map[dtypes]
         # set index mode
         self.index_mode = index_mode
         # set n_clusters
         self.n_clusters = n_clusters
         # set dim
         self.dim = dim
         # set chunk size
         self.chunk_size = chunk_size
         # set filter path
-        self._filter_path = self.database_path_parent / 'id_filter.mvdb'
+        self._filter_path = self.collections_path_parent / 'id_filter.mvdb'
 
-        # set database path
-        self.database_path = self.database_path_parent / Path(database_path).name.split('.mvdb')[0]
+        # set collection path
+        self.collections_path = self.collections_path_parent  # / Path(collection_path).name
 
         # set scalar quantization bits
         self.scaler_bits = scaler_bits if scaler_bits is not None else None
         self.scaler = None
         if self.scaler_bits is not None:
             self._initialize_scalar_quantization()
 
         # initialize the storage worker
-        self.storage_worker = StorageWorker(self.database_path_parent, self.dim,
+        self.storage_worker = StorageWorker(self.collections_path_parent, self.dim,
                                             self.chunk_size,
                                             quantizer=None if self.scaler_bits is None else self.scaler,
                                             warm_up=warm_up)
 
-        self.logger.info(f"Initializing database folder path: '{'.mvdb'.join(database_path.split('.mvdb')[:-1])}/'")
-
-        # ============== Loading or create one empty database ==============
-        # first of all, initialize a database
+        # ============== Loading or create one empty collection ==============
+        # first of all, initialize a collection
         self.database = []
         self.indices = []
         self.fields = []
 
-        self._initialize_fields_mapper()
+        self._initialize_fields_index()
         self._initialize_ann_model()
-        self._initialize_id_filter()
+        self._initialize_id_checker()
 
         self.cluster_worker = ClusterWorker(
             logger=self.logger,
-            iterable_dataloader=self.iterable_dataloader,
+            iterable_dataloader=self.dataloader,
             ann_model=self.ann_model,
             storage_worker=self.storage_worker,
             save_data=self.save_data,
             n_clusters=self.n_clusters
         )
 
         if self._get_cluster_dataset_num() > 0 and self.index_mode == 'FLAT':
             # cause the index mode is FLAT, but the cluster dataset is not empty,
             # so the clustered datasets will also be traversed during querying.
             self.logger.warning('The index mode is FLAT, but the cluster dataset is not empty, '
                                 'so the clustered datasets will also be traversed during querying.')
 
-    def _initialize_parent_path(self, database_path):
+    def _initialize_parent_path(self, collections_path):
         """make directory if not exist"""
-        self.database_path_parent = Path(database_path).parent.absolute() / Path(
-            '.mvdb'.join(Path(database_path).absolute().name.split('.mvdb')[:-1]))
+        self.collections_path_parent = (Path(collections_path).parent.absolute() /
+                                        Path(collections_path).absolute().name)
 
-        self.database_path_parent.mkdir(parents=True, exist_ok=True)
+        self.collections_path_parent.mkdir(parents=True, exist_ok=True)
 
     def _initialize_scalar_quantization(self):
-        if Path(self.database_path_parent / 'sq_model.mvdb').exists():
-            self.scaler = ScalarQuantization.load(self.database_path_parent / 'sq_model.mvdb')
+        if Path(self.collections_path_parent / 'sq_model.mvdb').exists():
+            self.scaler = ScalarQuantization.load(self.collections_path_parent / 'sq_model.mvdb')
         else:
             self.scaler = ScalarQuantization(bits=self.scaler_bits, decode_dtype=self.dtypes)
 
     def _initialize_ann_model(self):
         """initialize ann model"""
         if self.index_mode == 'IVF-FLAT':
             MVDB_KMEANS_EPOCHS = config.MVDB_KMEANS_EPOCHS
             self.ann_model = BatchKMeans(n_clusters=self.n_clusters, random_state=0,
                                          batch_size=10240, epochs=MVDB_KMEANS_EPOCHS)
 
-            if Path(self.database_path_parent / 'ann_model.mvdb').exists() and self.index_mode == 'IVF-FLAT':
-                self.ann_model = self.ann_model.load(self.database_path_parent / 'ann_model.mvdb')
+            if Path(self.collections_path_parent / 'ann_model.mvdb').exists() and self.index_mode == 'IVF-FLAT':
+                self.ann_model = self.ann_model.load(self.collections_path_parent / 'ann_model.mvdb')
                 if (self.ann_model.n_clusters != self.n_clusters or
                         self.ann_model.epochs != MVDB_KMEANS_EPOCHS or
                         self.ann_model.batch_size != 10240):
                     self.ann_model = BatchKMeans(n_clusters=self.n_clusters, random_state=0,
                                                  batch_size=10240, epochs=MVDB_KMEANS_EPOCHS)
         else:
             self.ann_model = None
 
-    def _initialize_fields_mapper(self):
-        """initialize fields mapper"""
-        if Path(self.database_path_parent / 'fields_mapper.mvdb').exists():
-            self.fields_mapper = FieldsMapper().load(self.database_path_parent / 'fields_mapper.mvdb')
+    def _initialize_fields_index(self):
+        """initialize fields index"""
+        if Path(self.collections_path_parent / 'fields_index.mvdb').exists():
+            self.fields_index = FieldIndex().load(self.collections_path_parent / 'fields_index.mvdb')
         else:
-            self.fields_mapper = FieldsMapper()
+            self.fields_index = FieldIndex()
 
-    def _initialize_id_filter(self):
-        """initialize id filter and shape"""
-        self.id_filter = IDFilter()
+    def _initialize_id_checker(self):
+        """initialize id checker and shape"""
+        self.id_filter = IDChecker()
 
         if self._filter_path.exists():
             self.id_filter.from_file(self._filter_path)
         else:
-            if self.database_path.exists():
-                for database, indices, fields in self.storage_worker.read(read_type='all'):
+            if self.collections_path.exists():
+                filenames = self.storage_worker.get_all_files(read_type='all')
+                for filename in filenames:
+                    database, indices = self.storage_worker.read(filename=filename)
                     self.id_filter.add(indices)
 
         self.last_id = self.id_filter.find_max_value()
 
     def check_commit(self):
         if not self.COMMIT_FLAG:
             raise ValueError("Did you forget to run `commit()` function ? Try to run `commit()` first.")
 
-    def reset_database(self):
+    def reset_collection(self):
         """Reset the database to its initial state with zeros."""
         self.database = []
         self.indices = []
         self.fields = []
 
     @io_checker
-    def iterable_dataloader(self, read_chunk_only=False, from_tail=False, mode='eager'):
+    def dataloader(self, filename, mode='eager'):
         """
         Generator for loading the database and index.
 
         Parameters:
-            read_chunk_only (bool): Whether to read only the chunk.
-            from_tail (bool): Whether to read from the end of the file.
+            filename (str): The name of the file to load.
             mode (str): The mode of the generator. Options are 'eager' or 'lazy'. Default is 'eager'.
 
         Yields:
             tuple: A tuple of (database, index, field).
 
         Raises:
             FileNotFoundError: If the file does not exist.
             IOError: If the file cannot be read.
             PermissionError: If the file cannot be read due to permission issues.
             UnKnownError: If an unknown error occurs.
         """
-        read_type = 'all' if not read_chunk_only else 'chunk'
-
-        for data, indices, fields in self.storage_worker.read(read_type=read_type, reverse=from_tail):
-            if data is None:
-                continue
-
-            if mode == 'lazy':
-                yield data, indices, fields
-            else:
-                yield data, indices, self.fields_mapper.decode(fields)
+        data, indices = self.storage_worker.read(filename=filename)
 
-    def cluster_dataloader(self, cluster_id, mode='eager'):
-        """
-        Generator for loading the database and index. Only used for querying when index_mode is IVF-FLAT.
-
-        Parameters:
-            cluster_id (int): The cluster id.
-            mode (str): The mode of the generator. Options are 'eager' or 'lazy'. Default is 'eager'.
-
-        Yields:
-            tuple: A tuple of (database, index, field).
-
-        Raises:
-            FileNotFoundError: If the file does not exist.
-            IOError: If the file cannot be read.
-            PermissionError: If the file cannot be read due to permission issues.
-            UnKnownError: If an unknown error occurs.
-        """
-        for data, indices, fields in self.storage_worker.read(read_type='cluster', cluster_id=str(cluster_id)):
-            if mode == 'lazy':
-                yield data, indices, fields
-            else:
-                yield data, indices, self.fields_mapper.decode(fields)
+        if mode == 'lazy':
+            return data, indices
+        else:
+            return data, indices
 
-    def _is_database_reset(self):
+    def _is_collection_reset(self):
         """
-        Check if the database is in its reset state (empty list).
+        Check if the collection is in its reset state (empty list).
 
         Returns:
-            bool: True if the database is reset, False otherwise.
+            bool: True if the collection is reset, False otherwise.
         """
         return not (self.database and self.indices and self.fields)
 
     def _length_checker(self):
         """
-        Check if the length of the database and index are equal.
-
         Raises:
             ValueError: If the lengths of the database, indices, and fields are not the same.
         """
-        if not self._is_database_reset() and not self.COMMIT_FLAG:
+        if not self._is_collection_reset() and not self.COMMIT_FLAG:
             if not (len(self.database) == len(self.indices) == len(self.fields)):
-                raise ValueError('The database, index length and field length not the same.')
+                raise ValueError('The database, index length and field length in collection are not the same.')
 
     def save_data(self, data, indices, fields, write_chunk=True, cluster_id=None, normalize=False):
         """Optimized method to save data to chunk or cluster group with reusable logic."""
+        if fields is not None and cluster_id is None:
+            for id, field in zip(indices, fields):
+                self.fields_index.store(field, id)
 
-        if isinstance(fields, str) or all(isinstance(i, str) for i in fields):
-            fields_indices = self.fields_mapper.encode(fields)
-        else:
-            fields_indices = fields
-
-        self.storage_worker.write(data, indices, fields_indices,
+        self.storage_worker.write(data, indices,
                                   write_type='chunk' if write_chunk else 'cluster',
                                   cluster_id=str(cluster_id) if cluster_id is not None else cluster_id,
                                   normalize=normalize)
 
     @io_checker
     def save_chunk_immediately(self, normalize=True):
         """
-        Save the current state of the database to a .mvdb file.
+        Save the current state of the collection to a .mvdb file.
 
         Returns:
-            Path: The path of the saved database file.
+            Path: The path of the saved collection file.
         """
         self._length_checker()
 
-        if self._is_database_reset():
+        if self._is_collection_reset():
             return []
 
         self.save_data(
             self.database,
             self.indices,
             self.fields,
             write_chunk=True,
             cluster_id=None,
             normalize=normalize
         )
 
-        self.reset_database()  # reset database, indices and fields
+        self.reset_collection()  # reset collection, indices and fields
 
     def auto_save_chunk(self, normalize=True):
         self._length_checker()
         if len(self.database) >= self.chunk_size:
             self.save_chunk_immediately(normalize=normalize)
 
         return
 
     def _get_cluster_dataset_num(self):
-        if not self.database_path.exists():
+        if not self.collections_path.exists():
             return 0
 
         return self.storage_worker.get_cluster_dataset_num()
 
     def commit(self):
         """
-        Save the database, ensuring that all data is written to disk.
+        Save the collection, ensuring that all data is written to disk.
         This method is required to be called after saving vectors to query them.
         """
         if not self.COMMIT_FLAG:
             self.logger.debug('Saving chunk immediately...')
             self.save_chunk_immediately(normalize=True)
 
             self.logger.debug('Saving id filter...')
             # save filter
             self.id_filter.to_file(self._filter_path)
 
-            # save fields mapper
-            self.logger.debug('Saving fields mapper...')
-            self.fields_mapper.save(self.database_path_parent / 'fields_mapper.mvdb')
+            # save fields index
+            self.logger.debug('Saving fields index...')
+            self.fields_index.save(self.collections_path_parent / 'fields_index.mvdb')
 
             chunk_partition_size = self.storage_worker.get_shape(read_type='chunk')[0]
             if chunk_partition_size >= 100000 and self.index_mode != 'FLAT':
                 self.logger.debug('Building index...')
                 # build index
                 self.build_index()
 
                 # save ivf index and k-means model
                 self.logger.debug('Saving ann model...')
-                self.ann_model.save(self.database_path_parent / 'ann_model.mvdb')
+                self.ann_model.save(self.collections_path_parent / 'ann_model.mvdb')
 
-            self.reset_database()
+            self.reset_collection()
 
             if self.scaler_bits is not None:
-                self.scaler.save(self.database_path_parent / 'sq_model.mvdb')
+                self.scaler.save(self.collections_path_parent / 'sq_model.mvdb')
 
             self.COMMIT_FLAG = True
 
             self.last_commit_time = datetime.now()
 
     def _generate_new_id(self):
         """
@@ -362,19 +328,19 @@
 
         if vector.dtype != self.dtypes:
             vector = vector.astype(self.dtypes)
 
         if vector.ndim == 1:
             vector = vector.reshape(1, -1)
 
-        return vector, index, field if field is not None else ''
+        return vector, index, field if field is not None else {}
 
     def bulk_add_items(self, vectors):
         """
-        Bulk add vectors to the database in batches.
+        Bulk add vectors to the collection in batches.
 
         Parameters: vectors (list or tuple): A list or tuple of vectors to be saved. Each vector can be a tuple of (
             vector, id, field).
 
         Returns:
             list: A list of indices where the vectors are stored.
         """
@@ -388,28 +354,33 @@
         for i in range(0, len(vectors), self.chunk_size):
             batch = vectors[i:i + self.chunk_size]
 
             for sample in batch:
                 if len(sample) == 1:
                     vector = sample[0]
                     index = None
-                    field = ''
+                    field = {}
                 elif len(sample) == 2:
                     vector, index = sample
-                    field = ''
+                    field = {}
                 else:
                     raise_if(ValueError, len(sample) != 3,
                              f'vectors must be tuple of (vector, id[optional], field[optional]).')
                     vector, index, field = sample
 
+                    raise_if(TypeError, not isinstance(field, dict), f'field must be dict, got {type(field)}')
+
+                if isinstance(vector, list):
+                    vector = np.array(vector)
+
                 index = self._generate_new_id() if index is None else index
 
                 raise_if(ValueError, index < 0, f'id must be greater than 0, got {index}')
 
-                field = '' if field is None else field
+                field = {} if field is None else field
                 vector, index, field = self._process_vector_item(vector, index, field)
 
                 self.database.append(vector)
                 internal_id = index if index is not None else self._generate_new_id()
                 self.indices.append(internal_id)
                 new_ids.append(internal_id)
                 self.fields.append(field)
@@ -418,38 +389,39 @@
             self.auto_save_chunk(normalize=True)
 
         if self.COMMIT_FLAG:
             self.COMMIT_FLAG = False
 
         return new_ids
 
-    def add_item(self, vector, *, index: int = None, field: str = None) -> int:
+    def add_item(self, vector, *, index: int = None, field: dict = None) -> int:
         """
-        Add a single vector to the database.
+        Add a single vector to the collection.
 
         Parameters:
             vector (np.ndarray): The vector to be added.
             index (int, optional, keyword-only): The ID of the vector. If None, a new ID will be generated.
-            field (str, optional, keyword-only): The field of the vector. Default is None. If None, the field will be
+            field (dict, optional, keyword-only): The field of the vector. Default is None. If None, the field will be
                 set to an empty string.
         Returns:
             int: The ID of the added vector.
 
         Raises:
             ValueError: If the vector dimensions don't match or the ID already exists.
         """
         raise_if(ValueError, len(vector) != self.dim,
                  f'vector dim error, expect {self.dim}, got {len(vector)}')
+        if isinstance(vector, list):
+            vector = np.array(vector)
+
         raise_if(ValueError, vector.ndim != 1, f'vector dim error, expect 1, got {vector.ndim}')
-        raise_if(ValueError, field is not None and not isinstance(field, str),
-                 f'field must be str, got {type(field)}')
+        raise_if(ValueError, field is not None and not isinstance(field, dict),
+                 f'field must be dict, got {type(field)}')
         raise_if(ValueError, index is not None and not isinstance(index, int), f'id must be int, got {type(index)}')
         raise_if(ValueError, index is not None and index < 0, f'id must be greater than 0, got {index}')
-        raise_if(ValueError, field is not None and not isinstance(field, str),
-                 f'field must be str, got {type(field)}')
 
         index = self._generate_new_id() if index is None else index
 
         raise_if(ValueError, index in self.id_filter, f'id {index} already exists')
 
         vector, index, field = self._process_vector_item(vector, index, field)
 
@@ -464,33 +436,33 @@
 
         if self.COMMIT_FLAG:
             self.COMMIT_FLAG = False
 
         return index
 
     def delete(self):
-        """Delete database."""
-        if not self.database_path_parent.exists():
+        """Delete collection."""
+        if not self.collections_path_parent.exists():
             return None
 
         try:
-            shutil.rmtree(self.database_path_parent)
+            shutil.rmtree(self.collections_path_parent)
         except FileNotFoundError:
             pass
 
         self.IS_DELETED = True
-        self.reset_database()
+        self.reset_collection()
 
         # reinitialize
         if self.scaler_bits is not None:
             self._initialize_scalar_quantization()
 
-        self._initialize_fields_mapper()
+        self._initialize_fields_index()
         self._initialize_ann_model()
-        self._initialize_id_filter()
+        self._initialize_id_checker()
 
         # clear cache
         self.storage_worker.clear_cache()
 
     def build_index(self):
         """
         Build the IVF index.
```

### Comparing `minvectordb-0.2.7/min_vec/execution_layer/query.py` & `minvectordb-0.3.0/min_vec/execution_layer/query.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """query.py: this file is used to query the database for the vectors most similar to the given vector."""
 from concurrent.futures import ThreadPoolExecutor
 import numpy as np
-from spinesUtils.asserts import raise_if
 
 from min_vec.computational_layer.engines import to_normalize
 from min_vec.configs.config import config
-from min_vec.computational_layer.engines import argsort_topk, cosine_distance, euclidean_distance
+from min_vec.computational_layer.engines import cosine_distance
 from min_vec.execution_layer.matrix_serializer import MatrixSerializer
+from min_vec.structures.filter import IDCondition, Filter
 from min_vec.utils.utils import QueryVectorCache
-from min_vec.data_structures.limited_sort import LimitedSorted
+from min_vec.structures.limited_sort import LimitedSorted
 
 
 class Query:
     """Query the database for the vectors most similar to the given vector."""
 
     def __init__(self, matrix_serializer: MatrixSerializer, n_threads=10, distance='cosine') -> None:
         """
@@ -26,174 +26,164 @@
         """
         self.matrix_serializer = matrix_serializer
 
         self.logger = self.matrix_serializer.logger
         # attributes
         self.dtypes = self.matrix_serializer.dtypes
         self.distance = distance
-        self.is_reversed = -1 if self.distance == 'cosine' else 1
         self.chunk_size = self.matrix_serializer.chunk_size
 
-        self.fields_mapper = self.matrix_serializer.fields_mapper
+        self.fields_index = self.matrix_serializer.fields_index
 
         self.n_threads = n_threads
 
         self.scaler = getattr(self.matrix_serializer, 'scaler', None)
 
         self.executors = ThreadPoolExecutor(max_workers=self.n_threads)
+        self.limited_sorted = LimitedSorted(dim=self.matrix_serializer.dim, dtype=self.dtypes,
+                                            scaler=self.scaler, chunk_size=self.chunk_size)
 
-    def _query_chunk(self, database_chunk, index_chunk, vector_field, vector, field, subset_indices, limited_sorted):
+    def _query_chunk(self, vector, query_filter, dataloader, filename):
         """
         Query a single database chunk for the vectors most similar to the given vector.
 
         Parameters:
-            database_chunk (np.ndarray): The database chunk to be queried.
-            index_chunk (np.ndarray): The indices of the vectors in the database chunk.
-            vector_field (np.ndarray): The field of the vectors.
             vector (np.ndarray): The query vector.
-            field (str or list, optional): The target field for filtering the vectors.
-            subset_indices (list, optional): The subset of indices to query.
-            limited_sorted (HeapqSorted): The heapq object to store the top k nearest vectors.
+            query_filter (Filter, optional): The field filter to apply to the query.
 
         Returns:
             Tuple: The indices and similarity scores of the nearest vectors in the chunk.
         """
-        field_condition = None
-        si_condition = None
+        database_chunk, index_chunk = dataloader(filename, mode='lazy')
 
-        if field is not None:
-            field = [self.fields_mapper.fields_str_mapper.get(f, -1) for f in field]
+        if query_filter is not None:
+            subset_indices = []
+            field_filters_must = []
+            field_filters_any = []
+
+            if query_filter.must:
+                for condition_filter in query_filter.must:
+                    if isinstance(condition_filter, IDCondition):
+                        subset_indices.extend(condition_filter.evaluate(index_chunk))
+                    else:
+                        field_filters_must.append(condition_filter)
+
+            if query_filter.any:
+                for condition_filter in query_filter.any:
+                    if isinstance(condition_filter, IDCondition):
+                        subset_indices.extend(condition_filter.evaluate(index_chunk))
+                    else:
+                        field_filters_any.append(condition_filter)
+
+            if field_filters_must or field_filters_any:
+                _fids = self.fields_index.query(
+                    Filter(
+                        must=field_filters_must if field_filters_must else None,
+                        any=field_filters_any if field_filters_any else None
+                    ),
+                    filter_ids=None,
+                    return_ids_only=True
+                )
+                subset_indices = list(set(subset_indices).union(set(_fids)))
+            else:
+                subset_indices = list(set(subset_indices))
 
-            field_condition = np.isin(vector_field, field)
-
-        if subset_indices:
-            si_condition = np.isin(index_chunk, subset_indices)
-
-        if field_condition is not None and si_condition is not None:
-            condition = np.logical_and(field_condition, si_condition)
-        elif field_condition is not None:
-            condition = field_condition
-        elif si_condition is not None:
-            condition = si_condition
-        else:
-            condition = False
-
-        if condition is not False:
-            database_chunk = database_chunk[condition]
-            index_chunk = index_chunk[condition]
+            database_chunk = database_chunk[np.isin(index_chunk, subset_indices, assume_unique=True)]
+            index_chunk = index_chunk[np.isin(index_chunk, subset_indices, assume_unique=True)]
 
         if len(index_chunk) == 0:
             return [], []
 
         # Distance calculation core code
         scores = cosine_distance(vector, database_chunk)
 
         if scores.ndim != 1:
             if scores.ndim == 0:
                 scores = np.array([scores])
             elif scores.ndim == 2:
                 scores = scores.squeeze()
 
-        if limited_sorted is not None:
-            limited_sorted.add(scores, index_chunk, database_chunk)
+        self.limited_sorted.add(scores, index_chunk, database_chunk)
 
         return index_chunk, scores
 
     @QueryVectorCache(config.MVDB_QUERY_CACHE_SIZE)
-    def query(self, vector, k=12,
-              fields=None, subset_indices=None, distance=None, return_similarity=False, **kwargs):
+    def query(self, vector, k=12, query_filter=None, distance=None, **kwargs):
         """
         Query the database for the vectors most similar to the given vector in batches.
 
         Parameters:
-            vector (np.ndarray): The query vector.
+            vector (np.ndarray or list): The query vector.
             k (int): The number of nearest vectors to return.
-            fields (list, optional): The target of the vector.
-            subset_indices (list, optional): The subset of indices to query.
+            query_filter (Filter, optional): The field filter to apply to the query.
             distance (str): The distance metric to use for the query.
                 .. versionadded:: 0.2.7
-            return_similarity (bool): Whether to return the similarity scores of the nearest vectors.
-                .. versionadded:: 0.2.5
 
         Returns:
             Tuple: The indices and similarity scores of the top k nearest vectors.
 
         Raises:
             ValueError: If the database is empty.
         """
-        if distance is not None:
-            is_reversed = -1 if distance == 'cosine' else 1
-        else:
-            is_reversed = self.is_reversed
-            distance = self.distance
+        self.limited_sorted.clear()
+
+        distance = distance or self.distance
+
+        if isinstance(vector, list):
+            vector = np.array(vector)
 
         vector = vector.astype(self.dtypes) if vector.dtype != self.dtypes else vector
 
         vector = to_normalize(vector)
 
-        if return_similarity:
-            limited_sorted = LimitedSorted(vector, k, self.scaler, distance=distance, chunk_size=self.chunk_size)
-        else:
-            limited_sorted = None
+        self.limited_sorted.set_n(k)
 
-        all_scores = []
         all_index = []
 
-        def sort_results(all_s, all_i):
-            return np.array(all_i)[argsort_topk(is_reversed * np.array(all_s), k)], None
-
-        def batch_query(vector, fields=None, subset_indices=None, is_ivf=True, cluster_id=None, sort=True):
-            nonlocal all_scores, all_index, limited_sorted
+        def batch_query(is_ivf=True, cid=None, sort=True):
+            nonlocal all_index
 
-            dataloader = self.matrix_serializer.cluster_dataloader(cluster_id, mode='lazy') \
-                if is_ivf and self.matrix_serializer.ann_model \
-                else self.matrix_serializer.iterable_dataloader(mode='lazy')
+            filenames = self.matrix_serializer.storage_worker.get_all_files(
+                read_type='chunk' if not is_ivf else 'cluster', cluster_id=cid)
 
             futures = [i for i in self.executors.map(
-                lambda x: self._query_chunk(x[0], x[1], x[2], vector, fields,
-                                            subset_indices, limited_sorted), dataloader)
+                lambda x: self._query_chunk(vector, query_filter, self.matrix_serializer.dataloader, x),
+                filenames)
                        if len(i[0]) != 0]
 
-            if return_similarity and sort:
-                return limited_sorted.get_top_n()
-
             if not futures:
                 return None, None
 
+            if sort:
+                return self.limited_sorted.get_top_n(vector=vector, distance=distance)
+
             index, scores = zip(*futures)
 
             # if index[0] is iterable, then index is a tuple of numpy ndarray, so we need to flatten it
             if len(index[0].shape) > 0:
                 index = np.concatenate(index).ravel()
-                scores = np.concatenate(scores).ravel()
 
-            all_scores.extend(scores)
             all_index.extend(index)
 
-            return sort_results(all_scores, all_index) if sort else None
-
         # if the index mode is FLAT, use FLAT
         if not (self.matrix_serializer.ann_model is not None and self.matrix_serializer.ann_model.fitted):
-            return batch_query(vector, fields, subset_indices, False)
+            return batch_query(is_ivf=False)
 
         # otherwise, use IVF-FLAT
         cluster_id_sorted = np.argsort(
             -cosine_distance(vector, self.matrix_serializer.ann_model.cluster_centers_)
         )
 
         for cluster_id in cluster_id_sorted:
-            batch_query(vector, fields, subset_indices, cluster_id=cluster_id, sort=False)
+            batch_query(cid=cluster_id, sort=False)
 
             if len(all_index) >= k:
                 break
 
-        if return_similarity:
-            return limited_sorted.get_top_n()
-
-        return sort_results(all_scores, all_index)
+        return self.limited_sorted.get_top_n(vector=vector, distance=distance)
 
     def __del__(self):
         self.executors.shutdown(wait=True)
         self.logger.debug('DatabaseQuery executor shutdown.')
 
     def delete(self):
         self.__del__()
```

### Comparing `minvectordb-0.2.7/min_vec/utils/utils.py` & `minvectordb-0.3.0/min_vec/utils/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """utils.py: this file contains some useful functions and decorators."""
 
 from functools import wraps
+from pathlib import Path
 
 
 class UnKnownError(Exception):
     pass
 
 
 def io_checker(func):
@@ -88,14 +89,29 @@
 
 
 def unavailable_if_deleted(func):
     """A decorator that detects if the function is called after the object is deleted."""
 
     @wraps(func)
     def wrapper(*args, **kwargs):
-        # self is the first parameter
-        if args[0]._matrix_serializer.IS_DELETED:
-            print("The database has been deleted, and the operation is invalid.")
-            return None
+        if hasattr(args[0], '_initialize_as_collection'):
+            # self is the first parameter
+            if args[0]._initialize_as_collection:
+                unit_name = 'collection'
+            else:
+                unit_name = 'database'
+
+            db_name = Path(args[0]._database_path).name
+
+            if args[0]._matrix_serializer.IS_DELETED:
+                raise ValueError(f"The {unit_name} `{db_name}` has been deleted, and the `{func.__name__}` function "
+                                 f"is unavailable.")
+        else:
+            db_name = Path(args[0].root_path).name
+
+            if args[0].STATUS == 'DELETED':
+                raise ValueError(f"The `{db_name}` has been deleted, and the `{func.__name__}` function "
+                                 f"is unavailable.")
+
         return func(*args, **kwargs)
 
     return wrapper
```

### Comparing `minvectordb-0.2.7/setup.py` & `minvectordb-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,23 +5,22 @@
 
 def read_requirements(path):
     return list(Path(path).read_text().splitlines())
 
 
 reqs = read_requirements(Path('.').parent.joinpath("requirements.txt"))
 
-
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='MinVectorDB',
-    version="0.2.7",
-    description='MinVectorDB is a pure Python-implemented, lightweight, serverless vector, locally deployed database' \
-                'that offers clear and concise Python APIs, aimed at lowering the barrier to ' \
+    version="0.3.0",
+    description='MinVectorDB is a pure Python-implemented, lightweight, serverless vector, locally deployed database' 
+                'that offers clear and concise Python APIs, aimed at lowering the barrier to ' 
                 'the use of vector databases.',
     keywords='vector database',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         'Intended Audience :: Science/Research',
```

### Comparing `minvectordb-0.2.7/test/test_initial.py` & `minvectordb-0.3.0/test/test_smvdb_initial.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,50 @@
-from test import MinVectorDB
+import pytest
+
+from test import StandaloneMinVectorDB
 import numpy as np
 
 
 def test_modify_exists_database_parameter():
-    db = MinVectorDB(dim=1024, database_path='test_mvdb.mvdb', chunk_size=10000, dtypes='float32')
+    db = StandaloneMinVectorDB(dim=1024, database_path='test_mvdb', chunk_size=10000, dtypes='float32')
 
     # insert data
     with db.insert_session():
         for i in range(10):
-            db.add_item(np.random.rand(1024), index=i)
+            db.add_item(np.random.rand(1024), id=i)
 
     # modify exists database
-    db = MinVectorDB(dim=1023, database_path='test_mvdb.mvdb', chunk_size=10002, dtypes='float16')
+    db = StandaloneMinVectorDB(dim=1023, database_path='test_mvdb', chunk_size=10002, dtypes='float16')
 
     assert db._matrix_serializer.dim == 1024  # not modified
     assert db._matrix_serializer.chunk_size == 10000  # not modified
     assert db._matrix_serializer.dtypes == np.float32  # not modified
 
     # delete database
     db.delete()
 
 
 def test_using_api_after_database_deleted(capfd):
-    db = MinVectorDB(dim=1024, database_path='test_mvdb.mvdb', chunk_size=10000, dtypes='float32')
+    db = StandaloneMinVectorDB(dim=1024, database_path='test_mvdb', chunk_size=10000, dtypes='float32')
 
     # insert data
     with db.insert_session():
         for i in range(10):
-            db.add_item(np.random.rand(1024), index=i)
+            db.add_item(np.random.rand(1024), id=i)
 
     # delete database
     db.delete()
 
-    # using add_item function after database deleted, it should print "The database has been deleted,
-    # and the operation is invalid."
-    db.add_item(np.random.rand(1024), index=11)
-    out, err = capfd.readouterr()
-    assert out == "The database has been deleted, and the operation is invalid.\n"
-
-    # bulk_add_items
-    db.bulk_add_items([(np.random.rand(1024), 11)])
-    out, err = capfd.readouterr()
-    assert out == "The database has been deleted, and the operation is invalid.\n"
-
-    # query
-    db.query(np.random.rand(1024))
-    out, err = capfd.readouterr()
-    assert out == "The database has been deleted, and the operation is invalid.\n"
+    # using add_item function after database deleted, it should raise ValueError
+    with pytest.raises(ValueError):
+        db.add_item(np.random.rand(1024), id=11)
+
+    # using bulk_add_items function after database deleted, it should raise ValueError
+    with pytest.raises(ValueError):
+        db.bulk_add_items([(np.random.rand(1024), 11)])
+
+    # using query function after database deleted, it should raise ValueError
+    with pytest.raises(ValueError):
+        db.query(np.random.rand(1024))
 
     # delete database
     db.delete()
-    out, err = capfd.readouterr()
-    assert out == "The database has been deleted, and the operation is invalid.\n"
```

