# Comparing `tmp/jaycopilot_client-0.1.0.tar.gz` & `tmp/jaycopilot_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaycopilot_client-0.1.0.tar", max compression
+gzip compressed data, was "jaycopilot_client-0.1.1.tar", max compression
```

## Comparing `jaycopilot_client-0.1.0.tar` & `jaycopilot_client-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-24 10:34:45.943395 jaycopilot_client-0.1.0/jaycopilot_client/__init__.py
--rw-r--r--   0        0        0     6129 2024-04-23 15:41:07.337332 jaycopilot_client-0.1.0/jaycopilot_client/app/__pycache__/client.cpython-310.pyc
--rw-r--r--   0        0        0      401 2024-04-23 15:39:08.163998 jaycopilot_client-0.1.0/jaycopilot_client/app/__pycache__/config.cpython-310.pyc
--rw-r--r--   0        0        0      524 2024-04-23 14:46:51.199391 jaycopilot_client-0.1.0/jaycopilot_client/app/__pycache__/schemas.cpython-310.pyc
--rw-r--r--   0        0        0     6703 2024-04-23 15:57:51.005805 jaycopilot_client-0.1.0/jaycopilot_client/app/client.py
--rw-r--r--   0        0        0      552 2024-04-23 15:39:04.921668 jaycopilot_client-0.1.0/jaycopilot_client/app/config.py
--rw-r--r--   0        0        0      747 2024-04-16 13:46:17.682638 jaycopilot_client-0.1.0/jaycopilot_client/app/exception/__pycache__/client_exception.cpython-310.pyc
--rw-r--r--   0        0        0      291 2024-04-03 07:43:14.679363 jaycopilot_client-0.1.0/jaycopilot_client/app/exception/client_exception.py
--rw-r--r--   0        0        0      220 2024-04-23 10:22:43.551951 jaycopilot_client-0.1.0/jaycopilot_client/app/schemas.py
--rw-r--r--   0        0        0      459 2024-04-24 10:33:20.877276 jaycopilot_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       17 2024-04-24 10:04:36.490531 jaycopilot_client-0.1.0/README.md
--rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 jaycopilot_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-24 10:34:45.943395 jaycopilot_client-0.1.1/jaycopilot_client/__init__.py
+-rw-r--r--   0        0        0     6736 2024-04-24 10:52:01.772429 jaycopilot_client-0.1.1/jaycopilot_client/client.py
+-rw-r--r--   0        0        0      552 2024-04-23 15:39:04.921668 jaycopilot_client-0.1.1/jaycopilot_client/config.py
+-rw-r--r--   0        0        0      747 2024-04-16 13:46:17.682638 jaycopilot_client-0.1.1/jaycopilot_client/exception/__pycache__/client_exception.cpython-310.pyc
+-rw-r--r--   0        0        0      291 2024-04-03 07:43:14.679363 jaycopilot_client-0.1.1/jaycopilot_client/exception/client_exception.py
+-rw-r--r--   0        0        0      220 2024-04-23 10:22:43.551951 jaycopilot_client-0.1.1/jaycopilot_client/schemas.py
+-rw-r--r--   0        0        0      459 2024-04-24 10:51:26.704575 jaycopilot_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       17 2024-04-24 10:04:36.490531 jaycopilot_client-0.1.1/README.md
+-rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 jaycopilot_client-0.1.1/PKG-INFO
```

### Comparing `jaycopilot_client-0.1.0/jaycopilot_client/app/client.py` & `jaycopilot_client-0.1.1/jaycopilot_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import Any
+
 import requests
+from config import JAY_COPILOT_API_KEY
+from exception.client_exception import (ApiServiceError, CantCreateApplication,
+                                        CantCreateDialogWithApp)
 from pydantic import HttpUrl
-from app.exception.client_exception import ApiServiceError, CantCreateApplication, CantCreateDialogWithApp
-from app.config import JAY_COPILOT_API_KEY
-from app.schemas import AppType
+from schemas import AppType
 
 
 class JayCopilot():
 
     HEADERS = {
         "X-API-KEY": JAY_COPILOT_API_KEY,
         "Content-Type": "application/json",
```

### Comparing `jaycopilot_client-0.1.0/jaycopilot_client/app/config.py` & `jaycopilot_client-0.1.1/jaycopilot_client/config.py`

 * *Files identical despite different names*

### Comparing `jaycopilot_client-0.1.0/jaycopilot_client/app/exception/__pycache__/client_exception.cpython-310.pyc` & `jaycopilot_client-0.1.1/jaycopilot_client/exception/__pycache__/client_exception.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jaycopilot_client-0.1.0/PKG-INFO` & `jaycopilot_client-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaycopilot_client
-Version: 0.1.0
+Version: 0.1.1
 Summary: Request client to Jay Copilot
 Author: Самигулин Тимур
 Author-email: samigulint@sovcombank.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

