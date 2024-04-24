# Comparing `tmp/chess2vec-0.3.5.tar.gz` & `tmp/chess2vec-0.3.5b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.3.5.tar", max compression
+gzip compressed data, was "chess2vec-0.3.5b1.tar", max compression
```

## Comparing `chess2vec-0.3.5.tar` & `chess2vec-0.3.5b1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-20 10:13:12.779868 chess2vec-0.3.5/README.md
--rw-r--r--   0        0        0     1659 2024-04-24 17:02:22.226590 chess2vec-0.3.5/chess2vec/__init__.py
--rw-r--r--   0        0        0     2371 2024-04-24 16:53:32.576893 chess2vec-0.3.5/chess2vec/components.py
--rw-r--r--   0        0        0      287 2024-04-23 21:18:28.472128 chess2vec-0.3.5/chess2vec/pgn.py
--rw-r--r--   0        0        0      701 2024-04-24 17:02:17.210041 chess2vec-0.3.5/chess2vec/utils/__init__.py
--rw-r--r--   0        0        0      583 2024-04-20 10:13:12.779868 chess2vec-0.3.5/chess2vec/utils/vector.py
--rw-r--r--   0        0        0      374 2024-04-24 17:02:27.823127 chess2vec-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 chess2vec-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 10:13:12.779868 chess2vec-0.3.5b1/README.md
+-rw-r--r--   0        0        0     1298 2024-04-24 17:10:34.155651 chess2vec-0.3.5b1/chess2vec/__init__.py
+-rw-r--r--   0        0        0     2371 2024-04-24 17:08:34.148985 chess2vec-0.3.5b1/chess2vec/components.py
+-rw-r--r--   0        0        0      287 2024-04-23 21:18:28.472128 chess2vec-0.3.5b1/chess2vec/pgn.py
+-rw-r--r--   0        0        0      701 2024-04-24 17:02:17.210041 chess2vec-0.3.5b1/chess2vec/utils/__init__.py
+-rw-r--r--   0        0        0      583 2024-04-20 10:13:12.779868 chess2vec-0.3.5b1/chess2vec/utils/vector.py
+-rw-r--r--   0        0        0      376 2024-04-24 17:10:45.872343 chess2vec-0.3.5b1/pyproject.toml
+-rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 chess2vec-0.3.5b1/PKG-INFO
```

### Comparing `chess2vec-0.3.5/chess2vec/components.py` & `chess2vec-0.3.5b1/chess2vec/components.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.3.5/chess2vec/utils/__init__.py` & `chess2vec-0.3.5b1/chess2vec/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.3.5/chess2vec/utils/vector.py` & `chess2vec-0.3.5b1/chess2vec/utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.3.5/PKG-INFO` & `chess2vec-0.3.5b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.3.5
+Version: 0.3.5b1
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

