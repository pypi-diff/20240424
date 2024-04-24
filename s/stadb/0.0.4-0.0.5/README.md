# Comparing `tmp/stadb-0.0.4.tar.gz` & `tmp/stadb-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stadb-0.0.4.tar", last modified: Mon Apr 15 10:50:50 2024, max compression
+gzip compressed data, was "stadb-0.0.5.tar", last modified: Wed Apr 24 13:07:51 2024, max compression
```

## Comparing `stadb-0.0.4.tar` & `stadb-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-15 10:50:50.953537 stadb-0.0.4/
--rw-rw-r--   0 enoc      (1000) enoc      (1000)     1069 2024-04-04 09:35:28.000000 stadb-0.0.4/LICENSE
--rw-r--r--   0 enoc      (1000) enoc      (1000)     2949 2024-04-15 10:50:50.953537 stadb-0.0.4/PKG-INFO
--rw-rw-r--   0 enoc      (1000) enoc      (1000)      565 2024-04-15 10:48:07.000000 stadb-0.0.4/README.md
--rw-rw-r--   0 enoc      (1000) enoc      (1000)     2281 2024-04-15 10:48:07.000000 stadb-0.0.4/pyproject.toml
--rw-rw-r--   0 enoc      (1000) enoc      (1000)       38 2024-04-15 10:50:50.953537 stadb-0.0.4/setup.cfg
-drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-15 10:50:50.949537 stadb-0.0.4/src/
-drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-15 10:50:50.949537 stadb-0.0.4/src/stadb/
--rw-rw-r--   0 enoc      (1000) enoc      (1000)       43 2024-04-04 10:50:06.000000 stadb-0.0.4/src/stadb/__init__.py
--rw-rw-r--   0 enoc      (1000) enoc      (1000)     1262 2024-04-04 11:35:04.000000 stadb-0.0.4/src/stadb/logger.py
--rw-rw-r--   0 enoc      (1000) enoc      (1000)     5895 2024-04-04 14:18:57.000000 stadb-0.0.4/src/stadb/postgresql.py
--rw-rw-r--   0 enoc      (1000) enoc      (1000)    42150 2024-04-15 10:50:18.000000 stadb-0.0.4/src/stadb/sensorthings.py
--rw-rw-r--   0 enoc      (1000) enoc      (1000)    12469 2024-04-04 12:39:51.000000 stadb-0.0.4/src/stadb/timescaledb.py
--rw-rw-r--   0 enoc      (1000) enoc      (1000)     4356 2024-04-04 11:29:48.000000 stadb-0.0.4/src/stadb/utils.py
-drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-15 10:50:50.953537 stadb-0.0.4/src/stadb.egg-info/
--rw-r--r--   0 enoc      (1000) enoc      (1000)     2949 2024-04-15 10:50:50.000000 stadb-0.0.4/src/stadb.egg-info/PKG-INFO
--rw-rw-r--   0 enoc      (1000) enoc      (1000)      344 2024-04-15 10:50:50.000000 stadb-0.0.4/src/stadb.egg-info/SOURCES.txt
--rw-rw-r--   0 enoc      (1000) enoc      (1000)        1 2024-04-15 10:50:50.000000 stadb-0.0.4/src/stadb.egg-info/dependency_links.txt
--rw-rw-r--   0 enoc      (1000) enoc      (1000)       50 2024-04-15 10:50:50.000000 stadb-0.0.4/src/stadb.egg-info/requires.txt
--rw-rw-r--   0 enoc      (1000) enoc      (1000)       11 2024-04-15 10:50:50.000000 stadb-0.0.4/src/stadb.egg-info/top_level.txt
--rw-rw-r--   0 enoc      (1000) enoc      (1000)      234 2024-04-04 10:49:56.000000 stadb-0.0.4/src/test.py
+drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-24 13:07:51.901108 stadb-0.0.5/
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     1069 2024-04-04 09:35:28.000000 stadb-0.0.5/LICENSE
+-rw-r--r--   0 enoc      (1000) enoc      (1000)     2949 2024-04-24 13:07:51.901108 stadb-0.0.5/PKG-INFO
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)      565 2024-04-24 13:07:47.000000 stadb-0.0.5/README.md
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     2281 2024-04-24 13:07:47.000000 stadb-0.0.5/pyproject.toml
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)       38 2024-04-24 13:07:51.901108 stadb-0.0.5/setup.cfg
+drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-24 13:07:51.897108 stadb-0.0.5/src/
+drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-24 13:07:51.901108 stadb-0.0.5/src/stadb/
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)       43 2024-04-04 10:50:06.000000 stadb-0.0.5/src/stadb/__init__.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     1262 2024-04-04 11:35:04.000000 stadb-0.0.5/src/stadb/logger.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     5895 2024-04-04 14:18:57.000000 stadb-0.0.5/src/stadb/postgresql.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)    42168 2024-04-24 13:07:19.000000 stadb-0.0.5/src/stadb/sensorthings.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)    12469 2024-04-04 12:39:51.000000 stadb-0.0.5/src/stadb/timescaledb.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     4356 2024-04-04 11:29:48.000000 stadb-0.0.5/src/stadb/utils.py
+drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-24 13:07:51.901108 stadb-0.0.5/src/stadb.egg-info/
+-rw-r--r--   0 enoc      (1000) enoc      (1000)     2949 2024-04-24 13:07:51.000000 stadb-0.0.5/src/stadb.egg-info/PKG-INFO
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)      344 2024-04-24 13:07:51.000000 stadb-0.0.5/src/stadb.egg-info/SOURCES.txt
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)        1 2024-04-24 13:07:51.000000 stadb-0.0.5/src/stadb.egg-info/dependency_links.txt
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)       50 2024-04-24 13:07:51.000000 stadb-0.0.5/src/stadb.egg-info/requires.txt
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)       11 2024-04-24 13:07:51.000000 stadb-0.0.5/src/stadb.egg-info/top_level.txt
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)      234 2024-04-04 10:49:56.000000 stadb-0.0.5/src/test.py
```

### Comparing `stadb-0.0.4/LICENSE` & `stadb-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `stadb-0.0.4/PKG-INFO` & `stadb-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stadb
-Version: 0.0.4
+Version: 0.0.5
 Summary: SensorThings API database connector for advanced functionalities
 Author-email: Enoc Martínez <enoc.martinez@upc.edu>
 Maintainer-email: Enoc Martínez <enoc.martinez@upc.edu>
 License: MIT License
         
         Copyright (c) 2024 EnocMartinez
         
@@ -51,10 +51,10 @@
 Database connector for SensorThings API database for advanced interaction. It is based on [FROST-Server](https://github.com/FraunhoferIOSB/FROST-Server) implementation.
 
 It also adds specific support for time-series data by extending the database with [TimescaleDB](https://www.timescale.com/), which allows for faster queries and optimized storage. 
 
 ### Contact info ###
 
 * **author**: Enoc Martínez  
-* **version**: 0.0.4
+* **version**: 0.0.5
 * **organization**: Universitat Politècnica de Catalunya (UPC)  
 * **contact**: enoc.martinez@upc.edu
```

### Comparing `stadb-0.0.4/README.md` & `stadb-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,10 +2,10 @@
 Database connector for SensorThings API database for advanced interaction. It is based on [FROST-Server](https://github.com/FraunhoferIOSB/FROST-Server) implementation.
 
 It also adds specific support for time-series data by extending the database with [TimescaleDB](https://www.timescale.com/), which allows for faster queries and optimized storage. 
 
 ### Contact info ###
 
 * **author**: Enoc Martínez  
-* **version**: 0.0.4
+* **version**: 0.0.5
 * **organization**: Universitat Politècnica de Catalunya (UPC)  
 * **contact**: enoc.martinez@upc.edu
```

### Comparing `stadb-0.0.4/pyproject.toml` & `stadb-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 
 
 [project]
 
 name = "stadb"  # REQUIRED, is the only field that cannot be marked as dynamic.
-version = "0.0.4"  # REQUIRED, although can be dynamic
+version = "0.0.5"  # REQUIRED, although can be dynamic
 description = "SensorThings API database connector for advanced functionalities"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["sta", "setuptools", "development", "sensorthings"]
 
 authors = [
```

### Comparing `stadb-0.0.4/src/stadb/logger.py` & `stadb-0.0.5/src/stadb/logger.py`

 * *Files identical despite different names*

### Comparing `stadb-0.0.4/src/stadb/postgresql.py` & `stadb-0.0.5/src/stadb/postgresql.py`

 * *Files identical despite different names*

### Comparing `stadb-0.0.4/src/stadb/sensorthings.py` & `stadb-0.0.5/src/stadb/sensorthings.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 email: enoc.martinez@upc.edu
 license: MIT
 created: 4/10/23
 """
 
 from .postgresql import PgDatabaseConnector
 from .logger import LoggerSuperclass
-from .utils import reverse_dictionary, dataframe_to_dict, run_subprocess, merge_dataframes_by_columns
+from .utils import reverse_dictionary, dataframe_to_dict, run_subprocess, merge_dataframes_by_columns, slice_dataframes
 import json
 import pandas as pd
 import numpy as np
 from .timescaledb import TimescaleDB
 import rich
 from rich.progress import Progress
 import time
```

### Comparing `stadb-0.0.4/src/stadb/timescaledb.py` & `stadb-0.0.5/src/stadb/timescaledb.py`

 * *Files identical despite different names*

### Comparing `stadb-0.0.4/src/stadb/utils.py` & `stadb-0.0.5/src/stadb/utils.py`

 * *Files identical despite different names*

### Comparing `stadb-0.0.4/src/stadb.egg-info/PKG-INFO` & `stadb-0.0.5/src/stadb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stadb
-Version: 0.0.4
+Version: 0.0.5
 Summary: SensorThings API database connector for advanced functionalities
 Author-email: Enoc Martínez <enoc.martinez@upc.edu>
 Maintainer-email: Enoc Martínez <enoc.martinez@upc.edu>
 License: MIT License
         
         Copyright (c) 2024 EnocMartinez
         
@@ -51,10 +51,10 @@
 Database connector for SensorThings API database for advanced interaction. It is based on [FROST-Server](https://github.com/FraunhoferIOSB/FROST-Server) implementation.
 
 It also adds specific support for time-series data by extending the database with [TimescaleDB](https://www.timescale.com/), which allows for faster queries and optimized storage. 
 
 ### Contact info ###
 
 * **author**: Enoc Martínez  
-* **version**: 0.0.4
+* **version**: 0.0.5
 * **organization**: Universitat Politècnica de Catalunya (UPC)  
 * **contact**: enoc.martinez@upc.edu
```

