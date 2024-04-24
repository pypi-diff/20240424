# Comparing `tmp/waylay_sdk_storage-0.4.1.20240423.tar.gz` & `tmp/waylay-sdk-storage-0.4.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk_storage-0.4.1.20240423.tar", last modified: Tue Apr 23 16:14:44 2024, max compression
+gzip compressed data, was "waylay-sdk-storage-0.4.1b1.tar", last modified: Thu Mar 28 13:38:29 2024, max compression
```

## Comparing `waylay_sdk_storage-0.4.1.20240423.tar` & `waylay-sdk-storage-0.4.1b1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:14:44.956015 waylay_sdk_storage-0.4.1.20240423/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-23 16:14:40.000000 waylay_sdk_storage-0.4.1.20240423/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-23 16:14:44.956015 waylay_sdk_storage-0.4.1.20240423/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-23 16:14:40.000000 waylay_sdk_storage-0.4.1.20240423/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-23 16:14:40.000000 waylay_sdk_storage-0.4.1.20240423/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:14:44.956015 waylay_sdk_storage-0.4.1.20240423/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:14:44.948015 waylay_sdk_storage-0.4.1.20240423/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:14:44.948015 waylay_sdk_storage-0.4.1.20240423/src/waylay/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:14:44.948015 waylay_sdk_storage-0.4.1.20240423/src/waylay/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:14:44.948015 waylay_sdk_storage-0.4.1.20240423/src/waylay/services/storage/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:14:44.952015 waylay_sdk_storage-0.4.1.20240423/src/waylay/services/storage/api/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-23 16:14:40.000000 waylay_sdk_storage-0.4.1.20240423/src/waylay/services/storage/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11794 2024-04-23 16:14:40.000000 waylay_sdk_storage-0.4.1.20240423/src/waylay/services/storage/api/about_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-04-23 16:14:40.000000 waylay_sdk_storage-0.4.1.20240423/src/waylay/services/storage/api/bucket_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27934 2024-04-23 16:14:40.000000 waylay_sdk_storage-0.4.1.20240423/src/waylay/services/storage/api/object_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:14:40.000000 waylay_sdk_storage-0.4.1.20240423/src/waylay/services/storage/api/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    44677 2024-04-23 16:14:40.000000 waylay_sdk_storage-0.4.1.20240423/src/waylay/services/storage/api/subscription_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:14:44.952015 waylay_sdk_storage-0.4.1.20240423/src/waylay/services/storage/service/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-23 16:14:40.000000 waylay_sdk_storage-0.4.1.20240423/src/waylay/services/storage/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:14:40.000000 waylay_sdk_storage-0.4.1.20240423/src/waylay/services/storage/service/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-23 16:14:40.000000 waylay_sdk_storage-0.4.1.20240423/src/waylay/services/storage/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:14:44.952015 waylay_sdk_storage-0.4.1.20240423/src/waylay_sdk_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-23 16:14:44.000000 waylay_sdk_storage-0.4.1.20240423/src/waylay_sdk_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-23 16:14:44.000000 waylay_sdk_storage-0.4.1.20240423/src/waylay_sdk_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:14:44.000000 waylay_sdk_storage-0.4.1.20240423/src/waylay_sdk_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 16:14:44.000000 waylay_sdk_storage-0.4.1.20240423/src/waylay_sdk_storage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-23 16:14:44.000000 waylay_sdk_storage-0.4.1.20240423/src/waylay_sdk_storage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 16:14:44.000000 waylay_sdk_storage-0.4.1.20240423/src/waylay_sdk_storage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:38:29.703975 waylay-sdk-storage-0.4.1b1/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-03-28 13:38:29.703975 waylay-sdk-storage-0.4.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 13:38:29.703975 waylay-sdk-storage-0.4.1b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:38:29.695974 waylay-sdk-storage-0.4.1b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:38:29.695974 waylay-sdk-storage-0.4.1b1/src/waylay/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:38:29.695974 waylay-sdk-storage-0.4.1b1/src/waylay/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:38:29.695974 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:38:29.699974 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11094 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/api/about_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11200 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/api/bucket_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26534 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/api/object_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    42225 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/api/subscription_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:38:29.699974 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/service/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-28 13:38:25.000000 waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:38:29.699974 waylay-sdk-storage-0.4.1b1/src/waylay_sdk_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-03-28 13:38:29.000000 waylay-sdk-storage-0.4.1b1/src/waylay_sdk_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-28 13:38:29.000000 waylay-sdk-storage-0.4.1b1/src/waylay_sdk_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 13:38:29.000000 waylay-sdk-storage-0.4.1b1/src/waylay_sdk_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-28 13:38:29.000000 waylay-sdk-storage-0.4.1b1/src/waylay_sdk_storage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-28 13:38:29.000000 waylay-sdk-storage-0.4.1b1/src/waylay_sdk_storage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-28 13:38:29.000000 waylay-sdk-storage-0.4.1b1/src/waylay_sdk_storage.egg-info/top_level.txt
```

### Comparing `waylay_sdk_storage-0.4.1.20240423/LICENSE.txt` & `waylay-sdk-storage-0.4.1b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage-0.4.1.20240423/PKG-INFO` & `waylay-sdk-storage-0.4.1b1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-storage
-Version: 0.4.1.20240423
+Version: 0.4.1b1
 Summary: Waylay Storage
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,22 +13,21 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-storage-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/storage.html
 Keywords: Waylay Storage
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.1
+Requires-Dist: waylay-sdk~=0.0.4rc5
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -48,38 +47,38 @@
 
 # Waylay Storage Service
 
 Manage storage buckets and subscriptions.
 
 
 This Python package is automatically generated based on the 
-Waylay Storage OpenAPI specification (API version: 0.4.1)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/storage.html).
+Waylay Storage OpenAPI specification (API version: v0.4.1)
 
-It consists of a plugin for the waylay-sdk-core package, and contains the Storage api methods.
+It consists of a plugin for the waylay-sdk package, and contains the Storage api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-storage-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-storage is included in:
-- ```pip install waylay-sdk-core[storage]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[storage]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-storage and waylay-sdk-storage-types are included in:
-- ```pip install waylay-sdk-core[storage,storage-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[storage,storage-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-storage-types` is installed
@@ -91,8 +90,7 @@
     print("The response of storage.about.version:\n")
     pprint(api_response)
 except ApiError as e:
     print("Exception when calling storage.about.version: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_storage-0.4.1.20240423/README.md` & `waylay-sdk-storage-0.4.1b1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # Waylay Storage Service
 
 Manage storage buckets and subscriptions.
 
 
 This Python package is automatically generated based on the 
-Waylay Storage OpenAPI specification (API version: 0.4.1)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/storage.html).
+Waylay Storage OpenAPI specification (API version: v0.4.1)
 
-It consists of a plugin for the waylay-sdk-core package, and contains the Storage api methods.
+It consists of a plugin for the waylay-sdk package, and contains the Storage api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-storage-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-storage is included in:
-- ```pip install waylay-sdk-core[storage]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[storage]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-storage and waylay-sdk-storage-types are included in:
-- ```pip install waylay-sdk-core[storage,storage-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[storage,storage-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-storage-types` is installed
@@ -43,8 +43,7 @@
     print("The response of storage.about.version:\n")
     pprint(api_response)
 except ApiError as e:
     print("Exception when calling storage.about.version: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_storage-0.4.1.20240423/pyproject.toml` & `waylay-sdk-storage-0.4.1b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-storage"
-version = "0.4.1.20240423"
+version = "0.4.1b1"
 description = "Waylay Storage"
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay Storage"]
 requires-python = ">= 3.9"
 dependencies = [
-    "waylay-sdk-core ~= 0.2.1",
+    "waylay-sdk ~= 0.0.4rc5",
     "pydantic ~= 2.6",
     "typing-extensions ~= 4.10",
     "eval-type-backport ~= 0.1.3; python_version < '3.10'",
 ]
 readme = "README.md"
 license={file = "LICENSE.txt"}
 
 [project.urls]
 Homepage = "https://www.waylay.io/"
-Documentation = "https://docs.waylay.io/#/api/?id=software-development-kits"
+Documentation = "https://docs.waylay.io/#/"
 Repository = "https://github.com/waylayio/waylay-sdk-storage-py.git"
-"Openapi Specification" = "https://docs.waylay.io/openapi/public/redocly/storage.html"
 
 [project.optional-dependencies]
 dev = [
     "mypy",
     "ruff",
     "types-python-jose",
     "types-appdirs",
```

### Comparing `waylay_sdk_storage-0.4.1.20240423/src/waylay/services/storage/api/about_api.py` & `waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/api/about_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -69,79 +69,73 @@
     async def status(
         self,
         *,
         query: StatusQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> TenantStatusReport: ...
 
     @overload
     async def status(
         self,
         *,
         query: StatusQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def status(
         self,
         *,
         query: StatusQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def status(
         self,
         *,
         query: StatusQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def status(
         self,
         *,
         query: StatusQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def status(
         self,
         *,
         query: StatusQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> TenantStatusReport | T | Response | Model:
         """Status.
 
         Validate consistency of buckets and notification queues for this tenant.
         :param query: URL Query parameters.
@@ -154,15 +148,14 @@
         :type query['include_queues']: bool
         :param query['include_disk_usage'] (dict) <br> query.include_disk_usage (Query) :
         :type query['include_disk_usage']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -173,22 +166,26 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(StatusQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": TenantStatusReport if not select_path else Model,
@@ -217,92 +214,85 @@
     async def version(
         self,
         *,
         query: VersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> str: ...
 
     @overload
     async def version(
         self,
         *,
         query: VersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def version(
         self,
         *,
         query: VersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def version(
         self,
         *,
         query: VersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def version(
         self,
         *,
         query: VersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def version(
         self,
         *,
         query: VersionQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> str | T | Response | Model:
         """Version.
 
         Get the application version.
         :param query: URL Query parameters.
         :type query: VersionQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -313,22 +303,26 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(VersionQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": str if not select_path else Model,
```

### Comparing `waylay_sdk_storage-0.4.1.20240423/src/waylay/services/storage/api/bucket_api.py` & `waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/api/bucket_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -82,84 +82,78 @@
         self,
         bucket_name: StrictStr,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Bucket: ...
 
     @overload
     async def get(
         self,
         bucket_name: StrictStr,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get(
         self,
         bucket_name: StrictStr,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get(
         self,
         bucket_name: StrictStr,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get(
         self,
         bucket_name: StrictStr,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get(
         self,
         bucket_name: StrictStr,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Bucket | T | Response | Model:
         """Get Bucket.
 
         Get a descriptive representation of a bucket.
         :param bucket_name: (required)
@@ -168,15 +162,14 @@
         :type query: GetQuery | QueryParamTypes, optional
         :param query['store'] (dict) <br> query.store (Query) :
         :type query['store']: str
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -187,24 +180,28 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "bucket_name": str(bucket_name),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": Bucket if not select_path else Model,
@@ -233,94 +230,87 @@
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> BucketListing: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> BucketListing | T | Response | Model:
         """List Buckets.
 
         List authorized buckets.
         :param query: URL Query parameters.
         :type query: ListQuery | QueryParamTypes, optional
         :param query['store'] (dict) <br> query.store (Query) :
         :type query['store']: str
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -331,22 +321,26 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(ListQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": BucketListing if not select_path else Model,
```

### Comparing `waylay_sdk_storage-0.4.1.20240423/src/waylay/services/storage/api/object_api.py` & `waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/api/object_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,89 +105,83 @@
         bucket_name: StrictStr,
         target_path: StrictStr,
         *,
         query: CopyOrMoveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> HALEntity: ...
 
     @overload
     async def copy_or_move(
         self,
         bucket_name: StrictStr,
         target_path: StrictStr,
         *,
         query: CopyOrMoveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def copy_or_move(
         self,
         bucket_name: StrictStr,
         target_path: StrictStr,
         *,
         query: CopyOrMoveQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def copy_or_move(
         self,
         bucket_name: StrictStr,
         target_path: StrictStr,
         *,
         query: CopyOrMoveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def copy_or_move(
         self,
         bucket_name: StrictStr,
         target_path: StrictStr,
         *,
         query: CopyOrMoveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def copy_or_move(
         self,
         bucket_name: StrictStr,
         target_path: StrictStr,
         *,
         query: CopyOrMoveQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> HALEntity | T | Response | Model:
         """Copy Or Move Object.
 
         Copy or move object to new location.
         :param bucket_name: (required)
@@ -202,15 +196,14 @@
         :type query['move']: bool
         :param query['store'] (dict) <br> query.store (Query) :
         :type query['store']: str
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -221,25 +214,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "bucket_name": str(bucket_name),
             "target_path": str(target_path),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(CopyOrMoveQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": HALEntity if not select_path else Model,
@@ -270,89 +267,83 @@
         bucket_name: StrictStr,
         object_path: StrictStr,
         *,
         query: CreateFolderQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> BucketObject: ...
 
     @overload
     async def create_folder(
         self,
         bucket_name: StrictStr,
         object_path: StrictStr,
         *,
         query: CreateFolderQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def create_folder(
         self,
         bucket_name: StrictStr,
         object_path: StrictStr,
         *,
         query: CreateFolderQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def create_folder(
         self,
         bucket_name: StrictStr,
         object_path: StrictStr,
         *,
         query: CreateFolderQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def create_folder(
         self,
         bucket_name: StrictStr,
         object_path: StrictStr,
         *,
         query: CreateFolderQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def create_folder(
         self,
         bucket_name: StrictStr,
         object_path: StrictStr,
         *,
         query: CreateFolderQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> BucketObject | T | Response | Model:
         """Create Folder.
 
         Create a (virtual) folder.  * (`all=true`) force creation of a hidden folder,   having a path element that starts with a `.`.
         :param bucket_name: (required)
@@ -365,15 +356,14 @@
         :type query['all']: bool
         :param query['store'] (dict) <br> query.store (Query) :
         :type query['store']: str
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -384,25 +374,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "bucket_name": str(bucket_name),
             "object_path": str(object_path),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(CreateFolderQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": BucketObject if not select_path else Model,
@@ -433,89 +427,83 @@
         bucket_name: StrictStr,
         object_path: StrictStr,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResponseList: ...
 
     @overload
     async def list(
         self,
         bucket_name: StrictStr,
         object_path: StrictStr,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def list(
         self,
         bucket_name: StrictStr,
         object_path: StrictStr,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def list(
         self,
         bucket_name: StrictStr,
         object_path: StrictStr,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def list(
         self,
         bucket_name: StrictStr,
         object_path: StrictStr,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def list(
         self,
         bucket_name: StrictStr,
         object_path: StrictStr,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResponseList | T | Response | Model:
         """List Objects.
 
         List, inspect or sign objects.  * list the objects of a bucket with {object_path} prefix     * (`recursive=true`) list content recursively     * (`all=true`) include hidden objects * (`stat=true`) get the meta of the object at {object_path} * (`sign=[GET,PUT,POST]`) fetch presigned urls to operate on {object_path}     * (`all=true`) allow link creation for hidden objects
         :param bucket_name: (required)
@@ -554,15 +542,14 @@
         :type query['content_length_max']: int
         :param query['content_type'] (dict) <br> query.content_type (Query) :
         :type query['content_type']: str
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -573,25 +560,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "bucket_name": str(bucket_name),
             "object_path": str(object_path),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(ListQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": ResponseList if not select_path else Model,
@@ -622,89 +613,83 @@
         bucket_name: StrictStr,
         object_path: StrictStr,
         *,
         query: RemoveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> HALEntity: ...
 
     @overload
     async def remove(
         self,
         bucket_name: StrictStr,
         object_path: StrictStr,
         *,
         query: RemoveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def remove(
         self,
         bucket_name: StrictStr,
         object_path: StrictStr,
         *,
         query: RemoveQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def remove(
         self,
         bucket_name: StrictStr,
         object_path: StrictStr,
         *,
         query: RemoveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def remove(
         self,
         bucket_name: StrictStr,
         object_path: StrictStr,
         *,
         query: RemoveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def remove(
         self,
         bucket_name: StrictStr,
         object_path: StrictStr,
         *,
         query: RemoveQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> HALEntity | T | Response | Model:
         """Remove Object Or Folder.
 
         Remove the object or folder at {object_path}.  An {object_path} ending in a `/` requests folder deletion of an empty folder unless: * (`recursive=true`) forces recursive deletion of a (non-empty) folder. * (`all=true`) forces recursive deletion, including hidden objects.
         :param bucket_name: (required)
@@ -723,15 +708,14 @@
         :type query['max_keys']: int
         :param query['store'] (dict) <br> query.store (Query) :
         :type query['store']: str
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -742,25 +726,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "bucket_name": str(bucket_name),
             "object_path": str(object_path),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(RemoveQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": HALEntity if not select_path else Model,
```

### Comparing `waylay_sdk_storage-0.4.1.20240423/src/waylay/services/storage/api/subscription_api.py` & `waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/api/subscription_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -132,89 +132,83 @@
         bucket_name: StrictStr,
         *,
         json: SubscriptionConfig,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> SubscriptionConfig: ...
 
     @overload
     async def create(
         self,
         bucket_name: StrictStr,
         *,
         json: SubscriptionConfig,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def create(
         self,
         bucket_name: StrictStr,
         *,
         json: SubscriptionConfig,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def create(
         self,
         bucket_name: StrictStr,
         *,
         json: SubscriptionConfig,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def create(
         self,
         bucket_name: StrictStr,
         *,
         json: SubscriptionConfig,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def create(
         self,
         bucket_name: StrictStr,
         *,
         json: SubscriptionConfig,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> SubscriptionConfig | T | Response | Model:
         """Create Bucket Subscription.
 
         Create a new notification subscription on a bucket with a given or generated id.
         :param bucket_name: (required)
@@ -225,15 +219,14 @@
         :type query: CreateQuery | QueryParamTypes, optional
         :param query['store'] (dict) <br> query.store (Query) :
         :type query['store']: str
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -244,28 +237,32 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "bucket_name": str(bucket_name),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
+        if json is not None and should_validate:
             body_adapter = TypeAdapter(SubscriptionConfig)
             json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
         body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(CreateQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": SubscriptionConfig if not select_path else Model,
@@ -295,84 +292,78 @@
         self,
         bucket_name: StrictStr,
         *,
         query: DeleteByQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> HALEntity: ...
 
     @overload
     async def delete_by(
         self,
         bucket_name: StrictStr,
         *,
         query: DeleteByQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def delete_by(
         self,
         bucket_name: StrictStr,
         *,
         query: DeleteByQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def delete_by(
         self,
         bucket_name: StrictStr,
         *,
         query: DeleteByQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def delete_by(
         self,
         bucket_name: StrictStr,
         *,
         query: DeleteByQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def delete_by(
         self,
         bucket_name: StrictStr,
         *,
         query: DeleteByQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> HALEntity | T | Response | Model:
         """Delete All Bucket Subscriptions.
 
         Remove all notification subscription on a bucket that match a given event and/or channel filter.
         :param bucket_name: (required)
@@ -395,15 +386,14 @@
         :type query['store']: str
         :param query['max_keys'] (dict) <br> query.max_keys (Query) :
         :type query['max_keys']: int
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -414,24 +404,28 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "bucket_name": str(bucket_name),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(DeleteByQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": HALEntity if not select_path else Model,
@@ -462,89 +456,83 @@
         bucket_name: StrictStr,
         subscription_id: StrictStr,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> SubscriptionConfig: ...
 
     @overload
     async def get(
         self,
         bucket_name: StrictStr,
         subscription_id: StrictStr,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get(
         self,
         bucket_name: StrictStr,
         subscription_id: StrictStr,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get(
         self,
         bucket_name: StrictStr,
         subscription_id: StrictStr,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get(
         self,
         bucket_name: StrictStr,
         subscription_id: StrictStr,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get(
         self,
         bucket_name: StrictStr,
         subscription_id: StrictStr,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> SubscriptionConfig | T | Response | Model:
         """Get Bucket Subscription.
 
         Fetch a notification subscription.
         :param bucket_name: (required)
@@ -555,15 +543,14 @@
         :type query: GetQuery | QueryParamTypes, optional
         :param query['store'] (dict) <br> query.store (Query) :
         :type query['store']: str
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -574,25 +561,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "bucket_name": str(bucket_name),
             "subscription_id": str(subscription_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": SubscriptionConfig if not select_path else Model,
@@ -621,79 +612,73 @@
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> SubscriptionsListing: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> SubscriptionsListing | T | Response | Model:
         """Query All Subscriptions.
 
         List notification subscriptions per bucket that have notification enabled.
         :param query: URL Query parameters.
@@ -712,15 +697,14 @@
         :type query['channel_id']: str
         :param query['max_keys'] (dict) <br> query.max_keys (Query) :
         :type query['max_keys']: int
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -731,22 +715,26 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(ListQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": SubscriptionsListing if not select_path else Model,
@@ -776,84 +764,78 @@
         self,
         bucket_name: StrictStr,
         *,
         query: QueryQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Subscriptions: ...
 
     @overload
     async def query(
         self,
         bucket_name: StrictStr,
         *,
         query: QueryQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def query(
         self,
         bucket_name: StrictStr,
         *,
         query: QueryQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def query(
         self,
         bucket_name: StrictStr,
         *,
         query: QueryQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def query(
         self,
         bucket_name: StrictStr,
         *,
         query: QueryQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def query(
         self,
         bucket_name: StrictStr,
         *,
         query: QueryQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Subscriptions | T | Response | Model:
         """Query Bucket Subscriptions.
 
         List notification subscriptions for given bucket.
         :param bucket_name: (required)
@@ -876,15 +858,14 @@
         :type query['channel_id']: str
         :param query['max_keys'] (dict) <br> query.max_keys (Query) :
         :type query['max_keys']: int
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -895,24 +876,28 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "bucket_name": str(bucket_name),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(QueryQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": Subscriptions if not select_path else Model,
@@ -943,89 +928,83 @@
         bucket_name: StrictStr,
         subscription_id: StrictStr,
         *,
         query: RemoveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> HALEntity: ...
 
     @overload
     async def remove(
         self,
         bucket_name: StrictStr,
         subscription_id: StrictStr,
         *,
         query: RemoveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def remove(
         self,
         bucket_name: StrictStr,
         subscription_id: StrictStr,
         *,
         query: RemoveQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def remove(
         self,
         bucket_name: StrictStr,
         subscription_id: StrictStr,
         *,
         query: RemoveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def remove(
         self,
         bucket_name: StrictStr,
         subscription_id: StrictStr,
         *,
         query: RemoveQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def remove(
         self,
         bucket_name: StrictStr,
         subscription_id: StrictStr,
         *,
         query: RemoveQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> HALEntity | T | Response | Model:
         """Delete Bucket Subscription.
 
         Remove a notification subscription.
         :param bucket_name: (required)
@@ -1036,15 +1015,14 @@
         :type query: RemoveQuery | QueryParamTypes, optional
         :param query['store'] (dict) <br> query.store (Query) :
         :type query['store']: str
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1055,25 +1033,29 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "bucket_name": str(bucket_name),
             "subscription_id": str(subscription_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(RemoveQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": HALEntity if not select_path else Model,
@@ -1105,15 +1087,14 @@
         subscription_id: StrictStr,
         *,
         json: SubscriptionConfig,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> SubscriptionConfig: ...
 
     @overload
     async def replace(
         self,
@@ -1121,15 +1102,14 @@
         subscription_id: StrictStr,
         *,
         json: SubscriptionConfig,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def replace(
         self,
@@ -1137,15 +1117,14 @@
         subscription_id: StrictStr,
         *,
         json: SubscriptionConfig,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def replace(
         self,
@@ -1153,15 +1132,14 @@
         subscription_id: StrictStr,
         *,
         json: SubscriptionConfig,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def replace(
         self,
@@ -1169,30 +1147,28 @@
         subscription_id: StrictStr,
         *,
         json: SubscriptionConfig,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def replace(
         self,
         bucket_name: StrictStr,
         subscription_id: StrictStr,
         *,
         json: SubscriptionConfig,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> SubscriptionConfig | T | Response | Model:
         """Replace Bucket Subscription.
 
         Create or replace a notification subscription on a bucket with a given id.
         :param bucket_name: (required)
@@ -1205,15 +1181,14 @@
         :type query: ReplaceQuery | QueryParamTypes, optional
         :param query['store'] (dict) <br> query.store (Query) :
         :type query['store']: str
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1224,29 +1199,33 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "bucket_name": str(bucket_name),
             "subscription_id": str(subscription_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
+        if json is not None and should_validate:
             body_adapter = TypeAdapter(SubscriptionConfig)
             json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
         body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(ReplaceQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": SubscriptionConfig if not select_path else Model,
```

### Comparing `waylay_sdk_storage-0.4.1.20240423/src/waylay/services/storage/service/service.py` & `waylay-sdk-storage-0.4.1b1/src/waylay/services/storage/service/service.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage-0.4.1.20240423/src/waylay_sdk_storage.egg-info/PKG-INFO` & `waylay-sdk-storage-0.4.1b1/src/waylay_sdk_storage.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-storage
-Version: 0.4.1.20240423
+Version: 0.4.1b1
 Summary: Waylay Storage
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,22 +13,21 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-storage-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/storage.html
 Keywords: Waylay Storage
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.1
+Requires-Dist: waylay-sdk~=0.0.4rc5
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -48,38 +47,38 @@
 
 # Waylay Storage Service
 
 Manage storage buckets and subscriptions.
 
 
 This Python package is automatically generated based on the 
-Waylay Storage OpenAPI specification (API version: 0.4.1)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/storage.html).
+Waylay Storage OpenAPI specification (API version: v0.4.1)
 
-It consists of a plugin for the waylay-sdk-core package, and contains the Storage api methods.
+It consists of a plugin for the waylay-sdk package, and contains the Storage api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-storage-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-storage is included in:
-- ```pip install waylay-sdk-core[storage]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[storage]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-storage and waylay-sdk-storage-types are included in:
-- ```pip install waylay-sdk-core[storage,storage-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[storage,storage-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-storage-types` is installed
@@ -91,8 +90,7 @@
     print("The response of storage.about.version:\n")
     pprint(api_response)
 except ApiError as e:
     print("Exception when calling storage.about.version: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_storage-0.4.1.20240423/src/waylay_sdk_storage.egg-info/SOURCES.txt` & `waylay-sdk-storage-0.4.1b1/src/waylay_sdk_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

