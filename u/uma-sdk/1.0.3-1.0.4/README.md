# Comparing `tmp/uma-sdk-1.0.3.zip` & `tmp/uma_sdk-1.0.4.zip`

## zipinfo {}

```diff
@@ -1,49 +1,49 @@
-Zip file size: 39674 bytes, number of entries: 47
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-02 16:55 uma-sdk-1.0.3/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-02 16:55 uma-sdk-1.0.3/uma/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-02 16:55 uma-sdk-1.0.3/uma_sdk.egg-info/
--rwxr-xr-x  2.0 unx       87 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/setup.py
--rw-r--r--  2.0 unx      648 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/setup.cfg
--rw-r--r--  2.0 unx      133 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/README.md
--rw-r--r--  2.0 unx    11352 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/LICENSE
--rw-r--r--  2.0 unx       81 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/pyproject.toml
--rw-r--r--  2.0 unx      631 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/PKG-INFO
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/
--rw-r--r--  2.0 unx     2160 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/__init__.py
--rw-r--r--  2.0 unx     1117 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/cert_utils.py
--rw-r--r--  2.0 unx     3407 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/JSONable.py
--rw-r--r--  2.0 unx      284 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/uma_invoice_creator.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/py.typed
--rw-r--r--  2.0 unx    30116 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/uma.py
--rw-r--r--  2.0 unx      266 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/urls.py
--rw-r--r--  2.0 unx     2061 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/nonce_cache.py
--rw-r--r--  2.0 unx     2878 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/version.py
--rw-r--r--  2.0 unx     1624 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/public_key_cache.py
--rw-r--r--  2.0 unx      868 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/exceptions.py
--rw-r--r--  2.0 unx      239 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/type_utils.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/v1/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/v0/
--rw-r--r--  2.0 unx      557 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/counterparty_data.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/__init__.py
--rw-r--r--  2.0 unx     1724 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/post_tx_callback.py
--rw-r--r--  2.0 unx     4498 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/pubkey_response.py
--rw-r--r--  2.0 unx      231 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/kyc_status.py
--rw-r--r--  2.0 unx     4609 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/currency.py
--rw-r--r--  2.0 unx      132 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/payee_data.py
--rw-r--r--  2.0 unx     3324 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/lnurlp_response.py
--rw-r--r--  2.0 unx     2307 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/payer_data.py
--rw-r--r--  2.0 unx     2591 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/lnurlp_request.py
--rw-r--r--  2.0 unx     6328 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/payreq.py
--rw-r--r--  2.0 unx     8829 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/payreq_response.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/v1/__init__.py
--rw-r--r--  2.0 unx     2702 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/v1/currency.py
--rw-r--r--  2.0 unx     4294 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/v1/payreq.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/v0/__init__.py
--rw-r--r--  2.0 unx     1950 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/v0/currency.py
--rw-r--r--  2.0 unx     1788 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma/protocol/v0/payreq.py
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma_sdk.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       30 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma_sdk.egg-info/requires.txt
--rw-r--r--  2.0 unx        4 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma_sdk.egg-info/top_level.txt
--rw-r--r--  2.0 unx      924 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma_sdk.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      631 b- defN 24-Apr-02 16:55 uma-sdk-1.0.3/uma_sdk.egg-info/PKG-INFO
-47 files, 105406 bytes uncompressed, 32846 bytes compressed:  68.8%
+Zip file size: 39790 bytes, number of entries: 47
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 17:34 uma_sdk-1.0.4/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 17:34 uma_sdk-1.0.4/uma_sdk.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 17:34 uma_sdk-1.0.4/uma/
+-rw-r--r--  2.0 unx    11352 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/LICENSE
+-rwxr-xr-x  2.0 unx       87 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/setup.py
+-rw-r--r--  2.0 unx      133 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/README.md
+-rw-r--r--  2.0 unx       81 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/pyproject.toml
+-rw-r--r--  2.0 unx      648 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/setup.cfg
+-rw-r--r--  2.0 unx      631 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/PKG-INFO
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma_sdk.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx      924 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma_sdk.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma_sdk.egg-info/top_level.txt
+-rw-r--r--  2.0 unx      631 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma_sdk.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       30 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma_sdk.egg-info/requires.txt
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/
+-rw-r--r--  2.0 unx     3407 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/JSONable.py
+-rw-r--r--  2.0 unx     1624 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/public_key_cache.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/py.typed
+-rw-r--r--  2.0 unx      284 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/uma_invoice_creator.py
+-rw-r--r--  2.0 unx     2878 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/version.py
+-rw-r--r--  2.0 unx      239 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/type_utils.py
+-rw-r--r--  2.0 unx     2061 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/nonce_cache.py
+-rw-r--r--  2.0 unx     2160 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/__init__.py
+-rw-r--r--  2.0 unx     1117 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/cert_utils.py
+-rw-r--r--  2.0 unx      266 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/urls.py
+-rw-r--r--  2.0 unx    30711 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/uma.py
+-rw-r--r--  2.0 unx      868 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/exceptions.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/v1/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/v0/
+-rw-r--r--  2.0 unx     2591 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/lnurlp_request.py
+-rw-r--r--  2.0 unx     8829 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/payreq_response.py
+-rw-r--r--  2.0 unx     1724 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/post_tx_callback.py
+-rw-r--r--  2.0 unx      132 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/payee_data.py
+-rw-r--r--  2.0 unx     2307 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/payer_data.py
+-rw-r--r--  2.0 unx      557 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/counterparty_data.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/__init__.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/lnurlp_response.py
+-rw-r--r--  2.0 unx     6328 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/payreq.py
+-rw-r--r--  2.0 unx     4498 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/pubkey_response.py
+-rw-r--r--  2.0 unx     4609 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/currency.py
+-rw-r--r--  2.0 unx      231 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/kyc_status.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/v1/__init__.py
+-rw-r--r--  2.0 unx     4294 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/v1/payreq.py
+-rw-r--r--  2.0 unx     2702 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/v1/currency.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/v0/__init__.py
+-rw-r--r--  2.0 unx     1788 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/v0/payreq.py
+-rw-r--r--  2.0 unx     1950 b- defN 24-Apr-24 17:34 uma_sdk-1.0.4/uma/protocol/v0/currency.py
+47 files, 106001 bytes uncompressed, 32962 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -1,142 +1,142 @@
-Filename: uma-sdk-1.0.3/
+Filename: uma_sdk-1.0.4/
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/
+Filename: uma_sdk-1.0.4/uma_sdk.egg-info/
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma_sdk.egg-info/
+Filename: uma_sdk-1.0.4/uma/
 Comment: 
 
-Filename: uma-sdk-1.0.3/setup.py
+Filename: uma_sdk-1.0.4/LICENSE
 Comment: 
 
-Filename: uma-sdk-1.0.3/setup.cfg
+Filename: uma_sdk-1.0.4/setup.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/README.md
+Filename: uma_sdk-1.0.4/README.md
 Comment: 
 
-Filename: uma-sdk-1.0.3/LICENSE
+Filename: uma_sdk-1.0.4/pyproject.toml
 Comment: 
 
-Filename: uma-sdk-1.0.3/pyproject.toml
+Filename: uma_sdk-1.0.4/setup.cfg
 Comment: 
 
-Filename: uma-sdk-1.0.3/PKG-INFO
+Filename: uma_sdk-1.0.4/PKG-INFO
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/protocol/
+Filename: uma_sdk-1.0.4/uma_sdk.egg-info/dependency_links.txt
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/__init__.py
+Filename: uma_sdk-1.0.4/uma_sdk.egg-info/SOURCES.txt
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/cert_utils.py
+Filename: uma_sdk-1.0.4/uma_sdk.egg-info/top_level.txt
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/JSONable.py
+Filename: uma_sdk-1.0.4/uma_sdk.egg-info/PKG-INFO
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/uma_invoice_creator.py
+Filename: uma_sdk-1.0.4/uma_sdk.egg-info/requires.txt
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/py.typed
+Filename: uma_sdk-1.0.4/uma/protocol/
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/uma.py
+Filename: uma_sdk-1.0.4/uma/JSONable.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/urls.py
+Filename: uma_sdk-1.0.4/uma/public_key_cache.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/nonce_cache.py
+Filename: uma_sdk-1.0.4/uma/py.typed
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/version.py
+Filename: uma_sdk-1.0.4/uma/uma_invoice_creator.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/public_key_cache.py
+Filename: uma_sdk-1.0.4/uma/version.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/exceptions.py
+Filename: uma_sdk-1.0.4/uma/type_utils.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/type_utils.py
+Filename: uma_sdk-1.0.4/uma/nonce_cache.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/protocol/v1/
+Filename: uma_sdk-1.0.4/uma/__init__.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/protocol/v0/
+Filename: uma_sdk-1.0.4/uma/cert_utils.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/protocol/counterparty_data.py
+Filename: uma_sdk-1.0.4/uma/urls.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/protocol/__init__.py
+Filename: uma_sdk-1.0.4/uma/uma.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/protocol/post_tx_callback.py
+Filename: uma_sdk-1.0.4/uma/exceptions.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/protocol/pubkey_response.py
+Filename: uma_sdk-1.0.4/uma/protocol/v1/
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/protocol/kyc_status.py
+Filename: uma_sdk-1.0.4/uma/protocol/v0/
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/protocol/currency.py
+Filename: uma_sdk-1.0.4/uma/protocol/lnurlp_request.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/protocol/payee_data.py
+Filename: uma_sdk-1.0.4/uma/protocol/payreq_response.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/protocol/lnurlp_response.py
+Filename: uma_sdk-1.0.4/uma/protocol/post_tx_callback.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/protocol/payer_data.py
+Filename: uma_sdk-1.0.4/uma/protocol/payee_data.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/protocol/lnurlp_request.py
+Filename: uma_sdk-1.0.4/uma/protocol/payer_data.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/protocol/payreq.py
+Filename: uma_sdk-1.0.4/uma/protocol/counterparty_data.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/protocol/payreq_response.py
+Filename: uma_sdk-1.0.4/uma/protocol/__init__.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/protocol/v1/__init__.py
+Filename: uma_sdk-1.0.4/uma/protocol/lnurlp_response.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/protocol/v1/currency.py
+Filename: uma_sdk-1.0.4/uma/protocol/payreq.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/protocol/v1/payreq.py
+Filename: uma_sdk-1.0.4/uma/protocol/pubkey_response.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/protocol/v0/__init__.py
+Filename: uma_sdk-1.0.4/uma/protocol/currency.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/protocol/v0/currency.py
+Filename: uma_sdk-1.0.4/uma/protocol/kyc_status.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma/protocol/v0/payreq.py
+Filename: uma_sdk-1.0.4/uma/protocol/v1/__init__.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma_sdk.egg-info/dependency_links.txt
+Filename: uma_sdk-1.0.4/uma/protocol/v1/payreq.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma_sdk.egg-info/requires.txt
+Filename: uma_sdk-1.0.4/uma/protocol/v1/currency.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma_sdk.egg-info/top_level.txt
+Filename: uma_sdk-1.0.4/uma/protocol/v0/__init__.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma_sdk.egg-info/SOURCES.txt
+Filename: uma_sdk-1.0.4/uma/protocol/v0/payreq.py
 Comment: 
 
-Filename: uma-sdk-1.0.3/uma_sdk.egg-info/PKG-INFO
+Filename: uma_sdk-1.0.4/uma/protocol/v0/currency.py
 Comment: 
 
 Zip file comment:
```

## Comparing `uma-sdk-1.0.3/setup.cfg` & `uma_sdk-1.0.4/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = uma-sdk
-version = 1.0.3
+version = 1.0.4
 description = Python SDK for UMA (universal money address)
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Lightspark Group, Inc.
 author_email = info@lightspark.com
 license = Apache-2.0
 license_files = LICENSE
```

## Comparing `uma-sdk-1.0.3/LICENSE` & `uma_sdk-1.0.4/LICENSE`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.3/PKG-INFO` & `uma_sdk-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uma-sdk
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python SDK for UMA (universal money address)
 Author: Lightspark Group, Inc.
 Author-email: info@lightspark.com
 License: Apache-2.0
 Project-URL: Documentation, https://app.lightspark.com/docs/uma-sdk/introduction
 Project-URL: Source Code, https://github.com/uma-universal-money-address/uma-python-sdk/
 Description-Content-Type: text/markdown
```

## Comparing `uma-sdk-1.0.3/uma/__init__.py` & `uma_sdk-1.0.4/uma/__init__.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.3/uma/cert_utils.py` & `uma_sdk-1.0.4/uma/cert_utils.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.3/uma/JSONable.py` & `uma_sdk-1.0.4/uma/JSONable.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.3/uma/uma.py` & `uma_sdk-1.0.4/uma/uma.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 from uma.exceptions import (
     InvalidCurrencyException,
     InvalidRequestException,
     InvalidSignatureException,
     UnsupportedVersionException,
 )
 from uma.nonce_cache import INonceCache
-from uma.protocol.counterparty_data import CounterpartyDataOptions
+from uma.protocol.counterparty_data import (
+    CounterpartyDataOption,
+    CounterpartyDataOptions,
+)
 from uma.protocol.currency import Currency
 from uma.protocol.kyc_status import KycStatus
 from uma.protocol.lnurlp_request import LnurlpRequest
 from uma.protocol.lnurlp_response import LnurlComplianceResponse, LnurlpResponse
 from uma.protocol.payer_data import (
     CompliancePayerData,
     PayerData,
@@ -263,14 +266,19 @@
             but not for regular LNURL payments.
         requested_payee_data: the additional data about the payee which is requested by the sending
             VASP, if any.
         comment: A comment that the sender wants to add to the payment. This can only be included
             if the receiver included the `commentAllowed` field in the lnurlp response. The length of
             the comment must be less than or equal to the value of `commentAllowed`.
     """
+    if uma_major_version == 0 and not is_amount_in_receiving_currency:
+        raise InvalidRequestException(
+            "UMA v0 does not support sending amounts in msats. Please set is_amount_in_receiving_currency to True."
+        )
+
     sending_currency_code = (
         receiving_currency_code if is_amount_in_receiving_currency else None
     )
     return PayRequest(
         receiving_currency_code=receiving_currency_code,
         sending_amount_currency_code=sending_currency_code,
         amount=amount,
@@ -619,14 +627,21 @@
         receiver_kyc_status=receiver_kyc_status,
     )
     _validate_currency_options(currency_options)
     # Ensure correct serializing for UMA V0:
     if ParsedVersion.load(uma_version).major == 0:
         for currency in currency_options:
             currency.uma_major_version = 0
+
+    # compliance and identifier are mandatory fields for UMA
+    if "compliance" not in payer_data_options:
+        payer_data_options["compliance"] = CounterpartyDataOption(mandatory=True)
+    if "identifier" not in payer_data_options:
+        payer_data_options["identifier"] = CounterpartyDataOption(mandatory=True)
+
     return LnurlpResponse(
         tag="payRequest",
         callback=callback,
         min_sendable=min_sendable_sats * 1000,
         max_sendable=max_sendable_sats * 1000,
         encoded_metadata=encoded_metadata,
         currencies=currency_options,
```

## Comparing `uma-sdk-1.0.3/uma/nonce_cache.py` & `uma_sdk-1.0.4/uma/nonce_cache.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.3/uma/version.py` & `uma_sdk-1.0.4/uma/version.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.3/uma/public_key_cache.py` & `uma_sdk-1.0.4/uma/public_key_cache.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.3/uma/exceptions.py` & `uma_sdk-1.0.4/uma/exceptions.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.3/uma/protocol/counterparty_data.py` & `uma_sdk-1.0.4/uma/protocol/counterparty_data.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.3/uma/protocol/post_tx_callback.py` & `uma_sdk-1.0.4/uma/protocol/post_tx_callback.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.3/uma/protocol/pubkey_response.py` & `uma_sdk-1.0.4/uma/protocol/pubkey_response.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.3/uma/protocol/currency.py` & `uma_sdk-1.0.4/uma/protocol/currency.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.3/uma/protocol/lnurlp_response.py` & `uma_sdk-1.0.4/uma/protocol/lnurlp_response.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.3/uma/protocol/payer_data.py` & `uma_sdk-1.0.4/uma/protocol/payer_data.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.3/uma/protocol/lnurlp_request.py` & `uma_sdk-1.0.4/uma/protocol/lnurlp_request.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.3/uma/protocol/payreq.py` & `uma_sdk-1.0.4/uma/protocol/payreq.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.3/uma/protocol/payreq_response.py` & `uma_sdk-1.0.4/uma/protocol/payreq_response.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.3/uma/protocol/v1/currency.py` & `uma_sdk-1.0.4/uma/protocol/v1/currency.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.3/uma/protocol/v1/payreq.py` & `uma_sdk-1.0.4/uma/protocol/v1/payreq.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.3/uma/protocol/v0/currency.py` & `uma_sdk-1.0.4/uma/protocol/v0/currency.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.3/uma/protocol/v0/payreq.py` & `uma_sdk-1.0.4/uma/protocol/v0/payreq.py`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.3/uma_sdk.egg-info/SOURCES.txt` & `uma_sdk-1.0.4/uma_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `uma-sdk-1.0.3/uma_sdk.egg-info/PKG-INFO` & `uma_sdk-1.0.4/uma_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uma-sdk
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python SDK for UMA (universal money address)
 Author: Lightspark Group, Inc.
 Author-email: info@lightspark.com
 License: Apache-2.0
 Project-URL: Documentation, https://app.lightspark.com/docs/uma-sdk/introduction
 Project-URL: Source Code, https://github.com/uma-universal-money-address/uma-python-sdk/
 Description-Content-Type: text/markdown
```

