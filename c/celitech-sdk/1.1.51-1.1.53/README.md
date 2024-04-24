# Comparing `tmp/celitech_sdk-1.1.51.tar.gz` & `tmp/celitech_sdk-1.1.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celitech_sdk-1.1.51.tar", last modified: Mon Apr 22 14:59:37 2024, max compression
+gzip compressed data, was "celitech_sdk-1.1.53.tar", last modified: Wed Apr 24 10:47:37 2024, max compression
```

## Comparing `celitech_sdk-1.1.51.tar` & `celitech_sdk-1.1.53.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:59:37.421286 celitech_sdk-1.1.51/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15044 2024-04-22 14:59:37.421286 celitech_sdk-1.1.51/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 14:59:37.421286 celitech_sdk-1.1.51/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:59:37.409286 celitech_sdk-1.1.51/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:59:37.413287 celitech_sdk-1.1.51/src/celitech/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:59:37.413287 celitech_sdk-1.1.51/src/celitech/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/hooks/hook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:59:37.413287 celitech_sdk-1.1.51/src/celitech/models/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/models/create_purchase_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/models/create_purchase_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/models/edit_purchase_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/models/edit_purchase_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/models/get_esim_device_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/models/get_esim_history_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/models/get_esim_mac_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/models/get_esim_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/models/get_purchase_consumption_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/models/list_destinations_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/models/list_packages_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/models/list_purchases_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/models/top_up_esim_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/models/top_up_esim_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:59:37.417286 celitech_sdk-1.1.51/src/celitech/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/models/utils/cast_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/models/utils/json_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:59:37.417286 celitech_sdk-1.1.51/src/celitech/net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:59:37.417286 celitech_sdk-1.1.51/src/celitech/net/environment/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/net/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/net/environment/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:59:37.417286 celitech_sdk-1.1.51/src/celitech/net/headers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/net/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/net/headers/base_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:59:37.417286 celitech_sdk-1.1.51/src/celitech/net/request_chain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/net/request_chain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:59:37.417286 celitech_sdk-1.1.51/src/celitech/net/request_chain/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/net/request_chain/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/net/request_chain/handlers/base_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/net/request_chain/handlers/hook_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/net/request_chain/handlers/http_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/net/request_chain/handlers/retry_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/net/request_chain/request_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:59:37.421286 celitech_sdk-1.1.51/src/celitech/net/transport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/net/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/net/transport/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/net/transport/request_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/net/transport/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/net/transport/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/net/transport/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:59:37.421286 celitech_sdk-1.1.51/src/celitech/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/services/destinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/services/e_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/services/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/services/purchases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:59:37.421286 celitech_sdk-1.1.51/src/celitech/services/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/services/utils/base_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/services/utils/default_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-04-22 14:59:26.000000 celitech_sdk-1.1.51/src/celitech/services/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:59:37.421286 celitech_sdk-1.1.51/src/celitech_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15044 2024-04-22 14:59:37.000000 celitech_sdk-1.1.51/src/celitech_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-22 14:59:37.000000 celitech_sdk-1.1.51/src/celitech_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 14:59:37.000000 celitech_sdk-1.1.51/src/celitech_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 14:59:37.000000 celitech_sdk-1.1.51/src/celitech_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-22 14:59:37.000000 celitech_sdk-1.1.51/src/celitech_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:37.183675 celitech_sdk-1.1.53/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15044 2024-04-24 10:47:37.183675 celitech_sdk-1.1.53/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 10:47:37.183675 celitech_sdk-1.1.53/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:37.171675 celitech_sdk-1.1.53/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:37.171675 celitech_sdk-1.1.53/src/celitech/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:37.171675 celitech_sdk-1.1.53/src/celitech/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/hooks/hook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:37.175675 celitech_sdk-1.1.53/src/celitech/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/models/create_purchase_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/models/create_purchase_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/models/edit_purchase_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/models/edit_purchase_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/models/get_esim_device_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/models/get_esim_history_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/models/get_esim_mac_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/models/get_esim_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/models/get_purchase_consumption_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/models/list_destinations_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/models/list_packages_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/models/list_purchases_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/models/top_up_esim_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/models/top_up_esim_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:37.179675 celitech_sdk-1.1.53/src/celitech/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/models/utils/cast_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/models/utils/json_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:37.179675 celitech_sdk-1.1.53/src/celitech/net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:37.179675 celitech_sdk-1.1.53/src/celitech/net/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/net/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/net/environment/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:37.179675 celitech_sdk-1.1.53/src/celitech/net/headers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/net/headers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/net/headers/base_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:37.179675 celitech_sdk-1.1.53/src/celitech/net/request_chain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/net/request_chain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:37.179675 celitech_sdk-1.1.53/src/celitech/net/request_chain/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/net/request_chain/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/net/request_chain/handlers/base_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/net/request_chain/handlers/hook_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/net/request_chain/handlers/http_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/net/request_chain/handlers/retry_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/net/request_chain/request_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:37.179675 celitech_sdk-1.1.53/src/celitech/net/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/net/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/net/transport/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/net/transport/request_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/net/transport/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/net/transport/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/net/transport/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:37.183675 celitech_sdk-1.1.53/src/celitech/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/services/destinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/services/e_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/services/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/services/purchases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:37.183675 celitech_sdk-1.1.53/src/celitech/services/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/services/utils/base_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/services/utils/default_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-04-24 10:47:23.000000 celitech_sdk-1.1.53/src/celitech/services/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:47:37.183675 celitech_sdk-1.1.53/src/celitech_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15044 2024-04-24 10:47:37.000000 celitech_sdk-1.1.53/src/celitech_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-24 10:47:37.000000 celitech_sdk-1.1.53/src/celitech_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:47:37.000000 celitech_sdk-1.1.53/src/celitech_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 10:47:37.000000 celitech_sdk-1.1.53/src/celitech_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 10:47:37.000000 celitech_sdk-1.1.53/src/celitech_sdk.egg-info/top_level.txt
```

### Comparing `celitech_sdk-1.1.51/LICENSE` & `celitech_sdk-1.1.53/LICENSE`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/PKG-INFO` & `celitech_sdk-1.1.53/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: celitech-sdk
-Version: 1.1.51
+Version: 1.1.53
 Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 
-# Celitech Python SDK 1.1.51
+# Celitech Python SDK 1.1.53
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.51
+- SDK version: 1.1.53
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
```

### Comparing `celitech_sdk-1.1.51/README.md` & `celitech_sdk-1.1.53/src/celitech_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,23 @@
-# Celitech Python SDK 1.1.51
+Metadata-Version: 2.1
+Name: celitech-sdk
+Version: 1.1.53
+Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
+License: MIT
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.31.0
+
+# Celitech Python SDK 1.1.53
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.51
+- SDK version: 1.1.53
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
```

### Comparing `celitech_sdk-1.1.51/src/celitech/hooks/hook.py` & `celitech_sdk-1.1.53/src/celitech/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/models/__init__.py` & `celitech_sdk-1.1.53/src/celitech/models/__init__.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/models/base.py` & `celitech_sdk-1.1.53/src/celitech/models/base.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/models/create_purchase_ok_response.py` & `celitech_sdk-1.1.53/src/celitech/models/create_purchase_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/models/create_purchase_request.py` & `celitech_sdk-1.1.53/src/celitech/models/create_purchase_request.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/models/edit_purchase_ok_response.py` & `celitech_sdk-1.1.53/src/celitech/models/edit_purchase_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/models/edit_purchase_request.py` & `celitech_sdk-1.1.53/src/celitech/models/edit_purchase_request.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/models/get_esim_device_ok_response.py` & `celitech_sdk-1.1.53/src/celitech/models/get_esim_device_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/models/get_esim_history_ok_response.py` & `celitech_sdk-1.1.53/src/celitech/models/get_esim_history_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/models/get_esim_mac_ok_response.py` & `celitech_sdk-1.1.53/src/celitech/models/get_esim_mac_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/models/get_esim_ok_response.py` & `celitech_sdk-1.1.53/src/celitech/models/get_esim_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/models/get_purchase_consumption_ok_response.py` & `celitech_sdk-1.1.53/src/celitech/models/get_purchase_consumption_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/models/list_destinations_ok_response.py` & `celitech_sdk-1.1.53/src/celitech/models/list_destinations_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/models/list_packages_ok_response.py` & `celitech_sdk-1.1.53/src/celitech/models/list_packages_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/models/list_purchases_ok_response.py` & `celitech_sdk-1.1.53/src/celitech/models/list_purchases_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/models/top_up_esim_ok_response.py` & `celitech_sdk-1.1.53/src/celitech/models/top_up_esim_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/models/top_up_esim_request.py` & `celitech_sdk-1.1.53/src/celitech/models/top_up_esim_request.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/models/utils/cast_models.py` & `celitech_sdk-1.1.53/src/celitech/models/utils/cast_models.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/models/utils/json_map.py` & `celitech_sdk-1.1.53/src/celitech/models/utils/json_map.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/net/request_chain/handlers/base_handler.py` & `celitech_sdk-1.1.53/src/celitech/net/request_chain/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/net/request_chain/handlers/hook_handler.py` & `celitech_sdk-1.1.53/src/celitech/net/request_chain/handlers/hook_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/net/request_chain/handlers/http_handler.py` & `celitech_sdk-1.1.53/src/celitech/net/request_chain/handlers/http_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/net/request_chain/handlers/retry_handler.py` & `celitech_sdk-1.1.53/src/celitech/net/request_chain/handlers/retry_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/net/request_chain/request_chain.py` & `celitech_sdk-1.1.53/src/celitech/net/request_chain/request_chain.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/net/transport/request.py` & `celitech_sdk-1.1.53/src/celitech/net/transport/request.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/net/transport/request_error.py` & `celitech_sdk-1.1.53/src/celitech/net/transport/request_error.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/net/transport/response.py` & `celitech_sdk-1.1.53/src/celitech/net/transport/response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/net/transport/serializer.py` & `celitech_sdk-1.1.53/src/celitech/net/transport/serializer.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/net/transport/utils.py` & `celitech_sdk-1.1.53/src/celitech/net/transport/utils.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/sdk.py` & `celitech_sdk-1.1.53/src/celitech/sdk.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/services/destinations.py` & `celitech_sdk-1.1.53/src/celitech/services/destinations.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/services/e_sim.py` & `celitech_sdk-1.1.53/src/celitech/services/e_sim.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/services/packages.py` & `celitech_sdk-1.1.53/src/celitech/services/packages.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/services/purchases.py` & `celitech_sdk-1.1.53/src/celitech/services/purchases.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/services/utils/base_service.py` & `celitech_sdk-1.1.53/src/celitech/services/utils/base_service.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/services/utils/default_headers.py` & `celitech_sdk-1.1.53/src/celitech/services/utils/default_headers.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech/services/utils/validator.py` & `celitech_sdk-1.1.53/src/celitech/services/utils/validator.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.51/src/celitech_sdk.egg-info/PKG-INFO` & `celitech_sdk-1.1.53/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,13 @@
-Metadata-Version: 2.1
-Name: celitech-sdk
-Version: 1.1.51
-Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.31.0
-
-# Celitech Python SDK 1.1.51
+# Celitech Python SDK 1.1.53
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.51
+- SDK version: 1.1.53
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
```

### Comparing `celitech_sdk-1.1.51/src/celitech_sdk.egg-info/SOURCES.txt` & `celitech_sdk-1.1.53/src/celitech_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

