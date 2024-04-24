# Comparing `tmp/jaycopilot_client-0.1.1.tar.gz` & `tmp/jaycopilot_client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaycopilot_client-0.1.1.tar", max compression
+gzip compressed data, was "jaycopilot_client-0.1.2.tar", max compression
```

## Comparing `jaycopilot_client-0.1.1.tar` & `jaycopilot_client-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-24 10:34:45.943395 jaycopilot_client-0.1.1/jaycopilot_client/__init__.py
--rw-r--r--   0        0        0     6736 2024-04-24 10:52:01.772429 jaycopilot_client-0.1.1/jaycopilot_client/client.py
--rw-r--r--   0        0        0      552 2024-04-23 15:39:04.921668 jaycopilot_client-0.1.1/jaycopilot_client/config.py
--rw-r--r--   0        0        0      747 2024-04-16 13:46:17.682638 jaycopilot_client-0.1.1/jaycopilot_client/exception/__pycache__/client_exception.cpython-310.pyc
--rw-r--r--   0        0        0      291 2024-04-03 07:43:14.679363 jaycopilot_client-0.1.1/jaycopilot_client/exception/client_exception.py
--rw-r--r--   0        0        0      220 2024-04-23 10:22:43.551951 jaycopilot_client-0.1.1/jaycopilot_client/schemas.py
--rw-r--r--   0        0        0      459 2024-04-24 10:51:26.704575 jaycopilot_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       17 2024-04-24 10:04:36.490531 jaycopilot_client-0.1.1/README.md
--rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 jaycopilot_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-24 10:34:45.943395 jaycopilot_client-0.1.2/jaycopilot_client/__init__.py
+-rw-r--r--   0        0        0     6736 2024-04-24 10:52:01.772429 jaycopilot_client-0.1.2/jaycopilot_client/client.py
+-rw-r--r--   0        0        0      283 2024-04-24 11:13:29.937743 jaycopilot_client-0.1.2/jaycopilot_client/config.py
+-rw-r--r--   0        0        0      747 2024-04-16 13:46:17.682638 jaycopilot_client-0.1.2/jaycopilot_client/exception/__pycache__/client_exception.cpython-310.pyc
+-rw-r--r--   0        0        0      291 2024-04-03 07:43:14.679363 jaycopilot_client-0.1.2/jaycopilot_client/exception/client_exception.py
+-rw-r--r--   0        0        0      220 2024-04-24 11:12:02.508720 jaycopilot_client-0.1.2/jaycopilot_client/schemas.py
+-rw-r--r--   0        0        0      459 2024-04-24 11:13:36.580552 jaycopilot_client-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       17 2024-04-24 10:04:36.490531 jaycopilot_client-0.1.2/README.md
+-rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 jaycopilot_client-0.1.2/PKG-INFO
```

### Comparing `jaycopilot_client-0.1.1/jaycopilot_client/client.py` & `jaycopilot_client-0.1.2/jaycopilot_client/client.py`

 * *Files identical despite different names*

### Comparing `jaycopilot_client-0.1.1/jaycopilot_client/exception/__pycache__/client_exception.cpython-310.pyc` & `jaycopilot_client-0.1.2/jaycopilot_client/exception/__pycache__/client_exception.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jaycopilot_client-0.1.1/PKG-INFO` & `jaycopilot_client-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaycopilot_client
-Version: 0.1.1
+Version: 0.1.2
 Summary: Request client to Jay Copilot
 Author: Самигулин Тимур
 Author-email: samigulint@sovcombank.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

