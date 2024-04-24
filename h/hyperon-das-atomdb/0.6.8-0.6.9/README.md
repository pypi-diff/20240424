# Comparing `tmp/hyperon_das_atomdb-0.6.8.tar.gz` & `tmp/hyperon_das_atomdb-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperon_das_atomdb-0.6.8.tar", max compression
+gzip compressed data, was "hyperon_das_atomdb-0.6.9.tar", max compression
```

## Comparing `hyperon_das_atomdb-0.6.8.tar` & `hyperon_das_atomdb-0.6.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1081 2024-04-22 16:57:31.788797 hyperon_das_atomdb-0.6.8/LICENCE
--rw-r--r--   0        0        0     2687 2024-04-22 16:57:31.788797 hyperon_das_atomdb-0.6.8/README.md
--rw-r--r--   0        0        0      306 2024-04-22 16:57:31.792797 hyperon_das_atomdb-0.6.8/hyperon_das_atomdb/__init__.py
--rw-r--r--   0        0        0      116 2024-04-22 16:57:31.792797 hyperon_das_atomdb-0.6.8/hyperon_das_atomdb/adapters/__init__.py
--rw-r--r--   0        0        0    20567 2024-04-22 16:57:31.792797 hyperon_das_atomdb-0.6.8/hyperon_das_atomdb/adapters/ram_only.py
--rw-r--r--   0        0        0    37515 2024-04-22 16:57:31.792797 hyperon_das_atomdb-0.6.8/hyperon_das_atomdb/adapters/redis_mongo_db.py
--rw-r--r--   0        0        0    20514 2024-04-22 16:57:31.792797 hyperon_das_atomdb-0.6.8/hyperon_das_atomdb/database.py
--rw-r--r--   0        0        0      939 2024-04-22 16:57:31.792797 hyperon_das_atomdb-0.6.8/hyperon_das_atomdb/exceptions.py
--rw-r--r--   0        0        0     1122 2024-04-22 16:57:31.792797 hyperon_das_atomdb-0.6.8/hyperon_das_atomdb/index.py
--rw-r--r--   0        0        0     1052 2024-04-22 16:57:31.792797 hyperon_das_atomdb-0.6.8/hyperon_das_atomdb/logger.py
--rw-r--r--   0        0        0        0 2024-04-22 16:57:31.792797 hyperon_das_atomdb-0.6.8/hyperon_das_atomdb/utils/__init__.py
--rw-r--r--   0        0        0     1947 2024-04-22 16:57:31.792797 hyperon_das_atomdb-0.6.8/hyperon_das_atomdb/utils/expression_hasher.py
--rw-r--r--   0        0        0     1388 2024-04-22 16:57:31.792797 hyperon_das_atomdb-0.6.8/hyperon_das_atomdb/utils/patterns.py
--rw-r--r--   0        0        0       65 2024-04-22 16:57:31.792797 hyperon_das_atomdb-0.6.8/hyperon_das_atomdb/utils/settings.py
--rw-r--r--   0        0        0     1114 2024-04-22 16:57:40.256777 hyperon_das_atomdb-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     3516 1970-01-01 00:00:00.000000 hyperon_das_atomdb-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-23 18:24:57.198577 hyperon_das_atomdb-0.6.9/LICENCE
+-rw-r--r--   0        0        0     2687 2024-04-23 18:24:57.198577 hyperon_das_atomdb-0.6.9/README.md
+-rw-r--r--   0        0        0      306 2024-04-23 18:24:57.202577 hyperon_das_atomdb-0.6.9/hyperon_das_atomdb/__init__.py
+-rw-r--r--   0        0        0      116 2024-04-23 18:24:57.202577 hyperon_das_atomdb-0.6.9/hyperon_das_atomdb/adapters/__init__.py
+-rw-r--r--   0        0        0    20567 2024-04-23 18:24:57.202577 hyperon_das_atomdb-0.6.9/hyperon_das_atomdb/adapters/ram_only.py
+-rw-r--r--   0        0        0    37515 2024-04-23 18:24:57.202577 hyperon_das_atomdb-0.6.9/hyperon_das_atomdb/adapters/redis_mongo_db.py
+-rw-r--r--   0        0        0    20514 2024-04-23 18:24:57.202577 hyperon_das_atomdb-0.6.9/hyperon_das_atomdb/database.py
+-rw-r--r--   0        0        0      939 2024-04-23 18:24:57.202577 hyperon_das_atomdb-0.6.9/hyperon_das_atomdb/exceptions.py
+-rw-r--r--   0        0        0     1122 2024-04-23 18:24:57.202577 hyperon_das_atomdb-0.6.9/hyperon_das_atomdb/index.py
+-rw-r--r--   0        0        0     1052 2024-04-23 18:24:57.202577 hyperon_das_atomdb-0.6.9/hyperon_das_atomdb/logger.py
+-rw-r--r--   0        0        0        0 2024-04-23 18:24:57.202577 hyperon_das_atomdb-0.6.9/hyperon_das_atomdb/utils/__init__.py
+-rw-r--r--   0        0        0     1947 2024-04-23 18:24:57.202577 hyperon_das_atomdb-0.6.9/hyperon_das_atomdb/utils/expression_hasher.py
+-rw-r--r--   0        0        0     1388 2024-04-23 18:24:57.202577 hyperon_das_atomdb-0.6.9/hyperon_das_atomdb/utils/patterns.py
+-rw-r--r--   0        0        0       65 2024-04-23 18:24:57.202577 hyperon_das_atomdb-0.6.9/hyperon_das_atomdb/utils/settings.py
+-rw-r--r--   0        0        0     1114 2024-04-23 18:25:11.222607 hyperon_das_atomdb-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     3516 1970-01-01 00:00:00.000000 hyperon_das_atomdb-0.6.9/PKG-INFO
```

### Comparing `hyperon_das_atomdb-0.6.8/LICENCE` & `hyperon_das_atomdb-0.6.9/LICENCE`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.8/README.md` & `hyperon_das_atomdb-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.8/hyperon_das_atomdb/adapters/ram_only.py` & `hyperon_das_atomdb-0.6.9/hyperon_das_atomdb/adapters/ram_only.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.8/hyperon_das_atomdb/adapters/redis_mongo_db.py` & `hyperon_das_atomdb-0.6.9/hyperon_das_atomdb/adapters/redis_mongo_db.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.8/hyperon_das_atomdb/database.py` & `hyperon_das_atomdb-0.6.9/hyperon_das_atomdb/database.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.8/hyperon_das_atomdb/exceptions.py` & `hyperon_das_atomdb-0.6.9/hyperon_das_atomdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.8/hyperon_das_atomdb/index.py` & `hyperon_das_atomdb-0.6.9/hyperon_das_atomdb/index.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.8/hyperon_das_atomdb/logger.py` & `hyperon_das_atomdb-0.6.9/hyperon_das_atomdb/logger.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.8/hyperon_das_atomdb/utils/expression_hasher.py` & `hyperon_das_atomdb-0.6.9/hyperon_das_atomdb/utils/expression_hasher.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.8/hyperon_das_atomdb/utils/patterns.py` & `hyperon_das_atomdb-0.6.9/hyperon_das_atomdb/utils/patterns.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.8/pyproject.toml` & `hyperon_das_atomdb-0.6.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperon-das-atomdb"
-version = "0.6.8"
+version = "0.6.9"
 description = "Persistence layer for Distributed AtomSpace"
 authors = ["marcocapozzoli <marcocapozzoli90@gmail.com>"]
 readme = "README.md"
 packages = [{include = "hyperon_das_atomdb"}]
 
 [tool.poetry.urls]
 "Code" = "https://github.com/singnet/das-atom-db"
```

### Comparing `hyperon_das_atomdb-0.6.8/PKG-INFO` & `hyperon_das_atomdb-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperon-das-atomdb
-Version: 0.6.8
+Version: 0.6.9
 Summary: Persistence layer for Distributed AtomSpace
 Author: marcocapozzoli
 Author-email: marcocapozzoli90@gmail.com
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

