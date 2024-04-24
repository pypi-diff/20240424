# Comparing `tmp/google-cloud-recaptcha-enterprise-1.8.3.tar.gz` & `tmp/google-cloud-recaptcha-enterprise-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-recaptcha-enterprise-1.8.3.tar", last modified: Mon Oct 10 16:24:22 2022, max compression
+gzip compressed data, was "google-cloud-recaptcha-enterprise-1.9.0.tar", last modified: Thu Oct 27 19:38:07 2022, max compression
```

## Comparing `google-cloud-recaptcha-enterprise-1.8.3.tar` & `google-cloud-recaptcha-enterprise-1.9.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:22.001365 google-cloud-recaptcha-enterprise-1.8.3/
--rw-rw-r--   0 root         (0)     1003    11358 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4614 2022-10-10 16:24:22.001365 google-cloud-recaptcha-enterprise-1.8.3/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3853 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:21.993365 google-cloud-recaptcha-enterprise-1.8.3/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:21.993365 google-cloud-recaptcha-enterprise-1.8.3/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:21.997365 google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise/
--rw-rw-r--   0 root         (0)     1003     2960 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise/__init__.py
--rw-rw-r--   0 root         (0)     1003       94 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:21.997365 google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/
--rw-rw-r--   0 root         (0)     1003     2780 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3681 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       94 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:21.997365 google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:21.997365 google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/
--rw-rw-r--   0 root         (0)     1003      817 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    58447 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    71020 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/client.py
--rw-rw-r--   0 root         (0)     1003    23431 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:22.001365 google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/transports/
--rw-rw-r--   0 root         (0)     1003     1309 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11716 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    25760 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    26326 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:22.001365 google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/types/
--rw-rw-r--   0 root         (0)     1003     2552 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    37445 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/types/recaptchaenterprise.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:22.001365 google-cloud-recaptcha-enterprise-1.8.3/google_cloud_recaptcha_enterprise.egg-info/
--rw-r--r--   0 root         (0)     1003     4614 2022-10-10 16:24:21.000000 google-cloud-recaptcha-enterprise-1.8.3/google_cloud_recaptcha_enterprise.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1794 2022-10-10 16:24:21.000000 google-cloud-recaptcha-enterprise-1.8.3/google_cloud_recaptcha_enterprise.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:24:21.000000 google-cloud-recaptcha-enterprise-1.8.3/google_cloud_recaptcha_enterprise.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-10-10 16:24:21.000000 google-cloud-recaptcha-enterprise-1.8.3/google_cloud_recaptcha_enterprise.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:24:21.000000 google-cloud-recaptcha-enterprise-1.8.3/google_cloud_recaptcha_enterprise.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      232 2022-10-10 16:24:21.000000 google-cloud-recaptcha-enterprise-1.8.3/google_cloud_recaptcha_enterprise.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-10-10 16:24:21.000000 google-cloud-recaptcha-enterprise-1.8.3/google_cloud_recaptcha_enterprise.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2022-10-10 16:24:22.001365 google-cloud-recaptcha-enterprise-1.8.3/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2285 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:22.001365 google-cloud-recaptcha-enterprise-1.8.3/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:22.001365 google-cloud-recaptcha-enterprise-1.8.3/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:22.001365 google-cloud-recaptcha-enterprise-1.8.3/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:24:22.001365 google-cloud-recaptcha-enterprise-1.8.3/tests/unit/gapic/recaptchaenterprise_v1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/tests/unit/gapic/recaptchaenterprise_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   176196 2022-10-10 16:20:48.000000 google-cloud-recaptcha-enterprise-1.8.3/tests/unit/gapic/recaptchaenterprise_v1/test_recaptcha_enterprise_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:38:07.004879 google-cloud-recaptcha-enterprise-1.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4614 2022-10-27 19:38:07.004879 google-cloud-recaptcha-enterprise-1.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3853 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:38:06.996880 google-cloud-recaptcha-enterprise-1.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:38:06.996880 google-cloud-recaptcha-enterprise-1.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:38:07.000880 google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise/
+-rw-rw-r--   0 root         (0)     1003     3110 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise/__init__.py
+-rw-rw-r--   0 root         (0)     1003       94 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:38:07.000880 google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/
+-rw-rw-r--   0 root         (0)     1003     2930 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3969 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       94 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:38:07.000880 google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:38:07.000880 google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/
+-rw-rw-r--   0 root         (0)     1003      817 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    62836 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    75643 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/client.py
+-rw-rw-r--   0 root         (0)     1003    23431 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:38:07.000880 google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1309 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12289 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    27217 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    27805 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:38:07.000880 google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2702 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    38900 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/types/recaptchaenterprise.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:38:07.004879 google-cloud-recaptcha-enterprise-1.9.0/google_cloud_recaptcha_enterprise.egg-info/
+-rw-r--r--   0 root         (0)     1003     4614 2022-10-27 19:38:06.000000 google-cloud-recaptcha-enterprise-1.9.0/google_cloud_recaptcha_enterprise.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1794 2022-10-27 19:38:06.000000 google-cloud-recaptcha-enterprise-1.9.0/google_cloud_recaptcha_enterprise.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-10-27 19:38:06.000000 google-cloud-recaptcha-enterprise-1.9.0/google_cloud_recaptcha_enterprise.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-10-27 19:38:06.000000 google-cloud-recaptcha-enterprise-1.9.0/google_cloud_recaptcha_enterprise.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-10-27 19:38:06.000000 google-cloud-recaptcha-enterprise-1.9.0/google_cloud_recaptcha_enterprise.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      232 2022-10-27 19:38:06.000000 google-cloud-recaptcha-enterprise-1.9.0/google_cloud_recaptcha_enterprise.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-10-27 19:38:06.000000 google-cloud-recaptcha-enterprise-1.9.0/google_cloud_recaptcha_enterprise.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2022-10-27 19:38:07.004879 google-cloud-recaptcha-enterprise-1.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2285 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:38:07.004879 google-cloud-recaptcha-enterprise-1.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:38:07.004879 google-cloud-recaptcha-enterprise-1.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:38:07.004879 google-cloud-recaptcha-enterprise-1.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:38:07.004879 google-cloud-recaptcha-enterprise-1.9.0/tests/unit/gapic/recaptchaenterprise_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/tests/unit/gapic/recaptchaenterprise_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   185344 2022-10-27 19:34:40.000000 google-cloud-recaptcha-enterprise-1.9.0/tests/unit/gapic/recaptchaenterprise_v1/test_recaptcha_enterprise_service.py
```

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/LICENSE` & `google-cloud-recaptcha-enterprise-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/MANIFEST.in` & `google-cloud-recaptcha-enterprise-1.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/PKG-INFO` & `google-cloud-recaptcha-enterprise-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-recaptcha-enterprise
-Version: 1.8.3
+Version: 1.9.0
 Home-page: https://github.com/googleapis/python-recaptcha-enterprise
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/README.rst` & `google-cloud-recaptcha-enterprise-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise/__init__.py` & `google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,16 @@
     ListRelatedAccountGroupsRequest,
     ListRelatedAccountGroupsResponse,
     Metrics,
     MigrateKeyRequest,
     PrivatePasswordLeakVerification,
     RelatedAccountGroup,
     RelatedAccountGroupMembership,
+    RetrieveLegacySecretKeyRequest,
+    RetrieveLegacySecretKeyResponse,
     RiskAnalysis,
     ScoreDistribution,
     ScoreMetrics,
     SearchRelatedAccountGroupMembershipsRequest,
     SearchRelatedAccountGroupMembershipsResponse,
     TestingOptions,
     TokenProperties,
@@ -82,14 +84,16 @@
     "ListRelatedAccountGroupsRequest",
     "ListRelatedAccountGroupsResponse",
     "Metrics",
     "MigrateKeyRequest",
     "PrivatePasswordLeakVerification",
     "RelatedAccountGroup",
     "RelatedAccountGroupMembership",
+    "RetrieveLegacySecretKeyRequest",
+    "RetrieveLegacySecretKeyResponse",
     "RiskAnalysis",
     "ScoreDistribution",
     "ScoreMetrics",
     "SearchRelatedAccountGroupMembershipsRequest",
     "SearchRelatedAccountGroupMembershipsResponse",
     "TestingOptions",
     "TokenProperties",
```

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/__init__.py` & `google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,14 +40,16 @@
     ListRelatedAccountGroupsRequest,
     ListRelatedAccountGroupsResponse,
     Metrics,
     MigrateKeyRequest,
     PrivatePasswordLeakVerification,
     RelatedAccountGroup,
     RelatedAccountGroupMembership,
+    RetrieveLegacySecretKeyRequest,
+    RetrieveLegacySecretKeyResponse,
     RiskAnalysis,
     ScoreDistribution,
     ScoreMetrics,
     SearchRelatedAccountGroupMembershipsRequest,
     SearchRelatedAccountGroupMembershipsResponse,
     TestingOptions,
     TokenProperties,
@@ -80,14 +82,16 @@
     "ListRelatedAccountGroupsResponse",
     "Metrics",
     "MigrateKeyRequest",
     "PrivatePasswordLeakVerification",
     "RecaptchaEnterpriseServiceClient",
     "RelatedAccountGroup",
     "RelatedAccountGroupMembership",
+    "RetrieveLegacySecretKeyRequest",
+    "RetrieveLegacySecretKeyResponse",
     "RiskAnalysis",
     "ScoreDistribution",
     "ScoreMetrics",
     "SearchRelatedAccountGroupMembershipsRequest",
     "SearchRelatedAccountGroupMembershipsResponse",
     "TestingOptions",
     "TokenProperties",
```

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/gapic_metadata.json` & `google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/gapic_metadata.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997996794871794%*

 * *Differences: {"'services'": "{'RecaptchaEnterpriseService': {'clients': {'grpc': {'rpcs': "*

 * *               "{'RetrieveLegacySecretKey': OrderedDict([('methods', "*

 * *               "['retrieve_legacy_secret_key'])])}}, 'grpc-async': {'rpcs': "*

 * *               "{'RetrieveLegacySecretKey': OrderedDict([('methods', "*

 * *               "['retrieve_legacy_secret_key'])])}}}}}"}*

```diff
@@ -56,14 +56,19 @@
                             ]
                         },
                         "MigrateKey": {
                             "methods": [
                                 "migrate_key"
                             ]
                         },
+                        "RetrieveLegacySecretKey": {
+                            "methods": [
+                                "retrieve_legacy_secret_key"
+                            ]
+                        },
                         "SearchRelatedAccountGroupMemberships": {
                             "methods": [
                                 "search_related_account_group_memberships"
                             ]
                         },
                         "UpdateKey": {
                             "methods": [
@@ -121,14 +126,19 @@
                             ]
                         },
                         "MigrateKey": {
                             "methods": [
                                 "migrate_key"
                             ]
                         },
+                        "RetrieveLegacySecretKey": {
+                            "methods": [
+                                "retrieve_legacy_secret_key"
+                            ]
+                        },
                         "SearchRelatedAccountGroupMemberships": {
                             "methods": [
                                 "search_related_account_group_memberships"
                             ]
                         },
                         "UpdateKey": {
                             "methods": [
```

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/services/__init__.py` & `google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/__init__.py` & `google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/async_client.py` & `google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -635,14 +635,120 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
+    async def retrieve_legacy_secret_key(
+        self,
+        request: Union[recaptchaenterprise.RetrieveLegacySecretKeyRequest, dict] = None,
+        *,
+        key: str = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: float = None,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> recaptchaenterprise.RetrieveLegacySecretKeyResponse:
+        r"""Returns the secret key related to the specified
+        public key. You must use the legacy secret key only in a
+        3rd party integration with legacy reCAPTCHA.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import recaptchaenterprise_v1
+
+            async def sample_retrieve_legacy_secret_key():
+                # Create a client
+                client = recaptchaenterprise_v1.RecaptchaEnterpriseServiceAsyncClient()
+
+                # Initialize request argument(s)
+                request = recaptchaenterprise_v1.RetrieveLegacySecretKeyRequest(
+                    key="key_value",
+                )
+
+                # Make the request
+                response = await client.retrieve_legacy_secret_key(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.recaptchaenterprise_v1.types.RetrieveLegacySecretKeyRequest, dict]):
+                The request object. The retrieve legacy secret key
+                request message.
+            key (:class:`str`):
+                Required. The public key name linked
+                to the requested secret key in the
+                format "projects/{project}/keys/{key}".
+
+                This corresponds to the ``key`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.recaptchaenterprise_v1.types.RetrieveLegacySecretKeyResponse:
+                Secret key is used only in legacy
+                reCAPTCHA. It must be used in a 3rd
+                party integration with legacy reCAPTCHA.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([key])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        request = recaptchaenterprise.RetrieveLegacySecretKeyRequest(request)
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if key is not None:
+            request.key = key
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.retrieve_legacy_secret_key,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("key", request.key),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
     async def get_key(
         self,
         request: Union[recaptchaenterprise.GetKeyRequest, dict] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
@@ -1180,15 +1286,15 @@
         ] = None,
         *,
         parent: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListRelatedAccountGroupMembershipsAsyncPager:
-        r"""Get the memberships in a group of related accounts.
+        r"""Get memberships in a group of related accounts.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -1335,25 +1441,26 @@
         Args:
             request (Union[google.cloud.recaptchaenterprise_v1.types.SearchRelatedAccountGroupMembershipsRequest, dict]):
                 The request object. The request message to search
                 related account group memberships.
             project (:class:`str`):
                 Required. The name of the project to
                 search related account group memberships
-                from, in the format
-                "projects/{project}".
+                from. Specify the project name in the
+                following format: "projects/{project}".
 
                 This corresponds to the ``project`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             hashed_account_id (:class:`bytes`):
                 Optional. The unique stable hashed user identifier we
                 should search connections to. The identifier should
                 correspond to a ``hashed_account_id`` provided in a
-                previous CreateAssessment or AnnotateAssessment call.
+                previous ``CreateAssessment`` or ``AnnotateAssessment``
+                call.
 
                 This corresponds to the ``hashed_account_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
```

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/client.py` & `google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -908,14 +908,122 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
+    def retrieve_legacy_secret_key(
+        self,
+        request: Union[recaptchaenterprise.RetrieveLegacySecretKeyRequest, dict] = None,
+        *,
+        key: str = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: float = None,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> recaptchaenterprise.RetrieveLegacySecretKeyResponse:
+        r"""Returns the secret key related to the specified
+        public key. You must use the legacy secret key only in a
+        3rd party integration with legacy reCAPTCHA.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import recaptchaenterprise_v1
+
+            def sample_retrieve_legacy_secret_key():
+                # Create a client
+                client = recaptchaenterprise_v1.RecaptchaEnterpriseServiceClient()
+
+                # Initialize request argument(s)
+                request = recaptchaenterprise_v1.RetrieveLegacySecretKeyRequest(
+                    key="key_value",
+                )
+
+                # Make the request
+                response = client.retrieve_legacy_secret_key(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.recaptchaenterprise_v1.types.RetrieveLegacySecretKeyRequest, dict]):
+                The request object. The retrieve legacy secret key
+                request message.
+            key (str):
+                Required. The public key name linked
+                to the requested secret key in the
+                format "projects/{project}/keys/{key}".
+
+                This corresponds to the ``key`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.recaptchaenterprise_v1.types.RetrieveLegacySecretKeyResponse:
+                Secret key is used only in legacy
+                reCAPTCHA. It must be used in a 3rd
+                party integration with legacy reCAPTCHA.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([key])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # Minor optimization to avoid making a copy if the user passes
+        # in a recaptchaenterprise.RetrieveLegacySecretKeyRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, recaptchaenterprise.RetrieveLegacySecretKeyRequest):
+            request = recaptchaenterprise.RetrieveLegacySecretKeyRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if key is not None:
+                request.key = key
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[
+            self._transport.retrieve_legacy_secret_key
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("key", request.key),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
     def get_key(
         self,
         request: Union[recaptchaenterprise.GetKeyRequest, dict] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
@@ -1459,15 +1567,15 @@
         ] = None,
         *,
         parent: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListRelatedAccountGroupMembershipsPager:
-        r"""Get the memberships in a group of related accounts.
+        r"""Get memberships in a group of related accounts.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -1620,25 +1728,26 @@
         Args:
             request (Union[google.cloud.recaptchaenterprise_v1.types.SearchRelatedAccountGroupMembershipsRequest, dict]):
                 The request object. The request message to search
                 related account group memberships.
             project (str):
                 Required. The name of the project to
                 search related account group memberships
-                from, in the format
-                "projects/{project}".
+                from. Specify the project name in the
+                following format: "projects/{project}".
 
                 This corresponds to the ``project`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             hashed_account_id (bytes):
                 Optional. The unique stable hashed user identifier we
                 should search connections to. The identifier should
                 correspond to a ``hashed_account_id`` provided in a
-                previous CreateAssessment or AnnotateAssessment call.
+                previous ``CreateAssessment`` or ``AnnotateAssessment``
+                call.
 
                 This corresponds to the ``hashed_account_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
```

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/pagers.py` & `google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/transports/__init__.py` & `google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/transports/base.py` & `google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/transports/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,19 @@
                 client_info=client_info,
             ),
             self.list_keys: gapic_v1.method.wrap_method(
                 self.list_keys,
                 default_timeout=600.0,
                 client_info=client_info,
             ),
+            self.retrieve_legacy_secret_key: gapic_v1.method.wrap_method(
+                self.retrieve_legacy_secret_key,
+                default_timeout=None,
+                client_info=client_info,
+            ),
             self.get_key: gapic_v1.method.wrap_method(
                 self.get_key,
                 default_timeout=600.0,
                 client_info=client_info,
             ),
             self.update_key: gapic_v1.method.wrap_method(
                 self.update_key,
@@ -240,14 +245,26 @@
             recaptchaenterprise.ListKeysResponse,
             Awaitable[recaptchaenterprise.ListKeysResponse],
         ],
     ]:
         raise NotImplementedError()
 
     @property
+    def retrieve_legacy_secret_key(
+        self,
+    ) -> Callable[
+        [recaptchaenterprise.RetrieveLegacySecretKeyRequest],
+        Union[
+            recaptchaenterprise.RetrieveLegacySecretKeyResponse,
+            Awaitable[recaptchaenterprise.RetrieveLegacySecretKeyResponse],
+        ],
+    ]:
+        raise NotImplementedError()
+
+    @property
     def get_key(
         self,
     ) -> Callable[
         [recaptchaenterprise.GetKeyRequest],
         Union[recaptchaenterprise.Key, Awaitable[recaptchaenterprise.Key]],
     ]:
         raise NotImplementedError()
```

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/transports/grpc.py` & `google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/transports/grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -341,14 +341,45 @@
                 "/google.cloud.recaptchaenterprise.v1.RecaptchaEnterpriseService/ListKeys",
                 request_serializer=recaptchaenterprise.ListKeysRequest.serialize,
                 response_deserializer=recaptchaenterprise.ListKeysResponse.deserialize,
             )
         return self._stubs["list_keys"]
 
     @property
+    def retrieve_legacy_secret_key(
+        self,
+    ) -> Callable[
+        [recaptchaenterprise.RetrieveLegacySecretKeyRequest],
+        recaptchaenterprise.RetrieveLegacySecretKeyResponse,
+    ]:
+        r"""Return a callable for the retrieve legacy secret key method over gRPC.
+
+        Returns the secret key related to the specified
+        public key. You must use the legacy secret key only in a
+        3rd party integration with legacy reCAPTCHA.
+
+        Returns:
+            Callable[[~.RetrieveLegacySecretKeyRequest],
+                    ~.RetrieveLegacySecretKeyResponse]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "retrieve_legacy_secret_key" not in self._stubs:
+            self._stubs["retrieve_legacy_secret_key"] = self.grpc_channel.unary_unary(
+                "/google.cloud.recaptchaenterprise.v1.RecaptchaEnterpriseService/RetrieveLegacySecretKey",
+                request_serializer=recaptchaenterprise.RetrieveLegacySecretKeyRequest.serialize,
+                response_deserializer=recaptchaenterprise.RetrieveLegacySecretKeyResponse.deserialize,
+            )
+        return self._stubs["retrieve_legacy_secret_key"]
+
+    @property
     def get_key(
         self,
     ) -> Callable[[recaptchaenterprise.GetKeyRequest], recaptchaenterprise.Key]:
         r"""Return a callable for the get key method over gRPC.
 
         Returns the specified key.
 
@@ -516,15 +547,15 @@
     ) -> Callable[
         [recaptchaenterprise.ListRelatedAccountGroupMembershipsRequest],
         recaptchaenterprise.ListRelatedAccountGroupMembershipsResponse,
     ]:
         r"""Return a callable for the list related account group
         memberships method over gRPC.
 
-        Get the memberships in a group of related accounts.
+        Get memberships in a group of related accounts.
 
         Returns:
             Callable[[~.ListRelatedAccountGroupMembershipsRequest],
                     ~.ListRelatedAccountGroupMembershipsResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
```

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/transports/grpc_asyncio.py` & `google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/services/recaptcha_enterprise_service/transports/grpc_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,14 +350,45 @@
                 "/google.cloud.recaptchaenterprise.v1.RecaptchaEnterpriseService/ListKeys",
                 request_serializer=recaptchaenterprise.ListKeysRequest.serialize,
                 response_deserializer=recaptchaenterprise.ListKeysResponse.deserialize,
             )
         return self._stubs["list_keys"]
 
     @property
+    def retrieve_legacy_secret_key(
+        self,
+    ) -> Callable[
+        [recaptchaenterprise.RetrieveLegacySecretKeyRequest],
+        Awaitable[recaptchaenterprise.RetrieveLegacySecretKeyResponse],
+    ]:
+        r"""Return a callable for the retrieve legacy secret key method over gRPC.
+
+        Returns the secret key related to the specified
+        public key. You must use the legacy secret key only in a
+        3rd party integration with legacy reCAPTCHA.
+
+        Returns:
+            Callable[[~.RetrieveLegacySecretKeyRequest],
+                    Awaitable[~.RetrieveLegacySecretKeyResponse]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "retrieve_legacy_secret_key" not in self._stubs:
+            self._stubs["retrieve_legacy_secret_key"] = self.grpc_channel.unary_unary(
+                "/google.cloud.recaptchaenterprise.v1.RecaptchaEnterpriseService/RetrieveLegacySecretKey",
+                request_serializer=recaptchaenterprise.RetrieveLegacySecretKeyRequest.serialize,
+                response_deserializer=recaptchaenterprise.RetrieveLegacySecretKeyResponse.deserialize,
+            )
+        return self._stubs["retrieve_legacy_secret_key"]
+
+    @property
     def get_key(
         self,
     ) -> Callable[
         [recaptchaenterprise.GetKeyRequest], Awaitable[recaptchaenterprise.Key]
     ]:
         r"""Return a callable for the get key method over gRPC.
 
@@ -533,15 +564,15 @@
     ) -> Callable[
         [recaptchaenterprise.ListRelatedAccountGroupMembershipsRequest],
         Awaitable[recaptchaenterprise.ListRelatedAccountGroupMembershipsResponse],
     ]:
         r"""Return a callable for the list related account group
         memberships method over gRPC.
 
-        Get the memberships in a group of related accounts.
+        Get memberships in a group of related accounts.
 
         Returns:
             Callable[[~.ListRelatedAccountGroupMembershipsRequest],
                     Awaitable[~.ListRelatedAccountGroupMembershipsResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
```

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/types/__init__.py` & `google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/types/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,14 +35,16 @@
     ListRelatedAccountGroupsRequest,
     ListRelatedAccountGroupsResponse,
     Metrics,
     MigrateKeyRequest,
     PrivatePasswordLeakVerification,
     RelatedAccountGroup,
     RelatedAccountGroupMembership,
+    RetrieveLegacySecretKeyRequest,
+    RetrieveLegacySecretKeyResponse,
     RiskAnalysis,
     ScoreDistribution,
     ScoreMetrics,
     SearchRelatedAccountGroupMembershipsRequest,
     SearchRelatedAccountGroupMembershipsResponse,
     TestingOptions,
     TokenProperties,
@@ -73,14 +75,16 @@
     "ListRelatedAccountGroupsRequest",
     "ListRelatedAccountGroupsResponse",
     "Metrics",
     "MigrateKeyRequest",
     "PrivatePasswordLeakVerification",
     "RelatedAccountGroup",
     "RelatedAccountGroupMembership",
+    "RetrieveLegacySecretKeyRequest",
+    "RetrieveLegacySecretKeyResponse",
     "RiskAnalysis",
     "ScoreDistribution",
     "ScoreMetrics",
     "SearchRelatedAccountGroupMembershipsRequest",
     "SearchRelatedAccountGroupMembershipsResponse",
     "TestingOptions",
     "TokenProperties",
```

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/google/cloud/recaptchaenterprise_v1/types/recaptchaenterprise.py` & `google-cloud-recaptcha-enterprise-1.9.0/google/cloud/recaptchaenterprise_v1/types/recaptchaenterprise.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,29 +19,31 @@
 
 __protobuf__ = proto.module(
     package="google.cloud.recaptchaenterprise.v1",
     manifest={
         "CreateAssessmentRequest",
         "AnnotateAssessmentRequest",
         "AnnotateAssessmentResponse",
+        "PrivatePasswordLeakVerification",
         "Assessment",
         "Event",
         "RiskAnalysis",
         "TokenProperties",
         "AccountDefenderAssessment",
-        "PrivatePasswordLeakVerification",
         "CreateKeyRequest",
         "ListKeysRequest",
         "ListKeysResponse",
+        "RetrieveLegacySecretKeyRequest",
         "GetKeyRequest",
         "UpdateKeyRequest",
         "DeleteKeyRequest",
         "MigrateKeyRequest",
         "GetMetricsRequest",
         "Metrics",
+        "RetrieveLegacySecretKeyResponse",
         "Key",
         "TestingOptions",
         "WebKeySettings",
         "AndroidKeySettings",
         "IOSKeySettings",
         "ScoreDistribution",
         "ScoreMetrics",
@@ -96,20 +98,20 @@
             empty to provide reasons that apply to an event
             without concluding whether the event is
             legitimate or fraudulent.
         reasons (Sequence[google.cloud.recaptchaenterprise_v1.types.AnnotateAssessmentRequest.Reason]):
             Optional. Optional reasons for the annotation
             that will be assigned to the Event.
         hashed_account_id (bytes):
-            Optional. Optional unique stable hashed user identifier to
-            apply to the assessment. This is an alternative to setting
-            the hashed_account_id in CreateAssessment, for example when
-            the account identifier is not yet known in the initial
-            request. It is recommended that the identifier is hashed
-            using hmac-sha256 with stable secret.
+            Optional. Unique stable hashed user identifier to apply to
+            the assessment. This is an alternative to setting the
+            hashed_account_id in CreateAssessment, for example when the
+            account identifier is not yet known in the initial request.
+            It is recommended that the identifier is hashed using
+            hmac-sha256 with stable secret.
     """
 
     class Annotation(proto.Enum):
         r"""Enum that represents the types of annotations."""
         ANNOTATION_UNSPECIFIED = 0
         LEGITIMATE = 1
         FRAUDULENT = 2
@@ -120,20 +122,25 @@
         r"""Enum that represents potential reasons for annotating an
         assessment.
         """
         REASON_UNSPECIFIED = 0
         CHARGEBACK = 1
         CHARGEBACK_FRAUD = 8
         CHARGEBACK_DISPUTE = 9
+        REFUND = 10
+        REFUND_FRAUD = 11
+        TRANSACTION_ACCEPTED = 12
+        TRANSACTION_DECLINED = 13
         PAYMENT_HEURISTICS = 2
         INITIATED_TWO_FACTOR = 7
         PASSED_TWO_FACTOR = 3
         FAILED_TWO_FACTOR = 4
         CORRECT_PASSWORD = 5
         INCORRECT_PASSWORD = 6
+        SOCIAL_SPAM = 14
 
     name = proto.Field(
         proto.STRING,
         number=1,
     )
     annotation = proto.Field(
         proto.ENUM,
@@ -151,14 +158,57 @@
     )
 
 
 class AnnotateAssessmentResponse(proto.Message):
     r"""Empty response for AnnotateAssessment."""
 
 
+class PrivatePasswordLeakVerification(proto.Message):
+    r"""Private password leak verification info.
+
+    Attributes:
+        lookup_hash_prefix (bytes):
+            Optional. Exactly 26-bit prefix of the
+            SHA-256 hash of the canonicalized username. It
+            is used to look up password leaks associated
+            with that hash prefix.
+        encrypted_user_credentials_hash (bytes):
+            Optional. Encrypted Scrypt hash of the canonicalized
+            username+password. It is re-encrypted by the server and
+            returned through ``reencrypted_user_credentials_hash``.
+        encrypted_leak_match_prefixes (Sequence[bytes]):
+            Output only. List of prefixes of the encrypted potential
+            password leaks that matched the given parameters. They must
+            be compared with the client-side decryption prefix of
+            ``reencrypted_user_credentials_hash``
+        reencrypted_user_credentials_hash (bytes):
+            Output only. Corresponds to the re-encryption of the
+            ``encrypted_user_credentials_hash`` field. It is used to
+            match potential password leaks within
+            ``encrypted_leak_match_prefixes``.
+    """
+
+    lookup_hash_prefix = proto.Field(
+        proto.BYTES,
+        number=1,
+    )
+    encrypted_user_credentials_hash = proto.Field(
+        proto.BYTES,
+        number=2,
+    )
+    encrypted_leak_match_prefixes = proto.RepeatedField(
+        proto.BYTES,
+        number=3,
+    )
+    reencrypted_user_credentials_hash = proto.Field(
+        proto.BYTES,
+        number=4,
+    )
+
+
 class Assessment(proto.Message):
     r"""A recaptcha assessment resource.
 
     Attributes:
         name (str):
             Output only. The resource name for the
             Assessment in the format
@@ -168,18 +218,21 @@
         risk_analysis (google.cloud.recaptchaenterprise_v1.types.RiskAnalysis):
             Output only. The risk analysis result for the
             event being assessed.
         token_properties (google.cloud.recaptchaenterprise_v1.types.TokenProperties):
             Output only. Properties of the provided event
             token.
         account_defender_assessment (google.cloud.recaptchaenterprise_v1.types.AccountDefenderAssessment):
-            Assessment returned by Account Defender when a
+            Assessment returned by account defender when a
             hashed_account_id is provided.
         private_password_leak_verification (google.cloud.recaptchaenterprise_v1.types.PrivatePasswordLeakVerification):
-            Password leak verification info.
+            The private password leak verification field
+            contains the parameters that are used to to
+            check for leaks privately without sharing user
+            credentials.
     """
 
     name = proto.Field(
         proto.STRING,
         number=1,
     )
     event = proto.Field(
@@ -231,18 +284,17 @@
         expected_action (str):
             Optional. The expected action for this type
             of event. This should be the same action
             provided at token generation time on client-side
             platforms already integrated with recaptcha
             enterprise.
         hashed_account_id (bytes):
-            Optional. Optional unique stable hashed user
-            identifier for the request. The identifier
-            should ideally be hashed using sha256 with
-            stable secret.
+            Optional. Unique stable hashed user
+            identifier for the request. The identifier must
+            be hashed using hmac-sha256 with stable secret.
     """
 
     token = proto.Field(
         proto.STRING,
         number=1,
     )
     site_key = proto.Field(
@@ -315,15 +367,15 @@
             Reason associated with the response when
             valid = false.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             The timestamp corresponding to the generation
             of the token.
         hostname (str):
             The hostname of the page on which the token
-            was generated.
+            was generated (Web keys only).
         action (str):
             Action name provided at token generation.
     """
 
     class InvalidReason(proto.Enum):
         r"""Enum that represents the types of invalid token reasons."""
         INVALID_REASON_UNSPECIFIED = 0
@@ -355,79 +407,36 @@
     action = proto.Field(
         proto.STRING,
         number=5,
     )
 
 
 class AccountDefenderAssessment(proto.Message):
-    r"""Account Defender risk assessment.
+    r"""Account defender risk assessment.
 
     Attributes:
         labels (Sequence[google.cloud.recaptchaenterprise_v1.types.AccountDefenderAssessment.AccountDefenderLabel]):
             Labels for this request.
     """
 
     class AccountDefenderLabel(proto.Enum):
-        r"""Labels returned by Account Defender for this request."""
+        r"""Labels returned by account defender for this request."""
         ACCOUNT_DEFENDER_LABEL_UNSPECIFIED = 0
         PROFILE_MATCH = 1
         SUSPICIOUS_LOGIN_ACTIVITY = 2
         SUSPICIOUS_ACCOUNT_CREATION = 3
         RELATED_ACCOUNTS_NUMBER_HIGH = 4
 
     labels = proto.RepeatedField(
         proto.ENUM,
         number=1,
         enum=AccountDefenderLabel,
     )
 
 
-class PrivatePasswordLeakVerification(proto.Message):
-    r"""Private password leak verification info.
-
-    Attributes:
-        lookup_hash_prefix (bytes):
-            Exactly 26-bit prefix of the SHA-256 hash of
-            the canonicalized username. It is used to look
-            up password leaks associated with that hash
-            prefix.
-        encrypted_user_credentials_hash (bytes):
-            Encrypted Scrypt hash of the canonicalized
-            username+password. It is re-encrypted by the server and
-            returned through ``reencrypted_user_credentials_hash``.
-        encrypted_leak_match_prefixes (Sequence[bytes]):
-            List of prefixes of the encrypted potential password leaks
-            that matched the given parameters. They should be compared
-            with the client-side decryption prefix of
-            ``reencrypted_user_credentials_hash``
-        reencrypted_user_credentials_hash (bytes):
-            Corresponds to the re-encryption of the
-            ``encrypted_user_credentials_hash`` field. Used to match
-            potential password leaks within
-            ``encrypted_leak_match_prefixes``.
-    """
-
-    lookup_hash_prefix = proto.Field(
-        proto.BYTES,
-        number=1,
-    )
-    encrypted_user_credentials_hash = proto.Field(
-        proto.BYTES,
-        number=2,
-    )
-    encrypted_leak_match_prefixes = proto.RepeatedField(
-        proto.BYTES,
-        number=3,
-    )
-    reencrypted_user_credentials_hash = proto.Field(
-        proto.BYTES,
-        number=4,
-    )
-
-
 class CreateKeyRequest(proto.Message):
     r"""The create key request message.
 
     Attributes:
         parent (str):
             Required. The name of the project in which
             the key will be created, in the format
@@ -500,14 +509,30 @@
     )
     next_page_token = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
+class RetrieveLegacySecretKeyRequest(proto.Message):
+    r"""The retrieve legacy secret key request message.
+
+    Attributes:
+        key (str):
+            Required. The public key name linked to the
+            requested secret key in the format
+            "projects/{project}/keys/{key}".
+    """
+
+    key = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+
+
 class GetKeyRequest(proto.Message):
     r"""The get key request message.
 
     Attributes:
         name (str):
             Required. The name of the requested key, in
             the format "projects/{project}/keys/{key}".
@@ -626,14 +651,34 @@
     challenge_metrics = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message="ChallengeMetrics",
     )
 
 
+class RetrieveLegacySecretKeyResponse(proto.Message):
+    r"""Secret key is used only in legacy reCAPTCHA. It must be used
+    in a 3rd party integration with legacy reCAPTCHA.
+
+    Attributes:
+        legacy_secret_key (str):
+            The secret key (also known as shared secret)
+            authorizes communication between your
+            application backend and the reCAPTCHA Enterprise
+            server to create an assessment.
+            The secret key needs to be kept safe for
+            security purposes.
+    """
+
+    legacy_secret_key = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+
+
 class Key(proto.Message):
     r"""A key used to identify and configure applications (web and/or
     mobile) that use reCAPTCHA Enterprise.
 
     This message has `oneof`_ fields (mutually exclusive fields).
     For each oneof, at most one member field can be set at the same time.
     Setting any member of the oneof automatically clears all other
@@ -960,18 +1005,18 @@
     Attributes:
         parent (str):
             Required. The resource name for the related account group in
             the format
             ``projects/{project}/relatedaccountgroups/{relatedaccountgroup}``.
         page_size (int):
             Optional. The maximum number of accounts to
-            return. The service may return fewer than this
-            value. If unspecified, at most 50 accounts will
-            be returned. The maximum value is 1000; values
-            above 1000 will be coerced to 1000.
+            return. The service might return fewer than this
+            value. If unspecified, at most 50 accounts are
+            returned. The maximum value is 1000; values
+            above 1000 are coerced to 1000.
         page_token (str):
             Optional. A page token, received from a previous
             ``ListRelatedAccountGroupMemberships`` call.
 
             When paginating, all other parameters provided to
             ``ListRelatedAccountGroupMemberships`` must match the call
             that provided the page token.
@@ -1024,18 +1069,18 @@
     Attributes:
         parent (str):
             Required. The name of the project to list
             related account groups from, in the format
             "projects/{project}".
         page_size (int):
             Optional. The maximum number of groups to
-            return. The service may return fewer than this
-            value. If unspecified, at most 50 groups will be
+            return. The service might return fewer than this
+            value. If unspecified, at most 50 groups are
             returned. The maximum value is 1000; values
-            above 1000 will be coerced to 1000.
+            above 1000 are coerced to 1000.
         page_token (str):
             Optional. A page token, received from a previous
             ``ListRelatedAccountGroups`` call. Provide this to retrieve
             the subsequent page.
 
             When paginating, all other parameters provided to
             ``ListRelatedAccountGroups`` must match the call that
@@ -1087,27 +1132,28 @@
 class SearchRelatedAccountGroupMembershipsRequest(proto.Message):
     r"""The request message to search related account group
     memberships.
 
     Attributes:
         project (str):
             Required. The name of the project to search
-            related account group memberships from, in the
-            format "projects/{project}".
+            related account group memberships from. Specify
+            the project name in the following format:
+            "projects/{project}".
         hashed_account_id (bytes):
             Optional. The unique stable hashed user identifier we should
             search connections to. The identifier should correspond to a
             ``hashed_account_id`` provided in a previous
-            CreateAssessment or AnnotateAssessment call.
+            ``CreateAssessment`` or ``AnnotateAssessment`` call.
         page_size (int):
             Optional. The maximum number of groups to
-            return. The service may return fewer than this
-            value. If unspecified, at most 50 groups will be
+            return. The service might return fewer than this
+            value. If unspecified, at most 50 groups are
             returned. The maximum value is 1000; values
-            above 1000 will be coerced to 1000.
+            above 1000 are coerced to 1000.
         page_token (str):
             Optional. A page token, received from a previous
             ``SearchRelatedAccountGroupMemberships`` call. Provide this
             to retrieve the subsequent page.
 
             When paginating, all other parameters provided to
             ``SearchRelatedAccountGroupMemberships`` must match the call
@@ -1166,15 +1212,16 @@
         name (str):
             Required. The resource name for this membership in the
             format
             ``projects/{project}/relatedaccountgroups/{relatedaccountgroup}/memberships/{membership}``.
         hashed_account_id (bytes):
             The unique stable hashed user identifier of the member. The
             identifier corresponds to a ``hashed_account_id`` provided
-            in a previous CreateAssessment or AnnotateAssessment call.
+            in a previous ``CreateAssessment`` or ``AnnotateAssessment``
+            call.
     """
 
     name = proto.Field(
         proto.STRING,
         number=1,
     )
     hashed_account_id = proto.Field(
```

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/google_cloud_recaptcha_enterprise.egg-info/PKG-INFO` & `google-cloud-recaptcha-enterprise-1.9.0/google_cloud_recaptcha_enterprise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-recaptcha-enterprise
-Version: 1.8.3
+Version: 1.9.0
 Home-page: https://github.com/googleapis/python-recaptcha-enterprise
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/google_cloud_recaptcha_enterprise.egg-info/SOURCES.txt` & `google-cloud-recaptcha-enterprise-1.9.0/google_cloud_recaptcha_enterprise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/setup.py` & `google-cloud-recaptcha-enterprise-1.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #
 
 import io
 import os
 
 import setuptools  # type: ignore
 
-version = "1.8.3"
+version = "1.9.0"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/tests/__init__.py` & `google-cloud-recaptcha-enterprise-1.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/tests/unit/__init__.py` & `google-cloud-recaptcha-enterprise-1.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/tests/unit/gapic/__init__.py` & `google-cloud-recaptcha-enterprise-1.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/tests/unit/gapic/recaptchaenterprise_v1/__init__.py` & `google-cloud-recaptcha-enterprise-1.9.0/tests/unit/gapic/recaptchaenterprise_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-recaptcha-enterprise-1.8.3/tests/unit/gapic/recaptchaenterprise_v1/test_recaptcha_enterprise_service.py` & `google-cloud-recaptcha-enterprise-1.9.0/tests/unit/gapic/recaptchaenterprise_v1/test_recaptcha_enterprise_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1714,14 +1714,261 @@
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
     [
+        recaptchaenterprise.RetrieveLegacySecretKeyRequest,
+        dict,
+    ],
+)
+def test_retrieve_legacy_secret_key(request_type, transport: str = "grpc"):
+    client = RecaptchaEnterpriseServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.retrieve_legacy_secret_key), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = recaptchaenterprise.RetrieveLegacySecretKeyResponse(
+            legacy_secret_key="legacy_secret_key_value",
+        )
+        response = client.retrieve_legacy_secret_key(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == recaptchaenterprise.RetrieveLegacySecretKeyRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, recaptchaenterprise.RetrieveLegacySecretKeyResponse)
+    assert response.legacy_secret_key == "legacy_secret_key_value"
+
+
+def test_retrieve_legacy_secret_key_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = RecaptchaEnterpriseServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.retrieve_legacy_secret_key), "__call__"
+    ) as call:
+        client.retrieve_legacy_secret_key()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == recaptchaenterprise.RetrieveLegacySecretKeyRequest()
+
+
+@pytest.mark.asyncio
+async def test_retrieve_legacy_secret_key_async(
+    transport: str = "grpc_asyncio",
+    request_type=recaptchaenterprise.RetrieveLegacySecretKeyRequest,
+):
+    client = RecaptchaEnterpriseServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.retrieve_legacy_secret_key), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            recaptchaenterprise.RetrieveLegacySecretKeyResponse(
+                legacy_secret_key="legacy_secret_key_value",
+            )
+        )
+        response = await client.retrieve_legacy_secret_key(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == recaptchaenterprise.RetrieveLegacySecretKeyRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, recaptchaenterprise.RetrieveLegacySecretKeyResponse)
+    assert response.legacy_secret_key == "legacy_secret_key_value"
+
+
+@pytest.mark.asyncio
+async def test_retrieve_legacy_secret_key_async_from_dict():
+    await test_retrieve_legacy_secret_key_async(request_type=dict)
+
+
+def test_retrieve_legacy_secret_key_field_headers():
+    client = RecaptchaEnterpriseServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = recaptchaenterprise.RetrieveLegacySecretKeyRequest()
+
+    request.key = "key_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.retrieve_legacy_secret_key), "__call__"
+    ) as call:
+        call.return_value = recaptchaenterprise.RetrieveLegacySecretKeyResponse()
+        client.retrieve_legacy_secret_key(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "key=key_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_retrieve_legacy_secret_key_field_headers_async():
+    client = RecaptchaEnterpriseServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = recaptchaenterprise.RetrieveLegacySecretKeyRequest()
+
+    request.key = "key_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.retrieve_legacy_secret_key), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            recaptchaenterprise.RetrieveLegacySecretKeyResponse()
+        )
+        await client.retrieve_legacy_secret_key(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "key=key_value",
+    ) in kw["metadata"]
+
+
+def test_retrieve_legacy_secret_key_flattened():
+    client = RecaptchaEnterpriseServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.retrieve_legacy_secret_key), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = recaptchaenterprise.RetrieveLegacySecretKeyResponse()
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        client.retrieve_legacy_secret_key(
+            key="key_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].key
+        mock_val = "key_value"
+        assert arg == mock_val
+
+
+def test_retrieve_legacy_secret_key_flattened_error():
+    client = RecaptchaEnterpriseServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.retrieve_legacy_secret_key(
+            recaptchaenterprise.RetrieveLegacySecretKeyRequest(),
+            key="key_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_retrieve_legacy_secret_key_flattened_async():
+    client = RecaptchaEnterpriseServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.retrieve_legacy_secret_key), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = recaptchaenterprise.RetrieveLegacySecretKeyResponse()
+
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            recaptchaenterprise.RetrieveLegacySecretKeyResponse()
+        )
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        response = await client.retrieve_legacy_secret_key(
+            key="key_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].key
+        mock_val = "key_value"
+        assert arg == mock_val
+
+
+@pytest.mark.asyncio
+async def test_retrieve_legacy_secret_key_flattened_error_async():
+    client = RecaptchaEnterpriseServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        await client.retrieve_legacy_secret_key(
+            recaptchaenterprise.RetrieveLegacySecretKeyRequest(),
+            key="key_value",
+        )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
         recaptchaenterprise.GetKeyRequest,
         dict,
     ],
 )
 def test_get_key(request_type, transport: str = "grpc"):
     client = RecaptchaEnterpriseServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -4074,14 +4321,15 @@
     # Every method on the transport should just blindly
     # raise NotImplementedError.
     methods = (
         "create_assessment",
         "annotate_assessment",
         "create_key",
         "list_keys",
+        "retrieve_legacy_secret_key",
         "get_key",
         "update_key",
         "delete_key",
         "migrate_key",
         "get_metrics",
         "list_related_account_groups",
         "list_related_account_group_memberships",
```

