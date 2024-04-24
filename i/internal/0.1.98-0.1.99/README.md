# Comparing `tmp/internal-0.1.98.tar.gz` & `tmp/internal-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internal-0.1.98.tar", max compression
+gzip compressed data, was "internal-0.1.99.tar", max compression
```

## Comparing `internal-0.1.98.tar` & `internal-0.1.99.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776995 internal-0.1.98/README.md
--rw-r--r--   0        0        0      454 2024-04-19 06:23:20.200647 internal-0.1.98/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776948 internal-0.1.98/src/internal/__init__.py
--rw-r--r--   0        0        0     1715 2024-04-19 06:23:20.193365 internal-0.1.98/src/internal/base_config.py
--rw-r--r--   0        0        0     7662 2024-04-19 06:23:20.198194 internal-0.1.98/src/internal/base_factory.py
--rw-r--r--   0        0        0        0 2024-02-13 10:57:40.969610 internal-0.1.98/src/internal/common_enum/__init__.py
--rw-r--r--   0        0        0      142 2024-02-13 11:01:26.248123 internal-0.1.98/src/internal/common_enum/contact_type.py
--rw-r--r--   0        0        0      114 2024-03-19 08:47:41.966209 internal-0.1.98/src/internal/common_enum/event_type.py
--rw-r--r--   0        0        0      125 2024-02-13 11:01:26.244153 internal-0.1.98/src/internal/common_enum/operator_type.py
--rw-r--r--   0        0        0      511 2024-04-09 02:21:45.907592 internal-0.1.98/src/internal/common_enum/service_ticket_event_trigger_type.py
--rw-r--r--   0        0        0     1025 2024-01-28 03:58:24.810115 internal-0.1.98/src/internal/const.py
--rw-r--r--   0        0        0     2124 2024-03-23 09:50:05.593678 internal-0.1.98/src/internal/database.py
--rw-r--r--   0        0        0        0 2023-12-15 06:58:26.332564 internal-0.1.98/src/internal/exception/__init__.py
--rw-r--r--   0        0        0      363 2024-01-28 10:00:28.362441 internal-0.1.98/src/internal/exception/base_exception.py
--rw-r--r--   0        0        0     1651 2024-03-04 06:00:01.259424 internal-0.1.98/src/internal/exception/internal_exception.py
--rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564151 internal-0.1.98/src/internal/ext/__init__.py
--rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564243 internal-0.1.98/src/internal/ext/amazon/__init__.py
--rw-r--r--   0        0        0      834 2024-01-29 02:46:13.060361 internal-0.1.98/src/internal/ext/amazon/aws/__init__.py
--rw-r--r--   0        0        0      109 2023-12-11 01:32:53.463567 internal-0.1.98/src/internal/ext/amazon/aws/const.py
--rw-r--r--   0        0        0        0 2023-11-10 12:37:53.063137 internal-0.1.98/src/internal/http/__init__.py
--rw-r--r--   0        0        0     1415 2024-02-07 01:42:57.122123 internal-0.1.98/src/internal/http/requests.py
--rw-r--r--   0        0        0     1590 2024-03-26 06:14:32.915504 internal-0.1.98/src/internal/http/responses.py
--rw-r--r--   0        0        0        0 2023-12-29 03:03:59.978251 internal-0.1.98/src/internal/interface/__init__.py
--rw-r--r--   0        0        0      340 2024-01-28 03:32:05.468971 internal-0.1.98/src/internal/interface/base_interface.py
--rw-r--r--   0        0        0        0 2023-11-29 11:18:12.218216 internal-0.1.98/src/internal/model/__init__.py
--rw-r--r--   0        0        0     3002 2024-03-04 06:15:08.376296 internal-0.1.98/src/internal/model/base_model.py
--rw-r--r--   0        0        0     1493 2024-02-13 11:01:26.240348 internal-0.1.98/src/internal/model/operate.py
--rw-r--r--   0        0        0     1509 2024-04-08 11:20:32.745396 internal-0.1.98/src/internal/utils.py
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 internal-0.1.98/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776995 internal-0.1.99/README.md
+-rw-r--r--   0        0        0      454 2024-04-23 08:00:52.571220 internal-0.1.99/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776948 internal-0.1.99/src/internal/__init__.py
+-rw-r--r--   0        0        0     1715 2024-04-19 06:23:20.193365 internal-0.1.99/src/internal/base_config.py
+-rw-r--r--   0        0        0     7662 2024-04-19 06:23:20.198194 internal-0.1.99/src/internal/base_factory.py
+-rw-r--r--   0        0        0        0 2024-02-13 10:57:40.969610 internal-0.1.99/src/internal/common_enum/__init__.py
+-rw-r--r--   0        0        0      142 2024-02-13 11:01:26.248123 internal-0.1.99/src/internal/common_enum/contact_type.py
+-rw-r--r--   0        0        0      114 2024-03-19 08:47:41.966209 internal-0.1.99/src/internal/common_enum/event_type.py
+-rw-r--r--   0        0        0      125 2024-02-13 11:01:26.244153 internal-0.1.99/src/internal/common_enum/operator_type.py
+-rw-r--r--   0        0        0      511 2024-04-09 02:21:45.907592 internal-0.1.99/src/internal/common_enum/service_ticket_event_trigger_type.py
+-rw-r--r--   0        0        0     1025 2024-01-28 03:58:24.810115 internal-0.1.99/src/internal/const.py
+-rw-r--r--   0        0        0     2124 2024-03-23 09:50:05.593678 internal-0.1.99/src/internal/database.py
+-rw-r--r--   0        0        0        0 2023-12-15 06:58:26.332564 internal-0.1.99/src/internal/exception/__init__.py
+-rw-r--r--   0        0        0      363 2024-01-28 10:00:28.362441 internal-0.1.99/src/internal/exception/base_exception.py
+-rw-r--r--   0        0        0     1651 2024-03-04 06:00:01.259424 internal-0.1.99/src/internal/exception/internal_exception.py
+-rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564151 internal-0.1.99/src/internal/ext/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564243 internal-0.1.99/src/internal/ext/amazon/__init__.py
+-rw-r--r--   0        0        0      834 2024-01-29 02:46:13.060361 internal-0.1.99/src/internal/ext/amazon/aws/__init__.py
+-rw-r--r--   0        0        0      109 2023-12-11 01:32:53.463567 internal-0.1.99/src/internal/ext/amazon/aws/const.py
+-rw-r--r--   0        0        0        0 2023-11-10 12:37:53.063137 internal-0.1.99/src/internal/http/__init__.py
+-rw-r--r--   0        0        0     1675 2024-04-23 08:00:48.112326 internal-0.1.99/src/internal/http/requests.py
+-rw-r--r--   0        0        0     1590 2024-03-26 06:14:32.915504 internal-0.1.99/src/internal/http/responses.py
+-rw-r--r--   0        0        0        0 2023-12-29 03:03:59.978251 internal-0.1.99/src/internal/interface/__init__.py
+-rw-r--r--   0        0        0      340 2024-01-28 03:32:05.468971 internal-0.1.99/src/internal/interface/base_interface.py
+-rw-r--r--   0        0        0        0 2023-11-29 11:18:12.218216 internal-0.1.99/src/internal/model/__init__.py
+-rw-r--r--   0        0        0     3002 2024-03-04 06:15:08.376296 internal-0.1.99/src/internal/model/base_model.py
+-rw-r--r--   0        0        0     1493 2024-02-13 11:01:26.240348 internal-0.1.99/src/internal/model/operate.py
+-rw-r--r--   0        0        0     1509 2024-04-08 11:20:32.745396 internal-0.1.99/src/internal/utils.py
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 internal-0.1.99/PKG-INFO
```

### Comparing `internal-0.1.98/src/internal/base_config.py` & `internal-0.1.99/src/internal/base_config.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.98/src/internal/base_factory.py` & `internal-0.1.99/src/internal/base_factory.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.98/src/internal/const.py` & `internal-0.1.99/src/internal/const.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.98/src/internal/database.py` & `internal-0.1.99/src/internal/database.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.98/src/internal/exception/internal_exception.py` & `internal-0.1.99/src/internal/exception/internal_exception.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.98/src/internal/ext/amazon/aws/__init__.py` & `internal-0.1.99/src/internal/ext/amazon/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.98/src/internal/http/requests.py` & `internal-0.1.99/src/internal/http/requests.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,18 @@
         else:
             kwargs["headers"] = {
                 "Authorization": f"Bearer {current_user.get('access_token')}"
             }
 
     try:
         async with httpx.AsyncClient(timeout=timeout, verify=False) as client:
+            app.state.logger.info(f"async_request() request, url: {url}, method: {method}, kwargs: {kwargs}")
             response = await client.request(method, url, **kwargs)
+            app.state.logger.info(
+                f"async_request() response, url: {url}, method: {method}, kwargs: {kwargs}, response: {response}")
             return response
     except httpx.TimeoutException as exc:
         app.state.logger.warn(
             f"async_request(), TimeoutException, exc: {exc}, url: {url}, method: {method}, kwargs: {kwargs}")
         raise GatewayTimeoutException(str(exc))
     except Exception as exc:
         app.state.logger.warn(
```

### Comparing `internal-0.1.98/src/internal/http/responses.py` & `internal-0.1.99/src/internal/http/responses.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.98/src/internal/model/base_model.py` & `internal-0.1.99/src/internal/model/base_model.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.98/src/internal/model/operate.py` & `internal-0.1.99/src/internal/model/operate.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.98/src/internal/utils.py` & `internal-0.1.99/src/internal/utils.py`

 * *Files identical despite different names*

### Comparing `internal-0.1.98/PKG-INFO` & `internal-0.1.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internal
-Version: 0.1.98
+Version: 0.1.99
 Summary: 
 Author: Ray
 Author-email: ray@cruisys.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

