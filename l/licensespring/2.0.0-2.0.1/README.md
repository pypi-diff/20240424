# Comparing `tmp/licensespring-2.0.0.tar.gz` & `tmp/licensespring-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "licensespring-2.0.0.tar", max compression
+gzip compressed data, was "licensespring-2.0.1.tar", max compression
```

## Comparing `licensespring-2.0.0.tar` & `licensespring-2.0.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0       64 2023-12-29 10:00:28.397852 licensespring-2.0.0/LICENSE
--rw-r--r--   0        0        0    23192 2024-03-22 07:52:05.771346 licensespring-2.0.0/README.md
--rw-r--r--   0        0        0       37 2024-03-22 07:52:05.771346 licensespring-2.0.0/licensespring/__init__.py
--rw-r--r--   0        0        0    23107 2024-03-22 07:52:05.771346 licensespring-2.0.0/licensespring/api/__init__.py
--rw-r--r--   0        0        0     1146 2024-03-22 07:52:05.771346 licensespring-2.0.0/licensespring/api/authorization.py
--rw-r--r--   0        0        0      551 2024-03-22 07:52:05.771346 licensespring-2.0.0/licensespring/api/error.py
--rw-r--r--   0        0        0     1804 2024-03-22 07:52:05.771346 licensespring-2.0.0/licensespring/api/signature.py
--rw-r--r--   0        0        0     2281 2024-03-22 07:52:05.771346 licensespring-2.0.0/licensespring/hardware/__init__.py
--rw-r--r--   0        0        0    15530 2024-03-22 07:52:05.771346 licensespring-2.0.0/licensespring/licensefile/__init__.py
--rw-r--r--   0        0        0     2471 2024-03-22 07:52:05.771346 licensespring-2.0.0/licensespring/licensefile/config.py
--rw-r--r--   0        0        0     6281 2024-03-22 07:52:05.781346 licensespring-2.0.0/licensespring/licensefile/data_storage.py
--rw-r--r--   0        0        0     1973 2024-03-22 07:52:05.781346 licensespring-2.0.0/licensespring/licensefile/default_crypto.py
--rw-r--r--   0        0        0     2381 2024-03-22 07:52:05.781346 licensespring-2.0.0/licensespring/licensefile/error.py
--rw-r--r--   0        0        0     5901 2024-03-22 07:52:05.781346 licensespring-2.0.0/licensespring/licensefile/license_data.py
--rw-r--r--   0        0        0     6527 2024-03-22 07:52:05.781346 licensespring-2.0.0/licensespring/licensefile/license_manager.py
--rw-r--r--   0        0        0      342 2024-01-04 12:24:20.611987 licensespring-2.0.0/licensespring/webhook/__init__.py
--rw-r--r--   0        0        0      300 2023-12-29 10:00:28.397852 licensespring-2.0.0/licensespring/webhook/error.py
--rw-r--r--   0        0        0     2086 2024-03-22 07:52:05.781346 licensespring-2.0.0/licensespring/webhook/signature.py
--rw-r--r--   0        0        0      980 2023-12-29 10:00:28.397852 licensespring-2.0.0/licensespring/webhook/utils.py
--rw-r--r--   0        0        0      671 2024-03-22 07:52:05.781346 licensespring-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    24025 1970-01-01 00:00:00.000000 licensespring-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0       64 2023-12-29 10:00:28.397852 licensespring-2.0.1/LICENSE
+-rw-r--r--   0        0        0    23192 2024-04-24 06:32:12.240855 licensespring-2.0.1/README.md
+-rw-r--r--   0        0        0       37 2024-04-24 06:32:12.240855 licensespring-2.0.1/licensespring/__init__.py
+-rw-r--r--   0        0        0    23871 2024-04-24 06:32:12.240855 licensespring-2.0.1/licensespring/api/__init__.py
+-rw-r--r--   0        0        0     1146 2024-03-22 07:52:05.771346 licensespring-2.0.1/licensespring/api/authorization.py
+-rw-r--r--   0        0        0      551 2024-03-22 07:52:05.771346 licensespring-2.0.1/licensespring/api/error.py
+-rw-r--r--   0        0        0     1804 2024-03-22 07:52:05.771346 licensespring-2.0.1/licensespring/api/signature.py
+-rw-r--r--   0        0        0     2281 2024-03-22 07:52:05.771346 licensespring-2.0.1/licensespring/hardware/__init__.py
+-rw-r--r--   0        0        0    24041 2024-04-24 06:32:12.240855 licensespring-2.0.1/licensespring/licensefile/__init__.py
+-rw-r--r--   0        0        0     2507 2024-04-24 06:32:12.240855 licensespring-2.0.1/licensespring/licensefile/config.py
+-rw-r--r--   0        0        0     5206 2024-04-24 06:32:12.240855 licensespring-2.0.1/licensespring/licensefile/data_storage.py
+-rw-r--r--   0        0        0     1984 2024-04-24 06:32:12.240855 licensespring-2.0.1/licensespring/licensefile/default_crypto.py
+-rw-r--r--   0        0        0     2612 2024-04-24 06:32:12.240855 licensespring-2.0.1/licensespring/licensefile/error.py
+-rw-r--r--   0        0        0     7856 2024-04-24 06:32:12.240855 licensespring-2.0.1/licensespring/licensefile/feature_manager.py
+-rw-r--r--   0        0        0    14587 2024-04-24 06:32:12.240855 licensespring-2.0.1/licensespring/licensefile/license_data.py
+-rw-r--r--   0        0        0     6729 2024-04-24 06:32:12.240855 licensespring-2.0.1/licensespring/licensefile/license_manager.py
+-rw-r--r--   0        0        0     7450 2024-04-24 06:32:12.240855 licensespring-2.0.1/licensespring/watchdog/__init__.py
+-rw-r--r--   0        0        0      342 2024-01-04 12:24:20.611987 licensespring-2.0.1/licensespring/webhook/__init__.py
+-rw-r--r--   0        0        0      300 2023-12-29 10:00:28.397852 licensespring-2.0.1/licensespring/webhook/error.py
+-rw-r--r--   0        0        0     2086 2024-03-22 07:52:05.781346 licensespring-2.0.1/licensespring/webhook/signature.py
+-rw-r--r--   0        0        0      980 2023-12-29 10:00:28.397852 licensespring-2.0.1/licensespring/webhook/utils.py
+-rw-r--r--   0        0        0      687 2024-04-24 06:32:12.240855 licensespring-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    24025 1970-01-01 00:00:00.000000 licensespring-2.0.1/PKG-INFO
```

### Comparing `licensespring-2.0.0/README.md` & `licensespring-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -758,8 +758,8 @@
 |--------------------|-----------|-----------------------------------------------------|----------------------------------------------------------|
 | certifi            | 2023.7.22 | Mozilla Public License 2.0 (MPL 2.0)                | https://github.com/certifi/python-certifi                |
 | charset-normalizer | 3.3.0     | MIT License                                         | https://github.com/Ousret/charset_normalizer             |
 | idna               | 3.4       | BSD License                                         | https://github.com/kjd/idna                              |
 | pycryptodome       | 3.19.0    | Apache Software License; BSD License; Public Domain | https://www.pycryptodome.org                             |
 | requests           | 2.31.0    | Apache Software License                             | https://requests.readthedocs.io                          |
 | urllib3            | 2.0.7     | MIT License                                         | https://github.com/urllib3/urllib3/blob/main/CHANGES.rst |
-| winregistry        | 1.1.1     | MIT License                                         | https://github.com/shpaker/winregistry                   |
+| winregistry        | 1.1.1     | UNKNOWN                                             | https://github.com/shpaker/winregistry                   |
```

### Comparing `licensespring-2.0.0/licensespring/api/__init__.py` & `licensespring-2.0.1/licensespring/api/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,20 +48,24 @@
         authorization_headers = autorization_headers(self.api_key, self.shared_key)
         return {**headers, **authorization_headers, **custom_headers}
 
     def request_generic_data(
         self,
         data,
         product,
+        bundle_code=None,
         hardware_id=None,
         license_key=None,
         username=None,
         password=None,
     ):
         data["product"] = product
+        if bundle_code:
+            data["bundle_code"] = bundle_code
+
         data["hardware_id"] = (
             hardware_id if hardware_id else self.hardware_id_provider.get_id()
         )
 
         if license_key:
             data["license_key"] = license_key
         if username:
@@ -156,14 +160,15 @@
         else:
             response.raise_for_status()
         return response
 
     def activate_license(
         self,
         product,
+        bundle_code=None,
         hardware_id=None,
         license_key=None,
         username=None,
         password=None,
         customer_account_code=None,
         id_token=None,
         code=None,
@@ -172,15 +177,15 @@
         hostname=None,
         ip=None,
         is_vm=None,
         vm_info=None,
         mac_address=None,
     ):
         data = self.request_generic_data(
-            {}, product, hardware_id, license_key, username, password
+            {}, product, bundle_code, hardware_id, license_key, username, password
         )
         data = self.request_sso_data(
             data,
             customer_account_code=customer_account_code,
             id_token=id_token,
             code=code,
         )
@@ -204,37 +209,44 @@
             self.signature_verifier.verify_license_signature_v2(
                 response.content, response.headers.get("LicenseSignature")
             )
 
         return response.json()
 
     def deactivate_license(
-        self, product, hardware_id=None, license_key=None, username=None, password=None
+        self,
+        product,
+        bundle_code=None,
+        hardware_id=None,
+        license_key=None,
+        username=None,
+        password=None,
     ):
         data = self.request_generic_data(
-            {}, product, hardware_id, license_key, username, password
+            {}, product, bundle_code, hardware_id, license_key, username, password
         )
 
         response = self.send_request(
             method="post",
             endpoint="/deactivate_license",
             json_data=data,
         )
         return response.content.decode()
 
     def check_license(
         self,
         product,
+        bundle_code=None,
         hardware_id=None,
         license_key=None,
         username=None,
         include_expired_features=None,
     ):
         data = self.request_generic_data(
-            {}, product, hardware_id, license_key, username, None
+            {}, product, bundle_code, hardware_id, license_key, username, None
         )
 
         data = self.request_additional_data(
             data=data,
             additional_data={
                 "include_expired_features": "true"
                 if include_expired_features
@@ -255,29 +267,30 @@
             )
 
         return response_json
 
     def activate_offline_dump(
         self,
         product,
+        bundle_code=None,
         hardware_id=None,
         license_key=None,
         username=None,
         password=None,
         app_ver=None,
         os_ver=None,
         hostname=None,
         ip=None,
         is_vm=None,
         vm_info=None,
         mac_address=None,
     ):
         data = {"request": "activation"}
         data = self.request_generic_data(
-            data, product, hardware_id, license_key, username, password
+            data, product, bundle_code, hardware_id, license_key, username, password
         )
         data = self.request_hardware_data(
             data=data,
             os_ver=os_ver,
             hostname=hostname,
             ip=ip,
             mac_address=mac_address,
@@ -340,29 +353,30 @@
             )
 
         return response_json
 
     def deactivate_offline_dump(
         self,
         product,
+        bundle_code=None,
         hardware_id=None,
         license_key=None,
         username=None,
         password=None,
         app_ver=None,
         os_ver=None,
         hostname=None,
         ip=None,
         mac_address=None,
         consumptions=None,
         product_features=None,
     ):
         data = {"request": "deactivation"}
         data = self.request_generic_data(
-            data, product, hardware_id, license_key, username, password
+            data, product, bundle_code, hardware_id, license_key, username, password
         )
         data = self.request_hardware_data(
             data=data,
             os_ver=os_ver,
             hostname=hostname,
             ip=ip,
             mac_address=mac_address,
@@ -394,24 +408,25 @@
         )
 
         return response.content.decode()
 
     def add_consumption(
         self,
         product,
+        bundle_code=None,
         hardware_id=None,
         license_key=None,
         username=None,
         password=None,
         consumptions=None,
         max_overages=None,
         allow_overages=None,
     ):
         data = self.request_generic_data(
-            {}, product, hardware_id, license_key, username, password
+            {}, product, bundle_code, hardware_id, license_key, username, password
         )
         data = self.request_additional_data(
             data=data,
             additional_data={
                 "consumptions": consumptions,
                 "max_overages": max_overages,
                 "allow_overages": allow_overages,
@@ -430,23 +445,24 @@
             )
 
         return response.json()
 
     def add_feature_consumption(
         self,
         product,
+        bundle_code=None,
         hardware_id=None,
         license_key=None,
         username=None,
         password=None,
         feature=None,
         consumptions=None,
     ):
         data = self.request_generic_data(
-            {}, product, hardware_id, license_key, username, password
+            {}, product, bundle_code, hardware_id, license_key, username, password
         )
         data["feature"] = feature
         data = self.request_additional_data(
             data=data,
             additional_data={
                 "consumptions": consumptions,
             },
@@ -536,21 +552,22 @@
             )
 
         return response.json()
 
     def track_device_variables(
         self,
         product,
+        bundle_code=None,
         hardware_id=None,
         license_key=None,
         username=None,
         variables=None,
     ):
         data = self.request_generic_data(
-            {}, product, hardware_id, license_key, username, None
+            {}, product, bundle_code, hardware_id, license_key, username, None
         )
         data["variables"] = variables
 
         response = self.send_request(
             method="post",
             endpoint="/track_device_variables",
             json_data=data,
@@ -562,41 +579,43 @@
             )
 
         return response.json()
 
     def floating_release(
         self,
         product,
+        bundle_code=None,
         hardware_id=None,
         license_key=None,
         username=None,
     ):
         data = self.request_generic_data(
-            {}, product, hardware_id, license_key, username, None
+            {}, product, bundle_code, hardware_id, license_key, username, None
         )
 
         response = self.send_request(
             method="post",
             endpoint="/floating/release",
             json_data=data,
         )
 
         return response.content.decode()
 
     def floating_borrow(
         self,
         product,
+        bundle_code=None,
         hardware_id=None,
         license_key=None,
         username=None,
         password=None,
         borrowed_until=None,
     ):
         data = self.request_generic_data(
-            {}, product, hardware_id, license_key, username, password
+            {}, product, bundle_code, hardware_id, license_key, username, password
         )
         data["borrowed_until"] = borrowed_until
 
         response = self.send_request(
             method="post",
             endpoint="/floating/borrow",
             json_data=data,
@@ -623,21 +642,22 @@
         )
 
         return response.content.decode()
 
     def versions(
         self,
         product,
+        bundle_code=None,
         hardware_id=None,
         license_key=None,
         username=None,
         env=None,
     ):
         data = self.request_generic_data(
-            {}, product, hardware_id, license_key, username, None
+            {}, product, bundle_code, hardware_id, license_key, username, None
         )
         data = self.request_additional_data(
             data=data,
             additional_data={
                 "env": env,
             },
         )
@@ -654,22 +674,23 @@
             )
 
         return response.json()
 
     def installation_file(
         self,
         product,
+        bundle_code=None,
         hardware_id=None,
         license_key=None,
         username=None,
         env=None,
         version=None,
     ):
         data = self.request_generic_data(
-            {}, product, hardware_id, license_key, username, None
+            {}, product, bundle_code, hardware_id, license_key, username, None
         )
         data = self.request_additional_data(
             data=data,
             additional_data={
                 "env": env,
                 "version": version,
             },
@@ -726,20 +747,21 @@
             )
 
         return response.json()
 
     def get_device_variables(
         self,
         product,
+        bundle_code=None,
         hardware_id=None,
         license_key=None,
         username=None,
     ):
         data = self.request_generic_data(
-            {}, product, hardware_id, license_key, username, None
+            {}, product, bundle_code, hardware_id, license_key, username, None
         )
 
         response = self.send_request(
             method="get",
             endpoint="/get_device_variables",
             params=data,
         )
@@ -748,18 +770,24 @@
             self.signature_verifier.verify_license_signature_v2(
                 response.content, response.headers.get("LicenseSignature")
             )
 
         return response.json()
 
     def check_license_feature(
-        self, product, feature, hardware_id=None, license_key=None, username=None
+        self,
+        product,
+        feature,
+        bundle_code=None,
+        hardware_id=None,
+        license_key=None,
+        username=None,
     ):
         data = self.request_generic_data(
-            {}, product, hardware_id, license_key, username, None
+            {}, product, bundle_code, hardware_id, license_key, username, None
         )
         data = self.request_additional_data(
             data=data,
             additional_data={
                 "feature": feature,
             },
         )
@@ -776,20 +804,21 @@
 
         return response.json()
 
     def floating_feature_release(
         self,
         product,
         feature,
+        bundle_code=None,
         hardware_id=None,
         license_key=None,
         username=None,
     ):
         data = self.request_generic_data(
-            {}, product, hardware_id, license_key, username, None
+            {}, product, bundle_code, hardware_id, license_key, username, None
         )
         data = self.request_additional_data(
             data=data,
             additional_data={
                 "feature": feature,
             },
         )
```

### Comparing `licensespring-2.0.0/licensespring/api/authorization.py` & `licensespring-2.0.1/licensespring/api/authorization.py`

 * *Files identical despite different names*

### Comparing `licensespring-2.0.0/licensespring/api/error.py` & `licensespring-2.0.1/licensespring/api/error.py`

 * *Files identical despite different names*

### Comparing `licensespring-2.0.0/licensespring/api/signature.py` & `licensespring-2.0.1/licensespring/api/signature.py`

 * *Files identical despite different names*

### Comparing `licensespring-2.0.0/licensespring/hardware/__init__.py` & `licensespring-2.0.1/licensespring/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `licensespring-2.0.0/licensespring/licensefile/__init__.py` & `licensespring-2.0.1/licensespring/licensefile/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,25 @@
+from __future__ import annotations
+
+import logging
 from datetime import datetime, timezone
+from typing import Callable
 
 from requests.exceptions import RequestException
 
 from licensespring.api.error import ClientError
 from licensespring.licensefile.error import (
     ClockTamperedException,
     ConfigurationMismatch,
-    ConsumptionError,
     ErrorType,
-    LicenseSpringTypeError,
     LicenseStateException,
     TimeoutExpiredException,
     VMIsNotAllowedException,
 )
+from licensespring.watchdog import LicenseWatchdog
 
 
 class License:
     """
     Represents and manages license operations including activation, deactivation,
     and consumption tracking for a software product.
 
@@ -27,28 +30,37 @@
         check_license_status(self): Verifies the current status of the license, raising exceptions if the license is not enabled, not active, or expired.
         check(self, include_expired_features=False, req_overages=-1): Performs an online check to sync license data with the backend
         deactivate(self, delete_license=False): Deactivates the license and optionally deletes the local license file.
         local_check(self): Performs a local check of the license against product code, hardware ID, and VM restrictions.
         add_local_consumption(self, consumptions=1): Adds local consumption records for consumption-based licenses,
         sync_consumption(self, req_overages=-1): Syncs local consumption data with the server, adjusting for overages if specified.
         is_grace_period(self, e: Exception): Determines if the current license state is within a grace period
+        setup_license_watch_dog(self,callback,timeout):Initializes and starts the license watchdog with the specified callback and timeout.
+        stop_license_watch_dog(self): Stops the license watchdog if it is currently running.
+        floating_borrow(self,borrow_until:str): Attempts to borrow a floating license until the specified date.
+        floating_release(self,throw_e:bool): Releases a borrowed floating license and updates the license status accordingly.
 
 
     Attributes:
         product (str): The software product this license is associated with.
         api_client: An instance responsible for communicating with the licensing API.
         licensefile_handler: Handles local license file operations such as reading and writing.
     """
 
     def __init__(self, product, api_client, licensefile_handler) -> None:
         self.product = product
         self.api_client = api_client
         self.licensefile_handler = licensefile_handler
+        self.watch_dog = None
 
     def is_floating_expired(self) -> bool:
+        if self.licensefile_handler._cache.is_floating_license():
+            return self.licensefile_handler._cache.floating_period < datetime.now(
+                timezone.utc
+            ).replace(tzinfo=None)
         return False
 
     def is_validity_period_expired(self) -> bool:
         """
         Determines whether the license's validity period has expired.
 
         Returns:
@@ -59,15 +71,15 @@
             return True
 
         if isinstance(self.licensefile_handler._cache.validity_period, datetime):
             if (
                 self.licensefile_handler._cache.validity_with_grace_period()
                 < datetime.now(timezone.utc).replace(tzinfo=None)
             ):
-                self.licensefile_handler._cache.is_expired = True
+                self.licensefile_handler._cache.set_boolean("is_expired", True)
 
                 return True
 
         return False
 
     def check_license_status(self) -> None:
         """
@@ -108,43 +120,64 @@
             dict: The response from the license check operation.
 
         Raises:
             Exceptions: Various exceptions can be raised depending on the API client's implementation and the response from the licensing server.
         """
 
         try:
+            # Add logic for floating server
+            logging.info("Online check started")
+
             response = self.api_client.check_license(
                 product=self.licensefile_handler._cache.product,
+                bundle_code=self.licensefile_handler._cache.bundle_code,
                 hardware_id=None,
                 license_key=self.licensefile_handler._cache.license_key,
                 username=self.licensefile_handler._cache.username,
                 include_expired_features=include_expired_features,
             )
 
-            self.licensefile_handler.update_cache("check_license", response)
+            self.licensefile_handler._cache.update_cache("check_license", response)
+            self.licensefile_handler._cache.update_floating_period(
+                self.licensefile_handler._cache.borrowed_until
+            )
+
+            for (
+                feature
+            ) in self.licensefile_handler._cache.feature_manager.return_features_list():
+                self.sync_feature_consumption(feature)
 
             if self.licensefile_handler._cache.license_type == "consumption":
                 self.sync_consumption(req_overages=-1)
 
             self.licensefile_handler._cache.reset_grace_period_start_date()
 
+            logging.info("Online check successful")
+
             return response
 
-        except ClientError as e:
-            self.licensefile_handler._cache.update_from_error_code(e.code)
+        except ClientError as ex:
+            self.licensefile_handler._cache.update_from_error_code(ex.code)
+
+            logging.info(ex)
+            raise ex
 
         except RequestException:
             if (
-                self.licensefile_handler._cache.is_floating == False
+                not self.licensefile_handler._cache.is_floating_license()
                 or self.licensefile_handler._cache.is_active_floating_cloud()
             ) and self.is_grace_period():
                 return None
 
             raise RequestException("Grace period not allowed/passed")
 
+        except Exception as ex:
+            logging.info(ex)
+            raise ex
+
         finally:
             self.licensefile_handler.save_licensefile()
             self.check_license_status()
 
     def deactivate(self, delete_license=False) -> None:
         """
         Deactivates the license and optionally deletes the local license file.
@@ -157,31 +190,26 @@
         if not self.licensefile_handler._cache.license_active:
             if delete_license:
                 self.licensefile_handler.delete_licensefile()
             return None
 
         self.api_client.deactivate_license(
             product=self.licensefile_handler._cache.product,
+            bundle_code=self.licensefile_handler._cache.bundle_code,
             hardware_id=None,
             license_key=self.licensefile_handler._cache.license_key,
             username=self.licensefile_handler._cache.username,
             password=self.licensefile_handler._cache.password,
         )
 
         if delete_license:
             self.licensefile_handler.delete_licensefile()
             return None
 
-        if self.licensefile_handler._cache.times_activated > 0:
-            self.licensefile_handler._cache.times_activated -= 1
-
-        else:
-            self.licensefile_handler._cache.times_activated = 0
-
-        self.licensefile_handler._cache.license_active = False
+        self.licensefile_handler._cache.deactivate()
         self.licensefile_handler.save_licensefile()
 
     def local_check(self) -> None:
         """
         Performs a local check of the license, ensuring product code, hardware ID, VM (virtual machine), and other conditions are met.
 
         Raises:
@@ -248,58 +276,103 @@
 
         response = self.api_client.change_password(
             self.licensefile_handler._cache.username,
             password=password,
             new_password=new_password,
         )
 
-        self.licensefile_handler._cache.password = new_password
+        self.licensefile_handler._cache.update_password(new_password)
 
         return response
 
-    def add_local_consumption(self, consumptions=1) -> dict:
+    def add_local_consumption(self, consumptions=1) -> None:
+        """
+        Adds local consumption to the license
+        Params:
+            consumptions (int,optional): Number of consumptions.
+
+        Returns: None
+        """
+
+        self.licensefile_handler._cache.update_consumption(consumptions)
+
+    def add_local_feature_consumption(self, feature: str, consumptions=1) -> None:
+        """
+        Adds local consumption to the feature.
+        Params:
+            feature (str): feature code.
+            consumptions (int,optional): Number of consumptions.
+        """
+
+        self.licensefile_handler._cache.update_feature_consumption(
+            feature, consumptions
+        )
+
+    def sync_feature_consumption(self, feature) -> bool:
         """
-        Adds local consumptions for consumption-based licenses.
+        Syncs the local consumption data with the server for consumption-based licenses.
 
         Args:
-            consumptions (int): The number of consumptions to add locally.
+            feature (str): feature code.
 
         Returns:
-            dict: The updated license cache reflecting the new consumption count.
+            bool: True if the consumption data was successfully synchronized; False otherwise.
 
-        Raises:
-            LicenseTypeError: If the license is not of type 'consumption'.
-            ConsumptionError: If adding the consumptions would exceed the allowed maximum.
         """
 
-        if self.licensefile_handler._cache.license_type != "consumption":
-            raise LicenseSpringTypeError(
-                ErrorType.WRONG_LICENSE_TYPE,
-                f" WRONG License Type: {self.licensefile_handler._cache.license_type}",
-            )
-
-        elif self.licensefile_handler._cache.allow_unlimited_consumptions:
-            self.licensefile_handler._cache.local_consumption += consumptions
-
-        elif (
-            self.licensefile_handler._cache.max_consumptions
-            + self.licensefile_handler._cache.max_overages
-            < self.licensefile_handler._cache.local_consumption
-            + consumptions
-            + self.licensefile_handler._cache.total_consumptions
-        ):
-            raise ConsumptionError(
-                ErrorType.NOT_ENOUGH_LICENSE_CONSUMPTIONS,
-                "Not enough conusmptions left!",
+        if not hasattr(self.licensefile_handler._cache.feature_manager, feature):
+            return False
+
+        feature_obj = getattr(self.licensefile_handler._cache.feature_manager, feature)
+
+        if not hasattr(feature_obj, "local_consumption"):
+            return False
+
+        if feature_obj.local_consumption == 0:
+            return False
+
+        try:
+            response = self.api_client.add_feature_consumption(
+                product=self.product,
+                bundle_code=self.licensefile_handler._cache.bundle_code,
+                hardware_id=None,
+                license_key=self.licensefile_handler._cache.license_key,
+                username=self.licensefile_handler._cache.username,
+                password=self.licensefile_handler._cache.password,
+                feature=feature,
+                consumptions=feature_obj.local_consumption,
             )
 
+        except ClientError as ex:
+            logging.info(ex)
+            raise ex
+
+        except RequestException as ex:
+            if self.is_grace_period():
+                self.licensefile_handler.save_licensefile()
+                self.check_license_status()
+
+                return False
+
+            raise RequestException("Grace period not allowed/passed")
+
+        except Exception as ex:
+            logging.info(ex)
+            raise ex
+
         else:
-            self.licensefile_handler._cache.local_consumption += consumptions
+            self.licensefile_handler._cache.update_cache(
+                "feature_consumption", response, feature
+            )
 
-            return self.licensefile_handler.cache
+            self.licensefile_handler._cache.reset_grace_period_start_date()
+
+            self.licensefile_handler.save_licensefile()
+
+            return True
 
     def sync_consumption(self, req_overages=-1) -> bool:
         """
         Syncs the local consumption data with the server for consumption-based licenses.
 
         Args:
             req_overages (int, optional): Specifies the behavior for requesting consumption overages.
@@ -330,38 +403,44 @@
 
             else:
                 max_overages = None
                 allow_overages = None
 
             response = self.api_client.add_consumption(
                 product=self.licensefile_handler._cache.product,
+                bundle_code=self.licensefile_handler._cache.bundle_code,
                 license_key=self.licensefile_handler._cache.license_key,
                 username=self.licensefile_handler._cache.username,
                 password=self.licensefile_handler._cache.password,
                 consumptions=self.licensefile_handler._cache.local_consumption,
                 max_overages=max_overages,
                 allow_overages=allow_overages,
             )
 
-        except ClientError as e:
-            raise e
+        except ClientError as ex:
+            logging.info(ex)
+            raise ex
 
-        except RequestException as e:
+        except RequestException as ex:
             if self.is_grace_period():
                 self.licensefile_handler.save_licensefile()
                 self.check_license_status()
 
                 return False
 
             raise RequestException("Grace period not allowed/passed")
 
-        else:
-            self.licensefile_handler._cache.local_consumption = 0
+        except Exception as ex:
+            logging.info(ex)
+            raise ex
 
-            self.licensefile_handler.update_cache("consumptions", response)
+        else:
+            self.licensefile_handler._cache.update_cache(
+                "license_consumption", response
+            )
 
             self.licensefile_handler._cache.reset_grace_period_start_date()
             self.licensefile_handler.save_licensefile()
 
             return True
 
     def is_grace_period(self) -> bool:
@@ -391,7 +470,174 @@
 
             return (
                 datetime.now(timezone.utc).replace(tzinfo=None)
                 < self.licensefile_handler._cache.grace_period_end_date()
             )
 
         return False
+
+    def setup_license_watch_dog(self, callback: Callable, timeout: int) -> None:
+        """
+        Initializes and starts the license watchdog with the specified callback and timeout.
+
+        Args:
+            callback: A callable to be executed by the watchdog in response to specific events or conditions.
+            timeout: The period in minutes after which the watchdog should perform its checks.
+
+        Side Effects:
+            - Instantiates the LicenseWatchdog class and stores the instance.
+            - Starts the watchdog thread.
+        """
+        self.watch_dog = LicenseWatchdog(self, callback, timeout)
+        self.watch_dog.run()
+
+    def stop_license_watch_dog(self) -> None:
+        """
+        Stops the license watchdog if it is currently running.
+
+        Side Effects:
+            - Stops the watchdog thread, if it exists.
+        """
+
+        if self.watch_dog:
+            self.watch_dog.stop()
+
+    def floating_borrow(self, borrow_until: str) -> None:
+        """
+        Attempts to borrow a floating license until the specified date.
+
+        Args:
+            borrow_until: A string representing the date until which the license should be borrowed.
+
+        Returns:
+            None
+
+        Side Effects:
+            - Checks if the license is floating or floating cloud type and attempts to borrow it.
+            - Updates the license cache and stops the license watchdog if borrowing is successful.
+        """
+
+        if not self.licensefile_handler._cache.is_floating_license():
+            return None
+
+        response = self.api_client.floating_borrow(
+            product=self.licensefile_handler._cache.product,
+            bundle_code=self.licensefile_handler._cache.bundle_code,
+            hardware_id=None,
+            license_key=self.licensefile_handler._cache.license_key,
+            username=self.licensefile_handler._cache.username,
+            borrowed_until=borrow_until,
+        )
+
+        self.licensefile_handler._cache.set_boolean("is_borrowed", True)
+
+        self.stop_license_watch_dog()
+
+        self.licensefile_handler._cache.update_cache("normal", response)
+        self.licensefile_handler._cache.update_floating_period(
+            self.licensefile_handler._cache.borrowed_until
+        )
+        self.licensefile_handler.save_licensefile()
+
+    def floating_release(self, throw_e: bool):
+        """
+        Releases a borrowed floating license and updates the license status accordingly.
+
+        Args:
+            throw_e: A boolean indicating whether to raise an exception on failure.
+
+        Returns:
+            None
+
+        Side Effects:
+            - Attempts to release the floating license and update the license cache.
+            - Logs and potentially raises an exception if an error occurs during release.
+        """
+
+        if not self.licensefile_handler._cache.is_floating_license():
+            return None
+
+        try:
+            self.check_license_status()
+
+            # Add logic for both floating cloud and floating license
+
+            if self.licensefile_handler._cache.is_active_floating_cloud():
+                self.api_client.floating_release(
+                    product=self.licensefile_handler._cache.product,
+                    bundle_code=self.licensefile_handler._cache.bundle_code,
+                    hardware_id=None,
+                    license_key=self.licensefile_handler._cache.license_key,
+                    username=self.licensefile_handler._cache.username,
+                )
+
+                self.licensefile_handler._cache.release_license()
+                self.licensefile_handler.save_licensefile()
+
+        except Exception as ex:
+            if throw_e:
+                logging.info(ex)
+                raise ex
+
+    def check_feature(self, feature: str, add_to_watchdog=False) -> None:
+        """
+        Checks for a specific license feature and updates the license cache accordingly.
+
+        Args:
+            feature: feature code.
+            add_to_watchdog: A boolean indicating whether to add the feature check to a watchdog routine.
+
+        Returns:
+            None
+
+
+        """
+        # Add watchdog logic
+        try:
+            response = self.api_client.check_license_feature(
+                product=self.licensefile_handler._cache.product,
+                feature=feature,
+                bundle_code=self.licensefile_handler._cache.bundle_code,
+                hardware_id=None,
+                license_key=self.licensefile_handler._cache.license_key,
+                username=self.licensefile_handler._cache.username,
+            )
+
+            self.licensefile_handler._cache.register_feature(feature)
+            self.licensefile_handler._cache.update_cache(
+                "register_feature", response, feature
+            )
+
+            self.licensefile_handler.save_licensefile()
+
+        except Exception as ex:
+            logging.info(ex)
+            raise ex
+
+    def release_feature(self, feature: str):
+        """
+        Releases a borrowed license feature and updates the license cache accordingly.
+
+        Args:
+            feature: The feature code.
+
+        Returns:
+            None
+        """
+
+        # Add watchdog logic
+        try:
+            self.api_client.floating_feature_release(
+                product=self.licensefile_handler._cache.product,
+                feature=feature,
+                bundle_code=self.licensefile_handler._cache.bundle_code,
+                hardware_id=None,
+                license_key=self.licensefile_handler._cache.license_key,
+                username=self.licensefile_handler._cache.username,
+            )
+
+            self.licensefile_handler._cache.release_feature(feature)
+            self.licensefile_handler.save_licensefile()
+
+        except Exception as ex:
+            logging.info(ex)
+            raise ex
```

### Comparing `licensespring-2.0.0/licensespring/licensefile/config.py` & `licensespring-2.0.1/licensespring/licensefile/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from licensespring.api.signature import SignatureVerifier
 from licensespring.hardware import HardwareIdProvider
 
 
 class Configuration:
     """
     A class to configure settings for a license management system.
```

### Comparing `licensespring-2.0.0/licensespring/licensefile/data_storage.py` & `licensespring-2.0.1/licensespring/licensefile/data_storage.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from __future__ import annotations
+
 import json
 import os
-from datetime import datetime, timezone
 
 from licensespring.licensefile.config import Configuration
 from licensespring.licensefile.default_crypto import DefaultCryptoProvider
 from licensespring.licensefile.error import ErrorType, LicenseDeleted
 from licensespring.licensefile.license_data import LicenseData
 
 
@@ -17,15 +18,14 @@
         _cache (LicenseData): Instance of LicenseData for managing license attributes in memory.
         _filename (str): The name of the file used for storing the license information.
         _license_path (str): The file path where the license file is stored.
 
     Methods:
         cache: Returns the current license data stored in memory.
         license_path: Returns the file path for the license file.
-        update_cache(method, response): Updates the license data in memory based on the response from a license operation.
         save_licensefile(): Encrypts and saves the license data to a file.
         load_licensefile(): Loads and decrypts the license data from a file.
         set_path(product_code, custom_path): Sets the file path for the license file based on the operating system.
         delete_licensefile(): Deletes the license file and clears the license data in memory.
     """
 
     def __init__(self, conf: Configuration):
@@ -39,74 +39,44 @@
         )
 
         self._filename = self._conf._filename
         self._license_path = self.set_path(self._conf._product, self._conf._file_path)
 
     @property
     def cache(self):
-        return self._cache.__dict__
+        return self._cache.to_json()
 
     @property
     def license_path(self):
         return self._license_path
 
-    def update_cache(self, method: str, response: dict):
-        """
-        Updates licensefile data inside memory.
-
-        Parameters:
-        response (dict): Response of license activation or license check.
-
-        Returns: None
-        """
-
-        self._cache.last_usage = datetime.now(timezone.utc).replace(tzinfo=None)
-
-        if method == "check_license":
-            self._cache.last_check = datetime.now(timezone.utc).replace(tzinfo=None)
-            self._cache.from_json_to_attr(response)
-            self._cache.features_setup()
-
-        elif method == "activate_license":
-            self._cache.from_json_to_attr(response)
-            self._cache.local_consumption_setup()
-            self._cache.features_setup()
-            self._cache.grace_period_setup()
-
-            self._cache.license_enabled = True
-            self._cache.is_expired = False
-            self._cache.license_active = True
-
-        elif method == "consumptions":
-            self._cache.from_json_to_attr(response)
-
     def save_licensefile(self):
         """
         Creates path for licensefile
         Saves encrypted string of licensefile JSON
         """
-
-        # Create the folder if it does not exist
-        if not os.path.exists(self.license_path):
-            os.makedirs(self.license_path)
-
         json_string_encrypted = self.encrypt(self._cache.to_json())
+        with self._cache._lock:
+            # Create the folder if it does not exist
+            if not os.path.exists(self.license_path):
+                os.makedirs(self.license_path)
 
-        with open(
-            os.path.join(self.license_path, self._filename + ".key"), "w"
-        ) as file:
-            file.write(json_string_encrypted)
+            with open(
+                os.path.join(self.license_path, self._filename + ".key"), "w"
+            ) as file:
+                file.write(json_string_encrypted)
 
     def load_licensefile(self) -> dict:
         """
         Loads and decrypts licensefile
 
         Returns:
             dict: licensefile
         """
+
         try:
             with open(
                 os.path.join(self.license_path, self._filename + ".key"), "r"
             ) as file:
                 json_string_encrypted = file.read()
 
             licensefile_dict = json.loads(self.decrypt(json_string_encrypted))
```

### Comparing `licensespring-2.0.0/licensespring/licensefile/default_crypto.py` & `licensespring-2.0.1/licensespring/licensefile/default_crypto.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from __future__ import annotations
+
 import base64
 import binascii
-import hashlib
-import os
 
 from Crypto.Cipher import AES
 from Crypto.Hash import SHA256
 from Crypto.Protocol.KDF import PBKDF2
 from Crypto.Random import get_random_bytes
 from Crypto.Util import Padding
```

### Comparing `licensespring-2.0.0/licensespring/licensefile/error.py` & `licensespring-2.0.1/licensespring/licensefile/error.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from enum import Enum, auto
 
 
 class ErrorType(Enum):
 
     """Licensefile error"""
 
@@ -24,14 +26,16 @@
     FLOATING_TIMEOUT = auto()
 
     CLOCK_TAMPERED = auto()
 
     NOT_ENOUGH_LICENSE_CONSUMPTIONS = auto()
     NOT_ENOUGH_FEATURE_CONSUMPTIONS = auto()
 
+    UNSUPPORTED_PRODUCT_FEATURE = auto()
+
 
 class LicenseSpringException(Exception):
     """Base exception class for all LicenseSpring-related errors."""
 
     def __init__(self, error_type: ErrorType, message):
         self.error_type = error_type
         self.message = message
@@ -82,7 +86,12 @@
     def __init__(self, error_type: ErrorType, message):
         super().__init__(error_type, message)
 
 
 class ConsumptionError(LicenseSpringException):
     def __init__(self, error_type: ErrorType, message):
         super().__init__(error_type, message)
+
+
+class ItemNotFoundError(LicenseSpringException):
+    def __init__(self, error_type: ErrorType, message):
+        super().__init__(error_type, message)
```

### Comparing `licensespring-2.0.0/licensespring/licensefile/license_manager.py` & `licensespring-2.0.1/licensespring/licensefile/license_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -105,14 +105,15 @@
         self.licensefile_handler.load_licensefile()
 
         return License(self._product, self.api_client, self.licensefile_handler)
 
     def activate_license(
         self,
         license_id: LicenseID,
+        bundle_code: str = None,
         hardware_id: str = None,
         customer_account_code: str = None,
         id_token: str = None,
         code: str = None,
         app_ver: str = None,
         os_ver: str = None,
         hostname: str = None,
@@ -125,14 +126,15 @@
         Activates a license with the license server and updates local license data accordingly.
 
         This method supports a variety of parameters to accommodate different licensing scenarios,
         including key-based activation, user-based activation
 
         Args:
             license_id (LicenseID): An instance containing the license key or user credentials.
+            bundle_code (str, optional): specify unique bundle_code of a bundle
             hardware_id (str, optional): A unique identifier for the hardware.
             customer_account_code (str, optional): An account code for the customer.
             id_token (str, optional): Token for identity verification.
             code (str, optional): An additional code for license verification.
             app_ver (str, optional): The version of the application requesting activation.
             os_ver (str, optional): The operating system version of the host.
             hostname (str, optional): The hostname of the device requesting activation.
@@ -143,14 +145,15 @@
 
         Returns:
             License: An instance of the License class reflecting the activated license.
         """
 
         response = self.api_client.activate_license(
             product=self._product,
+            bundle_code=bundle_code,
             hardware_id=hardware_id,
             license_key=license_id.key,
             username=license_id.username,
             password=license_id.password,
             customer_account_code=customer_account_code,
             id_token=id_token,
             code=code,
@@ -161,16 +164,16 @@
             is_vm=is_vm,
             vm_info=vm_info,
             mac_address=mac_address,
         )
 
         response["username"] = license_id.username
         response["password"] = license_id.password
-
-        self.licensefile_handler.update_cache("activate_license", response)
+        response["bundle_code"] = bundle_code
+        self.licensefile_handler._cache.update_cache("activate_license", response)
         self.licensefile_handler.save_licensefile()
 
         return License(
             self._product,
             api_client=self.api_client,
             licensefile_handler=self.licensefile_handler,
         )
```

### Comparing `licensespring-2.0.0/licensespring/webhook/signature.py` & `licensespring-2.0.1/licensespring/webhook/signature.py`

 * *Files identical despite different names*

### Comparing `licensespring-2.0.0/licensespring/webhook/utils.py` & `licensespring-2.0.1/licensespring/webhook/utils.py`

 * *Files identical despite different names*

### Comparing `licensespring-2.0.0/PKG-INFO` & `licensespring-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: licensespring
-Version: 2.0.0
+Version: 2.0.1
 Summary: LicenseSpring Python Library
 Home-page: https://licensespring.com/
 License: MIT
 Author: Toni Sredanović
 Author-email: toni@licensespring.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -780,9 +780,9 @@
 |--------------------|-----------|-----------------------------------------------------|----------------------------------------------------------|
 | certifi            | 2023.7.22 | Mozilla Public License 2.0 (MPL 2.0)                | https://github.com/certifi/python-certifi                |
 | charset-normalizer | 3.3.0     | MIT License                                         | https://github.com/Ousret/charset_normalizer             |
 | idna               | 3.4       | BSD License                                         | https://github.com/kjd/idna                              |
 | pycryptodome       | 3.19.0    | Apache Software License; BSD License; Public Domain | https://www.pycryptodome.org                             |
 | requests           | 2.31.0    | Apache Software License                             | https://requests.readthedocs.io                          |
 | urllib3            | 2.0.7     | MIT License                                         | https://github.com/urllib3/urllib3/blob/main/CHANGES.rst |
-| winregistry        | 1.1.1     | MIT License                                         | https://github.com/shpaker/winregistry                   |
+| winregistry        | 1.1.1     | UNKNOWN                                             | https://github.com/shpaker/winregistry                   |
```

