# Comparing `tmp/waylay_sdk_registry-2.13.0b20240415.tar.gz` & `tmp/waylay-sdk-registry-2.13.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk_registry-2.13.0b20240415.tar", last modified: Mon Apr 15 08:45:53 2024, max compression
+gzip compressed data, was "waylay-sdk-registry-2.13.0rc0.tar", last modified: Fri Mar 29 13:21:52 2024, max compression
```

## Comparing `waylay_sdk_registry-2.13.0b20240415.tar` & `waylay-sdk-registry-2.13.0rc0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:53.961551 waylay_sdk_registry-2.13.0b20240415/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-15 08:45:48.000000 waylay_sdk_registry-2.13.0b20240415/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-04-15 08:45:53.961551 waylay_sdk_registry-2.13.0b20240415/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-15 08:45:48.000000 waylay_sdk_registry-2.13.0b20240415/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-15 08:45:48.000000 waylay_sdk_registry-2.13.0b20240415/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:45:53.961551 waylay_sdk_registry-2.13.0b20240415/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:53.953551 waylay_sdk_registry-2.13.0b20240415/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:53.953551 waylay_sdk_registry-2.13.0b20240415/src/waylay/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:53.953551 waylay_sdk_registry-2.13.0b20240415/src/waylay/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:53.953551 waylay_sdk_registry-2.13.0b20240415/src/waylay/services/registry/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:53.957551 waylay_sdk_registry-2.13.0b20240415/src/waylay/services/registry/api/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-15 08:45:48.000000 waylay_sdk_registry-2.13.0b20240415/src/waylay/services/registry/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-04-15 08:45:48.000000 waylay_sdk_registry-2.13.0b20240415/src/waylay/services/registry/api/about_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18302 2024-04-15 08:45:48.000000 waylay_sdk_registry-2.13.0b20240415/src/waylay/services/registry/api/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   170780 2024-04-15 08:45:48.000000 waylay_sdk_registry-2.13.0b20240415/src/waylay/services/registry/api/models_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   178638 2024-04-15 08:45:48.000000 waylay_sdk_registry-2.13.0b20240415/src/waylay/services/registry/api/plugs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:48.000000 waylay_sdk_registry-2.13.0b20240415/src/waylay/services/registry/api/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    42593 2024-04-15 08:45:48.000000 waylay_sdk_registry-2.13.0b20240415/src/waylay/services/registry/api/runtimes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-04-15 08:45:48.000000 waylay_sdk_registry-2.13.0b20240415/src/waylay/services/registry/api/schemas_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   172019 2024-04-15 08:45:48.000000 waylay_sdk_registry-2.13.0b20240415/src/waylay/services/registry/api/webscripts_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:53.957551 waylay_sdk_registry-2.13.0b20240415/src/waylay/services/registry/service/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-15 08:45:48.000000 waylay_sdk_registry-2.13.0b20240415/src/waylay/services/registry/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:48.000000 waylay_sdk_registry-2.13.0b20240415/src/waylay/services/registry/service/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-15 08:45:48.000000 waylay_sdk_registry-2.13.0b20240415/src/waylay/services/registry/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:45:53.961551 waylay_sdk_registry-2.13.0b20240415/src/waylay_sdk_registry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-04-15 08:45:53.000000 waylay_sdk_registry-2.13.0b20240415/src/waylay_sdk_registry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-15 08:45:53.000000 waylay_sdk_registry-2.13.0b20240415/src/waylay_sdk_registry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:45:53.000000 waylay_sdk_registry-2.13.0b20240415/src/waylay_sdk_registry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 08:45:53.000000 waylay_sdk_registry-2.13.0b20240415/src/waylay_sdk_registry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-15 08:45:53.000000 waylay_sdk_registry-2.13.0b20240415/src/waylay_sdk_registry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 08:45:53.000000 waylay_sdk_registry-2.13.0b20240415/src/waylay_sdk_registry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.831539 waylay-sdk-registry-2.13.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-03-29 13:21:52.831539 waylay-sdk-registry-2.13.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 13:21:52.831539 waylay-sdk-registry-2.13.0rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.823539 waylay-sdk-registry-2.13.0rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.823539 waylay-sdk-registry-2.13.0rc0/src/waylay/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.823539 waylay-sdk-registry-2.13.0rc0/src/waylay/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.823539 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.827539 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17657 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   167061 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/models_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   174919 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/plugs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    42593 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/runtimes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/schemas_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   168300 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/webscripts_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.827539 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/service/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-29 13:21:48.000000 waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.831539 waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-03-29 13:21:52.000000 waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-29 13:21:52.000000 waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 13:21:52.000000 waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-29 13:21:52.000000 waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-29 13:21:52.000000 waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-29 13:21:52.000000 waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/top_level.txt
```

### Comparing `waylay_sdk_registry-2.13.0b20240415/LICENSE.txt` & `waylay-sdk-registry-2.13.0rc0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry-2.13.0b20240415/PKG-INFO` & `waylay-sdk-registry-2.13.0rc0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-registry
-Version: 2.13.0b20240415
+Version: 2.13.0rc0
 Summary: Waylay Function Registry
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
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-registry-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/registry.html
 Keywords: Waylay Function Registry
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.0
+Requires-Dist: waylay-sdk~=0.0.4rc5
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -46,52 +45,57 @@
 Provides-Extra: types
 Requires-Dist: waylay-sdk-registry-types; extra == "types"
 
 # Waylay Registry Service
 V2 API to build and deploy Waylay functions (plugs, webscripts, BYOML models).
 
 This Python package is automatically generated based on the 
-Waylay Registry OpenAPI specification (API version: 2.13.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/registry.html).
+Waylay Registry OpenAPI specification (API version: 2.13.0-beta.0)
 
-It consists of a plugin for the waylay-sdk-core package, and contains the Registry api methods.
+It consists of a plugin for the waylay-sdk package, and contains the Registry api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-registry-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-registry is included in:
-- ```pip install waylay-sdk-core[registry]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[registry]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-registry and waylay-sdk-registry-types are included in:
-- ```pip install waylay-sdk-core[registry,registry-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[registry,registry-types]``` to install `waylay-sdk` along with only this service including the typed models, or
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
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-registry-types` is installed
-from waylay.services.registry.models.root_page_response import RootPageResponse
+from registry.models.function_type import FunctionType
+from registry.models.job_state_result import JobStateResult
+from registry.models.job_type_schema import JobTypeSchema
+from registry.models.jobs_response import JobsResponse
 try:
-    # Get Service Status
-    # calls `GET /registry/v2/`
-    api_response = await waylay_client.registry.about.get(
+    # List Jobs
+    # calls `GET /registry/v2/jobs/`
+    api_response = await waylay_client.registry.jobs.list(
+        # query parameters:
+        query = {
+        },
     )
-    print("The response of registry.about.get:\n")
+    print("The response of registry.jobs.list:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling registry.about.get: %s\n" % e)
+    print("Exception when calling registry.jobs.list: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_registry-2.13.0b20240415/README.md` & `waylay-sdk-registry-2.13.0rc0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 # Waylay Registry Service
 V2 API to build and deploy Waylay functions (plugs, webscripts, BYOML models).
 
 This Python package is automatically generated based on the 
-Waylay Registry OpenAPI specification (API version: 2.13.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/registry.html).
+Waylay Registry OpenAPI specification (API version: 2.13.0-beta.0)
 
-It consists of a plugin for the waylay-sdk-core package, and contains the Registry api methods.
+It consists of a plugin for the waylay-sdk package, and contains the Registry api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-registry-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-registry is included in:
-- ```pip install waylay-sdk-core[registry]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[registry]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-registry and waylay-sdk-registry-types are included in:
-- ```pip install waylay-sdk-core[registry,registry-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[registry,registry-types]``` to install `waylay-sdk` along with only this service including the typed models, or
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
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-registry-types` is installed
-from waylay.services.registry.models.root_page_response import RootPageResponse
+from registry.models.function_type import FunctionType
+from registry.models.job_state_result import JobStateResult
+from registry.models.job_type_schema import JobTypeSchema
+from registry.models.jobs_response import JobsResponse
 try:
-    # Get Service Status
-    # calls `GET /registry/v2/`
-    api_response = await waylay_client.registry.about.get(
+    # List Jobs
+    # calls `GET /registry/v2/jobs/`
+    api_response = await waylay_client.registry.jobs.list(
+        # query parameters:
+        query = {
+        },
     )
-    print("The response of registry.about.get:\n")
+    print("The response of registry.jobs.list:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling registry.about.get: %s\n" % e)
+    print("Exception when calling registry.jobs.list: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_registry-2.13.0b20240415/pyproject.toml` & `waylay-sdk-registry-2.13.0rc0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-registry"
-version = "2.13.0b20240415"
+version = "2.13.0rc0"
 description = "Waylay Function Registry"
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay Function Registry"]
 requires-python = ">= 3.9"
 dependencies = [
-    "waylay-sdk-core ~= 0.2.0",
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
 Repository = "https://github.com/waylayio/waylay-sdk-registry-py.git"
-"Openapi Specification" = "https://docs.waylay.io/openapi/public/redocly/registry.html"
 
 [project.optional-dependencies]
 dev = [
     "mypy",
     "ruff",
     "types-python-jose",
     "types-appdirs",
```

### Comparing `waylay_sdk_registry-2.13.0b20240415/src/waylay/services/registry/api/about_api.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/default_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,35 +29,35 @@
     Response,
 )
 from waylay.sdk.api._models import Model
 from waylay.sdk.plugin import WithApiClient
 
 if TYPE_CHECKING:
     from waylay.services.registry.models import RootPageResponse
-    from waylay.services.registry.queries.about_api import GetQuery
+    from waylay.services.registry.queries.default_api import GetQuery
 
 
 try:
     from waylay.services.registry.models import RootPageResponse
-    from waylay.services.registry.queries.about_api import GetQuery
+    from waylay.services.registry.queries.default_api import GetQuery
 
     MODELS_AVAILABLE = True
 except ImportError:
     MODELS_AVAILABLE = False
 
     if not TYPE_CHECKING:
         GetQuery = dict
         RootPageResponse = Model
 
 
 T = TypeVar("T")
 
 
-class AboutApi(WithApiClient):
-    """AboutApi service methods.
+class DefaultApi(WithApiClient):
+    """DefaultApi service methods.
 
     NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
@@ -127,17 +127,17 @@
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> RootPageResponse | T | Response | Model:
-        """Get Service Status.
+        """Version.
 
-        Get the status and version of the function registry service.
+        Get the version of this function registry deployment.
         :param query: URL Query parameters.
         :type query: GetQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
         :param headers: Header parameters for this request
```

### Comparing `waylay_sdk_registry-2.13.0b20240415/src/waylay/services/registry/api/jobs_api.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/jobs_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 """
 
 from __future__ import annotations  # for Python 3.7–3.9
 
 from typing import (
     TYPE_CHECKING,
     Any,
-    AsyncIterator,
     Dict,
     Literal,
     TypeVar,
     overload,
 )
 
 from pydantic import (
@@ -27,15 +26,14 @@
 )
 from waylay.sdk.api import (
     HeaderTypes,
     QueryParamTypes,
     Response,
 )
 from waylay.sdk.api._models import Model
-from waylay.sdk.api.constants import STREAM_TIMEOUTS
 from waylay.sdk.plugin import WithApiClient
 
 if TYPE_CHECKING:
     from waylay.services.registry.models import (
         EventWithCloseSSE,
         JobResponse,
         JobsResponse,
@@ -94,92 +92,75 @@
         self,
         *,
         query: EventsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[EventWithCloseSSE]: ...
+    ) -> EventWithCloseSSE: ...
 
     @overload
     async def events(
         self,
         *,
         query: EventsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[T]: ...
+    ) -> T: ...
 
     @overload
     async def events(
         self,
         *,
         query: EventsQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def events(
         self,
         *,
         query: EventsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[Model]: ...
+    ) -> Model: ...
 
     @overload
     async def events(
         self,
         *,
         query: EventsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[T]: ...
+    ) -> T: ...
 
     async def events(
         self,
         *,
         query: EventsQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> (
-        AsyncIterator[EventWithCloseSSE]
-        | AsyncIterator[T]
-        | Response
-        | AsyncIterator[Model]
-    ):
+    ) -> EventWithCloseSSE | T | Response | Model:
         """Stream Events.
 
         Get an SSE stream of all job events for the users tenant.  The stream can be filtered on job type or on a specific job id.   When filtering on job id, the server will send a <code>close</code> event  upon completion of the job. The client should handle this event by closing the stream.
         :param query: URL Query parameters.
         :type query: EventsQuery | QueryParamTypes, optional
         :param query['type'] (dict) <br> query.type (Query) : The type of the job.
         :type query['type']: JobType
@@ -237,16 +218,14 @@
         return await self.api_client.request(
             method="GET",
             resource_path="/registry/v2/jobs/events",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
-            stream=stream,
-            timeout=timeout,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
```

### Comparing `waylay_sdk_registry-2.13.0b20240415/src/waylay/services/registry/api/models_api.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/models_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -380,28 +380,26 @@
         :type json: bytearray, optional
         :param content: The assets for a <em>model</em> function can be provided as   <ul>     <li>A single <em>tar</em> archive (optionally compressed), with one of the content types      <code>application/octet-stream</code>, <code>application/tar</code>, <code>application/tar+gzip</code>, <code>application/x-gzip</code>, <code>application/x-tar</code>, <code>application/gzip</code></li>     <li>Separate files in a <code>multipart/form-data</code> request</li>     <li>A reference to the assets of another <em>model</em> in the <code>copy</code> argument</li>   </ul>    The required <code>model.json</code> json file contains the function metadata,   and must have a <code>runtime</code> attribute that is one of the supported <em>runtime</em>s    (see <code>GET /registry/v2/runtimes?functionType=kfserving</code>).    For each <em>runtime</em> other files will be required or supported.
         :type content: ContentRequest, optional
         :param files: The files of a `content-type: multipart/form-data` request.
         :type files: FilesRequest, optional
         :param query: URL Query parameters.
         :type query: CreateQuery | QueryParamTypes, optional
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
         :param query['deprecatePrevious'] (dict) <br> query.deprecate_previous (Query) : Set the cleanup policy used to automatically deprecate/delete previous versions.
         :type query['deprecatePrevious']: DeprecatePreviousPolicy
         :param query['dryRun'] (dict) <br> query.dry_run (Query) : If set to <code>true</code>, validates the deployment conditions, but does not change anything.
         :type query['dryRun']: bool
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
+        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. Saves computing resources when the function is not to be used immediately.
+        :type query['scaleToZero']: bool
         :param query['version'] (dict) <br> query.version (Query) : If set, the function version will be an increment of the latest existing version that satisfies the `version` range. Note that this increment always takes precedence over an explicit `version` in the function manifest.
         :type query['version']: SemanticVersionRange
         :param query['name'] (dict) <br> query.name (Query) : If set, the value will be used as the function name instead of the one specified in the manifest.
         :type query['name']: str
         :param query['draft'] (dict) <br> query.draft (Query) : If set, the created function will be a draft function and its assets are still mutable. A build and deploy is initiated only in the case when all necessary assets are present and valid.
         :type query['draft']: bool
         :param query['runtime'] (dict) <br> query.runtime (Query) : If set, the created function will use the indicated runtime (latest version within specified range).  This takes precedence over the runtime specified in a function manifest (copied or from request body).
@@ -621,18 +619,14 @@
         :type name: str
         :param version: The version of the function. (required)
         :type version: str
         :param wildcard: Full path or path prefix of the asset within the archive (required)
         :type wildcard: str
         :param query: URL Query parameters.
         :type query: DeleteAssetQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['chown'] (dict) <br> query.chown (Query) : If set, ownership of the draft function is transferred to the current user.
         :type query['chown']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
@@ -2384,28 +2378,28 @@
         Rebuild and deploy a model with the original or updated base image.
         :param name: The name of the function. (required)
         :type name: str
         :param version: The version of the function. (required)
         :type version: str
         :param query: URL Query parameters.
         :type query: RebuildQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command.
-        :type query['scaleToZero']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['dryRun'] (dict) <br> query.dry_run (Query) : If set to <code>true</code>, checks whether rebuild jobs are needed, but do not start any jobs.
         :type query['dryRun']: bool
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
         :param query['upgrade'] (dict) <br> query.upgrade (Query) : If set, force a rebuild with the given <em>runtime</em> version selection policy. <ul>  <li><code>same</code> <b>patch</b> version.   This should only include backward compatible upgrades.  </li>  <li><code>minor</code> <b>major</b> version.   This might include an upgrade of e.g. the language runtime and/or provided   dependencies that could break compatiblity with the function. .</li> </ul>
         :type query['upgrade']: RebuildPolicy
         :param query['forceVersion'] (dict) <br> query.force_version (Query) : If set, force a rebuild with the given runtime version (including downgrades). This parameter is mutually exclusive to the `upgrade` parameter.
         :type query['forceVersion']: str
         :param query['ignoreChecks'] (dict) <br> query.ignore_checks (Query) : If set to true, checks that normally prevent a rebuild are overriden. These checks include: * function state in `pending`, `running`, `failed` or `undeployed` * backoff period due to recent failures * usage of deprecated dependencies * running jobs on entity * the `dryRun` option
         :type query['ignoreChecks']: bool
+        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful (re-)deployment. If not set, the function is scaled to zero only if it was not active before this command.
+        :type query['scaleToZero']: bool
         :param query['skipRebuild'] (dict) <br> query.skip_rebuild (Query) : If set, the function will not be rebuild. Always uses the current runtime version when re-deploying/re-verifying the function.
         :type query['skipRebuild']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
         :param headers: Header parameters for this request
@@ -2956,18 +2950,14 @@
         :type version: str
         :param wildcard: Full path or path prefix of the asset within the archive (required)
         :type wildcard: str
         :param content: A single asset file.
         :type content: ContentRequest, optional
         :param query: URL Query parameters.
         :type query: UpdateAssetQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['chown'] (dict) <br> query.chown (Query) : If set, ownership of the draft function is transferred to the current user.
         :type query['chown']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
@@ -3199,18 +3189,14 @@
         :type version: str
         :param content: The assets for a <em>model</em> function can be provided as either   <ul>     <li>a single <em>tar</em> archive (optionally compressed), with one of the content types      <code>application/octet-stream</code>, <code>application/tar</code>, <code>application/tar+gzip</code>, <code>application/x-gzip</code>, <code>application/x-tar</code>, <code>application/gzip</code></li>     <li>separate files in a <code>multipart/form-data</code> request</li>   </ul>    The provided assets will be added to the <em>model</em> function's collection of existing assets,   replacing any existing assets with the same name.    Please note that it is not allowed to update the model.json</code> json file with a changed value for any of the    <code>name</code>, <code>version</code> and/or <code>runtime</code> attributes.    For each <em>runtime</em> other files are supported.
         :type content: ContentRequest, optional
         :param files: The files of a `content-type: multipart/form-data` request.
         :type files: FilesRequest, optional
         :param query: URL Query parameters.
         :type query: UpdateAssetsQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['chown'] (dict) <br> query.chown (Query) : If set, ownership of the draft function is transferred to the current user.
         :type query['chown']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
@@ -3382,18 +3368,18 @@
         Verify health of model deployed on openfaas.
         :param name: The name of the function. (required)
         :type name: str
         :param version: The version of the function. (required)
         :type version: str
         :param query: URL Query parameters.
         :type query: VerifyQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command.
-        :type query['scaleToZero']: bool
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
+        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command.
+        :type query['scaleToZero']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
```

### Comparing `waylay_sdk_registry-2.13.0b20240415/src/waylay/services/registry/api/plugs_api.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/plugs_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -387,28 +387,26 @@
         :type json: bytearray, optional
         :param content: The assets for a <em>plug</em> function can be provided as   <ul>     <li>A single <em>tar</em> archive (optionally compressed), with one of the content types      <code>application/octet-stream</code>, <code>application/tar</code>, <code>application/tar+gzip</code>, <code>application/x-gzip</code>, <code>application/x-tar</code>, <code>application/gzip</code></li>     <li>Separate files in a <code>multipart/form-data</code> request</li>     <li>A reference to the assets of another <em>plug</em> in the <code>copy</code> argument</li>   </ul>    The required <code>plug.json</code> json file contains the function metadata,   and must have a <code>runtime</code> attribute that is one of the supported <em>runtime</em>s    (see <code>GET /registry/v2/runtimes?functionType=plugs</code>).    For each <em>runtime</em> other files will be required or supported.
         :type content: ContentRequest, optional
         :param files: The files of a `content-type: multipart/form-data` request.
         :type files: FilesRequest, optional
         :param query: URL Query parameters.
         :type query: CreateQuery | QueryParamTypes, optional
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
         :param query['deprecatePrevious'] (dict) <br> query.deprecate_previous (Query) : Set the cleanup policy used to automatically deprecate/delete previous versions.
         :type query['deprecatePrevious']: DeprecatePreviousPolicy
         :param query['dryRun'] (dict) <br> query.dry_run (Query) : If set to <code>true</code>, validates the deployment conditions, but does not change anything.
         :type query['dryRun']: bool
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
+        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. Saves computing resources when the function is not to be used immediately.
+        :type query['scaleToZero']: bool
         :param query['version'] (dict) <br> query.version (Query) : If set, the function version will be an increment of the latest existing version that satisfies the `version` range. Note that this increment always takes precedence over an explicit `version` in the function manifest.
         :type query['version']: SemanticVersionRange
         :param query['name'] (dict) <br> query.name (Query) : If set, the value will be used as the function name instead of the one specified in the manifest.
         :type query['name']: str
         :param query['draft'] (dict) <br> query.draft (Query) : If set, the created function will be a draft function and its assets are still mutable. A build and deploy is initiated only in the case when all necessary assets are present and valid.
         :type query['draft']: bool
         :param query['runtime'] (dict) <br> query.runtime (Query) : If set, the created function will use the indicated runtime (latest version within specified range).  This takes precedence over the runtime specified in a function manifest (copied or from request body).
@@ -626,18 +624,14 @@
         :type name: str
         :param version: The version of the function. (required)
         :type version: str
         :param wildcard: Full path or path prefix of the asset within the archive (required)
         :type wildcard: str
         :param query: URL Query parameters.
         :type query: DeleteAssetQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['chown'] (dict) <br> query.chown (Query) : If set, ownership of the draft function is transferred to the current user.
         :type query['chown']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
@@ -2573,28 +2567,28 @@
         Rebuild and deploy a plug with the original or updated base image.
         :param name: The name of the function. (required)
         :type name: str
         :param version: The version of the function. (required)
         :type version: str
         :param query: URL Query parameters.
         :type query: RebuildQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command.
-        :type query['scaleToZero']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['dryRun'] (dict) <br> query.dry_run (Query) : If set to <code>true</code>, checks whether rebuild jobs are needed, but do not start any jobs.
         :type query['dryRun']: bool
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
         :param query['upgrade'] (dict) <br> query.upgrade (Query) : If set, force a rebuild with the given <em>runtime</em> version selection policy. <ul>  <li><code>same</code> <b>patch</b> version.   This should only include backward compatible upgrades.  </li>  <li><code>minor</code> <b>major</b> version.   This might include an upgrade of e.g. the language runtime and/or provided   dependencies that could break compatiblity with the function. .</li> </ul>
         :type query['upgrade']: RebuildPolicy
         :param query['forceVersion'] (dict) <br> query.force_version (Query) : If set, force a rebuild with the given runtime version (including downgrades). This parameter is mutually exclusive to the `upgrade` parameter.
         :type query['forceVersion']: str
         :param query['ignoreChecks'] (dict) <br> query.ignore_checks (Query) : If set to true, checks that normally prevent a rebuild are overriden. These checks include: * function state in `pending`, `running`, `failed` or `undeployed` * backoff period due to recent failures * usage of deprecated dependencies * running jobs on entity * the `dryRun` option
         :type query['ignoreChecks']: bool
+        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful (re-)deployment. If not set, the function is scaled to zero only if it was not active before this command.
+        :type query['scaleToZero']: bool
         :param query['skipRebuild'] (dict) <br> query.skip_rebuild (Query) : If set, the function will not be rebuild. Always uses the current runtime version when re-deploying/re-verifying the function.
         :type query['skipRebuild']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
         :param headers: Header parameters for this request
@@ -3143,18 +3137,14 @@
         :type version: str
         :param wildcard: Full path or path prefix of the asset within the archive (required)
         :type wildcard: str
         :param content: A single asset file.
         :type content: ContentRequest, optional
         :param query: URL Query parameters.
         :type query: UpdateAssetQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['chown'] (dict) <br> query.chown (Query) : If set, ownership of the draft function is transferred to the current user.
         :type query['chown']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
@@ -3384,18 +3374,14 @@
         :type version: str
         :param content: The assets for a <em>plug</em> function can be provided as either   <ul>     <li>a single <em>tar</em> archive (optionally compressed), with one of the content types      <code>application/octet-stream</code>, <code>application/tar</code>, <code>application/tar+gzip</code>, <code>application/x-gzip</code>, <code>application/x-tar</code>, <code>application/gzip</code></li>     <li>separate files in a <code>multipart/form-data</code> request</li>   </ul>    The provided assets will be added to the <em>plug</em> function's collection of existing assets,   replacing any existing assets with the same name.    Please note that it is not allowed to update the plug.json</code> json file with a changed value for any of the    <code>name</code>, <code>version</code> and/or <code>runtime</code> attributes.    For each <em>runtime</em> other files are supported.
         :type content: ContentRequest, optional
         :param files: The files of a `content-type: multipart/form-data` request.
         :type files: FilesRequest, optional
         :param query: URL Query parameters.
         :type query: UpdateAssetsQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['chown'] (dict) <br> query.chown (Query) : If set, ownership of the draft function is transferred to the current user.
         :type query['chown']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
@@ -3567,18 +3553,18 @@
         Verify health of plug deployed on openfaas.
         :param name: The name of the function. (required)
         :type name: str
         :param version: The version of the function. (required)
         :type version: str
         :param query: URL Query parameters.
         :type query: VerifyQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command.
-        :type query['scaleToZero']: bool
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
+        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command.
+        :type query['scaleToZero']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
```

### Comparing `waylay_sdk_registry-2.13.0b20240415/src/waylay/services/registry/api/runtimes_api.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/runtimes_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry-2.13.0b20240415/src/waylay/services/registry/api/schemas_api.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/schemas_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry-2.13.0b20240415/src/waylay/services/registry/api/webscripts_api.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/api/webscripts_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -384,28 +384,26 @@
         :type json: bytearray, optional
         :param content: The assets for a <em>webscript</em> function can be provided as   <ul>     <li>A single <em>tar</em> archive (optionally compressed), with one of the content types      <code>application/octet-stream</code>, <code>application/tar</code>, <code>application/tar+gzip</code>, <code>application/x-gzip</code>, <code>application/x-tar</code>, <code>application/gzip</code></li>     <li>Separate files in a <code>multipart/form-data</code> request</li>     <li>A reference to the assets of another <em>webscript</em> in the <code>copy</code> argument</li>   </ul>    The required <code>webscript.json</code> json file contains the function metadata,   and must have a <code>runtime</code> attribute that is one of the supported <em>runtime</em>s    (see <code>GET /registry/v2/runtimes?functionType=webscripts</code>).    For each <em>runtime</em> other files will be required or supported.
         :type content: ContentRequest, optional
         :param files: The files of a `content-type: multipart/form-data` request.
         :type files: FilesRequest, optional
         :param query: URL Query parameters.
         :type query: CreateQuery | QueryParamTypes, optional
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
         :param query['deprecatePrevious'] (dict) <br> query.deprecate_previous (Query) : Set the cleanup policy used to automatically deprecate/delete previous versions.
         :type query['deprecatePrevious']: DeprecatePreviousPolicy
         :param query['dryRun'] (dict) <br> query.dry_run (Query) : If set to <code>true</code>, validates the deployment conditions, but does not change anything.
         :type query['dryRun']: bool
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
+        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. Saves computing resources when the function is not to be used immediately.
+        :type query['scaleToZero']: bool
         :param query['version'] (dict) <br> query.version (Query) : If set, the function version will be an increment of the latest existing version that satisfies the `version` range. Note that this increment always takes precedence over an explicit `version` in the function manifest.
         :type query['version']: SemanticVersionRange
         :param query['name'] (dict) <br> query.name (Query) : If set, the value will be used as the function name instead of the one specified in the manifest.
         :type query['name']: str
         :param query['draft'] (dict) <br> query.draft (Query) : If set, the created function will be a draft function and its assets are still mutable. A build and deploy is initiated only in the case when all necessary assets are present and valid.
         :type query['draft']: bool
         :param query['runtime'] (dict) <br> query.runtime (Query) : If set, the created function will use the indicated runtime (latest version within specified range).  This takes precedence over the runtime specified in a function manifest (copied or from request body).
@@ -629,18 +627,14 @@
         :type name: str
         :param version: The version of the function. (required)
         :type version: str
         :param wildcard: Full path or path prefix of the asset within the archive (required)
         :type wildcard: str
         :param query: URL Query parameters.
         :type query: DeleteAssetQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['chown'] (dict) <br> query.chown (Query) : If set, ownership of the draft function is transferred to the current user.
         :type query['chown']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
@@ -2400,28 +2394,28 @@
         Rebuild and deploy a webscript with the original or updated base image.
         :param name: The name of the function. (required)
         :type name: str
         :param version: The version of the function. (required)
         :type version: str
         :param query: URL Query parameters.
         :type query: RebuildQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command.
-        :type query['scaleToZero']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['dryRun'] (dict) <br> query.dry_run (Query) : If set to <code>true</code>, checks whether rebuild jobs are needed, but do not start any jobs.
         :type query['dryRun']: bool
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
         :param query['upgrade'] (dict) <br> query.upgrade (Query) : If set, force a rebuild with the given <em>runtime</em> version selection policy. <ul>  <li><code>same</code> <b>patch</b> version.   This should only include backward compatible upgrades.  </li>  <li><code>minor</code> <b>major</b> version.   This might include an upgrade of e.g. the language runtime and/or provided   dependencies that could break compatiblity with the function. .</li> </ul>
         :type query['upgrade']: RebuildPolicy
         :param query['forceVersion'] (dict) <br> query.force_version (Query) : If set, force a rebuild with the given runtime version (including downgrades). This parameter is mutually exclusive to the `upgrade` parameter.
         :type query['forceVersion']: str
         :param query['ignoreChecks'] (dict) <br> query.ignore_checks (Query) : If set to true, checks that normally prevent a rebuild are overriden. These checks include: * function state in `pending`, `running`, `failed` or `undeployed` * backoff period due to recent failures * usage of deprecated dependencies * running jobs on entity * the `dryRun` option
         :type query['ignoreChecks']: bool
+        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful (re-)deployment. If not set, the function is scaled to zero only if it was not active before this command.
+        :type query['scaleToZero']: bool
         :param query['skipRebuild'] (dict) <br> query.skip_rebuild (Query) : If set, the function will not be rebuild. Always uses the current runtime version when re-deploying/re-verifying the function.
         :type query['skipRebuild']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
         :param headers: Header parameters for this request
@@ -2976,18 +2970,14 @@
         :type version: str
         :param wildcard: Full path or path prefix of the asset within the archive (required)
         :type wildcard: str
         :param content: A single asset file.
         :type content: ContentRequest, optional
         :param query: URL Query parameters.
         :type query: UpdateAssetQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['chown'] (dict) <br> query.chown (Query) : If set, ownership of the draft function is transferred to the current user.
         :type query['chown']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
@@ -3223,18 +3213,14 @@
         :type version: str
         :param content: The assets for a <em>webscript</em> function can be provided as either   <ul>     <li>a single <em>tar</em> archive (optionally compressed), with one of the content types      <code>application/octet-stream</code>, <code>application/tar</code>, <code>application/tar+gzip</code>, <code>application/x-gzip</code>, <code>application/x-tar</code>, <code>application/gzip</code></li>     <li>separate files in a <code>multipart/form-data</code> request</li>   </ul>    The provided assets will be added to the <em>webscript</em> function's collection of existing assets,   replacing any existing assets with the same name.    Please note that it is not allowed to update the webscript.json</code> json file with a changed value for any of the    <code>name</code>, <code>version</code> and/or <code>runtime</code> attributes.    For each <em>runtime</em> other files are supported.
         :type content: ContentRequest, optional
         :param files: The files of a `content-type: multipart/form-data` request.
         :type files: FilesRequest, optional
         :param query: URL Query parameters.
         :type query: UpdateAssetsQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately.
-        :type query['scaleToZero']: bool
-        :param query['deploy'] (dict) <br> query.deploy (Query) : Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage.
-        :type query['deploy']: bool
         :param query['chown'] (dict) <br> query.chown (Query) : If set, ownership of the draft function is transferred to the current user.
         :type query['chown']: bool
         :param query['comment'] (dict) <br> query.comment (Query) : An optional user-specified comment corresponding to the operation.
         :type query['comment']: str
         :param query['author'] (dict) <br> query.author (Query) : Optionally changes the author metadata when updating a function.
         :type query['author']: str
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
@@ -3412,18 +3398,18 @@
         Verify health of webscript deployed on openfaas.
         :param name: The name of the function. (required)
         :type name: str
         :param version: The version of the function. (required)
         :type version: str
         :param query: URL Query parameters.
         :type query: VerifyQuery | QueryParamTypes, optional
-        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command.
-        :type query['scaleToZero']: bool
         :param query['async'] (dict) <br> query.var_async (Query) : Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs.
         :type query['async']: bool
+        :param query['scaleToZero'] (dict) <br> query.scale_to_zero (Query) : Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command.
+        :type query['scaleToZero']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
```

### Comparing `waylay_sdk_registry-2.13.0b20240415/src/waylay/services/registry/service/service.py` & `waylay-sdk-registry-2.13.0rc0/src/waylay/services/registry/service/service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """Registry Service."""
 
 from waylay.sdk import ApiClient, WaylayService
 
-from ..api.about_api import AboutApi
+from ..api.default_api import DefaultApi
 from ..api.jobs_api import JobsApi
 from ..api.models_api import ModelsApi
 from ..api.plugs_api import PlugsApi
 from ..api.runtimes_api import RuntimesApi
 from ..api.schemas_api import SchemasApi
 from ..api.webscripts_api import WebscriptsApi
 
 
 class RegistryService(WaylayService):
     """Registry Service Class."""
 
     name = "registry"
     title = "Registry Service"
 
-    about: AboutApi
     jobs: JobsApi
     models: ModelsApi
     plugs: PlugsApi
     runtimes: RuntimesApi
     schemas: SchemasApi
     webscripts: WebscriptsApi
+    default: DefaultApi
 
     def __init__(self, api_client: ApiClient):
         """Create the registry service."""
 
         super().__init__(api_client)
-        self.about = AboutApi(api_client)
         self.jobs = JobsApi(api_client)
         self.models = ModelsApi(api_client)
         self.plugs = PlugsApi(api_client)
         self.runtimes = RuntimesApi(api_client)
         self.schemas = SchemasApi(api_client)
         self.webscripts = WebscriptsApi(api_client)
+        self.default = DefaultApi(api_client)
```

### Comparing `waylay_sdk_registry-2.13.0b20240415/src/waylay_sdk_registry.egg-info/PKG-INFO` & `waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-registry
-Version: 2.13.0b20240415
+Version: 2.13.0rc0
 Summary: Waylay Function Registry
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
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-registry-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/registry.html
 Keywords: Waylay Function Registry
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.0
+Requires-Dist: waylay-sdk~=0.0.4rc5
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -46,52 +45,57 @@
 Provides-Extra: types
 Requires-Dist: waylay-sdk-registry-types; extra == "types"
 
 # Waylay Registry Service
 V2 API to build and deploy Waylay functions (plugs, webscripts, BYOML models).
 
 This Python package is automatically generated based on the 
-Waylay Registry OpenAPI specification (API version: 2.13.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/registry.html).
+Waylay Registry OpenAPI specification (API version: 2.13.0-beta.0)
 
-It consists of a plugin for the waylay-sdk-core package, and contains the Registry api methods.
+It consists of a plugin for the waylay-sdk package, and contains the Registry api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-registry-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-registry is included in:
-- ```pip install waylay-sdk-core[registry]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[registry]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-registry and waylay-sdk-registry-types are included in:
-- ```pip install waylay-sdk-core[registry,registry-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[registry,registry-types]``` to install `waylay-sdk` along with only this service including the typed models, or
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
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-registry-types` is installed
-from waylay.services.registry.models.root_page_response import RootPageResponse
+from registry.models.function_type import FunctionType
+from registry.models.job_state_result import JobStateResult
+from registry.models.job_type_schema import JobTypeSchema
+from registry.models.jobs_response import JobsResponse
 try:
-    # Get Service Status
-    # calls `GET /registry/v2/`
-    api_response = await waylay_client.registry.about.get(
+    # List Jobs
+    # calls `GET /registry/v2/jobs/`
+    api_response = await waylay_client.registry.jobs.list(
+        # query parameters:
+        query = {
+        },
     )
-    print("The response of registry.about.get:\n")
+    print("The response of registry.jobs.list:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling registry.about.get: %s\n" % e)
+    print("Exception when calling registry.jobs.list: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_registry-2.13.0b20240415/src/waylay_sdk_registry.egg-info/SOURCES.txt` & `waylay-sdk-registry-2.13.0rc0/src/waylay_sdk_registry.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 LICENSE.txt
 README.md
 pyproject.toml
 src/waylay/services/registry/api/__init__.py
-src/waylay/services/registry/api/about_api.py
+src/waylay/services/registry/api/default_api.py
 src/waylay/services/registry/api/jobs_api.py
 src/waylay/services/registry/api/models_api.py
 src/waylay/services/registry/api/plugs_api.py
 src/waylay/services/registry/api/py.typed
 src/waylay/services/registry/api/runtimes_api.py
 src/waylay/services/registry/api/schemas_api.py
 src/waylay/services/registry/api/webscripts_api.py
```

