# Comparing `tmp/tilebox_grpc-0.9.0.tar.gz` & `tmp/tilebox_grpc-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tilebox_grpc-0.9.0.tar", last modified: Wed Mar 13 13:24:47 2024, max compression
+gzip compressed data, was "tilebox_grpc-0.9.1.tar", last modified: Thu Mar 14 15:00:33 2024, max compression
```

## Comparing `tilebox_grpc-0.9.0.tar` & `tilebox_grpc-0.9.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:24:47.367507 tilebox_grpc-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-13 13:24:47.367507 tilebox_grpc-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-13 13:24:03.283242 tilebox_grpc-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:24:47.363507 tilebox_grpc-0.9.0/_tilebox/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:24:47.367507 tilebox_grpc-0.9.0/_tilebox/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 13:24:03.283242 tilebox_grpc-0.9.0/_tilebox/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:24:47.367507 tilebox_grpc-0.9.0/_tilebox/grpc/aio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 13:24:03.283242 tilebox_grpc-0.9.0/_tilebox/grpc/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-03-13 13:24:03.283242 tilebox_grpc-0.9.0/_tilebox/grpc/aio/producer_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-03-13 13:24:03.283242 tilebox_grpc-0.9.0/_tilebox/grpc/aio/syncify.py
--rw-r--r--   0 runner    (1001) docker     (127)     6133 2024-03-13 13:24:03.283242 tilebox_grpc-0.9.0/_tilebox/grpc/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-13 13:24:03.283242 tilebox_grpc-0.9.0/_tilebox/grpc/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-13 13:24:47.367507 tilebox_grpc-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:00:33.691332 tilebox_grpc-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-14 15:00:33.691332 tilebox_grpc-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-14 14:59:43.431642 tilebox_grpc-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:00:33.687332 tilebox_grpc-0.9.1/_tilebox/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:00:33.687332 tilebox_grpc-0.9.1/_tilebox/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 14:59:43.431642 tilebox_grpc-0.9.1/_tilebox/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:00:33.687332 tilebox_grpc-0.9.1/_tilebox/grpc/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 14:59:43.431642 tilebox_grpc-0.9.1/_tilebox/grpc/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-03-14 14:59:43.431642 tilebox_grpc-0.9.1/_tilebox/grpc/aio/producer_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-03-14 14:59:43.431642 tilebox_grpc-0.9.1/_tilebox/grpc/aio/syncify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6133 2024-03-14 14:59:43.431642 tilebox_grpc-0.9.1/_tilebox/grpc/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-14 14:59:43.431642 tilebox_grpc-0.9.1/_tilebox/grpc/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-14 15:00:33.691332 tilebox_grpc-0.9.1/pyproject.toml
```

### Comparing `tilebox_grpc-0.9.0/PKG-INFO` & `tilebox_grpc-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tilebox-grpc
-Version: 0.9.0
+Version: 0.9.1
 Summary: GRPC / Protocol Buffers functions for Tilebox
 Author: Tilebox
 Author-email: support@tilebox.com
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `tilebox_grpc-0.9.0/_tilebox/grpc/aio/producer_consumer.py` & `tilebox_grpc-0.9.1/_tilebox/grpc/aio/producer_consumer.py`

 * *Files identical despite different names*

### Comparing `tilebox_grpc-0.9.0/_tilebox/grpc/aio/syncify.py` & `tilebox_grpc-0.9.1/_tilebox/grpc/aio/syncify.py`

 * *Files identical despite different names*

### Comparing `tilebox_grpc-0.9.0/_tilebox/grpc/channel.py` & `tilebox_grpc-0.9.1/_tilebox/grpc/channel.py`

 * *Files identical despite different names*

### Comparing `tilebox_grpc-0.9.0/_tilebox/grpc/error.py` & `tilebox_grpc-0.9.1/_tilebox/grpc/error.py`

 * *Files identical despite different names*

### Comparing `tilebox_grpc-0.9.0/pyproject.toml` & `tilebox_grpc-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tilebox-grpc"
-version = "0.9.0"
+version = "0.9.1"
 description = "GRPC / Protocol Buffers functions for Tilebox"
 authors = [
     "Tilebox <support@tilebox.com>",
 ]
 readme = "README.md"
 packages = [
     { include = "_tilebox" },
```

