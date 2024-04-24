# Comparing `tmp/passage-identity-2.4.0.tar.gz` & `tmp/passage_identity-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passage-identity-2.4.0.tar", last modified: Mon Mar 25 14:40:38 2024, max compression
+gzip compressed data, was "passage_identity-2.5.0.tar", last modified: Wed Apr 24 18:14:01 2024, max compression
```

## Comparing `passage-identity-2.4.0.tar` & `passage_identity-2.5.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:40:38.778919 passage-identity-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-25 14:40:33.000000 passage-identity-2.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-03-25 14:40:38.778919 passage-identity-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-03-25 14:40:33.000000 passage-identity-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:40:38.778919 passage-identity-2.4.0/passage_identity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-03-25 14:40:38.000000 passage-identity-2.4.0/passage_identity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-03-25 14:40:38.000000 passage-identity-2.4.0/passage_identity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 14:40:38.000000 passage-identity-2.4.0/passage_identity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-25 14:40:38.000000 passage-identity-2.4.0/passage_identity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-25 14:40:38.000000 passage-identity-2.4.0/passage_identity.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:40:38.770919 passage-identity-2.4.0/passageidentity/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:40:38.770919 passage-identity-2.4.0/passageidentity/models/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/models/update_magic_link_auth_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/models/update_otp_auth_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/models/update_passkey_auth_method.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:40:38.770919 passage-identity-2.4.0/passageidentity/openapi_client/
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:40:38.770919 passage-identity-2.4.0/passageidentity/openapi_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11213 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/api/apps_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13306 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/api/magic_links_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11557 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/api/tokens_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22930 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/api/user_devices_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    94403 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25020 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14235 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:40:38.778919 passage-identity-2.4.0/passageidentity/openapi_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9871 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/app_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/app_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/apple_user_social_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/auth_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/create_magic_link_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/create_user_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     8852 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/element_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/font_family.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/github_user_social_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/google_user_social_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/layout_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/layouts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/link.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/list_devices_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/list_paginated_users_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/list_paginated_users_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/magic_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/magic_link_auth_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/magic_link_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/magic_link_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/magic_link_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/model400_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/model401_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/model403_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/model404_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/model500_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/nonce.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/otp_auth_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/paginated_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/passkeys_auth_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/technologies.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/ttl_display_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/update_user_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/user_event_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/user_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/user_metadata_field.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/user_metadata_field_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/user_recent_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/user_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/user_social_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/user_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/web_authn_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/web_authn_icons.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/models/web_authn_type.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/openapi_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)    12466 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/passage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-25 14:40:33.000000 passage-identity-2.4.0/passageidentity/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-25 14:40:33.000000 passage-identity-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 14:40:38.778919 passage-identity-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-03-25 14:40:33.000000 passage-identity-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:14:01.177063 passage_identity-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-24 18:13:50.000000 passage_identity-2.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-04-24 18:14:01.177063 passage_identity-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-24 18:13:50.000000 passage_identity-2.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:14:01.177063 passage_identity-2.5.0/passage_identity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-04-24 18:14:01.000000 passage_identity-2.5.0/passage_identity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-24 18:14:01.000000 passage_identity-2.5.0/passage_identity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:14:01.000000 passage_identity-2.5.0/passage_identity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-24 18:14:01.000000 passage_identity-2.5.0/passage_identity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 18:14:01.000000 passage_identity-2.5.0/passage_identity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:14:01.165063 passage_identity-2.5.0/passageidentity/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:14:01.165063 passage_identity-2.5.0/passageidentity/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/models/update_magic_link_auth_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/models/update_otp_auth_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/models/update_passkey_auth_method.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:14:01.169063 passage_identity-2.5.0/passageidentity/openapi_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:14:01.169063 passage_identity-2.5.0/passageidentity/openapi_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11213 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/api/apps_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13306 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/api/magic_links_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11557 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/api/tokens_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22930 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/api/user_devices_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94403 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25020 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14235 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:14:01.177063 passage_identity-2.5.0/passageidentity/openapi_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9871 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/app_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/app_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/apple_user_social_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/auth_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/create_magic_link_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/create_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8852 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/element_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/font_family.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/github_user_social_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/google_user_social_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/layout_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/list_devices_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/list_paginated_users_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/list_paginated_users_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/magic_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/magic_link_auth_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/magic_link_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/magic_link_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/magic_link_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/model400_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/model401_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/model403_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/model404_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/model500_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/nonce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/otp_auth_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/paginated_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/passkeys_auth_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/technologies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/ttl_display_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/update_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/user_event_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/user_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/user_metadata_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/user_metadata_field_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/user_recent_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/user_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/user_social_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/user_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/web_authn_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/web_authn_icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/models/web_authn_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/openapi_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13072 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/passage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-24 18:13:50.000000 passage_identity-2.5.0/passageidentity/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-24 18:13:50.000000 passage_identity-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 18:14:01.177063 passage_identity-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-24 18:13:50.000000 passage_identity-2.5.0/setup.py
```

### Comparing `passage-identity-2.4.0/LICENSE.txt` & `passage_identity-2.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/PKG-INFO` & `passage_identity-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passage-identity
-Version: 2.4.0
+Version: 2.5.0
 Summary: Python library to help manage your Passage application and users
 Home-page: https://github.com/passageidentity/passage-python
 Author: Passage Identity, Inc
 Author-email: support@passage.id
 Project-URL: Bug Tracker, https://github.com/passageidentity/passage-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `passage-identity-2.4.0/README.md` & `passage_identity-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passage_identity.egg-info/PKG-INFO` & `passage_identity-2.5.0/passage_identity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passage-identity
-Version: 2.4.0
+Version: 2.5.0
 Summary: Python library to help manage your Passage application and users
 Home-page: https://github.com/passageidentity/passage-python
 Author: Passage Identity, Inc
 Author-email: support@passage.id
 Project-URL: Bug Tracker, https://github.com/passageidentity/passage-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `passage-identity-2.4.0/passage_identity.egg-info/SOURCES.txt` & `passage_identity-2.5.0/passage_identity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/helper.py` & `passage_identity-2.5.0/passageidentity/helper.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/models/__init__.py` & `passage_identity-2.5.0/passageidentity/models/__init__.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/models/update_magic_link_auth_method.py` & `passage_identity-2.5.0/passageidentity/models/update_magic_link_auth_method.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/models/update_otp_auth_method.py` & `passage_identity-2.5.0/passageidentity/models/update_otp_auth_method.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/models/update_passkey_auth_method.py` & `passage_identity-2.5.0/passageidentity/models/update_passkey_auth_method.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/__init__.py` & `passage_identity-2.5.0/passageidentity/openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/api/apps_api.py` & `passage_identity-2.5.0/passageidentity/openapi_client/api/apps_api.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/api/magic_links_api.py` & `passage_identity-2.5.0/passageidentity/openapi_client/api/magic_links_api.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/api/tokens_api.py` & `passage_identity-2.5.0/passageidentity/openapi_client/api/tokens_api.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/api/user_devices_api.py` & `passage_identity-2.5.0/passageidentity/openapi_client/api/user_devices_api.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/api/users_api.py` & `passage_identity-2.5.0/passageidentity/openapi_client/api/users_api.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/api_client.py` & `passage_identity-2.5.0/passageidentity/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/api_response.py` & `passage_identity-2.5.0/passageidentity/openapi_client/api_response.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/configuration.py` & `passage_identity-2.5.0/passageidentity/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/exceptions.py` & `passage_identity-2.5.0/passageidentity/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/__init__.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/app_info.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/app_info.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/app_response.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/app_response.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/apple_user_social_connection.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/apple_user_social_connection.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/auth_methods.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/auth_methods.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/create_magic_link_request.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/create_magic_link_request.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/create_user_request.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/create_user_request.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/element_customization.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/element_customization.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/font_family.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/font_family.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/github_user_social_connection.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/github_user_social_connection.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/google_user_social_connection.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/google_user_social_connection.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/layout_config.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/layout_config.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/layouts.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/layouts.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/link.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/link.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/list_devices_response.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/list_devices_response.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/list_paginated_users_item.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/list_paginated_users_item.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/list_paginated_users_response.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/list_paginated_users_response.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/magic_link.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/magic_link.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/magic_link_auth_method.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/magic_link_auth_method.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/magic_link_channel.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/magic_link_channel.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/magic_link_response.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/magic_link_response.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/magic_link_type.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/magic_link_type.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/model400_error.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/model400_error.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/model401_error.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/model401_error.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/model403_error.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/model403_error.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/model404_error.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/model404_error.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/model500_error.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/model500_error.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/nonce.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/nonce.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/otp_auth_method.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/otp_auth_method.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/paginated_links.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/paginated_links.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/passkeys_auth_method.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/passkeys_auth_method.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/technologies.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/technologies.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/ttl_display_unit.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/ttl_display_unit.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/update_user_request.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/update_user_request.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/user_event_status.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/user_event_status.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/user_info.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/user_info.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/user_metadata_field.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/user_metadata_field.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/user_metadata_field_type.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/user_metadata_field_type.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/user_recent_event.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/user_recent_event.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/user_response.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/user_response.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/user_social_connections.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/user_social_connections.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/user_status.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/user_status.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/web_authn_devices.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/web_authn_devices.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/web_authn_icons.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/web_authn_icons.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/models/web_authn_type.py` & `passage_identity-2.5.0/passageidentity/openapi_client/models/web_authn_type.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/openapi_client/rest.py` & `passage_identity-2.5.0/passageidentity/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/passageidentity/passage.py` & `passage_identity-2.5.0/passageidentity/passage.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,24 +60,39 @@
         jwkItems = {}
         for jwk in jwks:
             jwkItems[jwk["kid"]] = jwk
 
         return jwkItems
 
     """
+    Fetch whether the app is hosted
+    """
+    def __fetchHosted(self):
+        r = requests.get(f"https://api.passage.id/v1/apps/{self.app_id}", api_key=self.passage_apikey)
+
+        if r.status_code != 200:
+            raise PassageError("Could not fetch app info for app id " + self.app_id, r.status_code, r.reason, r.json())
+
+        hosted = r.json()["app"]["hosted"]
+
+        return hosted
+
+    """
     This function will verify the JWT and return the user ID for the authenticated user, or throw
     a PassageError. Takes the place of the deprecated authenticateRequest() function.
     """
     def validateJwt(self, token):
         return self.authenticateJWT(token)
 
     def __refreshAuthCache(self):
         self.auth_origin = fetchApp(self.app_id)["auth_origin"]
         self.jwks = self.__fetchJWKS()
-        AUTH_CACHE[self.app_id] = {"jwks": self.jwks, "auth_origin": self.auth_origin}
+        hosted = self.__fetchHosted()
+
+        AUTH_CACHE[self.app_id] = {"jwks": self.jwks, "auth_origin": self.auth_origin, "hosted": hosted}
 
     """
     Authenticate a Flask or Django request that uses Passage for authentication.
     This function will verify the JWT and return the user ID for the authenticated user, or throw
     a PassageError
     """
     def authenticateRequest(self, request: Request) -> Union[str, PassageError]:
@@ -100,26 +115,28 @@
     for the authenticated user, or throw a PassageError.
     This function can be used to authenticate JWTs from Passage if they are not sent in a typical cookie or
     authorization header.
     """
     def authenticateJWT(self, token:str) -> Union[str, PassageError]:
         # load and parse the JWT
         try:
+            hosted = AUTH_CACHE[self.app_id]["hosted"]
             kid = jwt.get_unverified_header(token)["kid"]
             jwk = AUTH_CACHE[self.app_id]["jwks"][kid]
 
             # if the JWK can't be found, they might need to udpate the JWKS for this Passage intance
             # re-fetch the JWKS and try again
             if not jwk:
                 self.__refreshAuthCache
+                hosted = AUTH_CACHE[self.app_id]["hosted"]
                 kid = jwt.get_unverified_header(token)["kid"]
                 jwk = AUTH_CACHE[self.app_id]["jwks"][kid]
 
             public_key = jwt.algorithms.RSAAlgorithm.from_jwk(json.dumps(jwk))
-            claims = jwt.decode(token, public_key, audience=self.auth_origin, algorithms=["RS256"])
+            claims = jwt.decode(token, public_key, audience=[self.app_id] if hosted else self.auth_origin, algorithms=["RS256"])
             return claims["sub"]
         except Exception as e:
             raise PassageError(f"JWT is not valid: {e}")
 
     """
     Create Passage MagicLink
     """
```

### Comparing `passage-identity-2.4.0/passageidentity/requests.py` & `passage_identity-2.5.0/passageidentity/requests.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.4.0/setup.py` & `passage_identity-2.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="passage-identity",
-    version="2.4.0",
+    version="2.5.0",
     author="Passage Identity, Inc",
     author_email="support@passage.id",
     description="Python library to help manage your Passage application and users",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/passageidentity/passage-python",
     project_urls={
```

