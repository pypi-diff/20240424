# Comparing `tmp/langroid_client-0.1.8.tar.gz` & `tmp/langroid_client-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langroid_client-0.1.8.tar", max compression
+gzip compressed data, was "langroid_client-0.1.9.tar", max compression
```

## Comparing `langroid_client-0.1.8.tar` & `langroid_client-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       61 2024-03-04 16:08:23.434167 langroid_client-0.1.8/README.md
--rw-r--r--   0        0        0       34 2024-03-04 14:56:03.104134 langroid_client-0.1.8/langroid_client/__init__.py
--rw-r--r--   0        0        0     3300 2024-03-24 23:03:13.120151 langroid_client-0.1.8/langroid_client/client.py
--rw-r--r--   0        0        0      498 2024-03-24 23:05:40.188398 langroid_client-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 langroid_client-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       61 2024-03-04 16:08:23.434167 langroid_client-0.1.9/README.md
+-rw-r--r--   0        0        0       34 2024-03-04 14:56:03.104134 langroid_client-0.1.9/langroid_client/__init__.py
+-rw-r--r--   0        0        0     6941 2024-04-23 23:11:13.170814 langroid_client-0.1.9/langroid_client/client.py
+-rw-r--r--   0        0        0      498 2024-04-24 14:32:51.396701 langroid_client-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 langroid_client-0.1.9/PKG-INFO
```

### Comparing `langroid_client-0.1.8/PKG-INFO` & `langroid_client-0.1.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langroid-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Prasad Chalasani
 Author-email: pchalasani@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
```

