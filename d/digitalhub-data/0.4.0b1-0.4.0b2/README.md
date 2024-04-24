# Comparing `tmp/digitalhub_data-0.4.0b1.tar.gz` & `tmp/digitalhub_data-0.4.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub_data-0.4.0b1.tar", last modified: Fri Apr 19 08:58:53 2024, max compression
+gzip compressed data, was "digitalhub_data-0.4.0b2.tar", last modified: Wed Apr 24 07:52:12 2024, max compression
```

## Comparing `digitalhub_data-0.4.0b1.tar` & `digitalhub_data-0.4.0b2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:53.232596 digitalhub_data-0.4.0b1/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      946 2024-04-19 08:58:53.232596 digitalhub_data-0.4.0b1/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      468 2024-04-19 08:37:43.000000 digitalhub_data-0.4.0b1/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:53.228596 digitalhub_data-0.4.0b1/digitalhub_data/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      329 2024-04-19 08:14:48.000000 digitalhub_data-0.4.0b1/digitalhub_data/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:53.228596 digitalhub_data-0.4.0b1/digitalhub_data/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:56.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:53.228596 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:45.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3322 2024-04-19 08:14:48.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/builder.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6406 2024-04-19 08:14:48.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/crud.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:53.232596 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/entity/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-03-04 14:42:21.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/entity/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6489 2024-04-19 08:14:48.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/entity/_base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      180 2024-03-15 13:13:54.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/entity/dataitem.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      142 2024-03-04 15:16:25.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/entity/iceberg.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3134 2024-03-06 16:32:11.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/entity/table.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      582 2024-04-17 12:32:27.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1093 2024-04-08 13:12:06.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1418 2024-04-08 13:12:04.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      863 2024-03-15 12:04:24.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:53.232596 digitalhub_data-0.4.0b1/digitalhub_data/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-31 10:03:33.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6053 2024-04-19 08:14:48.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5909 2024-04-19 08:14:48.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      950 2024-02-15 10:15:41.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1050 2024-04-17 12:32:27.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:53.232596 digitalhub_data-0.4.0b1/digitalhub_data/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-22 14:51:32.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/runs/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      407 2024-03-08 13:54:39.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      351 2024-03-14 13:46:16.000000 digitalhub_data-0.4.0b1/digitalhub_data/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:53.232596 digitalhub_data-0.4.0b1/digitalhub_data/utils/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-29 10:07:05.000000 digitalhub_data-0.4.0b1/digitalhub_data/utils/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2440 2024-02-05 09:25:21.000000 digitalhub_data-0.4.0b1/digitalhub_data/utils/data_utils.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-19 08:58:53.232596 digitalhub_data-0.4.0b1/digitalhub_data.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      946 2024-04-19 08:58:53.000000 digitalhub_data-0.4.0b1/digitalhub_data.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1305 2024-04-19 08:58:53.000000 digitalhub_data-0.4.0b1/digitalhub_data.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-04-19 08:58:53.000000 digitalhub_data-0.4.0b1/digitalhub_data.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-19 08:58:53.000000 digitalhub_data-0.4.0b1/digitalhub_data.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-19 08:58:53.000000 digitalhub_data-0.4.0b1/digitalhub_data.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1056 2024-04-19 08:46:19.000000 digitalhub_data-0.4.0b1/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-04-19 08:58:53.232596 digitalhub_data-0.4.0b1/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:52:12.369888 digitalhub_data-0.4.0b2/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      946 2024-04-24 07:52:12.369888 digitalhub_data-0.4.0b2/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      468 2024-04-23 09:36:04.000000 digitalhub_data-0.4.0b2/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:52:12.361888 digitalhub_data-0.4.0b2/digitalhub_data/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      329 2024-04-19 08:14:48.000000 digitalhub_data-0.4.0b2/digitalhub_data/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:52:12.361888 digitalhub_data-0.4.0b2/digitalhub_data/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:56.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:52:12.365888 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:45.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3322 2024-04-23 09:36:04.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/builder.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6406 2024-04-19 08:14:48.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/crud.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:52:12.365888 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/entity/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-03-04 14:42:21.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/entity/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6489 2024-04-23 09:36:04.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/entity/_base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      180 2024-03-15 13:13:54.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/entity/dataitem.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      142 2024-03-04 15:16:25.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/entity/iceberg.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3042 2024-04-23 09:36:04.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/entity/table.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      582 2024-04-23 09:36:04.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1093 2024-04-08 13:12:06.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1418 2024-04-08 13:12:04.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      863 2024-03-15 12:04:24.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:52:12.365888 digitalhub_data-0.4.0b2/digitalhub_data/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-31 10:03:33.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6053 2024-04-19 08:14:48.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5909 2024-04-23 09:36:04.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      950 2024-02-15 10:15:41.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1050 2024-04-23 09:36:04.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:52:12.369888 digitalhub_data-0.4.0b2/digitalhub_data/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-22 14:51:32.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/runs/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      407 2024-03-08 13:54:39.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      351 2024-03-14 13:46:16.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:52:12.369888 digitalhub_data-0.4.0b2/digitalhub_data/utils/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-29 10:07:05.000000 digitalhub_data-0.4.0b2/digitalhub_data/utils/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2440 2024-02-05 09:25:21.000000 digitalhub_data-0.4.0b2/digitalhub_data/utils/data_utils.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:52:12.369888 digitalhub_data-0.4.0b2/digitalhub_data.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      946 2024-04-24 07:52:12.000000 digitalhub_data-0.4.0b2/digitalhub_data.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1305 2024-04-24 07:52:12.000000 digitalhub_data-0.4.0b2/digitalhub_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-04-24 07:52:12.000000 digitalhub_data-0.4.0b2/digitalhub_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-24 07:52:12.000000 digitalhub_data-0.4.0b2/digitalhub_data.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-24 07:52:12.000000 digitalhub_data-0.4.0b2/digitalhub_data.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1056 2024-04-23 13:34:39.000000 digitalhub_data-0.4.0b2/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-04-24 07:52:12.369888 digitalhub_data-0.4.0b2/setup.cfg
```

### Comparing `digitalhub_data-0.4.0b1/PKG-INFO` & `digitalhub_data-0.4.0b2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-data
-Version: 0.4.0b1
+Version: 0.4.0b2
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
```

### Comparing `digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/builder.py` & `digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/crud.py` & `digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/entity/_base.py` & `digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/entity/_base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/entity/table.py` & `digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/entity/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,17 +36,14 @@
             Keyword arguments.
 
         Returns
         -------
         pd.DataFrame
             Pandas DataFrame.
         """
-        if self.spec.path is None:
-            raise EntityError("Path is not specified.")
-
         store = get_store(self.spec.path)
         tmp_path = False
 
         # Download dataitem if not local
         if not self._check_local(self.spec.path):
             path = store.download(self.spec.path)
             tmp_path = True
```

### Comparing `digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/metadata.py` & `digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/models.py` & `digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/models.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/spec.py` & `digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b1/digitalhub_data/entities/dataitems/status.py` & `digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b1/digitalhub_data/entities/projects/crud.py` & `digitalhub_data-0.4.0b2/digitalhub_data/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b1/digitalhub_data/entities/projects/entity.py` & `digitalhub_data-0.4.0b2/digitalhub_data/entities/projects/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b1/digitalhub_data/entities/projects/spec.py` & `digitalhub_data-0.4.0b2/digitalhub_data/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b1/digitalhub_data/entities/registries.py` & `digitalhub_data-0.4.0b2/digitalhub_data/entities/registries.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b1/digitalhub_data/utils/data_utils.py` & `digitalhub_data-0.4.0b2/digitalhub_data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b1/digitalhub_data.egg-info/PKG-INFO` & `digitalhub_data-0.4.0b2/digitalhub_data.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-data
-Version: 0.4.0b1
+Version: 0.4.0b2
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
```

### Comparing `digitalhub_data-0.4.0b1/digitalhub_data.egg-info/SOURCES.txt` & `digitalhub_data-0.4.0b2/digitalhub_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b1/pyproject.toml` & `digitalhub_data-0.4.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-data"
-version = "0.4.0b1"
+version = "0.4.0b2"
 description = "Python SDK for DHCore"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -23,15 +23,15 @@
     "digitalhub-core~=0.3",
 ]
 
 [tool.setuptools.packages.find]
 exclude = ["modules*"]
 
 [tool.bumpver]
-current_version = "0.4.0b1"
+current_version = "0.4.0b2"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

