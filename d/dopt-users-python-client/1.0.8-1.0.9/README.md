# Comparing `tmp/dopt_users_python_client-1.0.8.tar.gz` & `tmp/dopt_users_python_client-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dopt_users_python_client-1.0.8.tar", max compression
+gzip compressed data, was "dopt_users_python_client-1.0.9.tar", max compression
```

## Comparing `dopt_users_python_client-1.0.8.tar` & `dopt_users_python_client-1.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1583 2023-10-02 18:22:32.285520 dopt_users_python_client-1.0.8/README.md
--rw-r--r--   0        0        0      403 2023-10-02 18:22:32.285520 dopt_users_python_client-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     1780 2023-10-02 18:22:32.285520 dopt_users_python_client-1.0.8/src/dopt/__init__.py
--rw-r--r--   0        0        0     1931 2023-10-02 18:22:32.285520 dopt_users_python_client-1.0.8/src/dopt/client.py
--rw-r--r--   0        0        0      519 2023-10-02 18:22:32.285520 dopt_users_python_client-1.0.8/src/dopt/core/__init__.py
--rw-r--r--   0        0        0      426 2023-10-02 18:22:32.285520 dopt_users_python_client-1.0.8/src/dopt/core/api_error.py
--rw-r--r--   0        0        0     1093 2023-10-02 18:22:32.285520 dopt_users_python_client-1.0.8/src/dopt/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2023-10-02 18:22:32.285520 dopt_users_python_client-1.0.8/src/dopt/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-10-02 18:22:32.285520 dopt_users_python_client-1.0.8/src/dopt/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2023-10-02 18:22:32.285520 dopt_users_python_client-1.0.8/src/dopt/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      155 2023-10-02 18:22:32.285520 dopt_users_python_client-1.0.8/src/dopt/environment.py
--rw-r--r--   0        0        0      292 2023-10-02 18:22:32.285520 dopt_users_python_client-1.0.8/src/dopt/errors/__init__.py
--rw-r--r--   0        0        0      330 2023-10-02 18:22:32.285520 dopt_users_python_client-1.0.8/src/dopt/errors/bad_request_error.py
--rw-r--r--   0        0        0      346 2023-10-02 18:22:32.285520 dopt_users_python_client-1.0.8/src/dopt/errors/internal_server_error.py
--rw-r--r--   0        0        0      337 2023-10-02 18:22:32.285520 dopt_users_python_client-1.0.8/src/dopt/errors/unauthorized_error.py
--rw-r--r--   0        0        0        0 2023-10-02 18:22:32.285520 dopt_users_python_client-1.0.8/src/dopt/py.typed
--rw-r--r--   0        0        0      124 2023-10-02 18:22:32.285520 dopt_users_python_client-1.0.8/src/dopt/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-10-02 18:22:32.285520 dopt_users_python_client-1.0.8/src/dopt/resources/groups/__init__.py
--rw-r--r--   0        0        0     4158 2023-10-02 18:22:32.285520 dopt_users_python_client-1.0.8/src/dopt/resources/groups/client.py
--rw-r--r--   0        0        0       65 2023-10-02 18:22:32.285520 dopt_users_python_client-1.0.8/src/dopt/resources/users/__init__.py
--rw-r--r--   0        0        0     8247 2023-10-02 18:22:32.285520 dopt_users_python_client-1.0.8/src/dopt/resources/users/client.py
--rw-r--r--   0        0        0     2194 2023-10-02 18:22:32.289520 dopt_users_python_client-1.0.8/src/dopt/types/__init__.py
--rw-r--r--   0        0        0      877 2023-10-02 18:22:32.289520 dopt_users_python_client-1.0.8/src/dopt/types/bad_request_error_response_body.py
--rw-r--r--   0        0        0      225 2023-10-02 18:22:32.289520 dopt_users_python_client-1.0.8/src/dopt/types/identify_batch_request_body.py
--rw-r--r--   0        0        0     1018 2023-10-02 18:22:32.289520 dopt_users_python_client-1.0.8/src/dopt/types/identify_batch_request_body_item.py
--rw-r--r--   0        0        0      850 2023-10-02 18:22:32.289520 dopt_users_python_client-1.0.8/src/dopt/types/identify_batch_request_body_item_groups_item.py
--rw-r--r--   0        0        0      789 2023-10-02 18:22:32.289520 dopt_users_python_client-1.0.8/src/dopt/types/identify_batch_response_body.py
--rw-r--r--   0        0        0      131 2023-10-02 18:22:32.289520 dopt_users_python_client-1.0.8/src/dopt/types/identify_request_body.py
--rw-r--r--   0        0        0      788 2023-10-02 18:22:32.289520 dopt_users_python_client-1.0.8/src/dopt/types/identify_request_params.py
--rw-r--r--   0        0        0      902 2023-10-02 18:22:32.289520 dopt_users_python_client-1.0.8/src/dopt/types/identify_segment_request_body.py
--rw-r--r--   0        0        0      967 2023-10-02 18:22:32.289520 dopt_users_python_client-1.0.8/src/dopt/types/identify_segment_request_body_group.py
--rw-r--r--   0        0        0      918 2023-10-02 18:22:32.289520 dopt_users_python_client-1.0.8/src/dopt/types/identify_segment_request_body_identify.py
--rw-r--r--   0        0        0      791 2023-10-02 18:22:32.289520 dopt_users_python_client-1.0.8/src/dopt/types/identify_segment_response_body.py
--rw-r--r--   0        0        0      845 2023-10-02 18:22:32.289520 dopt_users_python_client-1.0.8/src/dopt/types/identify_user_request_body_groups_item.py
--rw-r--r--   0        0        0      881 2023-10-02 18:22:32.289520 dopt_users_python_client-1.0.8/src/dopt/types/internal_server_error_response_body.py
--rw-r--r--   0        0        0      869 2023-10-02 18:22:32.289520 dopt_users_python_client-1.0.8/src/dopt/types/not_found_error_response_body.py
--rw-r--r--   0        0        0      897 2023-10-02 18:22:32.289520 dopt_users_python_client-1.0.8/src/dopt/types/segment_common.py
--rw-r--r--   0        0        0     1018 2023-10-02 18:22:32.289520 dopt_users_python_client-1.0.8/src/dopt/types/segment_group.py
--rw-r--r--   0        0        0      972 2023-10-02 18:22:32.289520 dopt_users_python_client-1.0.8/src/dopt/types/segment_identify.py
--rw-r--r--   0        0        0      874 2023-10-02 18:22:32.289520 dopt_users_python_client-1.0.8/src/dopt/types/timeout_error_response_body.py
--rw-r--r--   0        0        0      876 2023-10-02 18:22:32.289520 dopt_users_python_client-1.0.8/src/dopt/types/unauthorized_error_response_body.py
--rw-r--r--   0        0        0     2104 1970-01-01 00:00:00.000000 dopt_users_python_client-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1620 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/README.md
+-rw-r--r--   0        0        0      403 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1780 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/__init__.py
+-rw-r--r--   0        0        0     1931 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/client.py
+-rw-r--r--   0        0        0      519 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/core/api_error.py
+-rw-r--r--   0        0        0     1093 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      155 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/environment.py
+-rw-r--r--   0        0        0      292 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/errors/__init__.py
+-rw-r--r--   0        0        0      330 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/errors/bad_request_error.py
+-rw-r--r--   0        0        0      346 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/errors/internal_server_error.py
+-rw-r--r--   0        0        0      337 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/errors/unauthorized_error.py
+-rw-r--r--   0        0        0        0 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/py.typed
+-rw-r--r--   0        0        0      124 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/resources/groups/__init__.py
+-rw-r--r--   0        0        0     4158 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/resources/groups/client.py
+-rw-r--r--   0        0        0       65 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/resources/users/__init__.py
+-rw-r--r--   0        0        0     8247 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/resources/users/client.py
+-rw-r--r--   0        0        0     2194 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/types/__init__.py
+-rw-r--r--   0        0        0      877 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/types/bad_request_error_response_body.py
+-rw-r--r--   0        0        0      225 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/types/identify_batch_request_body.py
+-rw-r--r--   0        0        0     1018 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/types/identify_batch_request_body_item.py
+-rw-r--r--   0        0        0      850 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/types/identify_batch_request_body_item_groups_item.py
+-rw-r--r--   0        0        0      789 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/types/identify_batch_response_body.py
+-rw-r--r--   0        0        0      131 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/types/identify_request_body.py
+-rw-r--r--   0        0        0      788 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/types/identify_request_params.py
+-rw-r--r--   0        0        0      902 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/types/identify_segment_request_body.py
+-rw-r--r--   0        0        0      967 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/types/identify_segment_request_body_group.py
+-rw-r--r--   0        0        0      918 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/types/identify_segment_request_body_identify.py
+-rw-r--r--   0        0        0      791 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/types/identify_segment_response_body.py
+-rw-r--r--   0        0        0      845 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/types/identify_user_request_body_groups_item.py
+-rw-r--r--   0        0        0      881 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/types/internal_server_error_response_body.py
+-rw-r--r--   0        0        0      869 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/types/not_found_error_response_body.py
+-rw-r--r--   0        0        0      897 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/types/segment_common.py
+-rw-r--r--   0        0        0     1018 2024-04-24 19:19:41.670212 dopt_users_python_client-1.0.9/src/dopt/types/segment_group.py
+-rw-r--r--   0        0        0      972 2024-04-24 19:19:41.674212 dopt_users_python_client-1.0.9/src/dopt/types/segment_identify.py
+-rw-r--r--   0        0        0      874 2024-04-24 19:19:41.674212 dopt_users_python_client-1.0.9/src/dopt/types/timeout_error_response_body.py
+-rw-r--r--   0        0        0      876 2024-04-24 19:19:41.674212 dopt_users_python_client-1.0.9/src/dopt/types/unauthorized_error_response_body.py
+-rw-r--r--   0        0        0     2141 1970-01-01 00:00:00.000000 dopt_users_python_client-1.0.9/PKG-INFO
```

### Comparing `dopt_users_python_client-1.0.8/README.md` & `dopt_users_python_client-1.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Dopt Users Python Library
 
 [![pypi](https://img.shields.io/pypi/v/dopt-users-python-client.svg)](https://pypi.python.org/pypi/dopt-users-python-client)
-[![fern shield](https://img.shields.io/badge/%F0%9F%8C%BF-SDK%20generated%20by%20Fern-brightgreen)](https://github.com/fern-api/fern)
+[![fern shield](https://img.shields.io/badge/%F0%9F%8C%BF-SDK%20generated%20by%20Fern-brightgreen)](https://buildwithfern.com/?utm_source=dopt/users-python-client/readme)
 
 ## Installation
 
 Add this dependency to your project's build file:
 
 ```bash
 pip install dopt-users-python-client
```

### Comparing `dopt_users_python_client-1.0.8/src/dopt/__init__.py` & `dopt_users_python_client-1.0.9/src/dopt/__init__.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/client.py` & `dopt_users_python_client-1.0.9/src/dopt/client.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/core/__init__.py` & `dopt_users_python_client-1.0.9/src/dopt/core/__init__.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/core/client_wrapper.py` & `dopt_users_python_client-1.0.9/src/dopt/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self.api_key = api_key
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "dopt-users-python-client",
-            "X-Fern-SDK-Version": "1.0.8",
+            "X-Fern-SDK-Version": "1.0.9",
         }
         headers["x-api-key"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `dopt_users_python_client-1.0.8/src/dopt/core/datetime_utils.py` & `dopt_users_python_client-1.0.9/src/dopt/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/core/jsonable_encoder.py` & `dopt_users_python_client-1.0.9/src/dopt/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/resources/groups/client.py` & `dopt_users_python_client-1.0.9/src/dopt/resources/groups/client.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/resources/users/client.py` & `dopt_users_python_client-1.0.9/src/dopt/resources/users/client.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/types/__init__.py` & `dopt_users_python_client-1.0.9/src/dopt/types/__init__.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/types/bad_request_error_response_body.py` & `dopt_users_python_client-1.0.9/src/dopt/types/bad_request_error_response_body.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/types/identify_batch_request_body_item.py` & `dopt_users_python_client-1.0.9/src/dopt/types/identify_batch_request_body_item.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/types/identify_batch_request_body_item_groups_item.py` & `dopt_users_python_client-1.0.9/src/dopt/types/identify_batch_request_body_item_groups_item.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/types/identify_batch_response_body.py` & `dopt_users_python_client-1.0.9/src/dopt/types/identify_batch_response_body.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/types/identify_request_params.py` & `dopt_users_python_client-1.0.9/src/dopt/types/identify_request_params.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/types/identify_segment_request_body.py` & `dopt_users_python_client-1.0.9/src/dopt/types/identify_segment_request_body.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/types/identify_segment_request_body_group.py` & `dopt_users_python_client-1.0.9/src/dopt/types/identify_segment_request_body_group.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/types/identify_segment_request_body_identify.py` & `dopt_users_python_client-1.0.9/src/dopt/types/identify_segment_request_body_identify.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/types/identify_segment_response_body.py` & `dopt_users_python_client-1.0.9/src/dopt/types/identify_segment_response_body.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/types/identify_user_request_body_groups_item.py` & `dopt_users_python_client-1.0.9/src/dopt/types/identify_user_request_body_groups_item.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/types/internal_server_error_response_body.py` & `dopt_users_python_client-1.0.9/src/dopt/types/internal_server_error_response_body.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/types/not_found_error_response_body.py` & `dopt_users_python_client-1.0.9/src/dopt/types/not_found_error_response_body.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/types/segment_common.py` & `dopt_users_python_client-1.0.9/src/dopt/types/segment_common.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/types/segment_group.py` & `dopt_users_python_client-1.0.9/src/dopt/types/segment_group.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/types/segment_identify.py` & `dopt_users_python_client-1.0.9/src/dopt/types/segment_identify.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/types/timeout_error_response_body.py` & `dopt_users_python_client-1.0.9/src/dopt/types/timeout_error_response_body.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/src/dopt/types/unauthorized_error_response_body.py` & `dopt_users_python_client-1.0.9/src/dopt/types/unauthorized_error_response_body.py`

 * *Files identical despite different names*

### Comparing `dopt_users_python_client-1.0.8/PKG-INFO` & `dopt_users_python_client-1.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dopt-users-python-client
-Version: 1.0.8
+Version: 1.0.9
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -12,15 +12,15 @@
 Requires-Dist: httpx (>=0.21.2)
 Requires-Dist: pydantic (>=1.9.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Dopt Users Python Library
 
 [![pypi](https://img.shields.io/pypi/v/dopt-users-python-client.svg)](https://pypi.python.org/pypi/dopt-users-python-client)
-[![fern shield](https://img.shields.io/badge/%F0%9F%8C%BF-SDK%20generated%20by%20Fern-brightgreen)](https://github.com/fern-api/fern)
+[![fern shield](https://img.shields.io/badge/%F0%9F%8C%BF-SDK%20generated%20by%20Fern-brightgreen)](https://buildwithfern.com/?utm_source=dopt/users-python-client/readme)
 
 ## Installation
 
 Add this dependency to your project's build file:
 
 ```bash
 pip install dopt-users-python-client
```

