# Comparing `tmp/waylay_sdk_rules-6.5.0.20240423.tar.gz` & `tmp/waylay-sdk-rules-6.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk_rules-6.5.0.20240423.tar", last modified: Wed Apr 24 06:58:22 2024, max compression
+gzip compressed data, was "waylay-sdk-rules-6.5.0rc1.tar", last modified: Wed Mar 27 15:35:55 2024, max compression
```

## Comparing `waylay_sdk_rules-6.5.0.20240423.tar` & `waylay-sdk-rules-6.5.0rc1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:58:22.240153 waylay_sdk_rules-6.5.0.20240423/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-24 06:58:18.000000 waylay_sdk_rules-6.5.0.20240423/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-24 06:58:22.240153 waylay_sdk_rules-6.5.0.20240423/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-24 06:58:18.000000 waylay_sdk_rules-6.5.0.20240423/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-24 06:58:18.000000 waylay_sdk_rules-6.5.0.20240423/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 06:58:22.240153 waylay_sdk_rules-6.5.0.20240423/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:58:22.236153 waylay_sdk_rules-6.5.0.20240423/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:58:22.236153 waylay_sdk_rules-6.5.0.20240423/src/waylay/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:58:22.236153 waylay_sdk_rules-6.5.0.20240423/src/waylay/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:58:22.236153 waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:58:22.236153 waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/api/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-24 06:58:18.000000 waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-04-24 06:58:18.000000 waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/api/about_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    47021 2024-04-24 06:58:18.000000 waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/api/plugs_execution_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-04-24 06:58:18.000000 waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/api/push_data_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 06:58:18.000000 waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/api/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    28530 2024-04-24 06:58:18.000000 waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/api/task_nodes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    51392 2024-04-24 06:58:18.000000 waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/api/tasks_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14118 2024-04-24 06:58:18.000000 waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/api/tasks_batch_operations_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18357 2024-04-24 06:58:18.000000 waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/api/template_runs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    50333 2024-04-24 06:58:18.000000 waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/api/templates_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:58:22.240153 waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/service/
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-24 06:58:18.000000 waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 06:58:18.000000 waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/service/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-24 06:58:18.000000 waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 06:58:22.240153 waylay_sdk_rules-6.5.0.20240423/src/waylay_sdk_rules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-24 06:58:22.000000 waylay_sdk_rules-6.5.0.20240423/src/waylay_sdk_rules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-24 06:58:22.000000 waylay_sdk_rules-6.5.0.20240423/src/waylay_sdk_rules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 06:58:22.000000 waylay_sdk_rules-6.5.0.20240423/src/waylay_sdk_rules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 06:58:22.000000 waylay_sdk_rules-6.5.0.20240423/src/waylay_sdk_rules.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-24 06:58:22.000000 waylay_sdk_rules-6.5.0.20240423/src/waylay_sdk_rules.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 06:58:22.000000 waylay_sdk_rules-6.5.0.20240423/src/waylay_sdk_rules.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:55.224704 waylay-sdk-rules-6.5.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-03-27 15:35:55.224704 waylay-sdk-rules-6.5.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 15:35:55.224704 waylay-sdk-rules-6.5.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:55.216704 waylay-sdk-rules-6.5.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:55.216704 waylay-sdk-rules-6.5.0rc1/src/waylay/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:55.216704 waylay-sdk-rules-6.5.0rc1/src/waylay/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:55.216704 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:55.220704 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36569 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/plugs_execution_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/push_data_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    25993 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/task_nodes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46698 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/tasks_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/tasks_batch_operations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/template_runs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45622 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/version_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:55.220704 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/service/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-03-27 15:35:44.000000 waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:35:55.224704 waylay-sdk-rules-6.5.0rc1/src/waylay_sdk_rules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-03-27 15:35:55.000000 waylay-sdk-rules-6.5.0rc1/src/waylay_sdk_rules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-27 15:35:55.000000 waylay-sdk-rules-6.5.0rc1/src/waylay_sdk_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 15:35:55.000000 waylay-sdk-rules-6.5.0rc1/src/waylay_sdk_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-27 15:35:55.000000 waylay-sdk-rules-6.5.0rc1/src/waylay_sdk_rules.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-27 15:35:55.000000 waylay-sdk-rules-6.5.0rc1/src/waylay_sdk_rules.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-27 15:35:55.000000 waylay-sdk-rules-6.5.0rc1/src/waylay_sdk_rules.egg-info/top_level.txt
```

### Comparing `waylay_sdk_rules-6.5.0.20240423/LICENSE.txt` & `waylay-sdk-rules-6.5.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay_sdk_rules-6.5.0.20240423/PKG-INFO` & `waylay-sdk-rules-6.5.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-rules
-Version: 6.5.0.20240423
+Version: 6.5.0rc1
 Summary: Waylay rules engine
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,22 +13,22 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-rules-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/rules.html
 Keywords: Waylay rules engine
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.1
+Requires-Dist: waylay-sdk~=0.0.4rc5
+Requires-Dist: waylay-sdk-rules==6.5.0rc1
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -47,51 +47,53 @@
 Requires-Dist: waylay-sdk-rules-types; extra == "types"
 
 # Waylay Rules Service
 The REST api to manage rule tasks and rule templates in the Waylay platform.
 
 This Python package is automatically generated based on the 
 Waylay Rules OpenAPI specification (API version: 6.5.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/rules.html).
 
-It consists of a plugin for the waylay-sdk-core package, and contains the Rules api methods.
+It consists of a plugin for the waylay-sdk package, and contains the Rules api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-rules-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-rules is included in:
-- ```pip install waylay-sdk-core[rules]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[rules]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-rules and waylay-sdk-rules-types are included in:
-- ```pip install waylay-sdk-core[rules,rules-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[rules,rules-types]``` to install `waylay-sdk` along with only this service including the typed models, or
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
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-rules-types` is installed
-from waylay.services.rules.models.version_response import VersionResponse
+from rules.models.execute_plugs_specification import ExecutePlugsSpecification
+from rules.models.transformer_execution_result import TransformerExecutionResult
 try:
-    # Get Service Information
-    # calls `GET /rules/v1`
-    api_response = await waylay_client.rules.about.get(
+    # Execute Specified Transformer Version
+    # calls `POST /rules/v1/transformers/{name}/versions/{version}`
+    api_response = await waylay_client.rules.plugs_execution.execute_transformer_version(
+        'name_example', # name | path param "name"
+        'version_example', # version | path param "version"
     )
-    print("The response of rules.about.get:\n")
+    print("The response of rules.plugs_execution.execute_transformer_version:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling rules.about.get: %s\n" % e)
+    print("Exception when calling rules.plugs_execution.execute_transformer_version: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_rules-6.5.0.20240423/README.md` & `waylay-sdk-rules-6.5.0rc1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 # Waylay Rules Service
 The REST api to manage rule tasks and rule templates in the Waylay platform.
 
 This Python package is automatically generated based on the 
 Waylay Rules OpenAPI specification (API version: 6.5.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/rules.html).
 
-It consists of a plugin for the waylay-sdk-core package, and contains the Rules api methods.
+It consists of a plugin for the waylay-sdk package, and contains the Rules api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-rules-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-rules is included in:
-- ```pip install waylay-sdk-core[rules]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[rules]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-rules and waylay-sdk-rules-types are included in:
-- ```pip install waylay-sdk-core[rules,rules-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[rules,rules-types]``` to install `waylay-sdk` along with only this service including the typed models, or
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
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-rules-types` is installed
-from waylay.services.rules.models.version_response import VersionResponse
+from rules.models.execute_plugs_specification import ExecutePlugsSpecification
+from rules.models.transformer_execution_result import TransformerExecutionResult
 try:
-    # Get Service Information
-    # calls `GET /rules/v1`
-    api_response = await waylay_client.rules.about.get(
+    # Execute Specified Transformer Version
+    # calls `POST /rules/v1/transformers/{name}/versions/{version}`
+    api_response = await waylay_client.rules.plugs_execution.execute_transformer_version(
+        'name_example', # name | path param "name"
+        'version_example', # version | path param "version"
     )
-    print("The response of rules.about.get:\n")
+    print("The response of rules.plugs_execution.execute_transformer_version:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling rules.about.get: %s\n" % e)
+    print("Exception when calling rules.plugs_execution.execute_transformer_version: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_rules-6.5.0.20240423/pyproject.toml` & `waylay-sdk-rules-6.5.0rc1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-rules"
-version = "6.5.0.20240423"
+version = "6.5.0rc1"
 description = "Waylay rules engine"
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay rules engine"]
 requires-python = ">= 3.9"
 dependencies = [
-    "waylay-sdk-core ~= 0.2.1",
+    "waylay-sdk ~= 0.0.4rc5",
+    "waylay-sdk-rules == 6.5.0rc1",
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
 Repository = "https://github.com/waylayio/waylay-sdk-rules-py.git"
-"Openapi Specification" = "https://docs.waylay.io/openapi/public/redocly/rules.html"
 
 [project.optional-dependencies]
 dev = [
     "mypy",
     "ruff",
     "types-python-jose",
     "types-appdirs",
```

### Comparing `waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/api/__init__.py` & `waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Waylay rules engine: apis."""
 
 # import apis into api package
-from .about_api import AboutApi
 from .plugs_execution_api import PlugsExecutionApi
 from .push_data_api import PushDataApi
 from .task_nodes_api import TaskNodesApi
 from .tasks_api import TasksApi
 from .tasks_batch_operations_api import TasksBatchOperationsApi
 from .template_runs_api import TemplateRunsApi
 from .templates_api import TemplatesApi
+from .version_api import VersionApi
 
 __all__ = [
-    "AboutApi",
     "PlugsExecutionApi",
     "PushDataApi",
     "TaskNodesApi",
     "TasksApi",
     "TasksBatchOperationsApi",
     "TemplateRunsApi",
     "TemplatesApi",
+    "VersionApi",
 ]
```

### Comparing `waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/api/about_api.py` & `waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/version_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,35 +29,35 @@
     Response,
 )
 from waylay.sdk.api._models import Model
 from waylay.sdk.plugin import WithApiClient
 
 if TYPE_CHECKING:
     from waylay.services.rules.models import VersionResponse
-    from waylay.services.rules.queries.about_api import GetQuery
+    from waylay.services.rules.queries.version_api import GetQuery
 
 
 try:
     from waylay.services.rules.models import VersionResponse
-    from waylay.services.rules.queries.about_api import GetQuery
+    from waylay.services.rules.queries.version_api import GetQuery
 
     MODELS_AVAILABLE = True
 except ImportError:
     MODELS_AVAILABLE = False
 
     if not TYPE_CHECKING:
         GetQuery = dict
         VersionResponse = Model
 
 
 T = TypeVar("T")
 
 
-class AboutApi(WithApiClient):
-    """AboutApi service methods.
+class VersionApi(WithApiClient):
+    """VersionApi service methods.
 
     NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
@@ -65,92 +65,85 @@
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> VersionResponse: ...
 
     @overload
     async def get(
         self,
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
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> VersionResponse | T | Response | Model:
-        """Get Service Information.
+        """Get Version.
 
-        Get the name and version of the service.
+        Get the status and version of the service.
         :param query: URL Query parameters.
         :type query: GetQuery | QueryParamTypes, optional
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
@@ -161,22 +154,26 @@
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
             query = TypeAdapter(GetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": VersionResponse if not select_path else Model,
```

### Comparing `waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/api/plugs_execution_api.py` & `waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/tasks_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from __future__ import annotations  # for Python 3.7–3.9
 
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
+    List,
     Literal,
     TypeVar,
     overload,
 )
 
 from pydantic import (
     Field,
@@ -34,239 +35,199 @@
     Response,
 )
 from waylay.sdk.api._models import Model
 from waylay.sdk.plugin import WithApiClient
 
 if TYPE_CHECKING:
     from waylay.services.rules.models import (
-        ActuatorExecutionResult,
+        CreateTask201Response,
         ErrorResponse,
-        ExecutePlugsSpecification,
-        SensorExecutionResult,
-        TransformerExecutionResult,
+        ErrorWithDetailsResponse,
+        TaskEntity,
+        TaskSpecification,
     )
-    from waylay.services.rules.queries.plugs_execution_api import (
-        ExecuteActuatorQuery,
-        ExecuteActuatorVersionQuery,
-        ExecuteSensorQuery,
-        ExecuteSensorVersionQuery,
-        ExecuteTransformerQuery,
-        ExecuteTransformerVersionQuery,
+    from waylay.services.rules.queries.tasks_api import (
+        CreateQuery,
+        DeleteQuery,
+        GetConfigurationQuery,
+        GetQuery,
+        ListQuery,
+        ReplaceQuery,
+        StartQuery,
+        StopQuery,
     )
 
 
 try:
     from waylay.services.rules.models import (
-        ActuatorExecutionResult,
+        CreateTask201Response,
         ErrorResponse,
-        ExecutePlugsSpecification,
-        SensorExecutionResult,
-        TransformerExecutionResult,
+        ErrorWithDetailsResponse,
+        TaskEntity,
+        TaskSpecification,
     )
-    from waylay.services.rules.queries.plugs_execution_api import (
-        ExecuteActuatorQuery,
-        ExecuteActuatorVersionQuery,
-        ExecuteSensorQuery,
-        ExecuteSensorVersionQuery,
-        ExecuteTransformerQuery,
-        ExecuteTransformerVersionQuery,
+    from waylay.services.rules.queries.tasks_api import (
+        CreateQuery,
+        DeleteQuery,
+        GetConfigurationQuery,
+        GetQuery,
+        ListQuery,
+        ReplaceQuery,
+        StartQuery,
+        StopQuery,
     )
 
     MODELS_AVAILABLE = True
 except ImportError:
     MODELS_AVAILABLE = False
 
     if not TYPE_CHECKING:
-        ExecutePlugsSpecification = Model
+        TaskSpecification = Model
 
-        ExecuteActuatorQuery = dict
-        ActuatorExecutionResult = Model
+        CreateQuery = dict
+        CreateTask201Response = Model
 
-        ActuatorExecutionResult = Model
+        ErrorWithDetailsResponse = Model
 
-        ErrorResponse = Model
-
-        ExecutePlugsSpecification = Model
-
-        ExecuteActuatorVersionQuery = dict
-        ActuatorExecutionResult = Model
-
-        ActuatorExecutionResult = Model
+        DeleteQuery = dict
 
         ErrorResponse = Model
 
-        ExecutePlugsSpecification = Model
+        GetConfigurationQuery = dict
+        TaskSpecification = Model
 
-        ExecuteSensorQuery = dict
-        SensorExecutionResult = Model
+        ErrorResponse = Model
 
-        SensorExecutionResult = Model
+        GetQuery = dict
+        TaskEntity = Model
 
         ErrorResponse = Model
 
-        ExecutePlugsSpecification = Model
+        ListQuery = dict
+        TaskEntity = Model
 
-        ExecuteSensorVersionQuery = dict
-        SensorExecutionResult = Model
+        TaskSpecification = Model
 
-        SensorExecutionResult = Model
+        ReplaceQuery = dict
+        TaskEntity = Model
 
-        ErrorResponse = Model
-
-        ExecutePlugsSpecification = Model
+        ErrorWithDetailsResponse = Model
 
-        ExecuteTransformerQuery = dict
-        TransformerExecutionResult = Model
+        ErrorResponse = Model
 
-        TransformerExecutionResult = Model
+        StartQuery = dict
+        TaskEntity = Model
 
         ErrorResponse = Model
 
-        ExecutePlugsSpecification = Model
+        ErrorResponse = Model
 
-        ExecuteTransformerVersionQuery = dict
-        TransformerExecutionResult = Model
+        StopQuery = dict
+        TaskEntity = Model
 
-        TransformerExecutionResult = Model
+        ErrorResponse = Model
 
         ErrorResponse = Model
 
 
 T = TypeVar("T")
 
 
-class PlugsExecutionApi(WithApiClient):
-    """PlugsExecutionApi service methods.
+class TasksApi(WithApiClient):
+    """TasksApi service methods.
 
     NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     @overload
-    async def execute_actuator(
+    async def create(
         self,
-        name: StrictStr,
         *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteActuatorQuery | QueryParamTypes | None = None,
+        query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> ActuatorExecutionResult: ...
+    ) -> CreateTask201Response: ...
 
     @overload
-    async def execute_actuator(
+    async def create(
         self,
-        name: StrictStr,
         *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteActuatorQuery | QueryParamTypes | None = None,
+        query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
-    async def execute_actuator(
+    async def create(
         self,
-        name: StrictStr,
         *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteActuatorQuery | QueryParamTypes | None = None,
+        query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
-    async def execute_actuator(
+    async def create(
         self,
-        name: StrictStr,
         *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteActuatorQuery | QueryParamTypes | None = None,
+        query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
-    async def execute_actuator(
+    async def create(
         self,
-        name: StrictStr,
         *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteActuatorQuery | QueryParamTypes | None = None,
+        query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
-    async def execute_actuator(
+    async def create(
         self,
-        name: StrictStr,
         *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteActuatorQuery | QueryParamTypes | None = None,
+        query: CreateQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> ActuatorExecutionResult | T | Response | Model:
-        """Execute Latest Actuator Version.
+    ) -> CreateTask201Response | T | Response | Model:
+        """Create Task.
 
-        Execute latest version of an actuator.
-        :param name: (required)
-        :type name: str
-        :param json: Specification to execute a plug.
-        :type json: ExecutePlugsSpecification, optional
+        Create a new task.
         :param query: URL Query parameters.
-        :type query: ExecuteActuatorQuery | QueryParamTypes, optional
+        :type query: CreateQuery | QueryParamTypes, optional
+        :param query['failOnWarning'] (dict) <br> query.fail_on_warning (Query) : If `true` and there are task warnings, the response will be a `400 Validation failed`
+        :type query['failOnWarning']: bool
+        :param query['returnWarnings'] (dict) <br> query.return_warnings (Query) : If `true`, result body will contain a list of task warnings that where detected
+        :type query['returnWarnings']: bool
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
@@ -277,202 +238,290 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
+        # path parameters
+        path_params: Dict[str, str] = {}
+
+        ## named body parameters
+        body_args: Dict[str, Any] = {}
+
+        # query parameters
+        if query is not None and should_validate:
+            query = TypeAdapter(CreateQuery).validate_python(query)
+
+        response_types_map: Dict[str, Any] = (
+            {"2XX": response_type}
+            if response_type is not None
+            else {
+                "201": CreateTask201Response if not select_path else Model,
+            }
+        )
+        non_200_response_types_map: Dict[str, Any] = {
+            "400": ErrorWithDetailsResponse,
+        }
+        response_types_map.update(non_200_response_types_map)
+
+        ## peform request
+        return await self.api_client.request(
+            method="POST",
+            resource_path="/rules/v1/tasks",
+            path_params=path_params,
+            params=query,
+            **body_args,
+            headers=headers,
+            **kwargs,
+            response_type=response_types_map,
+            select_path=select_path,
+            raw_response=raw_response,
+        )
+
+    @overload
+    async def delete(
+        self,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        *,
+        query: DeleteQuery | QueryParamTypes | None = None,
+        raw_response: Literal[False] = False,
+        select_path: Literal[""] = "",
+        response_type: Literal[None] = None,
+        headers: HeaderTypes | None = None,
+        **kwargs,
+    ) -> None: ...
+
+    @overload
+    async def delete(
+        self,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        *,
+        query: DeleteQuery | QueryParamTypes | None = None,
+        raw_response: Literal[False] = False,
+        select_path: Literal[""] = "",
+        response_type: T,
+        headers: HeaderTypes | None = None,
+        **kwargs,
+    ) -> T: ...
+
+    @overload
+    async def delete(
+        self,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        *,
+        query: DeleteQuery | QueryParamTypes | None = None,
+        raw_response: Literal[True],
+        select_path: Literal["_not_used_"] = "_not_used_",
+        response_type: Literal[None] = None,  # not used
+        headers: HeaderTypes | None = None,
+        **kwargs,
+    ) -> Response: ...
+
+    @overload
+    async def delete(
+        self,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        *,
+        query: DeleteQuery | QueryParamTypes | None = None,
+        raw_response: Literal[False] = False,
+        select_path: str,
+        response_type: Literal[None] = None,
+        headers: HeaderTypes | None = None,
+        **kwargs,
+    ) -> None: ...
+
+    @overload
+    async def delete(
+        self,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        *,
+        query: DeleteQuery | QueryParamTypes | None = None,
+        raw_response: Literal[False] = False,
+        select_path: str,
+        response_type: T,
+        headers: HeaderTypes | None = None,
+        **kwargs,
+    ) -> T: ...
+
+    async def delete(
+        self,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        *,
+        query: DeleteQuery | QueryParamTypes | None = None,
+        raw_response: StrictBool = False,
+        select_path: str = "",
+        response_type: T | None = None,
+        headers: HeaderTypes | None = None,
+        **kwargs,
+    ) -> None | T | Response:
+        """Delete Task.
+
+        Delete a task.
+        :param task_id: Unique Task identifier (required)
+        :type task_id: str
+        :param query: URL Query parameters.
+        :type query: DeleteQuery | QueryParamTypes, optional
+        :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
+        :param select_path: Denotes the json path applied to the response object before returning it.
+                Set it to the empty string `""` to receive the full response object.
+        :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param headers: Header parameters for this request
+        :type headers: dict, optional
+        :param `**kwargs`: Additional parameters passed on to the http client.
+            See below.
+        :Keyword Arguments:
+            * timeout: a single numeric timeout in seconds,
+                or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
+            * stream: if true, the response will be in streaming mode
+            * cookies
+            * extensions
+            * auth
+            * follow_redirects: bool
+
+        :return: Returns the result object if the http request succeeded with status code '2XX'.
+        :raises APIError: If the http request has a status code different from `2XX`. This
+            object wraps both the http Response and any parsed data.
+        """
+
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
-            "name": str(name),
+            "taskId": str(task_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
-            body_adapter = TypeAdapter(
-                Annotated[
-                    ExecutePlugsSpecification,
-                    Field(description="Specification to execute a plug."),
-                ]
-            )
-            json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
-        body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
-            query = TypeAdapter(ExecuteActuatorQuery).validate_python(query)
+        if query is not None and should_validate:
+            query = TypeAdapter(DeleteQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
-                "200": ActuatorExecutionResult if not select_path else Model,
+                "204": None,
             }
         )
         non_200_response_types_map: Dict[str, Any] = {
-            "400": ActuatorExecutionResult,
-            "404": ErrorResponse,
+            "400": ErrorResponse,
         }
         response_types_map.update(non_200_response_types_map)
 
         ## peform request
         return await self.api_client.request(
-            method="POST",
-            resource_path="/rules/v1/actions/{name}",
+            method="DELETE",
+            resource_path="/rules/v1/tasks/{taskId}",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
-    async def execute_actuator_version(
+    async def get_configuration(
         self,
-        name: StrictStr,
-        version: Annotated[
-            str, Field(strict=True, description="Version number of plugin")
-        ],
-        *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteActuatorVersionQuery | QueryParamTypes | None = None,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        *,
+        query: GetConfigurationQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> ActuatorExecutionResult: ...
+    ) -> TaskSpecification: ...
 
     @overload
-    async def execute_actuator_version(
+    async def get_configuration(
         self,
-        name: StrictStr,
-        version: Annotated[
-            str, Field(strict=True, description="Version number of plugin")
-        ],
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteActuatorVersionQuery | QueryParamTypes | None = None,
+        query: GetConfigurationQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
-    async def execute_actuator_version(
+    async def get_configuration(
         self,
-        name: StrictStr,
-        version: Annotated[
-            str, Field(strict=True, description="Version number of plugin")
-        ],
-        *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteActuatorVersionQuery | QueryParamTypes | None = None,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        *,
+        query: GetConfigurationQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
-    async def execute_actuator_version(
+    async def get_configuration(
         self,
-        name: StrictStr,
-        version: Annotated[
-            str, Field(strict=True, description="Version number of plugin")
-        ],
-        *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteActuatorVersionQuery | QueryParamTypes | None = None,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        *,
+        query: GetConfigurationQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
-    async def execute_actuator_version(
+    async def get_configuration(
         self,
-        name: StrictStr,
-        version: Annotated[
-            str, Field(strict=True, description="Version number of plugin")
-        ],
-        *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteActuatorVersionQuery | QueryParamTypes | None = None,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        *,
+        query: GetConfigurationQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
-    async def execute_actuator_version(
+    async def get_configuration(
         self,
-        name: StrictStr,
-        version: Annotated[
-            str, Field(strict=True, description="Version number of plugin")
-        ],
-        *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteActuatorVersionQuery | QueryParamTypes | None = None,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        *,
+        query: GetConfigurationQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> ActuatorExecutionResult | T | Response | Model:
-        """Execute Specified Actuator Version.
+    ) -> TaskSpecification | T | Response | Model:
+        """Get Task Configuration.
 
-        Execute specified version of an actuator.
-        :param name: (required)
-        :type name: str
-        :param version: Version number of plugin (required)
-        :type version: str
-        :param json: Specification to execute a plug.
-        :type json: ExecutePlugsSpecification, optional
+        Getting the configuration of an existing task.
+        :param task_id: Unique Task identifier (required)
+        :type task_id: str
         :param query: URL Query parameters.
-        :type query: ExecuteActuatorVersionQuery | QueryParamTypes, optional
+        :type query: GetConfigurationQuery | QueryParamTypes, optional
+        :param query['format'] (dict) <br> query.format (Query) : Format of the graph definition
+        :type query['format']: ListTasksFormatParameter
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
@@ -483,183 +532,145 @@
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
-            "name": str(name),
-            "version": str(version),
+            "taskId": str(task_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
-            body_adapter = TypeAdapter(
-                Annotated[
-                    ExecutePlugsSpecification,
-                    Field(description="Specification to execute a plug."),
-                ]
-            )
-            json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
-        body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
-            query = TypeAdapter(ExecuteActuatorVersionQuery).validate_python(query)
+        if query is not None and should_validate:
+            query = TypeAdapter(GetConfigurationQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
-                "200": ActuatorExecutionResult if not select_path else Model,
+                "200": TaskSpecification if not select_path else Model,
             }
         )
         non_200_response_types_map: Dict[str, Any] = {
-            "400": ActuatorExecutionResult,
             "404": ErrorResponse,
         }
         response_types_map.update(non_200_response_types_map)
 
         ## peform request
         return await self.api_client.request(
-            method="POST",
-            resource_path="/rules/v1/actions/{name}/versions/{version}",
+            method="GET",
+            resource_path="/rules/v1/tasks/{taskId}/conf",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
-    async def execute_sensor(
+    async def get(
         self,
-        name: StrictStr,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteSensorQuery | QueryParamTypes | None = None,
+        query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> SensorExecutionResult: ...
+    ) -> TaskEntity: ...
 
     @overload
-    async def execute_sensor(
+    async def get(
         self,
-        name: StrictStr,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteSensorQuery | QueryParamTypes | None = None,
+        query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
-    async def execute_sensor(
+    async def get(
         self,
-        name: StrictStr,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteSensorQuery | QueryParamTypes | None = None,
+        query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
-    async def execute_sensor(
+    async def get(
         self,
-        name: StrictStr,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteSensorQuery | QueryParamTypes | None = None,
+        query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
-    async def execute_sensor(
+    async def get(
         self,
-        name: StrictStr,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteSensorQuery | QueryParamTypes | None = None,
+        query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
-    async def execute_sensor(
+    async def get(
         self,
-        name: StrictStr,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteSensorQuery | QueryParamTypes | None = None,
+        query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> SensorExecutionResult | T | Response | Model:
-        """Execute Latest Sensor Version.
+    ) -> TaskEntity | T | Response | Model:
+        """Retrieve Task Details.
 
-        Execute latest version of a sensor.
-        :param name: (required)
-        :type name: str
-        :param json: Specification to execute a plug.
-        :type json: ExecutePlugsSpecification, optional
+        Retrieve the details of a task.
+        :param task_id: Unique Task identifier (required)
+        :type task_id: str
         :param query: URL Query parameters.
-        :type query: ExecuteSensorQuery | QueryParamTypes, optional
+        :type query: GetQuery | QueryParamTypes, optional
+        :param query['format'] (dict) <br> query.format (Query) : Format of the graph definition
+        :type query['format']: ListTasksFormatParameter
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
@@ -670,202 +681,169 @@
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
-            "name": str(name),
+            "taskId": str(task_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
-            body_adapter = TypeAdapter(
-                Annotated[
-                    ExecutePlugsSpecification,
-                    Field(description="Specification to execute a plug."),
-                ]
-            )
-            json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
-        body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
-            query = TypeAdapter(ExecuteSensorQuery).validate_python(query)
+        if query is not None and should_validate:
+            query = TypeAdapter(GetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
-                "200": SensorExecutionResult if not select_path else Model,
+                "200": TaskEntity if not select_path else Model,
             }
         )
         non_200_response_types_map: Dict[str, Any] = {
-            "400": SensorExecutionResult,
             "404": ErrorResponse,
         }
         response_types_map.update(non_200_response_types_map)
 
         ## peform request
         return await self.api_client.request(
-            method="POST",
-            resource_path="/rules/v1/sensors/{name}",
+            method="GET",
+            resource_path="/rules/v1/tasks/{taskId}",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
-    async def execute_sensor_version(
+    async def list(
         self,
-        name: StrictStr,
-        version: Annotated[
-            str, Field(strict=True, description="Version number of plugin")
-        ],
-        *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteSensorVersionQuery | QueryParamTypes | None = None,
+        *,
+        query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> SensorExecutionResult: ...
+    ) -> List[TaskEntity]: ...
 
     @overload
-    async def execute_sensor_version(
+    async def list(
         self,
-        name: StrictStr,
-        version: Annotated[
-            str, Field(strict=True, description="Version number of plugin")
-        ],
         *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteSensorVersionQuery | QueryParamTypes | None = None,
+        query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
-    async def execute_sensor_version(
+    async def list(
         self,
-        name: StrictStr,
-        version: Annotated[
-            str, Field(strict=True, description="Version number of plugin")
-        ],
-        *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteSensorVersionQuery | QueryParamTypes | None = None,
+        *,
+        query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
-    async def execute_sensor_version(
+    async def list(
         self,
-        name: StrictStr,
-        version: Annotated[
-            str, Field(strict=True, description="Version number of plugin")
-        ],
-        *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteSensorVersionQuery | QueryParamTypes | None = None,
+        *,
+        query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
-    async def execute_sensor_version(
+    async def list(
         self,
-        name: StrictStr,
-        version: Annotated[
-            str, Field(strict=True, description="Version number of plugin")
-        ],
-        *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteSensorVersionQuery | QueryParamTypes | None = None,
+        *,
+        query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
-    async def execute_sensor_version(
+    async def list(
         self,
-        name: StrictStr,
-        version: Annotated[
-            str, Field(strict=True, description="Version number of plugin")
-        ],
-        *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteSensorVersionQuery | QueryParamTypes | None = None,
+        *,
+        query: ListQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> SensorExecutionResult | T | Response | Model:
-        """Execute Specified Sensor Version.
+    ) -> List[TaskEntity] | T | Response | Model:
+        """Query Multiple Tasks.
 
-        Execute the specified version of a sensor.
-        :param name: (required)
-        :type name: str
-        :param version: Version number of plugin (required)
-        :type version: str
-        :param json: Specification to execute a plug.
-        :type json: ExecutePlugsSpecification, optional
+        Query multiple tasks.
         :param query: URL Query parameters.
-        :type query: ExecuteSensorVersionQuery | QueryParamTypes, optional
+        :type query: ListQuery | QueryParamTypes, optional
+        :param query['hits'] (dict) <br> query.hits (Query) : (Paging) maximal number of items returned
+        :type query['hits']: int
+        :param query['startIndex'] (dict) <br> query.start_index (Query) : (Paging) items to skip in the listing
+        :type query['startIndex']: int
+        :param query['format'] (dict) <br> query.format (Query) : Format of the graph definition
+        :type query['format']: ListTasksFormatParameter
+        :param query['name'] (dict) <br> query.name (Query) :
+        :type query['name']: str
+        :param query['resource'] (dict) <br> query.resource (Query) :
+        :type query['resource']: str
+        :param query['resourceType'] (dict) <br> query.resource_type (Query) :
+        :type query['resourceType']: str
+        :param query['type'] (dict) <br> query.type (Query) :
+        :type query['type']: TaskScenarioType
+        :param query['status'] (dict) <br> query.status (Query) :
+        :type query['status']: TaskStatus
+        :param query['ids'] (dict) <br> query.ids (Query) :
+        :type query['ids']: List[str]
+        :param query['id'] (dict) <br> query.id (Query) :
+        :type query['id']: str
+        :param query['plugin'] (dict) <br> query.plugin (Query) :
+        :type query['plugin']: str
+        :param query['template'] (dict) <br> query.template (Query) :
+        :type query['template']: str
+        :param query['filter'] (dict) <br> query.filter (Query) : fuzzy search on multiple properties
+        :type query['filter']: str
+        :param query['tags.key'] (dict) <br> query.tags_key (Query) : Parameter is `form` style serialized, with explode: true  See [Query multiple tasks tag examples](/#/api/rules/?id=queryTagExamples)  You can add the same tag query parameter multiple times with different values, which will be applied with a logical OR.  You can specify the `tags.<key>` query parameter without a value, tasks which have a value for tag `<key>` will be returned
+        :type query['tags.key']: ListTasksTagsKeyParameter
+        :param query['finishedBefore'] (dict) <br> query.finished_before (Query) : Tasks stopped before provided time will be returned.
+        :type query['finishedBefore']: int
+        :param query['createdAfter'] (dict) <br> query.created_after (Query) : Tasks created after provided time will be returned.
+        :type query['createdAfter']: int
+        :param query['createdBefore'] (dict) <br> query.created_before (Query) : Tasks created before provided time will be returned
+        :type query['createdBefore']: int
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
@@ -876,183 +854,287 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
+        # path parameters
+        path_params: Dict[str, str] = {}
+
+        ## named body parameters
+        body_args: Dict[str, Any] = {}
+
+        # query parameters
+        if query is not None and should_validate:
+            query = TypeAdapter(ListQuery).validate_python(query)
+
+        response_types_map: Dict[str, Any] = (
+            {"2XX": response_type}
+            if response_type is not None
+            else {
+                "200": List[TaskEntity] if not select_path else Model,
+            }
+        )
+        non_200_response_types_map: Dict[str, Any] = {}
+        response_types_map.update(non_200_response_types_map)
+
+        ## peform request
+        return await self.api_client.request(
+            method="GET",
+            resource_path="/rules/v1/tasks",
+            path_params=path_params,
+            params=query,
+            **body_args,
+            headers=headers,
+            **kwargs,
+            response_type=response_types_map,
+            select_path=select_path,
+            raw_response=raw_response,
+        )
+
+    @overload
+    async def replace(
+        self,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        *,
+        query: ReplaceQuery | QueryParamTypes | None = None,
+        raw_response: Literal[False] = False,
+        select_path: Literal[""] = "",
+        response_type: Literal[None] = None,
+        headers: HeaderTypes | None = None,
+        **kwargs,
+    ) -> TaskEntity: ...
+
+    @overload
+    async def replace(
+        self,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        *,
+        query: ReplaceQuery | QueryParamTypes | None = None,
+        raw_response: Literal[False] = False,
+        select_path: Literal[""] = "",
+        response_type: T,
+        headers: HeaderTypes | None = None,
+        **kwargs,
+    ) -> T: ...
+
+    @overload
+    async def replace(
+        self,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        *,
+        query: ReplaceQuery | QueryParamTypes | None = None,
+        raw_response: Literal[True],
+        select_path: Literal["_not_used_"] = "_not_used_",
+        response_type: Literal[None] = None,  # not used
+        headers: HeaderTypes | None = None,
+        **kwargs,
+    ) -> Response: ...
+
+    @overload
+    async def replace(
+        self,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        *,
+        query: ReplaceQuery | QueryParamTypes | None = None,
+        raw_response: Literal[False] = False,
+        select_path: str,
+        response_type: Literal[None] = None,
+        headers: HeaderTypes | None = None,
+        **kwargs,
+    ) -> Model: ...
+
+    @overload
+    async def replace(
+        self,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        *,
+        query: ReplaceQuery | QueryParamTypes | None = None,
+        raw_response: Literal[False] = False,
+        select_path: str,
+        response_type: T,
+        headers: HeaderTypes | None = None,
+        **kwargs,
+    ) -> T: ...
+
+    async def replace(
+        self,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        *,
+        query: ReplaceQuery | QueryParamTypes | None = None,
+        raw_response: StrictBool = False,
+        select_path: str = "",
+        response_type: T | None = None,
+        headers: HeaderTypes | None = None,
+        **kwargs,
+    ) -> TaskEntity | T | Response | Model:
+        """Update Task.
+
+        Update a task.  Remark that the full specification of the task must be given
+        :param task_id: Unique Task identifier (required)
+        :type task_id: str
+        :param query: URL Query parameters.
+        :type query: ReplaceQuery | QueryParamTypes, optional
+        :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
+        :param select_path: Denotes the json path applied to the response object before returning it.
+                Set it to the empty string `""` to receive the full response object.
+        :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param headers: Header parameters for this request
+        :type headers: dict, optional
+        :param `**kwargs`: Additional parameters passed on to the http client.
+            See below.
+        :Keyword Arguments:
+            * timeout: a single numeric timeout in seconds,
+                or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
+            * stream: if true, the response will be in streaming mode
+            * cookies
+            * extensions
+            * auth
+            * follow_redirects: bool
+
+        :return: Returns the result object if the http request succeeded with status code '2XX'.
+        :raises APIError: If the http request has a status code different from `2XX`. This
+            object wraps both the http Response and any parsed data.
+        """
+
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
-            "name": str(name),
-            "version": str(version),
+            "taskId": str(task_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
-            body_adapter = TypeAdapter(
-                Annotated[
-                    ExecutePlugsSpecification,
-                    Field(description="Specification to execute a plug."),
-                ]
-            )
-            json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
-        body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
-            query = TypeAdapter(ExecuteSensorVersionQuery).validate_python(query)
+        if query is not None and should_validate:
+            query = TypeAdapter(ReplaceQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
-                "200": SensorExecutionResult if not select_path else Model,
+                "200": TaskEntity if not select_path else Model,
             }
         )
         non_200_response_types_map: Dict[str, Any] = {
-            "400": SensorExecutionResult,
+            "400": ErrorWithDetailsResponse,
             "404": ErrorResponse,
         }
         response_types_map.update(non_200_response_types_map)
 
         ## peform request
         return await self.api_client.request(
-            method="POST",
-            resource_path="/rules/v1/sensors/{name}/versions/{version}",
+            method="PUT",
+            resource_path="/rules/v1/tasks/{taskId}",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
-    async def execute_transformer(
+    async def start(
         self,
-        name: StrictStr,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteTransformerQuery | QueryParamTypes | None = None,
+        query: StartQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> TransformerExecutionResult: ...
+    ) -> TaskEntity: ...
 
     @overload
-    async def execute_transformer(
+    async def start(
         self,
-        name: StrictStr,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteTransformerQuery | QueryParamTypes | None = None,
+        query: StartQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
-    async def execute_transformer(
+    async def start(
         self,
-        name: StrictStr,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteTransformerQuery | QueryParamTypes | None = None,
+        query: StartQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
-    async def execute_transformer(
+    async def start(
         self,
-        name: StrictStr,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteTransformerQuery | QueryParamTypes | None = None,
+        query: StartQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
-    async def execute_transformer(
+    async def start(
         self,
-        name: StrictStr,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteTransformerQuery | QueryParamTypes | None = None,
+        query: StartQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
-    async def execute_transformer(
+    async def start(
         self,
-        name: StrictStr,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteTransformerQuery | QueryParamTypes | None = None,
+        query: StartQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> TransformerExecutionResult | T | Response | Model:
-        """Execute Latest Transformer Version.
+    ) -> TaskEntity | T | Response | Model:
+        """Start Task.
 
-        Execute the latest transformer version.
-        :param name: (required)
-        :type name: str
-        :param json: Specification to execute a plug.
-        :type json: ExecutePlugsSpecification, optional
+        Start a task.
+        :param task_id: Unique Task identifier (required)
+        :type task_id: str
         :param query: URL Query parameters.
-        :type query: ExecuteTransformerQuery | QueryParamTypes, optional
+        :type query: StartQuery | QueryParamTypes, optional
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
@@ -1063,202 +1145,144 @@
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
-            "name": str(name),
+            "taskId": str(task_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
-            body_adapter = TypeAdapter(
-                Annotated[
-                    ExecutePlugsSpecification,
-                    Field(description="Specification to execute a plug."),
-                ]
-            )
-            json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
-        body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
-            query = TypeAdapter(ExecuteTransformerQuery).validate_python(query)
+        if query is not None and should_validate:
+            query = TypeAdapter(StartQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
-                "200": TransformerExecutionResult if not select_path else Model,
+                "200": TaskEntity if not select_path else Model,
             }
         )
         non_200_response_types_map: Dict[str, Any] = {
-            "400": TransformerExecutionResult,
+            "400": ErrorResponse,
             "404": ErrorResponse,
         }
         response_types_map.update(non_200_response_types_map)
 
         ## peform request
         return await self.api_client.request(
             method="POST",
-            resource_path="/rules/v1/transformers/{name}",
+            resource_path="/rules/v1/tasks/{taskId}/command/start",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
-    async def execute_transformer_version(
+    async def stop(
         self,
-        name: StrictStr,
-        version: Annotated[
-            str, Field(strict=True, description="Version number of plugin")
-        ],
-        *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteTransformerVersionQuery | QueryParamTypes | None = None,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        *,
+        query: StopQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> TransformerExecutionResult: ...
+    ) -> TaskEntity: ...
 
     @overload
-    async def execute_transformer_version(
+    async def stop(
         self,
-        name: StrictStr,
-        version: Annotated[
-            str, Field(strict=True, description="Version number of plugin")
-        ],
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteTransformerVersionQuery | QueryParamTypes | None = None,
+        query: StopQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
-    async def execute_transformer_version(
+    async def stop(
         self,
-        name: StrictStr,
-        version: Annotated[
-            str, Field(strict=True, description="Version number of plugin")
-        ],
-        *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteTransformerVersionQuery | QueryParamTypes | None = None,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        *,
+        query: StopQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
-    async def execute_transformer_version(
+    async def stop(
         self,
-        name: StrictStr,
-        version: Annotated[
-            str, Field(strict=True, description="Version number of plugin")
-        ],
-        *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteTransformerVersionQuery | QueryParamTypes | None = None,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        *,
+        query: StopQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
-    async def execute_transformer_version(
+    async def stop(
         self,
-        name: StrictStr,
-        version: Annotated[
-            str, Field(strict=True, description="Version number of plugin")
-        ],
-        *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteTransformerVersionQuery | QueryParamTypes | None = None,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        *,
+        query: StopQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
-    async def execute_transformer_version(
+    async def stop(
         self,
-        name: StrictStr,
-        version: Annotated[
-            str, Field(strict=True, description="Version number of plugin")
-        ],
-        *,
-        json: Annotated[
-            ExecutePlugsSpecification,
-            Field(description="Specification to execute a plug."),
-        ],
-        query: ExecuteTransformerVersionQuery | QueryParamTypes | None = None,
+        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        *,
+        query: StopQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> TransformerExecutionResult | T | Response | Model:
-        """Execute Specified Transformer Version.
+    ) -> TaskEntity | T | Response | Model:
+        """Stop Task.
 
-        Execute specified version of a transformer.
-        :param name: (required)
-        :type name: str
-        :param version: Version number of plugin (required)
-        :type version: str
-        :param json: Specification to execute a plug.
-        :type json: ExecutePlugsSpecification, optional
+        Stop a task.
+        :param task_id: Unique Task identifier (required)
+        :type task_id: str
         :param query: URL Query parameters.
-        :type query: ExecuteTransformerVersionQuery | QueryParamTypes, optional
+        :type query: StopQuery | QueryParamTypes, optional
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
@@ -1269,53 +1293,47 @@
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
-            "name": str(name),
-            "version": str(version),
+            "taskId": str(task_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
-            body_adapter = TypeAdapter(
-                Annotated[
-                    ExecutePlugsSpecification,
-                    Field(description="Specification to execute a plug."),
-                ]
-            )
-            json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
-        body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
-            query = TypeAdapter(ExecuteTransformerVersionQuery).validate_python(query)
+        if query is not None and should_validate:
+            query = TypeAdapter(StopQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
-                "200": TransformerExecutionResult if not select_path else Model,
+                "200": TaskEntity if not select_path else Model,
             }
         )
         non_200_response_types_map: Dict[str, Any] = {
-            "400": TransformerExecutionResult,
+            "400": ErrorResponse,
             "404": ErrorResponse,
         }
         response_types_map.update(non_200_response_types_map)
 
         ## peform request
         return await self.api_client.request(
             method="POST",
-            resource_path="/rules/v1/transformers/{name}/versions/{version}",
+            resource_path="/rules/v1/tasks/{taskId}/command/stop",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
```

### Comparing `waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/api/push_data_api.py` & `waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/push_data_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,21 +16,17 @@
     Dict,
     Literal,
     TypeVar,
     overload,
 )
 
 from pydantic import (
-    Field,
     StrictBool,
     TypeAdapter,
 )
-from typing_extensions import (
-    Annotated,  # >=3.9,
-)
 from waylay.sdk.api import (
     HeaderTypes,
     QueryParamTypes,
     Response,
 )
 from waylay.sdk.api._models import Model
 from waylay.sdk.plugin import WithApiClient
@@ -68,116 +64,89 @@
     Do not edit the class manually.
     """
 
     @overload
     async def push(
         self,
         *,
-        json: Annotated[
-            StreamData, Field(description="Push (real-time) Data Specification")
-        ],
         query: PushQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> object: ...
 
     @overload
     async def push(
         self,
         *,
-        json: Annotated[
-            StreamData, Field(description="Push (real-time) Data Specification")
-        ],
         query: PushQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def push(
         self,
         *,
-        json: Annotated[
-            StreamData, Field(description="Push (real-time) Data Specification")
-        ],
         query: PushQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def push(
         self,
         *,
-        json: Annotated[
-            StreamData, Field(description="Push (real-time) Data Specification")
-        ],
         query: PushQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def push(
         self,
         *,
-        json: Annotated[
-            StreamData, Field(description="Push (real-time) Data Specification")
-        ],
         query: PushQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def push(
         self,
         *,
-        json: Annotated[
-            StreamData, Field(description="Push (real-time) Data Specification")
-        ],
         query: PushQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> object | T | Response | Model:
         """Push Streaming Data.
 
         Push (real-time) streaming data.
-        :param json: Push (real-time) Data Specification
-        :type json: StreamData, optional
         :param query: URL Query parameters.
         :type query: PushQuery | QueryParamTypes, optional
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
@@ -188,30 +157,26 @@
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
-        if json is not None and validate_request:
-            body_adapter = TypeAdapter(
-                Annotated[
-                    StreamData, Field(description="Push (real-time) Data Specification")
-                ]
-            )
-            json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
-        body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(PushQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": object if not select_path else Model,
```

### Comparing `waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/api/task_nodes_api.py` & `waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/task_nodes_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 )
 from typing_extensions import (
     Annotated,  # >=3.9,
 )
 from waylay.sdk.api import (
     HeaderTypes,
     QueryParamTypes,
-    RequestContent,
     Response,
 )
 from waylay.sdk.api._models import Model
 from waylay.sdk.plugin import WithApiClient
 
 if TYPE_CHECKING:
     from waylay.services.rules.models import ErrorResponse, NodeStateSpecification
@@ -96,89 +95,83 @@
         task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
         *,
         query: GetStatesQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> object: ...
 
     @overload
     async def get_states(
         self,
         task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
         *,
         query: GetStatesQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get_states(
         self,
         task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
         *,
         query: GetStatesQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get_states(
         self,
         task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
         *,
         query: GetStatesQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get_states(
         self,
         task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
         *,
         query: GetStatesQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get_states(
         self,
         task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
         *,
         query: GetStatesQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> object | T | Response | Model:
         """Get Supported States.
 
         Get the supported states of a node.  #### visibility This definition has visibility status `deprecated`.
         :param task_id: Unique Task identifier (required)
@@ -187,15 +180,14 @@
         :type node_id: str
         :param query: URL Query parameters.
         :type query: GetStatesQuery | QueryParamTypes, optional
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
@@ -206,25 +198,29 @@
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
             "taskId": str(task_id),
             "nodeId": str(node_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetStatesQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": object if not select_path else Model,
@@ -253,89 +249,83 @@
         task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> object: ...
 
     @overload
     async def get(
         self,
         task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
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
         task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
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
         task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
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
         task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
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
         task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> object | T | Response | Model:
         """Get Current States.
 
         Get current states (posteriors) and raw data of the node.  #### visibility This definition has visibility status `deprecated`.
         :param task_id: Unique Task identifier (required)
@@ -344,15 +334,14 @@
         :type node_id: str
         :param query: URL Query parameters.
         :type query: GetQuery | QueryParamTypes, optional
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
@@ -363,25 +352,29 @@
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
             "taskId": str(task_id),
             "nodeId": str(node_id),
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
                 "200": object if not select_path else Model,
@@ -413,15 +406,14 @@
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
         *,
         json: NodeStateSpecification,
         query: PatchQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> object: ...
 
     @overload
     async def patch(
         self,
@@ -429,15 +421,14 @@
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
         *,
         json: NodeStateSpecification,
         query: PatchQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def patch(
         self,
@@ -445,15 +436,14 @@
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
         *,
         json: NodeStateSpecification,
         query: PatchQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def patch(
         self,
@@ -461,15 +451,14 @@
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
         *,
         json: NodeStateSpecification,
         query: PatchQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def patch(
         self,
@@ -477,30 +466,28 @@
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
         *,
         json: NodeStateSpecification,
         query: PatchQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def patch(
         self,
         task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
         *,
         json: NodeStateSpecification,
         query: PatchQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> object | T | Response | Model:
         """Set Node State.
 
         Set the current state and rawData for the node. This can only be done for a running task
         :param task_id: Unique Task identifier (required)
@@ -511,15 +498,14 @@
         :type json: NodeStateSpecification, optional
         :param query: URL Query parameters.
         :type query: PatchQuery | QueryParamTypes, optional
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
@@ -530,29 +516,33 @@
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
             "taskId": str(task_id),
             "nodeId": str(node_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
+        if json is not None and should_validate:
             body_adapter = TypeAdapter(NodeStateSpecification)
             json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
         body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(PatchQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": object if not select_path else Model,
@@ -580,136 +570,103 @@
 
     @overload
     async def update(
         self,
         task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
         *,
-        content: Annotated[
-            RequestContent | None,
-            Field(description="Command string to apply to a node of a task."),
-        ] = None,
         query: UpdateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> object: ...
 
     @overload
     async def update(
         self,
         task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
         *,
-        content: Annotated[
-            RequestContent | None,
-            Field(description="Command string to apply to a node of a task."),
-        ] = None,
         query: UpdateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def update(
         self,
         task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
         *,
-        content: Annotated[
-            RequestContent | None,
-            Field(description="Command string to apply to a node of a task."),
-        ] = None,
         query: UpdateQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def update(
         self,
         task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
         *,
-        content: Annotated[
-            RequestContent | None,
-            Field(description="Command string to apply to a node of a task."),
-        ] = None,
         query: UpdateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def update(
         self,
         task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
         *,
-        content: Annotated[
-            RequestContent | None,
-            Field(description="Command string to apply to a node of a task."),
-        ] = None,
         query: UpdateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def update(
         self,
         task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         node_id: Annotated[StrictStr, Field(description="Unique node label")],
         *,
-        content: Annotated[
-            RequestContent | None,
-            Field(description="Command string to apply to a node of a task."),
-        ] = None,
         query: UpdateQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> object | T | Response | Model:
         """Set Current State.
 
         Set the current state of the node.  This call is deprecated. Please use `PATCH /rules/v1/tasks/{taskId}/nodes/{nodeId}`  #### visibility This definition has visibility status `deprecated`.
         :param task_id: Unique Task identifier (required)
         :type task_id: str
         :param node_id: Unique node label (required)
         :type node_id: str
-        :param content: Command string to apply to a node of a task.
-        :type content: ContentRequest, optional
         :param query: URL Query parameters.
         :type query: UpdateQuery | QueryParamTypes, optional
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
@@ -720,26 +677,29 @@
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
             "taskId": str(task_id),
             "nodeId": str(node_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        body_args["content"] = content
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(UpdateQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": object if not select_path else Model,
```

### Comparing `waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/api/tasks_api.py` & `waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/templates_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -35,214 +35,201 @@
     Response,
 )
 from waylay.sdk.api._models import Model
 from waylay.sdk.plugin import WithApiClient
 
 if TYPE_CHECKING:
     from waylay.services.rules.models import (
-        CreateTask201Response,
+        CreateTemplate201Response,
         ErrorResponse,
         ErrorWithDetailsResponse,
-        TaskEntity,
-        TaskSpecification,
+        ReplaceTemplate200Response,
+        TemplateDetails,
+        TemplateEntity,
+        TemplateEntityMetadata,
+        TemplateModification,
+        UpgradePluginsTemplates200Response,
     )
-    from waylay.services.rules.queries.tasks_api import (
+    from waylay.services.rules.queries.templates_api import (
         CreateQuery,
         DeleteQuery,
-        GetConfigurationQuery,
+        GetDiscoveryQuery,
         GetQuery,
         ListQuery,
         ReplaceQuery,
-        StartQuery,
-        StopQuery,
+        SetQuery,
+        UpgradePluginsQuery,
     )
 
 
 try:
     from waylay.services.rules.models import (
-        CreateTask201Response,
+        CreateTemplate201Response,
         ErrorResponse,
         ErrorWithDetailsResponse,
-        TaskEntity,
-        TaskSpecification,
+        ReplaceTemplate200Response,
+        TemplateDetails,
+        TemplateEntity,
+        TemplateEntityMetadata,
+        TemplateModification,
+        UpgradePluginsTemplates200Response,
     )
-    from waylay.services.rules.queries.tasks_api import (
+    from waylay.services.rules.queries.templates_api import (
         CreateQuery,
         DeleteQuery,
-        GetConfigurationQuery,
+        GetDiscoveryQuery,
         GetQuery,
         ListQuery,
         ReplaceQuery,
-        StartQuery,
-        StopQuery,
+        SetQuery,
+        UpgradePluginsQuery,
     )
 
     MODELS_AVAILABLE = True
 except ImportError:
     MODELS_AVAILABLE = False
 
     if not TYPE_CHECKING:
-        TaskSpecification = Model
+        TemplateEntity = Model
 
         CreateQuery = dict
-        CreateTask201Response = Model
+        CreateTemplate201Response = Model
 
         ErrorWithDetailsResponse = Model
 
         DeleteQuery = dict
 
         ErrorResponse = Model
 
-        GetConfigurationQuery = dict
-        TaskSpecification = Model
-
         ErrorResponse = Model
 
+        GetDiscoveryQuery = dict
+        TemplateDetails = Model
+
         GetQuery = dict
-        TaskEntity = Model
+        TemplateDetails = Model
 
         ErrorResponse = Model
 
         ListQuery = dict
-        TaskEntity = Model
+        TemplateEntityMetadata = Model
 
-        TaskSpecification = Model
+        TemplateEntity = Model
 
         ReplaceQuery = dict
-        TaskEntity = Model
+        ReplaceTemplate200Response = Model
 
         ErrorWithDetailsResponse = Model
 
         ErrorResponse = Model
 
-        StartQuery = dict
-        TaskEntity = Model
+        SetQuery = dict
+        TemplateDetails = Model
 
         ErrorResponse = Model
 
-        ErrorResponse = Model
+        TemplateModification = Model
 
-        StopQuery = dict
-        TaskEntity = Model
-
-        ErrorResponse = Model
+        UpgradePluginsQuery = dict
+        UpgradePluginsTemplates200Response = Model
 
         ErrorResponse = Model
 
 
 T = TypeVar("T")
 
 
-class TasksApi(WithApiClient):
-    """TasksApi service methods.
+class TemplatesApi(WithApiClient):
+    """TemplatesApi service methods.
 
     NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     @overload
     async def create(
         self,
         *,
-        json: Annotated[TaskSpecification, Field(description="Task Specification")],
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> CreateTask201Response: ...
+    ) -> CreateTemplate201Response: ...
 
     @overload
     async def create(
         self,
         *,
-        json: Annotated[TaskSpecification, Field(description="Task Specification")],
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
         *,
-        json: Annotated[TaskSpecification, Field(description="Task Specification")],
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
         *,
-        json: Annotated[TaskSpecification, Field(description="Task Specification")],
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
         *,
-        json: Annotated[TaskSpecification, Field(description="Task Specification")],
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
         *,
-        json: Annotated[TaskSpecification, Field(description="Task Specification")],
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> CreateTask201Response | T | Response | Model:
-        """Create Task.
+    ) -> CreateTemplate201Response | T | Response | Model:
+        """Create Template.
 
-        Create a new task.
-        :param json: Task Specification
-        :type json: TaskSpecification, optional
+        Create a template.
         :param query: URL Query parameters.
         :type query: CreateQuery | QueryParamTypes, optional
-        :param query['failOnWarning'] (dict) <br> query.fail_on_warning (Query) : If `true` and there are task warnings, the response will be a `400 Validation failed`
-        :type query['failOnWarning']: bool
-        :param query['returnWarnings'] (dict) <br> query.return_warnings (Query) : If `true`, result body will contain a list of task warnings that where detected
-        :type query['returnWarnings']: bool
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
@@ -253,150 +240,141 @@
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
-        if json is not None and validate_request:
-            body_adapter = TypeAdapter(
-                Annotated[TaskSpecification, Field(description="Task Specification")]
-            )
-            json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
-        body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(CreateQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
-                "201": CreateTask201Response if not select_path else Model,
+                "201": CreateTemplate201Response if not select_path else Model,
             }
         )
         non_200_response_types_map: Dict[str, Any] = {
             "400": ErrorWithDetailsResponse,
         }
         response_types_map.update(non_200_response_types_map)
 
         ## peform request
         return await self.api_client.request(
             method="POST",
-            resource_path="/rules/v1/tasks",
+            resource_path="/rules/v1/templates",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
     async def delete(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> None: ...
 
     @overload
     async def delete(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def delete(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def delete(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> None: ...
 
     @overload
     async def delete(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def delete(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> None | T | Response:
-        """Delete Task.
+        """Delete Template.
 
-        Delete a task.
-        :param task_id: Unique Task identifier (required)
-        :type task_id: str
+        Delete a template.
+        :param name: Unique Template identifier (required)
+        :type name: str
         :param query: URL Query parameters.
         :type query: DeleteQuery | QueryParamTypes, optional
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
@@ -407,148 +385,136 @@
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
-            "taskId": str(task_id),
+            "name": str(name),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(DeleteQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "204": None,
             }
         )
         non_200_response_types_map: Dict[str, Any] = {
             "400": ErrorResponse,
+            "404": ErrorResponse,
         }
         response_types_map.update(non_200_response_types_map)
 
         ## peform request
         return await self.api_client.request(
             method="DELETE",
-            resource_path="/rules/v1/tasks/{taskId}",
+            resource_path="/rules/v1/templates/{name}",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
-    async def get_configuration(
+    async def get_discovery(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        query: GetConfigurationQuery | QueryParamTypes | None = None,
+        query: GetDiscoveryQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> TaskSpecification: ...
+    ) -> TemplateDetails | None: ...
 
     @overload
-    async def get_configuration(
+    async def get_discovery(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        query: GetConfigurationQuery | QueryParamTypes | None = None,
+        query: GetDiscoveryQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
-    async def get_configuration(
+    async def get_discovery(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        query: GetConfigurationQuery | QueryParamTypes | None = None,
+        query: GetDiscoveryQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
-    async def get_configuration(
+    async def get_discovery(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        query: GetConfigurationQuery | QueryParamTypes | None = None,
+        query: GetDiscoveryQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
-    async def get_configuration(
+    async def get_discovery(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        query: GetConfigurationQuery | QueryParamTypes | None = None,
+        query: GetDiscoveryQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
-    async def get_configuration(
+    async def get_discovery(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        query: GetConfigurationQuery | QueryParamTypes | None = None,
+        query: GetDiscoveryQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> TaskSpecification | T | Response | Model:
-        """Get Task Configuration.
+    ) -> TemplateDetails | None | T | Response | Model:
+        """Retrieve Discovery Template.
 
-        Getting the configuration of an existing task.
-        :param task_id: Unique Task identifier (required)
-        :type task_id: str
+        Get the discovery template.
         :param query: URL Query parameters.
-        :type query: GetConfigurationQuery | QueryParamTypes, optional
-        :param query['format'] (dict) <br> query.format (Query) : Format of the graph definition
-        :type query['format']: ListTasksFormatParameter
+        :type query: GetDiscoveryQuery | QueryParamTypes, optional
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
@@ -559,148 +525,142 @@
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
-        path_params: Dict[str, str] = {
-            "taskId": str(task_id),
-        }
+        path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
-            query = TypeAdapter(GetConfigurationQuery).validate_python(query)
+        if query is not None and should_validate:
+            query = TypeAdapter(GetDiscoveryQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
-                "200": TaskSpecification if not select_path else Model,
+                "200": TemplateDetails if not select_path else Model,
+                "204": None,
             }
         )
-        non_200_response_types_map: Dict[str, Any] = {
-            "404": ErrorResponse,
-        }
+        non_200_response_types_map: Dict[str, Any] = {}
         response_types_map.update(non_200_response_types_map)
 
         ## peform request
         return await self.api_client.request(
             method="GET",
-            resource_path="/rules/v1/tasks/{taskId}/conf",
+            resource_path="/rules/v1/discoveryTemplate",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
     async def get(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> TaskEntity: ...
+    ) -> TemplateDetails: ...
 
     @overload
     async def get(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
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
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
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
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
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
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
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
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> TaskEntity | T | Response | Model:
-        """Retrieve Task Details.
+    ) -> TemplateDetails | T | Response | Model:
+        """Retrieve Template Details.
 
-        Retrieve the details of a task.
-        :param task_id: Unique Task identifier (required)
-        :type task_id: str
+        Retrieve the details of a template.
+        :param name: Unique Template identifier (required)
+        :type name: str
         :param query: URL Query parameters.
         :type query: GetQuery | QueryParamTypes, optional
         :param query['format'] (dict) <br> query.format (Query) : Format of the graph definition
         :type query['format']: ListTasksFormatParameter
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
@@ -711,42 +671,46 @@
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
-            "taskId": str(task_id),
+            "name": str(name),
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
-                "200": TaskEntity if not select_path else Model,
+                "200": TemplateDetails if not select_path else Model,
             }
         )
         non_200_response_types_map: Dict[str, Any] = {
             "404": ErrorResponse,
         }
         response_types_map.update(non_200_response_types_map)
 
         ## peform request
         return await self.api_client.request(
             method="GET",
-            resource_path="/rules/v1/tasks/{taskId}",
+            resource_path="/rules/v1/templates/{name}",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
@@ -757,126 +721,99 @@
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
-    ) -> List[TaskEntity]: ...
+    ) -> List[TemplateEntityMetadata]: ...
 
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
-    ) -> List[TaskEntity] | T | Response | Model:
-        """Query Multiple Tasks.
+    ) -> List[TemplateEntityMetadata] | T | Response | Model:
+        """List Templates.
 
-        Query multiple tasks.
+        Query templates.
         :param query: URL Query parameters.
         :type query: ListQuery | QueryParamTypes, optional
         :param query['hits'] (dict) <br> query.hits (Query) : (Paging) maximal number of items returned
         :type query['hits']: int
         :param query['startIndex'] (dict) <br> query.start_index (Query) : (Paging) items to skip in the listing
         :type query['startIndex']: int
-        :param query['format'] (dict) <br> query.format (Query) : Format of the graph definition
-        :type query['format']: ListTasksFormatParameter
-        :param query['name'] (dict) <br> query.name (Query) :
-        :type query['name']: str
-        :param query['resource'] (dict) <br> query.resource (Query) :
-        :type query['resource']: str
-        :param query['resourceType'] (dict) <br> query.resource_type (Query) :
-        :type query['resourceType']: str
-        :param query['type'] (dict) <br> query.type (Query) :
-        :type query['type']: TaskScenarioType
-        :param query['status'] (dict) <br> query.status (Query) :
-        :type query['status']: TaskStatus
-        :param query['ids'] (dict) <br> query.ids (Query) :
+        :param query['filter'] (dict) <br> query.filter (Query) : fuzzy search on multiple properties
+        :type query['filter']: str
+        :param query['ids'] (dict) <br> query.ids (Query) : comma separated string of template names
         :type query['ids']: List[str]
-        :param query['id'] (dict) <br> query.id (Query) :
+        :param query['id'] (dict) <br> query.id (Query) : filter on template name
         :type query['id']: str
-        :param query['plugin'] (dict) <br> query.plugin (Query) :
+        :param query['plugin'] (dict) <br> query.plugin (Query) : either name of a plugin (e.g. `mySensor`), or full version specification of the plug (e.g `mySensor:1.0.3`)
         :type query['plugin']: str
-        :param query['template'] (dict) <br> query.template (Query) :
-        :type query['template']: str
-        :param query['filter'] (dict) <br> query.filter (Query) : fuzzy search on multiple properties
-        :type query['filter']: str
-        :param query['tags.key'] (dict) <br> query.tags_key (Query) : Parameter is `form` style serialized, with explode: true  See [Query multiple tasks tag examples](/#/api/rules/?id=queryTagExamples)  You can add the same tag query parameter multiple times with different values, which will be applied with a logical OR.  You can specify the `tags.<key>` query parameter without a value, tasks which have a value for tag `<key>` will be returned
-        :type query['tags.key']: ListTasksTagsKeyParameter
-        :param query['finishedBefore'] (dict) <br> query.finished_before (Query) : Tasks stopped before provided time will be returned.
-        :type query['finishedBefore']: int
-        :param query['createdAfter'] (dict) <br> query.created_after (Query) : Tasks created after provided time will be returned.
-        :type query['createdAfter']: int
-        :param query['createdBefore'] (dict) <br> query.created_before (Query) : Tasks created before provided time will be returned
-        :type query['createdBefore']: int
+        :param query['tags.X'] (dict) <br> query.tags_x (Query) :
+        :type query['tags.X']: str
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
@@ -887,150 +824,139 @@
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
-                "200": List[TaskEntity] if not select_path else Model,
+                "200": List[TemplateEntityMetadata] if not select_path else Model,
             }
         )
         non_200_response_types_map: Dict[str, Any] = {}
         response_types_map.update(non_200_response_types_map)
 
         ## peform request
         return await self.api_client.request(
             method="GET",
-            resource_path="/rules/v1/tasks",
+            resource_path="/rules/v1/templates",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
     async def replace(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
-        json: Annotated[TaskSpecification, Field(description="Task Specification")],
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> TaskEntity: ...
+    ) -> ReplaceTemplate200Response: ...
 
     @overload
     async def replace(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
-        json: Annotated[TaskSpecification, Field(description="Task Specification")],
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
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
-        json: Annotated[TaskSpecification, Field(description="Task Specification")],
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
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
-        json: Annotated[TaskSpecification, Field(description="Task Specification")],
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
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
-        json: Annotated[TaskSpecification, Field(description="Task Specification")],
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
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
+        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
-        json: Annotated[TaskSpecification, Field(description="Task Specification")],
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> TaskEntity | T | Response | Model:
-        """Update Task.
+    ) -> ReplaceTemplate200Response | T | Response | Model:
+        """Update Template.
 
-        Update a task.  Remark that the full specification of the task must be given
-        :param task_id: Unique Task identifier (required)
-        :type task_id: str
-        :param json: Task Specification
-        :type json: TaskSpecification, optional
+        Update a template. Note that this will not update any tasks using the template. You will need to do a batch reload operation on the tasks to accomplish that.
+        :param name: Unique Template identifier (required)
+        :type name: str
         :param query: URL Query parameters.
         :type query: ReplaceQuery | QueryParamTypes, optional
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
@@ -1041,153 +967,138 @@
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
-            "taskId": str(task_id),
+            "name": str(name),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
-            body_adapter = TypeAdapter(
-                Annotated[TaskSpecification, Field(description="Task Specification")]
-            )
-            json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
-        body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(ReplaceQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
-                "200": TaskEntity if not select_path else Model,
+                "200": ReplaceTemplate200Response if not select_path else Model,
             }
         )
         non_200_response_types_map: Dict[str, Any] = {
             "400": ErrorWithDetailsResponse,
             "404": ErrorResponse,
         }
         response_types_map.update(non_200_response_types_map)
 
         ## peform request
         return await self.api_client.request(
             method="PUT",
-            resource_path="/rules/v1/tasks/{taskId}",
+            resource_path="/rules/v1/templates/{name}",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
-    async def start(
+    async def set(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        query: StartQuery | QueryParamTypes | None = None,
+        query: SetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> TaskEntity: ...
+    ) -> TemplateDetails | None: ...
 
     @overload
-    async def start(
+    async def set(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        query: StartQuery | QueryParamTypes | None = None,
+        query: SetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
-    async def start(
+    async def set(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        query: StartQuery | QueryParamTypes | None = None,
+        query: SetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
-    async def start(
+    async def set(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        query: StartQuery | QueryParamTypes | None = None,
+        query: SetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
-    async def start(
+    async def set(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        query: StartQuery | QueryParamTypes | None = None,
+        query: SetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
-    async def start(
+    async def set(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        query: StartQuery | QueryParamTypes | None = None,
+        query: SetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> TaskEntity | T | Response | Model:
-        """Start Task.
+    ) -> TemplateDetails | None | T | Response | Model:
+        """Set Discovery Template.
 
-        Start a task.
-        :param task_id: Unique Task identifier (required)
-        :type task_id: str
+        Set the discovery template.
         :param query: URL Query parameters.
-        :type query: StartQuery | QueryParamTypes, optional
+        :type query: SetQuery | QueryParamTypes, optional
+        :param query['name'] (dict) <br> query.name (Query) : The template to set as discovery template. If you do not specify this parameter, the current discovery template will be cleared.
+        :type query['name']: str
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
@@ -1198,147 +1109,162 @@
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
-        path_params: Dict[str, str] = {
-            "taskId": str(task_id),
-        }
+        path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
-            query = TypeAdapter(StartQuery).validate_python(query)
+        if query is not None and should_validate:
+            query = TypeAdapter(SetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
-                "200": TaskEntity if not select_path else Model,
+                "200": TemplateDetails if not select_path else Model,
+                "204": None,
             }
         )
         non_200_response_types_map: Dict[str, Any] = {
-            "400": ErrorResponse,
             "404": ErrorResponse,
         }
         response_types_map.update(non_200_response_types_map)
 
         ## peform request
         return await self.api_client.request(
-            method="POST",
-            resource_path="/rules/v1/tasks/{taskId}/command/start",
+            method="PUT",
+            resource_path="/rules/v1/discoveryTemplate",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
-    async def stop(
+    async def upgrade_plugins(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        query: StopQuery | QueryParamTypes | None = None,
+        json: Annotated[
+            TemplateModification, Field(description="Plugin Update Specifications")
+        ],
+        query: UpgradePluginsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> TaskEntity: ...
+    ) -> UpgradePluginsTemplates200Response: ...
 
     @overload
-    async def stop(
+    async def upgrade_plugins(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        query: StopQuery | QueryParamTypes | None = None,
+        json: Annotated[
+            TemplateModification, Field(description="Plugin Update Specifications")
+        ],
+        query: UpgradePluginsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
-    async def stop(
+    async def upgrade_plugins(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        query: StopQuery | QueryParamTypes | None = None,
+        json: Annotated[
+            TemplateModification, Field(description="Plugin Update Specifications")
+        ],
+        query: UpgradePluginsQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
-    async def stop(
+    async def upgrade_plugins(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        query: StopQuery | QueryParamTypes | None = None,
+        json: Annotated[
+            TemplateModification, Field(description="Plugin Update Specifications")
+        ],
+        query: UpgradePluginsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
-    async def stop(
+    async def upgrade_plugins(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        query: StopQuery | QueryParamTypes | None = None,
+        json: Annotated[
+            TemplateModification, Field(description="Plugin Update Specifications")
+        ],
+        query: UpgradePluginsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
-    async def stop(
+    async def upgrade_plugins(
         self,
-        task_id: Annotated[StrictStr, Field(description="Unique Task identifier")],
         *,
-        query: StopQuery | QueryParamTypes | None = None,
+        json: Annotated[
+            TemplateModification, Field(description="Plugin Update Specifications")
+        ],
+        query: UpgradePluginsQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> TaskEntity | T | Response | Model:
-        """Stop Task.
+    ) -> UpgradePluginsTemplates200Response | T | Response | Model:
+        """Upgrade Plugins.
 
-        Stop a task.
-        :param task_id: Unique Task identifier (required)
-        :type task_id: str
+        Upgrade plugins on multiple templates.  The plugin upgrades specified in the body will be applied to all template that fullfil the query expresses by the query parameters. At least one of the query parameters must be specified.
+        :param json: Plugin Update Specifications
+        :type json: TemplateModification, optional
         :param query: URL Query parameters.
-        :type query: StopQuery | QueryParamTypes, optional
+        :type query: UpgradePluginsQuery | QueryParamTypes, optional
+        :param query['ids'] (dict) <br> query.ids (Query) : comma separated string of template names
+        :type query['ids']: List[str]
+        :param query['id'] (dict) <br> query.id (Query) : filter on template name
+        :type query['id']: str
+        :param query['plugin'] (dict) <br> query.plugin (Query) : either name of a plugin (e.g. `mySensor`), or full version specification of the plug (e.g `mySensor:1.0.3`)
+        :type query['plugin']: str
+        :param query['tags.X'] (dict) <br> query.tags_x (Query) :
+        :type query['tags.X']: str
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
@@ -1349,43 +1275,53 @@
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
-        path_params: Dict[str, str] = {
-            "taskId": str(task_id),
-        }
+        path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
+        if json is not None and should_validate:
+            body_adapter = TypeAdapter(
+                Annotated[
+                    TemplateModification,
+                    Field(description="Plugin Update Specifications"),
+                ]
+            )
+            json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
+        body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
-            query = TypeAdapter(StopQuery).validate_python(query)
+        if query is not None and should_validate:
+            query = TypeAdapter(UpgradePluginsQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
-                "200": TaskEntity if not select_path else Model,
+                "200": UpgradePluginsTemplates200Response if not select_path else Model,
             }
         )
         non_200_response_types_map: Dict[str, Any] = {
             "400": ErrorResponse,
-            "404": ErrorResponse,
         }
         response_types_map.update(non_200_response_types_map)
 
         ## peform request
         return await self.api_client.request(
-            method="POST",
-            resource_path="/rules/v1/tasks/{taskId}/command/stop",
+            method="PATCH",
+            resource_path="/rules/v1/templates",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
```

### Comparing `waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/api/tasks_batch_operations_api.py` & `waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/tasks_batch_operations_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -98,15 +98,14 @@
             StrictStr, Field(description="Unique Batch Operation identifier")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> GetBatchOperation200Response: ...
 
     @overload
     async def get(
         self,
@@ -114,15 +113,14 @@
             StrictStr, Field(description="Unique Batch Operation identifier")
         ],
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
@@ -130,15 +128,14 @@
             StrictStr, Field(description="Unique Batch Operation identifier")
         ],
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
@@ -146,15 +143,14 @@
             StrictStr, Field(description="Unique Batch Operation identifier")
         ],
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
@@ -162,45 +158,42 @@
             StrictStr, Field(description="Unique Batch Operation identifier")
         ],
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
         batch_id: Annotated[
             StrictStr, Field(description="Unique Batch Operation identifier")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> GetBatchOperation200Response | T | Response | Model:
         """Get Tasks Batch Operation Status.
 
         Get the results of the Tasks Batch Operation.
         :param batch_id: Unique Batch Operation identifier (required)
         :type batch_id: str
         :param query: URL Query parameters.
         :type query: GetQuery | QueryParamTypes, optional
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
@@ -211,24 +204,28 @@
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
             "batchId": str(batch_id),
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
                 "200": GetBatchOperation200Response if not select_path else Model,
@@ -253,122 +250,89 @@
             raw_response=raw_response,
         )
 
     @overload
     async def start(
         self,
         *,
-        json: Annotated[
-            ATasksBatchOperationSpecification,
-            Field(description="Tasks Batch Operation"),
-        ],
         query: StartQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> BatchOperationEnqueued: ...
 
     @overload
     async def start(
         self,
         *,
-        json: Annotated[
-            ATasksBatchOperationSpecification,
-            Field(description="Tasks Batch Operation"),
-        ],
         query: StartQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def start(
         self,
         *,
-        json: Annotated[
-            ATasksBatchOperationSpecification,
-            Field(description="Tasks Batch Operation"),
-        ],
         query: StartQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def start(
         self,
         *,
-        json: Annotated[
-            ATasksBatchOperationSpecification,
-            Field(description="Tasks Batch Operation"),
-        ],
         query: StartQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def start(
         self,
         *,
-        json: Annotated[
-            ATasksBatchOperationSpecification,
-            Field(description="Tasks Batch Operation"),
-        ],
         query: StartQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def start(
         self,
         *,
-        json: Annotated[
-            ATasksBatchOperationSpecification,
-            Field(description="Tasks Batch Operation"),
-        ],
         query: StartQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> BatchOperationEnqueued | T | Response | Model:
         """Start Batch Operations.
 
         Start a batch operation.
-        :param json: Tasks Batch Operation
-        :type json: ATasksBatchOperationSpecification, optional
         :param query: URL Query parameters.
         :type query: StartQuery | QueryParamTypes, optional
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
@@ -379,31 +343,26 @@
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
-        if json is not None and validate_request:
-            body_adapter = TypeAdapter(
-                Annotated[
-                    ATasksBatchOperationSpecification,
-                    Field(description="Tasks Batch Operation"),
-                ]
-            )
-            json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
-        body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(StartQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "202": BatchOperationEnqueued if not select_path else Model,
```

### Comparing `waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/api/template_runs_api.py` & `waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/template_runs_api.py`

 * *Files 22% similar despite different names*

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
@@ -31,15 +30,14 @@
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
     from waylay.services.rules.models import (
         ErrorResponse,
         ErrorWithDetailsResponse,
         TemplateRunInvocation,
@@ -93,143 +91,93 @@
     Do not edit the class manually.
     """
 
     @overload
     async def run_graph(
         self,
         *,
-        json: Annotated[
-            TemplateRunWithGraphSpecification,
-            Field(description="Specification to run template through graph/BN."),
-        ],
         query: RunGraphQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[TemplateRunInvocation]: ...
+    ) -> TemplateRunInvocation: ...
 
     @overload
     async def run_graph(
         self,
         *,
-        json: Annotated[
-            TemplateRunWithGraphSpecification,
-            Field(description="Specification to run template through graph/BN."),
-        ],
         query: RunGraphQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[T]: ...
+    ) -> T: ...
 
     @overload
     async def run_graph(
         self,
         *,
-        json: Annotated[
-            TemplateRunWithGraphSpecification,
-            Field(description="Specification to run template through graph/BN."),
-        ],
         query: RunGraphQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def run_graph(
         self,
         *,
-        json: Annotated[
-            TemplateRunWithGraphSpecification,
-            Field(description="Specification to run template through graph/BN."),
-        ],
         query: RunGraphQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[Model]: ...
+    ) -> Model: ...
 
     @overload
     async def run_graph(
         self,
         *,
-        json: Annotated[
-            TemplateRunWithGraphSpecification,
-            Field(description="Specification to run template through graph/BN."),
-        ],
         query: RunGraphQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[T]: ...
+    ) -> T: ...
 
     async def run_graph(
         self,
         *,
-        json: Annotated[
-            TemplateRunWithGraphSpecification,
-            Field(description="Specification to run template through graph/BN."),
-        ],
         query: RunGraphQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> (
-        AsyncIterator[TemplateRunInvocation]
-        | AsyncIterator[T]
-        | Response
-        | AsyncIterator[Model]
-    ):
+    ) -> TemplateRunInvocation | T | Response | Model:
         """Run Graph Or Bayesian Network.
 
         Run a graph or Bayesian Network. If `data` is specified, template will be run as reactive template. If `data` is not specified, template will be run as a one-time template (1 tick)
-        :param json: Specification to run template through graph/BN.
-        :type json: TemplateRunWithGraphSpecification, optional
         :param query: URL Query parameters.
         :type query: RunGraphQuery | QueryParamTypes, optional
         :param query['logLevel'] (dict) <br> query.log_level (Query) : sets the log level for filtering out logs to requested log level or higher from the template run output. Value `NONE` will disable all logs. If not specified all logs will be returned.
         :type query['logLevel']: RunTemplateLogLevelParameter
         :param query['targetNode'] (dict) <br> query.target_node (Query) : The sensors and actuators part of response will contain only elements related to the asked node of the graph. The returned logs also will be filtered and contain only logs related to the asked node(s).
         :type query['targetNode']: List[str]
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
@@ -240,33 +188,26 @@
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
-        if json is not None and validate_request:
-            body_adapter = TypeAdapter(
-                Annotated[
-                    TemplateRunWithGraphSpecification,
-                    Field(
-                        description="Specification to run template through graph/BN."
-                    ),
-                ]
-            )
-            json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
-        body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(RunGraphQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": TemplateRunInvocation if not select_path else Model,
@@ -281,157 +222,111 @@
         return await self.api_client.request(
             method="POST",
             resource_path="/rules/v1/templates/run",
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
     async def run(
         self,
         name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
-        json: Annotated[
-            TemplateRunSpecification, Field(description="Specification to run template")
-        ],
         query: RunQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[TemplateRunInvocation]: ...
+    ) -> TemplateRunInvocation: ...
 
     @overload
     async def run(
         self,
         name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
-        json: Annotated[
-            TemplateRunSpecification, Field(description="Specification to run template")
-        ],
         query: RunQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[T]: ...
+    ) -> T: ...
 
     @overload
     async def run(
         self,
         name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
-        json: Annotated[
-            TemplateRunSpecification, Field(description="Specification to run template")
-        ],
         query: RunQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def run(
         self,
         name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
-        json: Annotated[
-            TemplateRunSpecification, Field(description="Specification to run template")
-        ],
         query: RunQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[Model]: ...
+    ) -> Model: ...
 
     @overload
     async def run(
         self,
         name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
-        json: Annotated[
-            TemplateRunSpecification, Field(description="Specification to run template")
-        ],
         query: RunQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[T]: ...
+    ) -> T: ...
 
     async def run(
         self,
         name: Annotated[StrictStr, Field(description="Unique Template identifier")],
         *,
-        json: Annotated[
-            TemplateRunSpecification, Field(description="Specification to run template")
-        ],
         query: RunQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> (
-        AsyncIterator[TemplateRunInvocation]
-        | AsyncIterator[T]
-        | Response
-        | AsyncIterator[Model]
-    ):
+    ) -> TemplateRunInvocation | T | Response | Model:
         """Run Template.
 
         Run a template. If `data` is specified, template will be run as reactive template. If `data` is not specified, template will be run as a one-time template (1 tick)
         :param name: Unique Template identifier (required)
         :type name: str
-        :param json: Specification to run template
-        :type json: TemplateRunSpecification, optional
         :param query: URL Query parameters.
         :type query: RunQuery | QueryParamTypes, optional
         :param query['logLevel'] (dict) <br> query.log_level (Query) : sets the log level for filtering out logs to requested log level or higher from the template run output. Value `NONE` will disable all logs. If not specified all logs will be returned.
         :type query['logLevel']: RunTemplateLogLevelParameter
         :param query['targetNode'] (dict) <br> query.target_node (Query) : The sensors and actuators part of response will contain only elements related to the asked node of the graph. The returned logs also will be filtered and contain only logs related to the asked node(s).
         :type query['targetNode']: List[str]
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
@@ -442,33 +337,28 @@
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
             "name": str(name),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
-            body_adapter = TypeAdapter(
-                Annotated[
-                    TemplateRunSpecification,
-                    Field(description="Specification to run template"),
-                ]
-            )
-            json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
-        body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(RunQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": TemplateRunInvocation if not select_path else Model,
@@ -484,14 +374,12 @@
         return await self.api_client.request(
             method="POST",
             resource_path="/rules/v1/templates/{name}/run",
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
```

### Comparing `waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/api/templates_api.py` & `waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/api/plugs_execution_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 from __future__ import annotations  # for Python 3.7–3.9
 
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
-    List,
     Literal,
     TypeVar,
     overload,
 )
 
 from pydantic import (
     Field,
@@ -35,216 +34,206 @@
     Response,
 )
 from waylay.sdk.api._models import Model
 from waylay.sdk.plugin import WithApiClient
 
 if TYPE_CHECKING:
     from waylay.services.rules.models import (
-        CreateTemplate201Response,
+        ActuatorExecutionResult,
         ErrorResponse,
-        ErrorWithDetailsResponse,
-        ReplaceTemplate200Response,
-        TemplateDetails,
-        TemplateEntity,
-        TemplateEntityMetadata,
-        TemplateModification,
-        UpgradePluginsTemplates200Response,
+        ExecutePlugsSpecification,
+        SensorExecutionResult,
+        TransformerExecutionResult,
     )
-    from waylay.services.rules.queries.templates_api import (
-        CreateQuery,
-        DeleteQuery,
-        GetDiscoveryQuery,
-        GetQuery,
-        ListQuery,
-        ReplaceQuery,
-        SetQuery,
-        UpgradePluginsQuery,
+    from waylay.services.rules.queries.plugs_execution_api import (
+        ExecuteActuatorQuery,
+        ExecuteActuatorVersionQuery,
+        ExecuteSensorQuery,
+        ExecuteSensorVersionQuery,
+        ExecuteTransformerQuery,
+        ExecuteTransformerVersionQuery,
     )
 
 
 try:
     from waylay.services.rules.models import (
-        CreateTemplate201Response,
+        ActuatorExecutionResult,
         ErrorResponse,
-        ErrorWithDetailsResponse,
-        ReplaceTemplate200Response,
-        TemplateDetails,
-        TemplateEntity,
-        TemplateEntityMetadata,
-        TemplateModification,
-        UpgradePluginsTemplates200Response,
+        ExecutePlugsSpecification,
+        SensorExecutionResult,
+        TransformerExecutionResult,
     )
-    from waylay.services.rules.queries.templates_api import (
-        CreateQuery,
-        DeleteQuery,
-        GetDiscoveryQuery,
-        GetQuery,
-        ListQuery,
-        ReplaceQuery,
-        SetQuery,
-        UpgradePluginsQuery,
+    from waylay.services.rules.queries.plugs_execution_api import (
+        ExecuteActuatorQuery,
+        ExecuteActuatorVersionQuery,
+        ExecuteSensorQuery,
+        ExecuteSensorVersionQuery,
+        ExecuteTransformerQuery,
+        ExecuteTransformerVersionQuery,
     )
 
     MODELS_AVAILABLE = True
 except ImportError:
     MODELS_AVAILABLE = False
 
     if not TYPE_CHECKING:
-        TemplateEntity = Model
+        ExecutePlugsSpecification = Model
 
-        CreateQuery = dict
-        CreateTemplate201Response = Model
+        ExecuteActuatorQuery = dict
+        ActuatorExecutionResult = Model
 
-        ErrorWithDetailsResponse = Model
-
-        DeleteQuery = dict
+        ActuatorExecutionResult = Model
 
         ErrorResponse = Model
 
-        ErrorResponse = Model
+        ExecutePlugsSpecification = Model
 
-        GetDiscoveryQuery = dict
-        TemplateDetails = Model
+        ExecuteActuatorVersionQuery = dict
+        ActuatorExecutionResult = Model
 
-        GetQuery = dict
-        TemplateDetails = Model
+        ActuatorExecutionResult = Model
 
         ErrorResponse = Model
 
-        ListQuery = dict
-        TemplateEntityMetadata = Model
+        ExecutePlugsSpecification = Model
+
+        ExecuteSensorQuery = dict
+        SensorExecutionResult = Model
 
-        TemplateEntity = Model
+        SensorExecutionResult = Model
+
+        ErrorResponse = Model
 
-        ReplaceQuery = dict
-        ReplaceTemplate200Response = Model
+        ExecutePlugsSpecification = Model
 
-        ErrorWithDetailsResponse = Model
+        ExecuteSensorVersionQuery = dict
+        SensorExecutionResult = Model
+
+        SensorExecutionResult = Model
 
         ErrorResponse = Model
 
-        SetQuery = dict
-        TemplateDetails = Model
+        ExecutePlugsSpecification = Model
+
+        ExecuteTransformerQuery = dict
+        TransformerExecutionResult = Model
+
+        TransformerExecutionResult = Model
 
         ErrorResponse = Model
 
-        TemplateModification = Model
+        ExecutePlugsSpecification = Model
+
+        ExecuteTransformerVersionQuery = dict
+        TransformerExecutionResult = Model
 
-        UpgradePluginsQuery = dict
-        UpgradePluginsTemplates200Response = Model
+        TransformerExecutionResult = Model
 
         ErrorResponse = Model
 
 
 T = TypeVar("T")
 
 
-class TemplatesApi(WithApiClient):
-    """TemplatesApi service methods.
+class PlugsExecutionApi(WithApiClient):
+    """PlugsExecutionApi service methods.
 
     NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     @overload
-    async def create(
+    async def execute_actuator(
         self,
+        name: StrictStr,
         *,
-        json: Annotated[TemplateEntity, Field(description="Template Specification")],
-        query: CreateQuery | QueryParamTypes | None = None,
+        query: ExecuteActuatorQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> CreateTemplate201Response: ...
+    ) -> ActuatorExecutionResult: ...
 
     @overload
-    async def create(
+    async def execute_actuator(
         self,
+        name: StrictStr,
         *,
-        json: Annotated[TemplateEntity, Field(description="Template Specification")],
-        query: CreateQuery | QueryParamTypes | None = None,
+        query: ExecuteActuatorQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
-    async def create(
+    async def execute_actuator(
         self,
+        name: StrictStr,
         *,
-        json: Annotated[TemplateEntity, Field(description="Template Specification")],
-        query: CreateQuery | QueryParamTypes | None = None,
+        query: ExecuteActuatorQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
-    async def create(
+    async def execute_actuator(
         self,
+        name: StrictStr,
         *,
-        json: Annotated[TemplateEntity, Field(description="Template Specification")],
-        query: CreateQuery | QueryParamTypes | None = None,
+        query: ExecuteActuatorQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
-    async def create(
+    async def execute_actuator(
         self,
+        name: StrictStr,
         *,
-        json: Annotated[TemplateEntity, Field(description="Template Specification")],
-        query: CreateQuery | QueryParamTypes | None = None,
+        query: ExecuteActuatorQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
-    async def create(
+    async def execute_actuator(
         self,
+        name: StrictStr,
         *,
-        json: Annotated[TemplateEntity, Field(description="Template Specification")],
-        query: CreateQuery | QueryParamTypes | None = None,
+        query: ExecuteActuatorQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> CreateTemplate201Response | T | Response | Model:
-        """Create Template.
+    ) -> ActuatorExecutionResult | T | Response | Model:
+        """Execute Latest Actuator Version.
 
-        Create a template.
-        :param json: Template Specification
-        :type json: TemplateEntity, optional
+        Execute latest version of an actuator.
+        :param name: (required)
+        :type name: str
         :param query: URL Query parameters.
-        :type query: CreateQuery | QueryParamTypes, optional
+        :type query: ExecuteActuatorQuery | QueryParamTypes, optional
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
@@ -255,150 +244,164 @@
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
-        path_params: Dict[str, str] = {}
+        path_params: Dict[str, str] = {
+            "name": str(name),
+        }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
-            body_adapter = TypeAdapter(
-                Annotated[TemplateEntity, Field(description="Template Specification")]
-            )
-            json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
-        body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
-            query = TypeAdapter(CreateQuery).validate_python(query)
+        if query is not None and should_validate:
+            query = TypeAdapter(ExecuteActuatorQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
-                "201": CreateTemplate201Response if not select_path else Model,
+                "200": ActuatorExecutionResult if not select_path else Model,
             }
         )
         non_200_response_types_map: Dict[str, Any] = {
-            "400": ErrorWithDetailsResponse,
+            "400": ActuatorExecutionResult,
+            "404": ErrorResponse,
         }
         response_types_map.update(non_200_response_types_map)
 
         ## peform request
         return await self.api_client.request(
             method="POST",
-            resource_path="/rules/v1/templates",
+            resource_path="/rules/v1/actions/{name}",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
-    async def delete(
+    async def execute_actuator_version(
         self,
-        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
+        name: StrictStr,
+        version: Annotated[
+            str, Field(strict=True, description="Version number of plugin")
+        ],
         *,
-        query: DeleteQuery | QueryParamTypes | None = None,
+        query: ExecuteActuatorVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> None: ...
+    ) -> ActuatorExecutionResult: ...
 
     @overload
-    async def delete(
+    async def execute_actuator_version(
         self,
-        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
+        name: StrictStr,
+        version: Annotated[
+            str, Field(strict=True, description="Version number of plugin")
+        ],
         *,
-        query: DeleteQuery | QueryParamTypes | None = None,
+        query: ExecuteActuatorVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
-    async def delete(
+    async def execute_actuator_version(
         self,
-        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
+        name: StrictStr,
+        version: Annotated[
+            str, Field(strict=True, description="Version number of plugin")
+        ],
         *,
-        query: DeleteQuery | QueryParamTypes | None = None,
+        query: ExecuteActuatorVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
-    async def delete(
+    async def execute_actuator_version(
         self,
-        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
+        name: StrictStr,
+        version: Annotated[
+            str, Field(strict=True, description="Version number of plugin")
+        ],
         *,
-        query: DeleteQuery | QueryParamTypes | None = None,
+        query: ExecuteActuatorVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> None: ...
+    ) -> Model: ...
 
     @overload
-    async def delete(
+    async def execute_actuator_version(
         self,
-        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
+        name: StrictStr,
+        version: Annotated[
+            str, Field(strict=True, description="Version number of plugin")
+        ],
         *,
-        query: DeleteQuery | QueryParamTypes | None = None,
+        query: ExecuteActuatorVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
-    async def delete(
+    async def execute_actuator_version(
         self,
-        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
+        name: StrictStr,
+        version: Annotated[
+            str, Field(strict=True, description="Version number of plugin")
+        ],
         *,
-        query: DeleteQuery | QueryParamTypes | None = None,
+        query: ExecuteActuatorVersionQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> None | T | Response:
-        """Delete Template.
+    ) -> ActuatorExecutionResult | T | Response | Model:
+        """Execute Specified Actuator Version.
 
-        Delete a template.
-        :param name: Unique Template identifier (required)
+        Execute specified version of an actuator.
+        :param name: (required)
         :type name: str
+        :param version: Version number of plugin (required)
+        :type version: str
         :param query: URL Query parameters.
-        :type query: DeleteQuery | QueryParamTypes, optional
+        :type query: ExecuteActuatorVersionQuery | QueryParamTypes, optional
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
@@ -409,139 +412,145 @@
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
             "name": str(name),
+            "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
-            query = TypeAdapter(DeleteQuery).validate_python(query)
+        if query is not None and should_validate:
+            query = TypeAdapter(ExecuteActuatorVersionQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
-                "204": None,
+                "200": ActuatorExecutionResult if not select_path else Model,
             }
         )
         non_200_response_types_map: Dict[str, Any] = {
-            "400": ErrorResponse,
+            "400": ActuatorExecutionResult,
             "404": ErrorResponse,
         }
         response_types_map.update(non_200_response_types_map)
 
         ## peform request
         return await self.api_client.request(
-            method="DELETE",
-            resource_path="/rules/v1/templates/{name}",
+            method="POST",
+            resource_path="/rules/v1/actions/{name}/versions/{version}",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
-    async def get_discovery(
+    async def execute_sensor(
         self,
+        name: StrictStr,
         *,
-        query: GetDiscoveryQuery | QueryParamTypes | None = None,
+        query: ExecuteSensorQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> TemplateDetails | None: ...
+    ) -> SensorExecutionResult: ...
 
     @overload
-    async def get_discovery(
+    async def execute_sensor(
         self,
+        name: StrictStr,
         *,
-        query: GetDiscoveryQuery | QueryParamTypes | None = None,
+        query: ExecuteSensorQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
-    async def get_discovery(
+    async def execute_sensor(
         self,
+        name: StrictStr,
         *,
-        query: GetDiscoveryQuery | QueryParamTypes | None = None,
+        query: ExecuteSensorQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
-    async def get_discovery(
+    async def execute_sensor(
         self,
+        name: StrictStr,
         *,
-        query: GetDiscoveryQuery | QueryParamTypes | None = None,
+        query: ExecuteSensorQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
-    async def get_discovery(
+    async def execute_sensor(
         self,
+        name: StrictStr,
         *,
-        query: GetDiscoveryQuery | QueryParamTypes | None = None,
+        query: ExecuteSensorQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
-    async def get_discovery(
+    async def execute_sensor(
         self,
+        name: StrictStr,
         *,
-        query: GetDiscoveryQuery | QueryParamTypes | None = None,
+        query: ExecuteSensorQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> TemplateDetails | None | T | Response | Model:
-        """Retrieve Discovery Template.
+    ) -> SensorExecutionResult | T | Response | Model:
+        """Execute Latest Sensor Version.
 
-        Get the discovery template.
+        Execute latest version of a sensor.
+        :param name: (required)
+        :type name: str
         :param query: URL Query parameters.
-        :type query: GetDiscoveryQuery | QueryParamTypes, optional
+        :type query: ExecuteSensorQuery | QueryParamTypes, optional
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
@@ -552,301 +561,164 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        # path parameters
-        path_params: Dict[str, str] = {}
-
-        ## named body parameters
-        body_args: Dict[str, Any] = {}
-
-        # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
-            query = TypeAdapter(GetDiscoveryQuery).validate_python(query)
-
-        response_types_map: Dict[str, Any] = (
-            {"2XX": response_type}
-            if response_type is not None
-            else {
-                "200": TemplateDetails if not select_path else Model,
-                "204": None,
-            }
-        )
-        non_200_response_types_map: Dict[str, Any] = {}
-        response_types_map.update(non_200_response_types_map)
-
-        ## peform request
-        return await self.api_client.request(
-            method="GET",
-            resource_path="/rules/v1/discoveryTemplate",
-            path_params=path_params,
-            params=query,
-            **body_args,
-            headers=headers,
-            **kwargs,
-            response_type=response_types_map,
-            select_path=select_path,
-            raw_response=raw_response,
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
         )
 
-    @overload
-    async def get(
-        self,
-        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
-        *,
-        query: GetQuery | QueryParamTypes | None = None,
-        raw_response: Literal[False] = False,
-        select_path: Literal[""] = "",
-        response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
-        headers: HeaderTypes | None = None,
-        **kwargs,
-    ) -> TemplateDetails: ...
-
-    @overload
-    async def get(
-        self,
-        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
-        *,
-        query: GetQuery | QueryParamTypes | None = None,
-        raw_response: Literal[False] = False,
-        select_path: Literal[""] = "",
-        response_type: T,
-        validate_request: StrictBool = True,
-        headers: HeaderTypes | None = None,
-        **kwargs,
-    ) -> T: ...
-
-    @overload
-    async def get(
-        self,
-        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
-        *,
-        query: GetQuery | QueryParamTypes | None = None,
-        raw_response: Literal[True],
-        select_path: Literal["_not_used_"] = "_not_used_",
-        response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
-        headers: HeaderTypes | None = None,
-        **kwargs,
-    ) -> Response: ...
-
-    @overload
-    async def get(
-        self,
-        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
-        *,
-        query: GetQuery | QueryParamTypes | None = None,
-        raw_response: Literal[False] = False,
-        select_path: str,
-        response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
-        headers: HeaderTypes | None = None,
-        **kwargs,
-    ) -> Model: ...
-
-    @overload
-    async def get(
-        self,
-        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
-        *,
-        query: GetQuery | QueryParamTypes | None = None,
-        raw_response: Literal[False] = False,
-        select_path: str,
-        response_type: T,
-        validate_request: StrictBool = True,
-        headers: HeaderTypes | None = None,
-        **kwargs,
-    ) -> T: ...
-
-    async def get(
-        self,
-        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
-        *,
-        query: GetQuery | QueryParamTypes | None = None,
-        raw_response: StrictBool = False,
-        select_path: str = "",
-        response_type: T | None = None,
-        validate_request: StrictBool = True,
-        headers: HeaderTypes | None = None,
-        **kwargs,
-    ) -> TemplateDetails | T | Response | Model:
-        """Retrieve Template Details.
-
-        Retrieve the details of a template.
-        :param name: Unique Template identifier (required)
-        :type name: str
-        :param query: URL Query parameters.
-        :type query: GetQuery | QueryParamTypes, optional
-        :param query['format'] (dict) <br> query.format (Query) : Format of the graph definition
-        :type query['format']: ListTasksFormatParameter
-        :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
-        :param select_path: Denotes the json path applied to the response object before returning it.
-                Set it to the empty string `""` to receive the full response object.
-        :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
-        :param headers: Header parameters for this request
-        :type headers: dict, optional
-        :param `**kwargs`: Additional parameters passed on to the http client.
-            See below.
-        :Keyword Arguments:
-            * timeout: a single numeric timeout in seconds,
-                or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
-            * stream: if true, the response will be in streaming mode
-            * cookies
-            * extensions
-            * auth
-            * follow_redirects: bool
-
-        :return: Returns the result object if the http request succeeded with status code '2XX'.
-        :raises APIError: If the http request has a status code different from `2XX`. This
-            object wraps both the http Response and any parsed data.
-        """
-
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
-            query = TypeAdapter(GetQuery).validate_python(query)
+        if query is not None and should_validate:
+            query = TypeAdapter(ExecuteSensorQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
-                "200": TemplateDetails if not select_path else Model,
+                "200": SensorExecutionResult if not select_path else Model,
             }
         )
         non_200_response_types_map: Dict[str, Any] = {
+            "400": SensorExecutionResult,
             "404": ErrorResponse,
         }
         response_types_map.update(non_200_response_types_map)
 
         ## peform request
         return await self.api_client.request(
-            method="GET",
-            resource_path="/rules/v1/templates/{name}",
+            method="POST",
+            resource_path="/rules/v1/sensors/{name}",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
-    async def list(
+    async def execute_sensor_version(
         self,
+        name: StrictStr,
+        version: Annotated[
+            str, Field(strict=True, description="Version number of plugin")
+        ],
         *,
-        query: ListQuery | QueryParamTypes | None = None,
+        query: ExecuteSensorVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> List[TemplateEntityMetadata]: ...
+    ) -> SensorExecutionResult: ...
 
     @overload
-    async def list(
+    async def execute_sensor_version(
         self,
+        name: StrictStr,
+        version: Annotated[
+            str, Field(strict=True, description="Version number of plugin")
+        ],
         *,
-        query: ListQuery | QueryParamTypes | None = None,
+        query: ExecuteSensorVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
-    async def list(
+    async def execute_sensor_version(
         self,
+        name: StrictStr,
+        version: Annotated[
+            str, Field(strict=True, description="Version number of plugin")
+        ],
         *,
-        query: ListQuery | QueryParamTypes | None = None,
+        query: ExecuteSensorVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
-    async def list(
+    async def execute_sensor_version(
         self,
+        name: StrictStr,
+        version: Annotated[
+            str, Field(strict=True, description="Version number of plugin")
+        ],
         *,
-        query: ListQuery | QueryParamTypes | None = None,
+        query: ExecuteSensorVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
-    async def list(
+    async def execute_sensor_version(
         self,
+        name: StrictStr,
+        version: Annotated[
+            str, Field(strict=True, description="Version number of plugin")
+        ],
         *,
-        query: ListQuery | QueryParamTypes | None = None,
+        query: ExecuteSensorVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
-    async def list(
+    async def execute_sensor_version(
         self,
+        name: StrictStr,
+        version: Annotated[
+            str, Field(strict=True, description="Version number of plugin")
+        ],
         *,
-        query: ListQuery | QueryParamTypes | None = None,
+        query: ExecuteSensorVersionQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> List[TemplateEntityMetadata] | T | Response | Model:
-        """List Templates.
+    ) -> SensorExecutionResult | T | Response | Model:
+        """Execute Specified Sensor Version.
 
-        Query templates.
+        Execute the specified version of a sensor.
+        :param name: (required)
+        :type name: str
+        :param version: Version number of plugin (required)
+        :type version: str
         :param query: URL Query parameters.
-        :type query: ListQuery | QueryParamTypes, optional
-        :param query['hits'] (dict) <br> query.hits (Query) : (Paging) maximal number of items returned
-        :type query['hits']: int
-        :param query['startIndex'] (dict) <br> query.start_index (Query) : (Paging) items to skip in the listing
-        :type query['startIndex']: int
-        :param query['filter'] (dict) <br> query.filter (Query) : fuzzy search on multiple properties
-        :type query['filter']: str
-        :param query['ids'] (dict) <br> query.ids (Query) : comma separated string of template names
-        :type query['ids']: List[str]
-        :param query['id'] (dict) <br> query.id (Query) : filter on template name
-        :type query['id']: str
-        :param query['plugin'] (dict) <br> query.plugin (Query) : either name of a plugin (e.g. `mySensor`), or full version specification of the plug (e.g `mySensor:1.0.3`)
-        :type query['plugin']: str
-        :param query['tags.X'] (dict) <br> query.tags_x (Query) :
-        :type query['tags.X']: str
+        :type query: ExecuteSensorVersionQuery | QueryParamTypes, optional
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
@@ -857,301 +729,145 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        # path parameters
-        path_params: Dict[str, str] = {}
-
-        ## named body parameters
-        body_args: Dict[str, Any] = {}
-
-        # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
-            query = TypeAdapter(ListQuery).validate_python(query)
-
-        response_types_map: Dict[str, Any] = (
-            {"2XX": response_type}
-            if response_type is not None
-            else {
-                "200": List[TemplateEntityMetadata] if not select_path else Model,
-            }
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
         )
-        non_200_response_types_map: Dict[str, Any] = {}
-        response_types_map.update(non_200_response_types_map)
-
-        ## peform request
-        return await self.api_client.request(
-            method="GET",
-            resource_path="/rules/v1/templates",
-            path_params=path_params,
-            params=query,
-            **body_args,
-            headers=headers,
-            **kwargs,
-            response_type=response_types_map,
-            select_path=select_path,
-            raw_response=raw_response,
-        )
-
-    @overload
-    async def replace(
-        self,
-        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
-        *,
-        json: Annotated[TemplateEntity, Field(description="Template Specification")],
-        query: ReplaceQuery | QueryParamTypes | None = None,
-        raw_response: Literal[False] = False,
-        select_path: Literal[""] = "",
-        response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
-        headers: HeaderTypes | None = None,
-        **kwargs,
-    ) -> ReplaceTemplate200Response: ...
-
-    @overload
-    async def replace(
-        self,
-        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
-        *,
-        json: Annotated[TemplateEntity, Field(description="Template Specification")],
-        query: ReplaceQuery | QueryParamTypes | None = None,
-        raw_response: Literal[False] = False,
-        select_path: Literal[""] = "",
-        response_type: T,
-        validate_request: StrictBool = True,
-        headers: HeaderTypes | None = None,
-        **kwargs,
-    ) -> T: ...
-
-    @overload
-    async def replace(
-        self,
-        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
-        *,
-        json: Annotated[TemplateEntity, Field(description="Template Specification")],
-        query: ReplaceQuery | QueryParamTypes | None = None,
-        raw_response: Literal[True],
-        select_path: Literal["_not_used_"] = "_not_used_",
-        response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
-        headers: HeaderTypes | None = None,
-        **kwargs,
-    ) -> Response: ...
-
-    @overload
-    async def replace(
-        self,
-        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
-        *,
-        json: Annotated[TemplateEntity, Field(description="Template Specification")],
-        query: ReplaceQuery | QueryParamTypes | None = None,
-        raw_response: Literal[False] = False,
-        select_path: str,
-        response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
-        headers: HeaderTypes | None = None,
-        **kwargs,
-    ) -> Model: ...
-
-    @overload
-    async def replace(
-        self,
-        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
-        *,
-        json: Annotated[TemplateEntity, Field(description="Template Specification")],
-        query: ReplaceQuery | QueryParamTypes | None = None,
-        raw_response: Literal[False] = False,
-        select_path: str,
-        response_type: T,
-        validate_request: StrictBool = True,
-        headers: HeaderTypes | None = None,
-        **kwargs,
-    ) -> T: ...
-
-    async def replace(
-        self,
-        name: Annotated[StrictStr, Field(description="Unique Template identifier")],
-        *,
-        json: Annotated[TemplateEntity, Field(description="Template Specification")],
-        query: ReplaceQuery | QueryParamTypes | None = None,
-        raw_response: StrictBool = False,
-        select_path: str = "",
-        response_type: T | None = None,
-        validate_request: StrictBool = True,
-        headers: HeaderTypes | None = None,
-        **kwargs,
-    ) -> ReplaceTemplate200Response | T | Response | Model:
-        """Update Template.
-
-        Update a template. Note that this will not update any tasks using the template. You will need to do a batch reload operation on the tasks to accomplish that.
-        :param name: Unique Template identifier (required)
-        :type name: str
-        :param json: Template Specification
-        :type json: TemplateEntity, optional
-        :param query: URL Query parameters.
-        :type query: ReplaceQuery | QueryParamTypes, optional
-        :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
-        :param select_path: Denotes the json path applied to the response object before returning it.
-                Set it to the empty string `""` to receive the full response object.
-        :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
-        :param headers: Header parameters for this request
-        :type headers: dict, optional
-        :param `**kwargs`: Additional parameters passed on to the http client.
-            See below.
-        :Keyword Arguments:
-            * timeout: a single numeric timeout in seconds,
-                or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
-            * stream: if true, the response will be in streaming mode
-            * cookies
-            * extensions
-            * auth
-            * follow_redirects: bool
-
-        :return: Returns the result object if the http request succeeded with status code '2XX'.
-        :raises APIError: If the http request has a status code different from `2XX`. This
-            object wraps both the http Response and any parsed data.
-        """
 
         # path parameters
         path_params: Dict[str, str] = {
             "name": str(name),
+            "version": str(version),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
-            body_adapter = TypeAdapter(
-                Annotated[TemplateEntity, Field(description="Template Specification")]
-            )
-            json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
-        body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
-            query = TypeAdapter(ReplaceQuery).validate_python(query)
+        if query is not None and should_validate:
+            query = TypeAdapter(ExecuteSensorVersionQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
-                "200": ReplaceTemplate200Response if not select_path else Model,
+                "200": SensorExecutionResult if not select_path else Model,
             }
         )
         non_200_response_types_map: Dict[str, Any] = {
-            "400": ErrorWithDetailsResponse,
+            "400": SensorExecutionResult,
             "404": ErrorResponse,
         }
         response_types_map.update(non_200_response_types_map)
 
         ## peform request
         return await self.api_client.request(
-            method="PUT",
-            resource_path="/rules/v1/templates/{name}",
+            method="POST",
+            resource_path="/rules/v1/sensors/{name}/versions/{version}",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
-    async def set(
+    async def execute_transformer(
         self,
+        name: StrictStr,
         *,
-        query: SetQuery | QueryParamTypes | None = None,
+        query: ExecuteTransformerQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> TemplateDetails | None: ...
+    ) -> TransformerExecutionResult: ...
 
     @overload
-    async def set(
+    async def execute_transformer(
         self,
+        name: StrictStr,
         *,
-        query: SetQuery | QueryParamTypes | None = None,
+        query: ExecuteTransformerQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
-    async def set(
+    async def execute_transformer(
         self,
+        name: StrictStr,
         *,
-        query: SetQuery | QueryParamTypes | None = None,
+        query: ExecuteTransformerQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
-    async def set(
+    async def execute_transformer(
         self,
+        name: StrictStr,
         *,
-        query: SetQuery | QueryParamTypes | None = None,
+        query: ExecuteTransformerQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
-    async def set(
+    async def execute_transformer(
         self,
+        name: StrictStr,
         *,
-        query: SetQuery | QueryParamTypes | None = None,
+        query: ExecuteTransformerQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
-    async def set(
+    async def execute_transformer(
         self,
+        name: StrictStr,
         *,
-        query: SetQuery | QueryParamTypes | None = None,
+        query: ExecuteTransformerQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> TemplateDetails | None | T | Response | Model:
-        """Set Discovery Template.
+    ) -> TransformerExecutionResult | T | Response | Model:
+        """Execute Latest Transformer Version.
 
-        Set the discovery template.
+        Execute the latest transformer version.
+        :param name: (required)
+        :type name: str
         :param query: URL Query parameters.
-        :type query: SetQuery | QueryParamTypes, optional
-        :param query['name'] (dict) <br> query.name (Query) : The template to set as discovery template. If you do not specify this parameter, the current discovery template will be cleared.
-        :type query['name']: str
+        :type query: ExecuteTransformerQuery | QueryParamTypes, optional
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
@@ -1162,165 +878,164 @@
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
-        path_params: Dict[str, str] = {}
+        path_params: Dict[str, str] = {
+            "name": str(name),
+        }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
-            query = TypeAdapter(SetQuery).validate_python(query)
+        if query is not None and should_validate:
+            query = TypeAdapter(ExecuteTransformerQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
-                "200": TemplateDetails if not select_path else Model,
-                "204": None,
+                "200": TransformerExecutionResult if not select_path else Model,
             }
         )
         non_200_response_types_map: Dict[str, Any] = {
+            "400": TransformerExecutionResult,
             "404": ErrorResponse,
         }
         response_types_map.update(non_200_response_types_map)
 
         ## peform request
         return await self.api_client.request(
-            method="PUT",
-            resource_path="/rules/v1/discoveryTemplate",
+            method="POST",
+            resource_path="/rules/v1/transformers/{name}",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
 
     @overload
-    async def upgrade_plugins(
+    async def execute_transformer_version(
         self,
-        *,
-        json: Annotated[
-            TemplateModification, Field(description="Plugin Update Specifications")
+        name: StrictStr,
+        version: Annotated[
+            str, Field(strict=True, description="Version number of plugin")
         ],
-        query: UpgradePluginsQuery | QueryParamTypes | None = None,
+        *,
+        query: ExecuteTransformerVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> UpgradePluginsTemplates200Response: ...
+    ) -> TransformerExecutionResult: ...
 
     @overload
-    async def upgrade_plugins(
+    async def execute_transformer_version(
         self,
-        *,
-        json: Annotated[
-            TemplateModification, Field(description="Plugin Update Specifications")
+        name: StrictStr,
+        version: Annotated[
+            str, Field(strict=True, description="Version number of plugin")
         ],
-        query: UpgradePluginsQuery | QueryParamTypes | None = None,
+        *,
+        query: ExecuteTransformerVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
-    async def upgrade_plugins(
+    async def execute_transformer_version(
         self,
-        *,
-        json: Annotated[
-            TemplateModification, Field(description="Plugin Update Specifications")
+        name: StrictStr,
+        version: Annotated[
+            str, Field(strict=True, description="Version number of plugin")
         ],
-        query: UpgradePluginsQuery | QueryParamTypes | None = None,
+        *,
+        query: ExecuteTransformerVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
-    async def upgrade_plugins(
+    async def execute_transformer_version(
         self,
-        *,
-        json: Annotated[
-            TemplateModification, Field(description="Plugin Update Specifications")
+        name: StrictStr,
+        version: Annotated[
+            str, Field(strict=True, description="Version number of plugin")
         ],
-        query: UpgradePluginsQuery | QueryParamTypes | None = None,
+        *,
+        query: ExecuteTransformerVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
-    async def upgrade_plugins(
+    async def execute_transformer_version(
         self,
-        *,
-        json: Annotated[
-            TemplateModification, Field(description="Plugin Update Specifications")
+        name: StrictStr,
+        version: Annotated[
+            str, Field(strict=True, description="Version number of plugin")
         ],
-        query: UpgradePluginsQuery | QueryParamTypes | None = None,
+        *,
+        query: ExecuteTransformerVersionQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
-    async def upgrade_plugins(
+    async def execute_transformer_version(
         self,
-        *,
-        json: Annotated[
-            TemplateModification, Field(description="Plugin Update Specifications")
+        name: StrictStr,
+        version: Annotated[
+            str, Field(strict=True, description="Version number of plugin")
         ],
-        query: UpgradePluginsQuery | QueryParamTypes | None = None,
+        *,
+        query: ExecuteTransformerVersionQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
-    ) -> UpgradePluginsTemplates200Response | T | Response | Model:
-        """Upgrade Plugins.
+    ) -> TransformerExecutionResult | T | Response | Model:
+        """Execute Specified Transformer Version.
 
-        Upgrade plugins on multiple templates.  The plugin upgrades specified in the body will be applied to all template that fullfil the query expresses by the query parameters. At least one of the query parameters must be specified.
-        :param json: Plugin Update Specifications
-        :type json: TemplateModification, optional
+        Execute specified version of a transformer.
+        :param name: (required)
+        :type name: str
+        :param version: Version number of plugin (required)
+        :type version: str
         :param query: URL Query parameters.
-        :type query: UpgradePluginsQuery | QueryParamTypes, optional
-        :param query['ids'] (dict) <br> query.ids (Query) : comma separated string of template names
-        :type query['ids']: List[str]
-        :param query['id'] (dict) <br> query.id (Query) : filter on template name
-        :type query['id']: str
-        :param query['plugin'] (dict) <br> query.plugin (Query) : either name of a plugin (e.g. `mySensor`), or full version specification of the plug (e.g `mySensor:1.0.3`)
-        :type query['plugin']: str
-        :param query['tags.X'] (dict) <br> query.tags_x (Query) :
-        :type query['tags.X']: str
+        :type query: ExecuteTransformerVersionQuery | QueryParamTypes, optional
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
@@ -1331,49 +1046,48 @@
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
-        path_params: Dict[str, str] = {}
+        path_params: Dict[str, str] = {
+            "name": str(name),
+            "version": str(version),
+        }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
-            body_adapter = TypeAdapter(
-                Annotated[
-                    TemplateModification,
-                    Field(description="Plugin Update Specifications"),
-                ]
-            )
-            json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
-        body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
-            query = TypeAdapter(UpgradePluginsQuery).validate_python(query)
+        if query is not None and should_validate:
+            query = TypeAdapter(ExecuteTransformerVersionQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
-                "200": UpgradePluginsTemplates200Response if not select_path else Model,
+                "200": TransformerExecutionResult if not select_path else Model,
             }
         )
         non_200_response_types_map: Dict[str, Any] = {
-            "400": ErrorResponse,
+            "400": TransformerExecutionResult,
+            "404": ErrorResponse,
         }
         response_types_map.update(non_200_response_types_map)
 
         ## peform request
         return await self.api_client.request(
-            method="PATCH",
-            resource_path="/rules/v1/templates",
+            method="POST",
+            resource_path="/rules/v1/transformers/{name}/versions/{version}",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
```

### Comparing `waylay_sdk_rules-6.5.0.20240423/src/waylay/services/rules/service/service.py` & `waylay-sdk-rules-6.5.0rc1/src/waylay/services/rules/service/service.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """Rules Service."""
 
 from waylay.sdk import ApiClient, WaylayService
 
-from ..api.about_api import AboutApi
 from ..api.plugs_execution_api import PlugsExecutionApi
 from ..api.push_data_api import PushDataApi
 from ..api.task_nodes_api import TaskNodesApi
 from ..api.tasks_api import TasksApi
 from ..api.tasks_batch_operations_api import TasksBatchOperationsApi
 from ..api.template_runs_api import TemplateRunsApi
 from ..api.templates_api import TemplatesApi
+from ..api.version_api import VersionApi
 
 
 class RulesService(WaylayService):
     """Rules Service Class."""
 
     name = "rules"
     title = "Rules Service"
 
-    about: AboutApi
     plugs_execution: PlugsExecutionApi
     push_data: PushDataApi
     task_nodes: TaskNodesApi
     tasks: TasksApi
     tasks_batch_operations: TasksBatchOperationsApi
     template_runs: TemplateRunsApi
     templates: TemplatesApi
+    version: VersionApi
 
     def __init__(self, api_client: ApiClient):
         """Create the rules service."""
 
         super().__init__(api_client)
-        self.about = AboutApi(api_client)
         self.plugs_execution = PlugsExecutionApi(api_client)
         self.push_data = PushDataApi(api_client)
         self.task_nodes = TaskNodesApi(api_client)
         self.tasks = TasksApi(api_client)
         self.tasks_batch_operations = TasksBatchOperationsApi(api_client)
         self.template_runs = TemplateRunsApi(api_client)
         self.templates = TemplatesApi(api_client)
+        self.version = VersionApi(api_client)
```

### Comparing `waylay_sdk_rules-6.5.0.20240423/src/waylay_sdk_rules.egg-info/PKG-INFO` & `waylay-sdk-rules-6.5.0rc1/src/waylay_sdk_rules.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-rules
-Version: 6.5.0.20240423
+Version: 6.5.0rc1
 Summary: Waylay rules engine
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,22 +13,22 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-rules-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/rules.html
 Keywords: Waylay rules engine
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.1
+Requires-Dist: waylay-sdk~=0.0.4rc5
+Requires-Dist: waylay-sdk-rules==6.5.0rc1
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -47,51 +47,53 @@
 Requires-Dist: waylay-sdk-rules-types; extra == "types"
 
 # Waylay Rules Service
 The REST api to manage rule tasks and rule templates in the Waylay platform.
 
 This Python package is automatically generated based on the 
 Waylay Rules OpenAPI specification (API version: 6.5.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/rules.html).
 
-It consists of a plugin for the waylay-sdk-core package, and contains the Rules api methods.
+It consists of a plugin for the waylay-sdk package, and contains the Rules api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-rules-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-rules is included in:
-- ```pip install waylay-sdk-core[rules]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[rules]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-rules and waylay-sdk-rules-types are included in:
-- ```pip install waylay-sdk-core[rules,rules-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[rules,rules-types]``` to install `waylay-sdk` along with only this service including the typed models, or
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
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-rules-types` is installed
-from waylay.services.rules.models.version_response import VersionResponse
+from rules.models.execute_plugs_specification import ExecutePlugsSpecification
+from rules.models.transformer_execution_result import TransformerExecutionResult
 try:
-    # Get Service Information
-    # calls `GET /rules/v1`
-    api_response = await waylay_client.rules.about.get(
+    # Execute Specified Transformer Version
+    # calls `POST /rules/v1/transformers/{name}/versions/{version}`
+    api_response = await waylay_client.rules.plugs_execution.execute_transformer_version(
+        'name_example', # name | path param "name"
+        'version_example', # version | path param "version"
     )
-    print("The response of rules.about.get:\n")
+    print("The response of rules.plugs_execution.execute_transformer_version:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling rules.about.get: %s\n" % e)
+    print("Exception when calling rules.plugs_execution.execute_transformer_version: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_rules-6.5.0.20240423/src/waylay_sdk_rules.egg-info/SOURCES.txt` & `waylay-sdk-rules-6.5.0rc1/src/waylay_sdk_rules.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 LICENSE.txt
 README.md
 pyproject.toml
 src/waylay/services/rules/api/__init__.py
-src/waylay/services/rules/api/about_api.py
 src/waylay/services/rules/api/plugs_execution_api.py
 src/waylay/services/rules/api/push_data_api.py
 src/waylay/services/rules/api/py.typed
 src/waylay/services/rules/api/task_nodes_api.py
 src/waylay/services/rules/api/tasks_api.py
 src/waylay/services/rules/api/tasks_batch_operations_api.py
 src/waylay/services/rules/api/template_runs_api.py
 src/waylay/services/rules/api/templates_api.py
+src/waylay/services/rules/api/version_api.py
 src/waylay/services/rules/service/__init__.py
 src/waylay/services/rules/service/py.typed
 src/waylay/services/rules/service/service.py
 src/waylay_sdk_rules.egg-info/PKG-INFO
 src/waylay_sdk_rules.egg-info/SOURCES.txt
 src/waylay_sdk_rules.egg-info/dependency_links.txt
 src/waylay_sdk_rules.egg-info/entry_points.txt
```

