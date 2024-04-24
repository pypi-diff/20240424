# Comparing `tmp/pilot-platform-common-0.7.2.tar.gz` & `tmp/pilot-platform-common-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilot-platform-common-0.7.2.tar", last modified: Mon Apr 22 16:06:38 2024, max compression
+gzip compressed data, was "pilot-platform-common-0.7.3.tar", last modified: Wed Apr 24 14:07:32 2024, max compression
```

## Comparing `pilot-platform-common-0.7.2.tar` & `pilot-platform-common-0.7.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:06:38.293549 pilot-platform-common-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-22 16:06:38.289549 pilot-platform-common-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:06:38.281550 pilot-platform-common-0.7.2/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:06:38.281550 pilot-platform-common-0.7.2/common/geid/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/geid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/geid/geid_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:06:38.285549 pilot-platform-common-0.7.2/common/jwt_handler/
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/jwt_handler/JWTHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/jwt_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/jwt_handler/jwt_handler_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/jwt_handler/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:06:38.285549 pilot-platform-common-0.7.2/common/logging/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/logging/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/logging/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:06:38.285549 pilot-platform-common-0.7.2/common/models/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/models/config_center_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/models/service_id_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:06:38.285549 pilot-platform-common-0.7.2/common/object_storage_adaptor/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/object_storage_adaptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/object_storage_adaptor/base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/object_storage_adaptor/boto3_admin_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17073 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/object_storage_adaptor/boto3_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/object_storage_adaptor/minio_policy_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:06:38.285549 pilot-platform-common-0.7.2/common/permissions/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/permissions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/permissions/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/permissions/permissions_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/permissions/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:06:38.285549 pilot-platform-common-0.7.2/common/project/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8525 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/project/project_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/project/project_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:06:38.289549 pilot-platform-common-0.7.2/common/services/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/services/auth_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:06:38.289549 pilot-platform-common-0.7.2/common/vault/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/vault/vault_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/common/vault/vault_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:06:38.289549 pilot-platform-common-0.7.2/pilot_platform_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-22 16:06:38.000000 pilot-platform-common-0.7.2/pilot_platform_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-22 16:06:38.000000 pilot-platform-common-0.7.2/pilot_platform_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 16:06:38.000000 pilot-platform-common-0.7.2/pilot_platform_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-22 16:06:38.000000 pilot-platform-common-0.7.2/pilot_platform_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-22 16:06:38.000000 pilot-platform-common-0.7.2/pilot_platform_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 16:06:38.293549 pilot-platform-common-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:06:38.289549 pilot-platform-common-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:06:38.289549 pilot-platform-common-0.7.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/tests/fixtures/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/tests/fixtures/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:06:38.289549 pilot-platform-common-0.7.2/tests/permissions/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/tests/permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/tests/permissions/test_auth_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    19721 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/tests/permissions/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/tests/permissions/test_permissions_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/tests/test_geid_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/tests/test_jwt_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/tests/test_project_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-22 16:05:40.000000 pilot-platform-common-0.7.2/tests/test_vault_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.766475 pilot-platform-common-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-24 14:07:32.766475 pilot-platform-common-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.758475 pilot-platform-common-0.7.3/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.758475 pilot-platform-common-0.7.3/common/geid/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/geid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/geid/geid_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.758475 pilot-platform-common-0.7.3/common/jwt_handler/
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/jwt_handler/JWTHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/jwt_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/jwt_handler/jwt_handler_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/jwt_handler/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.758475 pilot-platform-common-0.7.3/common/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/logging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.762475 pilot-platform-common-0.7.3/common/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/models/config_center_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/models/service_id_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.762475 pilot-platform-common-0.7.3/common/object_storage_adaptor/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/object_storage_adaptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/object_storage_adaptor/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/object_storage_adaptor/boto3_admin_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17073 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/object_storage_adaptor/boto3_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/object_storage_adaptor/minio_policy_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.762475 pilot-platform-common-0.7.3/common/permissions/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/permissions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/permissions/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/permissions/permissions_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/permissions/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.762475 pilot-platform-common-0.7.3/common/project/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8525 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/project/project_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/project/project_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.762475 pilot-platform-common-0.7.3/common/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/services/auth_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.762475 pilot-platform-common-0.7.3/common/vault/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/vault/vault_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/common/vault/vault_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.762475 pilot-platform-common-0.7.3/pilot_platform_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-24 14:07:32.000000 pilot-platform-common-0.7.3/pilot_platform_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-24 14:07:32.000000 pilot-platform-common-0.7.3/pilot_platform_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:07:32.000000 pilot-platform-common-0.7.3/pilot_platform_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-24 14:07:32.000000 pilot-platform-common-0.7.3/pilot_platform_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 14:07:32.000000 pilot-platform-common-0.7.3/pilot_platform_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:07:32.766475 pilot-platform-common-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.766475 pilot-platform-common-0.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.766475 pilot-platform-common-0.7.3/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/fixtures/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/fixtures/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:07:32.766475 pilot-platform-common-0.7.3/tests/permissions/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/permissions/test_auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19843 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/permissions/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/permissions/test_permissions_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/test_geid_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/test_jwt_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/test_project_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-24 14:06:31.000000 pilot-platform-common-0.7.3/tests/test_vault_client.py
```

### Comparing `pilot-platform-common-0.7.2/PKG-INFO` & `pilot-platform-common-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilot-platform-common
-Version: 0.7.2
+Version: 0.7.3
 Summary: Generates entity ID and connects with Vault (secret engine) to retrieve credentials
 Author: Indoc Systems
 Author-email: etaylor@indocresearch.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `pilot-platform-common-0.7.2/README.md` & `pilot-platform-common-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/common/__init__.py` & `pilot-platform-common-0.7.3/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/common/geid/geid_client.py` & `pilot-platform-common-0.7.3/common/geid/geid_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/common/jwt_handler/JWTHandler.py` & `pilot-platform-common-0.7.3/common/jwt_handler/JWTHandler.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/common/jwt_handler/models.py` & `pilot-platform-common-0.7.3/common/jwt_handler/models.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/common/logging/formatter.py` & `pilot-platform-common-0.7.3/common/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/common/logging/logging.py` & `pilot-platform-common-0.7.3/common/logging/logging.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/common/models/config_center_policy.py` & `pilot-platform-common-0.7.3/common/models/config_center_policy.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/common/object_storage_adaptor/base_client.py` & `pilot-platform-common-0.7.3/common/object_storage_adaptor/base_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/common/object_storage_adaptor/boto3_admin_client.py` & `pilot-platform-common-0.7.3/common/object_storage_adaptor/boto3_admin_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/common/object_storage_adaptor/boto3_client.py` & `pilot-platform-common-0.7.3/common/object_storage_adaptor/boto3_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/common/object_storage_adaptor/minio_policy_client.py` & `pilot-platform-common-0.7.3/common/object_storage_adaptor/minio_policy_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/common/permissions/exceptions.py` & `pilot-platform-common-0.7.3/common/permissions/exceptions.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/common/permissions/permissions.py` & `pilot-platform-common-0.7.3/common/permissions/permissions.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         logger.info('Unsupport container type, permission denied')
         return False
     project_code = file_entity['container_code']
     username = current_identity['username']
     zone = 'greenroom' if file_entity['zone'] == 0 else 'core'
 
     folder_path_split = get_folder_path(file_entity)
-    root_folder = folder_path_split[0]
+    root_folder = folder_path_split[0] if folder_path_split else None
 
     if root_folder == 'shared':
         if len(folder_path_split) == 1:
             # We're checking the permission of the project folder itself
             project_folder_name = file_entity['name']
         else:
             project_folder_name = folder_path_split[1]
@@ -133,15 +133,19 @@
 
 
 def get_folder_path(file_entity: dict[str, str]) -> list[str]:
     if file_entity.get('status') in ['TRASHED', 'DELETED']:
         path_for_permissions = 'restore_path'
     else:
         path_for_permissions = 'parent_path'
-    return file_entity.get(path_for_permissions, '').split('/')
+    path = file_entity.get(path_for_permissions, '')
+    if path:
+        return path.split('/')
+    else:
+        return []
 
 
 def get_name_or_path(file_entity: dict[str, str], folder_path_split: list[str]) -> str:
     if len(folder_path_split) == 1:
         # We're checking the permission of the project folder itself
         folder_name = file_entity['name']
     else:
```

### Comparing `pilot-platform-common-0.7.2/common/permissions/permissions_manager.py` & `pilot-platform-common-0.7.3/common/permissions/permissions_manager.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/common/permissions/schemas.py` & `pilot-platform-common-0.7.3/common/permissions/schemas.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/common/project/project_client.py` & `pilot-platform-common-0.7.3/common/project/project_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/common/project/project_exceptions.py` & `pilot-platform-common-0.7.3/common/project/project_exceptions.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/common/services/auth_client.py` & `pilot-platform-common-0.7.3/common/services/auth_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/common/vault/vault_client.py` & `pilot-platform-common-0.7.3/common/vault/vault_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/pilot_platform_common.egg-info/PKG-INFO` & `pilot-platform-common-0.7.3/pilot_platform_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilot-platform-common
-Version: 0.7.2
+Version: 0.7.3
 Summary: Generates entity ID and connects with Vault (secret engine) to retrieve credentials
 Author: Indoc Systems
 Author-email: etaylor@indocresearch.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `pilot-platform-common-0.7.2/pilot_platform_common.egg-info/SOURCES.txt` & `pilot-platform-common-0.7.3/pilot_platform_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/pyproject.toml` & `pilot-platform-common-0.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "common"
-version = "0.7.2"
+version = "0.7.3"
 description = ""
 authors = ["Indoc Systems"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = ">=0.19.1"
 python-json-logger = ">= 0.1.11, <= 2.02"
```

### Comparing `pilot-platform-common-0.7.2/setup.py` & `pilot-platform-common-0.7.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setuptools.setup(
     name='pilot-platform-common',
-    version='0.7.2',
+    version='0.7.3',
     author='Indoc Systems',
     author_email='etaylor@indocresearch.org',
     description='Generates entity ID and connects with Vault (secret engine) to retrieve credentials',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `pilot-platform-common-0.7.2/tests/conftest.py` & `pilot-platform-common-0.7.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/tests/fixtures/metadata.py` & `pilot-platform-common-0.7.3/tests/fixtures/metadata.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/tests/permissions/test_auth_client.py` & `pilot-platform-common-0.7.3/tests/permissions/test_auth_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/tests/permissions/test_permissions.py` & `pilot-platform-common-0.7.3/tests/permissions/test_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,14 +375,16 @@
     async def test_has_file_permission_root_level_users(self, httpx_mock):
         file_data = {
             'type': 'root_folder',
             'name': 'users',
             'zone': 'core',
             'container_code': 'test_project',
             'container_type': 'project',
+            'parent_path': None,
+            'parent': None,
         }
         current_identity = {
             'username': 'test',
             'role': 'member',
             'realm_roles': ['test_project-admin'],
         }
         result = await has_file_permission('http://auth/', 'http://metadata/v1/', file_data, 'view', current_identity)
@@ -392,14 +394,16 @@
     async def test_has_file_permission_root_level_shared(self, httpx_mock):
         file_data = {
             'type': 'root_folder',
             'name': 'shared',
             'zone': 'core',
             'container_code': 'test_project',
             'container_type': 'project',
+            'parent_path': None,
+            'parent': None,
         }
         current_identity = {
             'username': 'test',
             'role': 'member',
             'realm_roles': ['test_project-admin'],
         }
         result = await has_file_permission('http://auth/', 'http://metadata/v1/', file_data, 'view', current_identity)
```

### Comparing `pilot-platform-common-0.7.2/tests/permissions/test_permissions_manager.py` & `pilot-platform-common-0.7.3/tests/permissions/test_permissions_manager.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/tests/test_formatter.py` & `pilot-platform-common-0.7.3/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/tests/test_geid_client.py` & `pilot-platform-common-0.7.3/tests/test_geid_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/tests/test_jwt_handler.py` & `pilot-platform-common-0.7.3/tests/test_jwt_handler.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/tests/test_logging.py` & `pilot-platform-common-0.7.3/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/tests/test_project_client.py` & `pilot-platform-common-0.7.3/tests/test_project_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.2/tests/test_vault_client.py` & `pilot-platform-common-0.7.3/tests/test_vault_client.py`

 * *Files identical despite different names*

