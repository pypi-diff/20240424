# Comparing `tmp/alphaz-next-0.4.2.tar.gz` & `tmp/alphaz-next-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphaz-next-0.4.2.tar", last modified: Thu Apr 18 22:13:19 2024, max compression
+gzip compressed data, was "alphaz-next-0.5.0.tar", last modified: Wed Apr 24 15:48:51 2024, max compression
```

## Comparing `alphaz-next-0.4.2.tar` & `alphaz-next-0.5.0.tar`

### file list

```diff
@@ -1,63 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.632899 alphaz-next-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-18 22:13:19.632899 alphaz-next-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.624899 alphaz-next-0.4.2/alphaz_next/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.624899 alphaz-next-0.4.2/alphaz_next/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/asyncio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.624899 alphaz-next-0.4.2/alphaz_next/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.628899 alphaz-next-0.4.2/alphaz_next/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    11271 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/exception_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.628899 alphaz-next-0.4.2/alphaz_next/core/responses/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/responses/file_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/responses/html_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/responses/json_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/responses/orjson_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/responses/plaintext_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/responses/redirect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/responses/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/responses/streaming_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/responses/ujson_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/uvicorn_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.628899 alphaz-next-0.4.2/alphaz_next/libs/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/libs/file_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/libs/httpx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.624899 alphaz-next-0.4.2/alphaz_next/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.628899 alphaz-next-0.4.2/alphaz_next/models/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/models/auth/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.628899 alphaz-next-0.4.2/alphaz_next/models/config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.628899 alphaz-next-0.4.2/alphaz_next/models/config/_base/
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/models/config/_base/internal_config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/models/config/_base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/models/config/alpha_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/models/config/api_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/models/config/apm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/models/config/config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/models/config/database_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/models/config/directories_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/models/config/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/models/config/openapi_config_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.624899 alphaz-next-0.4.2/alphaz_next/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.628899 alphaz-next-0.4.2/alphaz_next/tests/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.628899 alphaz-next-0.4.2/alphaz_next/tests/utils/mocking/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/tests/utils/mocking/mock_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    27232 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/tests/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.632899 alphaz-next-0.4.2/alphaz_next/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/utils/logging_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.624899 alphaz-next-0.4.2/alphaz_next.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-18 22:13:19.000000 alphaz-next-0.4.2/alphaz_next.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-18 22:13:19.000000 alphaz-next-0.4.2/alphaz_next.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 22:13:19.000000 alphaz-next-0.4.2/alphaz_next.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-18 22:13:19.000000 alphaz-next-0.4.2/alphaz_next.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 22:13:19.000000 alphaz-next-0.4.2/alphaz_next.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 22:13:19.632899 alphaz-next-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-18 22:13:19.000000 alphaz-next-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:48:51.150560 alphaz-next-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-24 15:48:51.146560 alphaz-next-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:48:51.142560 alphaz-next-0.5.0/alphaz_next/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:48:51.142560 alphaz-next-0.5.0/alphaz_next/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/asyncio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:48:51.142560 alphaz-next-0.5.0/alphaz_next/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:48:51.142560 alphaz-next-0.5.0/alphaz_next/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/core/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/core/_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/core/exception_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:48:51.146560 alphaz-next-0.5.0/alphaz_next/core/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/core/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/core/responses/file_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/core/responses/html_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/core/responses/json_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/core/responses/orjson_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/core/responses/plaintext_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/core/responses/redirect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/core/responses/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/core/responses/streaming_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/core/responses/ujson_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:48:51.146560 alphaz-next-0.5.0/alphaz_next/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/libs/file_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/libs/httpx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:48:51.142560 alphaz-next-0.5.0/alphaz_next/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:48:51.146560 alphaz-next-0.5.0/alphaz_next/models/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/models/auth/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:48:51.146560 alphaz-next-0.5.0/alphaz_next/models/config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:48:51.146560 alphaz-next-0.5.0/alphaz_next/models/config/_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/models/config/_base/internal_config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/models/config/_base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/models/config/alpha_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/models/config/api_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/models/config/apm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/models/config/config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/models/config/database_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/models/config/directories_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/models/config/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/models/config/openapi_config_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:48:51.142560 alphaz-next-0.5.0/alphaz_next/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:48:51.146560 alphaz-next-0.5.0/alphaz_next/tests/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:48:51.146560 alphaz-next-0.5.0/alphaz_next/tests/utils/mocking/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/tests/utils/mocking/mock_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27232 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/tests/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:48:51.146560 alphaz-next-0.5.0/alphaz_next/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-24 15:48:46.000000 alphaz-next-0.5.0/alphaz_next/utils/format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:48:51.142560 alphaz-next-0.5.0/alphaz_next.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-24 15:48:51.000000 alphaz-next-0.5.0/alphaz_next.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-24 15:48:51.000000 alphaz-next-0.5.0/alphaz_next.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:48:51.000000 alphaz-next-0.5.0/alphaz_next.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-24 15:48:51.000000 alphaz-next-0.5.0/alphaz_next.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 15:48:51.000000 alphaz-next-0.5.0/alphaz_next.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:48:51.150560 alphaz-next-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-24 15:48:48.000000 alphaz-next-0.5.0/setup.py
```

### Comparing `alphaz-next-0.4.2/PKG-INFO` & `alphaz-next-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.4.2
+Version: 0.5.0
 Summary: A project to make a lib to start FASTAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.4.2.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.5.0.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alphaz-next-0.4.2/README.md` & `alphaz-next-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/auth/auth.py` & `alphaz-next-0.5.0/alphaz_next/auth/auth.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/core/_base.py` & `alphaz-next-0.5.0/alphaz_next/core/_base.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/core/_middleware.py` & `alphaz-next-0.5.0/alphaz_next/core/_middleware.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/core/application.py` & `alphaz-next-0.5.0/alphaz_next/core/application.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # MODULES
-import logging as _logging
-from logging.handlers import TimedRotatingFileHandler as _TimedRotatingFileHandler
-from pathlib import Path as _Path
 import sys as _sys
 from typing import (
     Any as _Any,
     AsyncContextManager as _AsyncContextManager,
     Dict as _Dict,
     List as _List,
     Optional as _Optional,
     Sequence as _Sequence,
     Union as _Union,
 )
+import logging
+from loguru import logger
 
 # FASTAPI
 from fastapi import (
     APIRouter as _APIRouter,
     FastAPI as _FastAPI,
     HTTPException as _HTTPException,
     Request as _Request,
@@ -34,21 +33,14 @@
 from fastapi.responses import (
     HTMLResponse as _HTMLResponse,
     JSONResponse as _JSONResponse,
     PlainTextResponse as _PlainTextResponse,
     RedirectResponse as _RedirectResponse,
 )
 
-if "dependency_injector" in _sys.modules:
-    from dependency_injector import containers as _containers
-
-    _ContainerType = _containers.DeclarativeContainer
-else:
-    _ContainerType = _Any
-
 # ELASTICAPM
 from elasticapm.contrib.starlette import (
     make_apm_client as _make_apm_client,
     ElasticAPM as _ElasticAPM,
 )
 
 # MODELS
@@ -57,30 +49,25 @@
 )
 
 # CORE
 from alphaz_next.core._middleware import (
     log_request_middleware as _log_request_middleware,
     CORSMiddleware as _CORSMiddleware,
 )
-from alphaz_next.core.uvicorn_logger import UVICORN_LOGGER as _UVICORN_LOGGER
-
-# UTILS
-from alphaz_next.utils.logging_filters import (
-    ExcludeRoutersFilter as _ExcludeRoutersFilter,
-)
-from alphaz_next.utils.logger import (
-    DEFAULT_DATE_FORMAT as _DEFAULT_DATE_FORMAT,
-    DEFAULT_FORMAT as _DEFAULT_FORMAT,
-)
 
 
 # ELASTICAPM
 
 _DEFAULT_FAVICON_URL = "https://fastapi.tiangolo.com/img/favicon.png"
 
+_uvicorn_access = logging.getLogger("uvicorn.access")
+_uvicorn_access.disabled = True
+
+uvicorn_logger = logger.bind(service="uvicorn")
+
 
 def _custom_openapi(
     config: _AlphaConfigSchema, routes: _List[_BaseRoute]
 ) -> _Dict[str, _Any]:
     """
     Generate a custom OpenAPI schema based on the provided configuration and routes.
 
@@ -116,23 +103,21 @@
     return openapi_schema
 
 
 def create_app(
     config: _AlphaConfigSchema,
     routes: _Optional[_BaseRoute] = None,
     routers: _Optional[_List[_APIRouter]] = None,
-    container: _Optional[_ContainerType] = None,
     lifespan: _Optional[_AsyncContextManager] = None,
     allow_origins: _Sequence[str] = (),
     allow_methods: _Sequence[str] = ("GET",),
     allow_headers: _Sequence[str] = (),
     allow_credentials: bool = False,
     allow_private_network: bool = False,
     status_response: _Dict = {"status": "OK"},
-    uvicorn_formatter: _Optional[_logging.Formatter] = None,
 ) -> _FastAPI:
     """
     Create a FastAPI application with the specified configuration.
 
     Args:
         config (AlphaConfigSchema): The configuration for the application.
         routes (Optional[BaseRoute]): The list of routes to include in the application. Defaults to None.
@@ -140,59 +125,42 @@
         container (Optional[containers.DeclarativeContainer]): The dependency injection container. Defaults to None.
         allow_origins (Sequence[str]): The list of allowed origins for CORS. Defaults to ().
         allow_methods (Sequence[str]): The list of allowed HTTP methods for CORS. Defaults to ("GET",).
         allow_headers (Sequence[str]): The list of allowed headers for CORS. Defaults to ().
         allow_credentials (bool): Whether to allow credentials for CORS. Defaults to False.
         allow_private_network (bool): Whether to allow private network for CORS. Defaults to False.
         status_response (Dict): The response to return for the "/status" endpoint. Defaults to {"status": "OK"}.
-        uvicorn_formatter (Optional[_logging.Formatter]): The formatter used in time rotating file handler if time rotating logging config exists. If None, use the default one.
 
     Returns:
         FastAPI: The created FastAPI application.
     """
 
-    if (
-        config.api_config.logging is not None
-        and config.api_config.logging.time_rotating is not None
-    ):
-        if uvicorn_formatter is None:
-            uvicorn_formatter = _logging.Formatter(
-                _DEFAULT_FORMAT,
-                datefmt=_DEFAULT_DATE_FORMAT,
-            )
-
-        directory_path = _Path(config.api_config.directories.logs)
-        directory_path.mkdir(parents=True, exist_ok=True)
-
-        handler = _TimedRotatingFileHandler(
-            filename=directory_path / "uvicorn.log",
-            when=config.api_config.logging.time_rotating.when,
-            interval=config.api_config.logging.time_rotating.interval,
-            backupCount=config.api_config.logging.time_rotating.backup_count,
-        )
-        handler.setFormatter(uvicorn_formatter)
-
-        _UVICORN_LOGGER.addHandler(handler)
-
-        _UVICORN_LOGGER.addFilter(
-            _ExcludeRoutersFilter(
-                router_names=config.api_config.logging.excluded_routers
-            )
+    if config.api_config.logging is not None:
+        uvicorn_logger.add(
+            _sys.stderr,
+            level=config.api_config.logging.level.upper(),
+            filter=lambda record: all(
+                [
+                    record["service"] == "uvicorn",
+                    record["endpoint"]
+                    not in config.api_config.logging.excluded_routers,
+                ]
+            ),
+            colorize=True,
         )
 
     # APP
     app = _FastAPI(
         routes=routes,
         title=config.project_name.upper(),
         version=config.version,
         docs_url=None,
         redoc_url=None,
         lifespan=lifespan,
     )
-    app.container = container
 
     app.add_middleware(
         _CORSMiddleware,
         allow_origins=allow_origins,
         allow_credentials=allow_credentials,
         allow_methods=allow_methods,
         allow_headers=allow_headers,
@@ -239,15 +207,17 @@
         body = await request.body()
         query_params = request.query_params._dict
         detail = {
             "errors": exc.errors(),
             "body": body.decode(),
             "query_params": query_params,
         }
-        _UVICORN_LOGGER.info(detail)
+
+        with uvicorn_logger.contextualize(endpoint=request.base_url):
+            uvicorn_logger.info(detail)
         return await _request_validation_exception_handler(request, exc)
 
     @app.exception_handler(_HTTPException)
     async def http_exception_handler(
         request: _Request, exc: _HTTPException
     ) -> _Union[_JSONResponse, _Response]:
         """
@@ -269,17 +239,19 @@
         url = (
             f"{request.url.path}?{request.query_params}"
             if request.query_params
             else request.url.path
         )
         exception_type, exception_value, exception_traceback = _sys.exc_info()
         exception_name = getattr(exception_type, "__name__", None)
-        _UVICORN_LOGGER.error(
-            f'{host}:{port} - "{request.method} {url}" 500 Internal Server Error <{exception_name}: {exception_value}>'
-        )
+
+        with uvicorn_logger.contextualize(endpoint=request.base_url):
+            uvicorn_logger.error(
+                f'{host}:{port} - "{request.method} {url}" 500 Internal Server Error <{exception_name}: {exception_value}>'
+            )
         return _PlainTextResponse(str(exc), status_code=500)
 
     @app.get("/status", include_in_schema=False)
     async def get_api_status():
         return status_response
 
     @app.get("/docs", include_in_schema=False)
```

### Comparing `alphaz-next-0.4.2/alphaz_next/core/exception_handlers.py` & `alphaz-next-0.5.0/alphaz_next/core/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/core/exceptions.py` & `alphaz-next-0.5.0/alphaz_next/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/core/responses/__init__.py` & `alphaz-next-0.5.0/alphaz_next/core/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/core/responses/file_response.py` & `alphaz-next-0.5.0/alphaz_next/core/responses/file_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/core/responses/html_response.py` & `alphaz-next-0.5.0/alphaz_next/core/responses/html_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/core/responses/json_response.py` & `alphaz-next-0.5.0/alphaz_next/core/responses/json_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/core/responses/orjson_response.py` & `alphaz-next-0.5.0/alphaz_next/core/responses/orjson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/core/responses/plaintext_response.py` & `alphaz-next-0.5.0/alphaz_next/core/responses/plaintext_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/core/responses/redirect_response.py` & `alphaz-next-0.5.0/alphaz_next/core/responses/redirect_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/core/responses/response.py` & `alphaz-next-0.5.0/alphaz_next/core/responses/response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/core/responses/streaming_response.py` & `alphaz-next-0.5.0/alphaz_next/core/responses/streaming_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/core/responses/ujson_response.py` & `alphaz-next-0.5.0/alphaz_next/core/responses/ujson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/libs/httpx.py` & `alphaz-next-0.5.0/alphaz_next/libs/httpx.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/models/config/_base/internal_config_settings.py` & `alphaz-next-0.5.0/alphaz_next/models/config/_base/internal_config_settings.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/models/config/_base/utils.py` & `alphaz-next-0.5.0/alphaz_next/models/config/_base/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/models/config/alpha_config.py` & `alphaz-next-0.5.0/alphaz_next/models/config/alpha_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/models/config/api_config.py` & `alphaz-next-0.5.0/alphaz_next/models/config/api_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/models/config/apm_config.py` & `alphaz-next-0.5.0/alphaz_next/models/config/apm_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/models/config/config_settings.py` & `alphaz-next-0.5.0/alphaz_next/models/config/config_settings.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/models/config/database_config.py` & `alphaz-next-0.5.0/alphaz_next/models/config/database_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/models/config/logging_config.py` & `alphaz-next-0.5.0/alphaz_next/models/config/logging_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,64 @@
 # PYDANTIC
-from typing import Annotated as _Annotated, List as _List
+from typing import Annotated as _Annotated, List as _List, Optional as _Optional
+from loguru import _defaults
 
 # PYDANTIC
 from pydantic_core.core_schema import FieldValidationInfo as _FieldValidationInfo
 from pydantic import (
     BaseModel as _BaseModel,
     ConfigDict as _ConfigDict,
     Field as _Field,
-    PositiveInt as _PositiveInt,
     StringConstraints as _StringConstraints,
     computed_field as _computed_field,
     field_validator as _field_validator,
 )
 
 LOGGING_LEVEL = {
-    "CRITICAL": 50,
-    "FATAL": 50,
-    "ERROR": 40,
-    "WARNING": 30,
-    "WARN": 30,
-    "INFO": 20,
-    "DEBUG": 10,
-    "NOTSET": 0,
+    "CRITICAL": _defaults.LOGURU_CRITICAL_NO,
+    "ERROR": _defaults.LOGURU_ERROR_NO,
+    "WARNING": _defaults.LOGURU_WARNING_NO,
+    "SUCCESS": _defaults.LOGURU_SUCCESS_NO,
+    "INFO": _defaults.LOGURU_INFO_NO,
+    "DEBUG": _defaults.LOGURU_DEBUG_NO,
+    "TRACE": _defaults.LOGURU_TRACE_NO,
 }
 
 
-class TimeRotatingSchema(_BaseModel):
-    """
-    Represents the configuration schema for time-based rotating log files.
-
-    Attributes:
-        when (str): The time interval at which the log files should rotate.
-        interval (PositiveInt): The number of time units between each rotation.
-        backup_count (PositiveInt): The maximum number of backup log files to keep.
-    """
-
-    model_config = _ConfigDict(from_attributes=True)
-
-    when: str
-    interval: _PositiveInt
-    backup_count: _PositiveInt
-
-
 class LoggingSchema(_BaseModel):
     """
     Represents the configuration schema for logging.
 
     Attributes:
         model_config (ConfigDict): Configuration dictionary for the model.
         level (str): Logging level.
-        time_rotating (TimeRotatingSchema): Schema for time rotating configuration.
+        rotation (Optional[str]): Log rotation.
+        retention (Optional[int]): Log retention.
         excluded_routers (List[str]): List of excluded routers.
         level_code (int): Logging level code.
     """
 
     model_config = _ConfigDict(from_attributes=True)
 
     level: _Annotated[
         str,
         _StringConstraints(
             strip_whitespace=True,
             to_upper=True,
         ),
     ]
-    time_rotating: TimeRotatingSchema
+    rotation: _Optional[str] = _Field(default=None)
+    retention: _Optional[int] = _Field(default=None)
     excluded_routers: _List[str] = _Field(default_factory=lambda: [])
 
     @_field_validator("level")
     @classmethod
     def validate_level(cls, value: str, info: _FieldValidationInfo):
         if value not in LOGGING_LEVEL:
             raise ValueError(f"{info.field_name} is not valid")
 
         return value
 
     @_computed_field
     @property
     def level_code(self) -> int:
-        return LOGGING_LEVEL.get(self.level)
+        return LOGGING_LEVEL.get(self.level.upper(), 0)
```

### Comparing `alphaz-next-0.4.2/alphaz_next/models/config/openapi_config_schema.py` & `alphaz-next-0.5.0/alphaz_next/models/config/openapi_config_schema.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/tests/utils/utils.py` & `alphaz-next-0.5.0/alphaz_next/tests/utils/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next/utils/format.py` & `alphaz-next-0.5.0/alphaz_next/utils/format.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.2/alphaz_next.egg-info/PKG-INFO` & `alphaz-next-0.5.0/alphaz_next.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.4.2
+Version: 0.5.0
 Summary: A project to make a lib to start FASTAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.4.2.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.5.0.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alphaz-next-0.4.2/alphaz_next.egg-info/SOURCES.txt` & `alphaz-next-0.5.0/alphaz_next.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 alphaz_next/auth/auth.py
 alphaz_next/core/_base.py
 alphaz_next/core/_middleware.py
 alphaz_next/core/application.py
 alphaz_next/core/constants.py
 alphaz_next/core/exception_handlers.py
 alphaz_next/core/exceptions.py
-alphaz_next/core/uvicorn_logger.py
 alphaz_next/core/responses/__init__.py
 alphaz_next/core/responses/file_response.py
 alphaz_next/core/responses/html_response.py
 alphaz_next/core/responses/json_response.py
 alphaz_next/core/responses/orjson_response.py
 alphaz_next/core/responses/plaintext_response.py
 alphaz_next/core/responses/redirect_response.py
@@ -36,10 +35,8 @@
 alphaz_next/models/config/directories_config.py
 alphaz_next/models/config/logging_config.py
 alphaz_next/models/config/openapi_config_schema.py
 alphaz_next/models/config/_base/internal_config_settings.py
 alphaz_next/models/config/_base/utils.py
 alphaz_next/tests/utils/utils.py
 alphaz_next/tests/utils/mocking/mock_user.py
-alphaz_next/utils/format.py
-alphaz_next/utils/logger.py
-alphaz_next/utils/logging_filters.py
+alphaz_next/utils/format.py
```

### Comparing `alphaz-next-0.4.2/setup.py` & `alphaz-next-0.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.4.2"
+version = "0.5.0"
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 
 EXTRAS_REQUIRE = {
     "dependency-injector": ["dependency-injector"],
```

