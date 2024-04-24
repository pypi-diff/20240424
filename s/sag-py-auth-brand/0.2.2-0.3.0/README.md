# Comparing `tmp/sag-py-auth-brand-0.2.2.tar.gz` & `tmp/sag_py_auth_brand-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sag-py-auth-brand-0.2.2.tar", last modified: Thu May 25 12:56:58 2023, max compression
+gzip compressed data, was "sag_py_auth_brand-0.3.0.tar", last modified: Wed Apr 24 10:11:04 2024, max compression
```

## Comparing `sag-py-auth-brand-0.2.2.tar` & `sag_py_auth_brand-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:56:58.261049 sag-py-auth-brand-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-25 12:56:58.261049 sag-py-auth-brand-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:56:58.257049 sag-py-auth-brand-0.2.2/sag_py_auth_brand/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/sag_py_auth_brand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/sag_py_auth_brand/brand_jwt_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/sag_py_auth_brand/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/sag_py_auth_brand/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/sag_py_auth_brand/request_brand_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/sag_py_auth_brand/request_brand_logging_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:56:58.261049 sag-py-auth-brand-0.2.2/sag_py_auth_brand.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-25 12:56:58.000000 sag-py-auth-brand-0.2.2/sag_py_auth_brand.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-25 12:56:58.000000 sag-py-auth-brand-0.2.2/sag_py_auth_brand.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:56:58.000000 sag-py-auth-brand-0.2.2/sag_py_auth_brand.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-25 12:56:58.000000 sag-py-auth-brand-0.2.2/sag_py_auth_brand.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 12:56:58.000000 sag-py-auth-brand-0.2.2/sag_py_auth_brand.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 12:56:58.261049 sag-py-auth-brand-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:56:58.261049 sag-py-auth-brand-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/tests/test_brand_jwt_auth__call.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/tests/test_brand_jwt_auth__init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/tests/test_brand_jwt_auth__verify_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/tests/test_brand_jwt_auth__verify_brand_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/tests/test_request_brand_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-25 12:56:44.000000 sag-py-auth-brand-0.2.2/tests/test_request_brand_logging_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:11:04.915811 sag_py_auth_brand-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-24 10:11:04.915811 sag_py_auth_brand-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:11:04.911811 sag_py_auth_brand-0.3.0/sag_py_auth_brand/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/sag_py_auth_brand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/sag_py_auth_brand/brand_jwt_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/sag_py_auth_brand/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/sag_py_auth_brand/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/sag_py_auth_brand/request_brand_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/sag_py_auth_brand/request_brand_logging_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:11:04.911811 sag_py_auth_brand-0.3.0/sag_py_auth_brand.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-24 10:11:04.000000 sag_py_auth_brand-0.3.0/sag_py_auth_brand.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-24 10:11:04.000000 sag_py_auth_brand-0.3.0/sag_py_auth_brand.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:11:04.000000 sag_py_auth_brand-0.3.0/sag_py_auth_brand.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-24 10:11:04.000000 sag_py_auth_brand-0.3.0/sag_py_auth_brand.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 10:11:04.000000 sag_py_auth_brand-0.3.0/sag_py_auth_brand.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-24 10:11:04.915811 sag_py_auth_brand-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:11:04.911811 sag_py_auth_brand-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/tests/test_brand_jwt_auth__call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/tests/test_brand_jwt_auth__init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/tests/test_brand_jwt_auth__verify_brand.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/tests/test_request_brand_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-24 10:11:01.000000 sag_py_auth_brand-0.3.0/tests/test_request_brand_logging_filter.py
```

### Comparing `sag-py-auth-brand-0.2.2/LICENSE.txt` & `sag_py_auth_brand-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sag-py-auth-brand-0.2.2/PKG-INFO` & `sag_py_auth_brand-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-auth-brand
-Version: 0.2.2
+Version: 0.3.0
 Summary: Keycloak brand/instance authentication for python projects
 Home-page: https://github.com/SamhammerAG/sag_py_auth_brand
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_auth_brand
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_auth_brand/issues
@@ -14,16 +14,20 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE.txt
+Requires-Dist: contextvars>=2.4
+Requires-Dist: fastapi[all]>=0.104.1
+Requires-Dist: sag-py-auth>=0.1.4
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
 
 # sag_py_auth_brand
 
 [![Maintainability][codeclimate-image]][codeclimate-url]
 [![Coverage Status][coveralls-image]][coveralls-url]
 [![Known Vulnerabilities](https://snyk.io/test/github/SamhammerAG/sag_py_auth_brand/badge.svg)](https://snyk.io/test/github/SamhammerAG/sag_py_auth_brand)
 
@@ -34,15 +38,15 @@
 
 This provides a way to secure your fastapi with keycloak jwt bearer authentication.
 This library bases on sag_py_auth and adds support for instances/brands.
 
 ## What it does
 * Secure your api endpoints
 * Verifies auth tokens: signature, expiration, issuer, audience
-* Verifies the brand/customer over a token role (+ alias support)
+* Verifies the brand/customer over a token role
 * Verifies the instance over a token role
 * Verifies the stage over a realm role
 * Allows to set additional permissions by specifying further token roles
 * Supplies brand information from context
 
 ## How to use
 
@@ -80,15 +84,15 @@
 
 ### Get brand information
 
 See sag_py_auth to find out how to access the token and user info.
 
 Furthermore you can get the brand by accessing it over the context:
 ```python
-from sag_py_auth_brand.request_brand_context import get_brand as get_brand_from_context
+from sag_py_auth_brand.request_brand_context import get_request_brand as get_brand_from_context
 brand = get_brand_from_context()
 ```
 
 This works in async calls but not in sub threads (without additional changes).
 
 See:
 * https://docs.python.org/3/library/contextvars.html
@@ -103,15 +107,15 @@
 from sag_py_auth_brand.request_brand_logging_filter import RequestBrandLoggingFilter
 
 console_handler = logging.StreamHandler(sys.stdout)
 console_handler.addFilter(RequestBrandLoggingFilter())
 
 ```
 
-The filter provides the field request_brand and request_brand_alias with the brand.
+The filter provides the field request_brand with the brand.
 
 ### How a token has to look like
 
 ```json
 {
 
     "iss": "https://authserver.com/auth/realms/projectName",
@@ -128,25 +132,20 @@
             "roles": ["myInstance"]
         },
         "role-brand": {
             "roles": ["myBrand"]
         },
         "role-endpoint": {
             "roles": ["permissionOne", "permissionTwo"]
-        },
-        "role-brand-alias": {
-            "roles": ["myBrand", "myBrandAliasOne", "myBrandAliasTwo"]
         }
     }
 }
 ```
 
 * role-endpoint is just required for permission checks of the api endpoint
-* role-brand-alias is optional for the alias feature. If you don't use aliases it can be left ayway.
-* role-brand-alias must contain exactly one original brand (also called the compound brand alias) together with one or multiple aliases
 
 ## How to start developing
 
 ### With vscode
 
 Just install vscode with dev containers extension. All required extensions and configurations are prepared automatically.
 
@@ -166,7 +165,15 @@
 * Restart pycharm
 
 ## How to publish
 
 * Update the version in setup.py and commit your change
 * Create a tag with the same version number
 * Let github do the rest
+
+## How to test
+
+To avoid publishing to pypi unnecessarily you can do as follows
+
+* Tag your branch however you like
+* Use the chosen tag in the requirements.txt-file of the project you want to test this library in, eg. `sag_py_auth_brand==<your tag>`
+* Rebuild/redeploy your project
```

### Comparing `sag-py-auth-brand-0.2.2/README.md` & `sag_py_auth_brand-0.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 This provides a way to secure your fastapi with keycloak jwt bearer authentication.
 This library bases on sag_py_auth and adds support for instances/brands.
 
 ## What it does
 * Secure your api endpoints
 * Verifies auth tokens: signature, expiration, issuer, audience
-* Verifies the brand/customer over a token role (+ alias support)
+* Verifies the brand/customer over a token role
 * Verifies the instance over a token role
 * Verifies the stage over a realm role
 * Allows to set additional permissions by specifying further token roles
 * Supplies brand information from context
 
 ## How to use
 
@@ -57,15 +57,15 @@
 
 ### Get brand information
 
 See sag_py_auth to find out how to access the token and user info.
 
 Furthermore you can get the brand by accessing it over the context:
 ```python
-from sag_py_auth_brand.request_brand_context import get_brand as get_brand_from_context
+from sag_py_auth_brand.request_brand_context import get_request_brand as get_brand_from_context
 brand = get_brand_from_context()
 ```
 
 This works in async calls but not in sub threads (without additional changes).
 
 See:
 * https://docs.python.org/3/library/contextvars.html
@@ -80,15 +80,15 @@
 from sag_py_auth_brand.request_brand_logging_filter import RequestBrandLoggingFilter
 
 console_handler = logging.StreamHandler(sys.stdout)
 console_handler.addFilter(RequestBrandLoggingFilter())
 
 ```
 
-The filter provides the field request_brand and request_brand_alias with the brand.
+The filter provides the field request_brand with the brand.
 
 ### How a token has to look like
 
 ```json
 {
 
     "iss": "https://authserver.com/auth/realms/projectName",
@@ -105,25 +105,20 @@
             "roles": ["myInstance"]
         },
         "role-brand": {
             "roles": ["myBrand"]
         },
         "role-endpoint": {
             "roles": ["permissionOne", "permissionTwo"]
-        },
-        "role-brand-alias": {
-            "roles": ["myBrand", "myBrandAliasOne", "myBrandAliasTwo"]
         }
     }
 }
 ```
 
 * role-endpoint is just required for permission checks of the api endpoint
-* role-brand-alias is optional for the alias feature. If you don't use aliases it can be left ayway.
-* role-brand-alias must contain exactly one original brand (also called the compound brand alias) together with one or multiple aliases
 
 ## How to start developing
 
 ### With vscode
 
 Just install vscode with dev containers extension. All required extensions and configurations are prepared automatically.
 
@@ -143,7 +138,15 @@
 * Restart pycharm
 
 ## How to publish
 
 * Update the version in setup.py and commit your change
 * Create a tag with the same version number
 * Let github do the rest
+
+## How to test
+
+To avoid publishing to pypi unnecessarily you can do as follows
+
+* Tag your branch however you like
+* Use the chosen tag in the requirements.txt-file of the project you want to test this library in, eg. `sag_py_auth_brand==<your tag>`
+* Rebuild/redeploy your project
```

### Comparing `sag-py-auth-brand-0.2.2/sag_py_auth_brand/request_brand_logging_filter.py` & `sag_py_auth_brand-0.3.0/sag_py_auth_brand/request_brand_context.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-from logging import Filter, LogRecord
+from contextvars import ContextVar
+from typing import Optional
 
-from .request_brand_context import get_brand, get_request_brand, get_request_brand_alias
+_request_brand: ContextVar[Optional[str]] = ContextVar("request_brand", default=None)
 
 
-class RequestBrandLoggingFilter(Filter):
-    """Register this filter to get a field brand_name in log entries"""
+def get_request_brand() -> str:
+    """Gets the context local brand. This is always the brand of the request.
+    See library contextvars for details.
 
-    def __init__(self, name: str = "") -> None:
-        super().__init__(name=name)
+    Returns: The brand
+    """
+    current_brand: Optional[str] = _request_brand.get("")
+    return current_brand or ""
 
-    def filter(self, record: LogRecord) -> bool:
-        if request_brand := get_request_brand():
-            record.request_brand = request_brand
 
-        if request_brand_alias := get_request_brand_alias():
-            record.request_brand_alias = request_brand_alias
-
-        if brand := get_brand():
-            record.brand = brand
-
-        return True
+def set_request_brand(brand_to_set: Optional[str]) -> None:
+    """Sets the context local brand. This is always the brand of the request.
+    See library contextvars for details."""
+    _request_brand.set(brand_to_set)
```

### Comparing `sag-py-auth-brand-0.2.2/sag_py_auth_brand.egg-info/PKG-INFO` & `sag_py_auth_brand-0.3.0/sag_py_auth_brand.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-auth-brand
-Version: 0.2.2
+Version: 0.3.0
 Summary: Keycloak brand/instance authentication for python projects
 Home-page: https://github.com/SamhammerAG/sag_py_auth_brand
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_auth_brand
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_auth_brand/issues
@@ -14,16 +14,20 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE.txt
+Requires-Dist: contextvars>=2.4
+Requires-Dist: fastapi[all]>=0.104.1
+Requires-Dist: sag-py-auth>=0.1.4
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
 
 # sag_py_auth_brand
 
 [![Maintainability][codeclimate-image]][codeclimate-url]
 [![Coverage Status][coveralls-image]][coveralls-url]
 [![Known Vulnerabilities](https://snyk.io/test/github/SamhammerAG/sag_py_auth_brand/badge.svg)](https://snyk.io/test/github/SamhammerAG/sag_py_auth_brand)
 
@@ -34,15 +38,15 @@
 
 This provides a way to secure your fastapi with keycloak jwt bearer authentication.
 This library bases on sag_py_auth and adds support for instances/brands.
 
 ## What it does
 * Secure your api endpoints
 * Verifies auth tokens: signature, expiration, issuer, audience
-* Verifies the brand/customer over a token role (+ alias support)
+* Verifies the brand/customer over a token role
 * Verifies the instance over a token role
 * Verifies the stage over a realm role
 * Allows to set additional permissions by specifying further token roles
 * Supplies brand information from context
 
 ## How to use
 
@@ -80,15 +84,15 @@
 
 ### Get brand information
 
 See sag_py_auth to find out how to access the token and user info.
 
 Furthermore you can get the brand by accessing it over the context:
 ```python
-from sag_py_auth_brand.request_brand_context import get_brand as get_brand_from_context
+from sag_py_auth_brand.request_brand_context import get_request_brand as get_brand_from_context
 brand = get_brand_from_context()
 ```
 
 This works in async calls but not in sub threads (without additional changes).
 
 See:
 * https://docs.python.org/3/library/contextvars.html
@@ -103,15 +107,15 @@
 from sag_py_auth_brand.request_brand_logging_filter import RequestBrandLoggingFilter
 
 console_handler = logging.StreamHandler(sys.stdout)
 console_handler.addFilter(RequestBrandLoggingFilter())
 
 ```
 
-The filter provides the field request_brand and request_brand_alias with the brand.
+The filter provides the field request_brand with the brand.
 
 ### How a token has to look like
 
 ```json
 {
 
     "iss": "https://authserver.com/auth/realms/projectName",
@@ -128,25 +132,20 @@
             "roles": ["myInstance"]
         },
         "role-brand": {
             "roles": ["myBrand"]
         },
         "role-endpoint": {
             "roles": ["permissionOne", "permissionTwo"]
-        },
-        "role-brand-alias": {
-            "roles": ["myBrand", "myBrandAliasOne", "myBrandAliasTwo"]
         }
     }
 }
 ```
 
 * role-endpoint is just required for permission checks of the api endpoint
-* role-brand-alias is optional for the alias feature. If you don't use aliases it can be left ayway.
-* role-brand-alias must contain exactly one original brand (also called the compound brand alias) together with one or multiple aliases
 
 ## How to start developing
 
 ### With vscode
 
 Just install vscode with dev containers extension. All required extensions and configurations are prepared automatically.
 
@@ -166,7 +165,15 @@
 * Restart pycharm
 
 ## How to publish
 
 * Update the version in setup.py and commit your change
 * Create a tag with the same version number
 * Let github do the rest
+
+## How to test
+
+To avoid publishing to pypi unnecessarily you can do as follows
+
+* Tag your branch however you like
+* Use the chosen tag in the requirements.txt-file of the project you want to test this library in, eg. `sag_py_auth_brand==<your tag>`
+* Rebuild/redeploy your project
```

### Comparing `sag-py-auth-brand-0.2.2/sag_py_auth_brand.egg-info/SOURCES.txt` & `sag_py_auth_brand-0.3.0/sag_py_auth_brand.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 sag_py_auth_brand/__init__.py
 sag_py_auth_brand/brand_jwt_auth.py
-sag_py_auth_brand/constants.py
 sag_py_auth_brand/models.py
+sag_py_auth_brand/py.typed
 sag_py_auth_brand/request_brand_context.py
 sag_py_auth_brand/request_brand_logging_filter.py
 sag_py_auth_brand.egg-info/PKG-INFO
 sag_py_auth_brand.egg-info/SOURCES.txt
 sag_py_auth_brand.egg-info/dependency_links.txt
 sag_py_auth_brand.egg-info/requires.txt
 sag_py_auth_brand.egg-info/top_level.txt
 tests/test_brand_jwt_auth__call.py
 tests/test_brand_jwt_auth__init.py
 tests/test_brand_jwt_auth__verify_brand.py
-tests/test_brand_jwt_auth__verify_brand_alias.py
 tests/test_request_brand_context.py
 tests/test_request_brand_logging_filter.py
```

### Comparing `sag-py-auth-brand-0.2.2/setup.py` & `sag_py_auth_brand-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     REQS = fin.read().splitlines()
 
 with open("requirements-dev.txt", "r") as fin:
     REQS_DEV = [item for item in fin.read().splitlines() if not item.endswith(".txt")]
 
 setuptools.setup(
     name="sag-py-auth-brand",
-    version="0.2.2",
+    version="0.3.0",
     description="Keycloak brand/instance authentication for python projects",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/sag_py_auth_brand",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
```

### Comparing `sag-py-auth-brand-0.2.2/tests/test_brand_jwt_auth__call.py` & `sag_py_auth_brand-0.3.0/tests/test_brand_jwt_auth__call.py`

 * *Files identical despite different names*

### Comparing `sag-py-auth-brand-0.2.2/tests/test_brand_jwt_auth__init.py` & `sag_py_auth_brand-0.3.0/tests/test_brand_jwt_auth__init.py`

 * *Files identical despite different names*

### Comparing `sag-py-auth-brand-0.2.2/tests/test_request_brand_context.py` & `sag_py_auth_brand-0.3.0/tests/test_brand_jwt_auth__verify_brand.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,56 @@
-from sag_py_auth_brand.request_brand_context import get_brand as get_brand_from_context
-from sag_py_auth_brand.request_brand_context import get_request_brand as get_request_brand_from_context
-from sag_py_auth_brand.request_brand_context import get_request_brand_alias as get_request_brand_alias_from_context
-from sag_py_auth_brand.request_brand_context import set_request_brand as set_request_brand_to_context
-from sag_py_auth_brand.request_brand_context import set_request_brand_alias as set_request_brand_alias_to_context
-
-
-def test__get_brand__not_set() -> None:
-    # Arrange
-    set_request_brand_to_context(None)
-    set_request_brand_alias_to_context(None)
-
-    # Act
-    actual_request_brand: str = get_request_brand_from_context()
-    actual_request_brand_alias: str = get_request_brand_alias_from_context()
-    actual_brand: str = get_brand_from_context()
-
-    assert not actual_request_brand
-    assert not actual_request_brand_alias
-    assert not actual_brand
-
-
-def test__get_brand__with_previously_set_brand() -> None:
-    # Arrange
-    set_request_brand_to_context("myBrand")
-    set_request_brand_alias_to_context(None)
-
-    # Act
-    actual_request_brand: str = get_request_brand_from_context()
-    actual_request_brand_alias: str = get_request_brand_alias_from_context()
-    actual_brand: str = get_brand_from_context()
-
-    assert actual_request_brand == "myBrand"
-    assert not actual_request_brand_alias
-    assert actual_brand == "myBrand"
-
-
-def test__get_brand__with_previously_set_brand_alias() -> None:
-    # Arrange
-    set_request_brand_to_context(None)
-    set_request_brand_alias_to_context("myBrandAlias")
-
-    # Act
-    actual_request_brand: str = get_request_brand_from_context()
-    actual_request_brand_alias: str = get_request_brand_alias_from_context()
-    actual_brand: str = get_brand_from_context()
-
-    assert not actual_request_brand
-    assert actual_request_brand_alias == "myBrandAlias"
-    assert actual_brand == "myBrandAlias"
-
-
-def test__get_brand__with_previously_set_both() -> None:
-    # Arrange
-    set_request_brand_to_context("myBrand")
-    set_request_brand_alias_to_context("myBrandAlias")
-
-    # Act
-    actual_request_brand: str = get_request_brand_from_context()
-    actual_request_brand_alias: str = get_request_brand_alias_from_context()
-    actual_brand: str = get_brand_from_context()
-
-    # Assert
-    assert actual_request_brand == "myBrand"
-    assert actual_request_brand_alias == "myBrandAlias"
-    assert actual_brand == "myBrandAlias"
+from typing import Any, Dict, Optional
+from unittest import TestCase, main
+
+import mock
+import pytest
+from fastapi import HTTPException
+from mock import Mock
+from sag_py_auth.models import Token
+
+from sag_py_auth_brand.brand_jwt_auth import BrandJwtAuth
+
+from .helpers import build_sample_jwt_auth, get_token
+
+
+class TestVerifyBrand(TestCase):
+    @mock.patch("sag_py_auth_brand.brand_jwt_auth.set_request_brand_to_context")
+    def test__verify_brand__where_user_has_brand(self, mock_set_brand_to_context: Mock) -> None:
+        # Arrange
+        brand_jwt_auth: BrandJwtAuth = build_sample_jwt_auth(["myEndpoint"])
+
+        resource_access: Optional[Dict[str, Any]] = {"role-brand": {"roles": ["mybrandone", "mybrandtwo"]}}
+
+        token: Token = get_token(None, resource_access)
+
+        # Act
+        try:
+            brand_jwt_auth._verify_brand(token, "mybrandone")
+        except Exception:
+            pytest.fail("No exception expected if the brand is present in the token")
+
+        # Assert
+        mock_set_brand_to_context.assert_called_once_with("mybrandone")
+
+    @mock.patch("sag_py_auth_brand.brand_jwt_auth.set_request_brand_to_context")
+    def test__verify_brand__where_brand_is_missing(
+        self, mock_set_brand_to_context: Mock
+    ) -> None:
+        # Arrange
+        brand_jwt_auth: BrandJwtAuth = build_sample_jwt_auth(["myEndpoint"])
+
+        resource_access: Optional[Dict[str, Any]] = {"role-brand": {"roles": ["mybrandone", "mybrandtwo"]}}
+
+        token: Token = get_token(None, resource_access)
+
+        # Act
+        with pytest.raises(HTTPException) as exception:
+            brand_jwt_auth._verify_brand(token, "mybrandthree")
+
+        # Assert
+        assert exception.value.status_code == 403
+        assert exception.value.detail == "Missing brand."
+        mock_set_brand_to_context.assert_called_once_with(None)
+
+
+if __name__ == "__main__":
+    main()
```

