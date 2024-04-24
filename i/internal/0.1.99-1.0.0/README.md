# Comparing `tmp/internal-0.1.99.tar.gz` & `tmp/internal-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internal-0.1.99.tar", max compression
+gzip compressed data, was "internal-1.0.0.tar", max compression
```

## Comparing `internal-0.1.99.tar` & `internal-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776995 internal-0.1.99/README.md
--rw-r--r--   0        0        0      454 2024-04-23 08:00:52.571220 internal-0.1.99/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776948 internal-0.1.99/src/internal/__init__.py
--rw-r--r--   0        0        0     1715 2024-04-19 06:23:20.193365 internal-0.1.99/src/internal/base_config.py
--rw-r--r--   0        0        0     7662 2024-04-19 06:23:20.198194 internal-0.1.99/src/internal/base_factory.py
--rw-r--r--   0        0        0        0 2024-02-13 10:57:40.969610 internal-0.1.99/src/internal/common_enum/__init__.py
--rw-r--r--   0        0        0      142 2024-02-13 11:01:26.248123 internal-0.1.99/src/internal/common_enum/contact_type.py
--rw-r--r--   0        0        0      114 2024-03-19 08:47:41.966209 internal-0.1.99/src/internal/common_enum/event_type.py
--rw-r--r--   0        0        0      125 2024-02-13 11:01:26.244153 internal-0.1.99/src/internal/common_enum/operator_type.py
--rw-r--r--   0        0        0      511 2024-04-09 02:21:45.907592 internal-0.1.99/src/internal/common_enum/service_ticket_event_trigger_type.py
--rw-r--r--   0        0        0     1025 2024-01-28 03:58:24.810115 internal-0.1.99/src/internal/const.py
--rw-r--r--   0        0        0     2124 2024-03-23 09:50:05.593678 internal-0.1.99/src/internal/database.py
--rw-r--r--   0        0        0        0 2023-12-15 06:58:26.332564 internal-0.1.99/src/internal/exception/__init__.py
--rw-r--r--   0        0        0      363 2024-01-28 10:00:28.362441 internal-0.1.99/src/internal/exception/base_exception.py
--rw-r--r--   0        0        0     1651 2024-03-04 06:00:01.259424 internal-0.1.99/src/internal/exception/internal_exception.py
--rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564151 internal-0.1.99/src/internal/ext/__init__.py
--rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564243 internal-0.1.99/src/internal/ext/amazon/__init__.py
--rw-r--r--   0        0        0      834 2024-01-29 02:46:13.060361 internal-0.1.99/src/internal/ext/amazon/aws/__init__.py
--rw-r--r--   0        0        0      109 2023-12-11 01:32:53.463567 internal-0.1.99/src/internal/ext/amazon/aws/const.py
--rw-r--r--   0        0        0        0 2023-11-10 12:37:53.063137 internal-0.1.99/src/internal/http/__init__.py
--rw-r--r--   0        0        0     1675 2024-04-23 08:00:48.112326 internal-0.1.99/src/internal/http/requests.py
--rw-r--r--   0        0        0     1590 2024-03-26 06:14:32.915504 internal-0.1.99/src/internal/http/responses.py
--rw-r--r--   0        0        0        0 2023-12-29 03:03:59.978251 internal-0.1.99/src/internal/interface/__init__.py
--rw-r--r--   0        0        0      340 2024-01-28 03:32:05.468971 internal-0.1.99/src/internal/interface/base_interface.py
--rw-r--r--   0        0        0        0 2023-11-29 11:18:12.218216 internal-0.1.99/src/internal/model/__init__.py
--rw-r--r--   0        0        0     3002 2024-03-04 06:15:08.376296 internal-0.1.99/src/internal/model/base_model.py
--rw-r--r--   0        0        0     1493 2024-02-13 11:01:26.240348 internal-0.1.99/src/internal/model/operate.py
--rw-r--r--   0        0        0     1509 2024-04-08 11:20:32.745396 internal-0.1.99/src/internal/utils.py
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 internal-0.1.99/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776995 internal-1.0.0/README.md
+-rw-r--r--   0        0        0      453 2024-04-24 03:17:17.961755 internal-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776948 internal-1.0.0/src/internal/__init__.py
+-rw-r--r--   0        0        0     1715 2024-04-19 06:23:20.193365 internal-1.0.0/src/internal/base_config.py
+-rw-r--r--   0        0        0     7662 2024-04-19 06:23:20.198194 internal-1.0.0/src/internal/base_factory.py
+-rw-r--r--   0        0        0        0 2024-02-13 10:57:40.969610 internal-1.0.0/src/internal/common_enum/__init__.py
+-rw-r--r--   0        0        0      142 2024-02-13 11:01:26.248123 internal-1.0.0/src/internal/common_enum/contact_type.py
+-rw-r--r--   0        0        0      114 2024-03-19 08:47:41.966209 internal-1.0.0/src/internal/common_enum/event_type.py
+-rw-r--r--   0        0        0      125 2024-02-13 11:01:26.244153 internal-1.0.0/src/internal/common_enum/operator_type.py
+-rw-r--r--   0        0        0      511 2024-04-09 02:21:45.907592 internal-1.0.0/src/internal/common_enum/service_ticket_event_trigger_type.py
+-rw-r--r--   0        0        0     1025 2024-01-28 03:58:24.810115 internal-1.0.0/src/internal/const.py
+-rw-r--r--   0        0        0     2124 2024-03-23 09:50:05.593678 internal-1.0.0/src/internal/database.py
+-rw-r--r--   0        0        0        0 2023-12-15 06:58:26.332564 internal-1.0.0/src/internal/exception/__init__.py
+-rw-r--r--   0        0        0      363 2024-01-28 10:00:28.362441 internal-1.0.0/src/internal/exception/base_exception.py
+-rw-r--r--   0        0        0     1651 2024-03-04 06:00:01.259424 internal-1.0.0/src/internal/exception/internal_exception.py
+-rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564151 internal-1.0.0/src/internal/ext/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564243 internal-1.0.0/src/internal/ext/amazon/__init__.py
+-rw-r--r--   0        0        0      834 2024-01-29 02:46:13.060361 internal-1.0.0/src/internal/ext/amazon/aws/__init__.py
+-rw-r--r--   0        0        0      109 2023-12-11 01:32:53.463567 internal-1.0.0/src/internal/ext/amazon/aws/const.py
+-rw-r--r--   0        0        0        0 2023-11-10 12:37:53.063137 internal-1.0.0/src/internal/http/__init__.py
+-rw-r--r--   0        0        0     1675 2024-04-23 08:00:48.112326 internal-1.0.0/src/internal/http/requests.py
+-rw-r--r--   0        0        0     1670 2024-04-24 03:16:19.444561 internal-1.0.0/src/internal/http/responses.py
+-rw-r--r--   0        0        0        0 2023-12-29 03:03:59.978251 internal-1.0.0/src/internal/interface/__init__.py
+-rw-r--r--   0        0        0      340 2024-01-28 03:32:05.468971 internal-1.0.0/src/internal/interface/base_interface.py
+-rw-r--r--   0        0        0        0 2023-11-29 11:18:12.218216 internal-1.0.0/src/internal/model/__init__.py
+-rw-r--r--   0        0        0     3002 2024-03-04 06:15:08.376296 internal-1.0.0/src/internal/model/base_model.py
+-rw-r--r--   0        0        0     1493 2024-02-13 11:01:26.240348 internal-1.0.0/src/internal/model/operate.py
+-rw-r--r--   0        0        0     1509 2024-04-08 11:20:32.745396 internal-1.0.0/src/internal/utils.py
+-rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 internal-1.0.0/PKG-INFO
```

### Comparing `internal-0.1.99/src/internal/base_config.py` & `internal-1.0.0/src/internal/base_config.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.99/src/internal/base_factory.py` & `internal-1.0.0/src/internal/base_factory.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.99/src/internal/const.py` & `internal-1.0.0/src/internal/const.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.99/src/internal/database.py` & `internal-1.0.0/src/internal/database.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.99/src/internal/exception/internal_exception.py` & `internal-1.0.0/src/internal/exception/internal_exception.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.99/src/internal/ext/amazon/aws/__init__.py` & `internal-1.0.0/src/internal/ext/amazon/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.99/src/internal/http/requests.py` & `internal-1.0.0/src/internal/http/requests.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.99/src/internal/http/responses.py` & `internal-1.0.0/src/internal/http/responses.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import httpx
 
 from fastapi import status
 from fastapi.responses import JSONResponse
+from fastapi.encoders import jsonable_encoder
 from beanie import Document, Link
 
 
 async def async_response(data=None, message=None, code=None, page_no=None, total_num=None, page_size=None,
                          status_code=status.HTTP_200_OK):
     def _serialize(data):
         if issubclass(type(data), Document):
@@ -23,14 +24,15 @@
                         data[field_name] = data[field_name]["id"]
         return data
 
     if isinstance(data, httpx.Response):
         return JSONResponse(status_code=data.status_code, content=data.json())
 
     ret = {}
+    data = jsonable_encoder(data)
     if isinstance(data, list):
         data = [_serialize(d) for d in data]
     else:
         data = _serialize(data)
 
     ret['code'] = code or "ok"
```

### Comparing `internal-0.1.99/src/internal/model/base_model.py` & `internal-1.0.0/src/internal/model/base_model.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.99/src/internal/model/operate.py` & `internal-1.0.0/src/internal/model/operate.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.99/src/internal/utils.py` & `internal-1.0.0/src/internal/utils.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.99/PKG-INFO` & `internal-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internal
-Version: 0.1.99
+Version: 1.0.0
 Summary: 
 Author: Ray
 Author-email: ray@cruisys.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

