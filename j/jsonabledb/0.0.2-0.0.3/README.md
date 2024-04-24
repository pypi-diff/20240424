# Comparing `tmp/jsonabledb-0.0.2.tar.gz` & `tmp/jsonabledb-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonabledb-0.0.2.tar", max compression
+gzip compressed data, was "jsonabledb-0.0.3.tar", max compression
```

## Comparing `jsonabledb-0.0.2.tar` & `jsonabledb-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1494 2024-04-20 23:35:29.430414 jsonabledb-0.0.2/LICENSE
--rw-r--r--   0        0        0     1339 2024-04-24 13:42:01.273554 jsonabledb-0.0.2/README.md
--rw-r--r--   0        0        0      192 2024-04-24 13:13:51.280920 jsonabledb-0.0.2/jsonable/__init__.py
--rw-r--r--   0        0        0    15689 2024-04-24 13:32:41.492328 jsonabledb-0.0.2/jsonable/jsonable.py
--rw-r--r--   0        0        0      497 2024-04-24 13:14:15.918490 jsonabledb-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2116 1970-01-01 00:00:00.000000 jsonabledb-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1494 2024-04-20 23:35:29.430414 jsonabledb-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1340 2024-04-24 13:56:27.788004 jsonabledb-0.0.3/README.md
+-rw-r--r--   0        0        0      192 2024-04-24 14:07:55.809377 jsonabledb-0.0.3/jsonable/__init__.py
+-rw-r--r--   0        0        0    15689 2024-04-24 14:07:31.774715 jsonabledb-0.0.3/jsonable/jsonable.py
+-rw-r--r--   0        0        0      497 2024-04-24 14:08:14.940953 jsonabledb-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2117 1970-01-01 00:00:00.000000 jsonabledb-0.0.3/PKG-INFO
```

### Comparing `jsonabledb-0.0.2/LICENSE` & `jsonabledb-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonabledb-0.0.2/README.md` & `jsonabledb-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 ## Quickstart
 
 Get your documents prepared
 
 ```python
 documents = [
-	{...},
+  {...},
   {...},
   ...
 ]
 ```
```

### Comparing `jsonabledb-0.0.2/jsonable/jsonable.py` & `jsonabledb-0.0.3/jsonable/jsonable.py`

 * *Files identical despite different names*

### Comparing `jsonabledb-0.0.2/PKG-INFO` & `jsonabledb-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonabledb
-Version: 0.0.2
+Version: 0.0.3
 Summary: A lightweight document-oriented database based on JSON
 Home-page: https://pypi.org/project/jsonabledb
 License: BSD-3-Clause
 Author: Yi ZHANG
 Author-email: yizhang.dev@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: BSD License
@@ -36,15 +36,15 @@
 
 ## Quickstart
 
 Get your documents prepared
 
 ```python
 documents = [
-	{...},
+  {...},
   {...},
   ...
 ]
 ```
```

