# Comparing `tmp/splight_lib-5.6.2.tar.gz` & `tmp/splight_lib-5.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight_lib-5.6.2.tar", max compression
+gzip compressed data, was "splight_lib-5.6.3.tar", max compression
```

## Comparing `splight_lib-5.6.2.tar` & `splight_lib-5.6.3.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0        0 2024-04-11 16:55:53.706802 splight_lib-5.6.2/LICENSE.txt
--rw-r--r--   0        0        0     1108 2024-04-11 16:55:53.706802 splight_lib-5.6.2/README.md
--rw-r--r--   0        0        0     1532 2024-04-11 16:55:53.706802 splight_lib-5.6.2/pyproject.toml
--rw-r--r--   0        0        0      114 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/abstract/__init__.py
--rw-r--r--   0        0        0     3358 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/abstract/client.py
--rw-r--r--   0        0        0      160 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/auth/__init__.py
--rw-r--r--   0        0        0      404 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/auth/exceptions.py
--rw-r--r--   0        0        0     2944 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/auth/mac_auth.py
--rw-r--r--   0        0        0      224 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/auth/token.py
--rw-r--r--   0        0        0        0 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/client/__init__.py
--rw-r--r--   0        0        0      358 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/client/database/__init__.py
--rw-r--r--   0        0        0      785 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/client/database/abstract.py
--rw-r--r--   0        0        0      582 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/client/database/builder.py
--rw-r--r--   0        0        0     1277 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/client/database/classmap.py
--rw-r--r--   0        0        0     6192 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/client/database/local_client.py
--rw-r--r--   0        0        0    12163 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/client/database/remote_client.py
--rw-r--r--   0        0        0      474 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/client/datalake/__init__.py
--rw-r--r--   0        0        0     1878 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/client/datalake/abstract.py
--rw-r--r--   0        0        0     1649 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/client/datalake/buffer.py
--rw-r--r--   0        0        0      944 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/client/datalake/builder.py
--rw-r--r--   0        0        0      210 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/client/datalake/exceptions.py
--rw-r--r--   0        0        0     3728 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/client/datalake/local_client.py
--rw-r--r--   0        0        0    13636 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/client/datalake/remote_client.py
--rw-r--r--   0        0        0     1505 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/client/datalake/schemas.py
--rw-r--r--   0        0        0      948 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/client/exceptions.py
--rw-r--r--   0        0        0      981 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/client/file_handler.py
--rw-r--r--   0        0        0      595 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/client/filter.py
--rw-r--r--   0        0        0       96 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/client/hub/__init__.py
--rw-r--r--   0        0        0      803 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/client/hub/abstract.py
--rw-r--r--   0        0        0     4662 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/client/hub/client.py
--rw-r--r--   0        0        0     5218 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/client/tests/test_database.py
--rw-r--r--   0        0        0     1623 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/client/tests/test_datalake.py
--rw-r--r--   0        0        0      105 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/component/__init__.py
--rw-r--r--   0        0        0     6963 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/component/abstract.py
--rw-r--r--   0        0        0      480 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/component/exceptions.py
--rw-r--r--   0        0        0     7844 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/component/spec.py
--rw-r--r--   0        0        0       49 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/component/tests/test_abstract.py
--rw-r--r--   0        0        0     4115 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/component/tests/test_spec.py
--rw-r--r--   0        0        0      210 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/constants.py
--rw-r--r--   0        0        0     2002 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/encryption.py
--rw-r--r--   0        0        0      303 2024-04-11 16:55:53.706802 splight_lib-5.6.2/splight_lib/execution/__init__.py
--rw-r--r--   0        0        0     3988 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/execution/engine.py
--rw-r--r--   0        0        0      282 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/execution/exceptions.py
--rw-r--r--   0        0        0     2990 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/execution/scheduling.py
--rw-r--r--   0        0        0     1932 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/execution/task.py
--rw-r--r--   0        0        0     1034 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/execution/tests/test_execution.py
--rw-r--r--   0        0        0     1048 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/execution/tests/test_scheduling.py
--rw-r--r--   0        0        0     1302 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/execution/trigger.py
--rw-r--r--   0        0        0      192 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/logging/__init__.py
--rw-r--r--   0        0        0     1516 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/logging/_internal.py
--rw-r--r--   0        0        0     1426 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/logging/component.py
--rw-r--r--   0        0        0      130 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/logging/constants.py
--rw-r--r--   0        0        0     4881 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/logging/logging.py
--rw-r--r--   0        0        0     4316 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/logging/tests/test_logging.py
--rw-r--r--   0        0        0     1271 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/models/__init__.py
--rw-r--r--   0        0        0     7791 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/models/alert.py
--rw-r--r--   0        0        0     1600 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/models/asset.py
--rw-r--r--   0        0        0      452 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/models/attribute.py
--rw-r--r--   0        0        0     6362 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/models/base.py
--rw-r--r--   0        0        0    18782 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/models/component.py
--rw-r--r--   0        0        0     2857 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/models/dashboard.py
--rw-r--r--   0        0        0     1024 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/models/data_address.py
--rw-r--r--   0        0        0      634 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/models/exceptions.py
--rw-r--r--   0        0        0     1869 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/models/file.py
--rw-r--r--   0        0        0     6710 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/models/function.py
--rw-r--r--   0        0        0      790 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/models/generic.py
--rw-r--r--   0        0        0     7153 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/models/hub.py
--rw-r--r--   0        0        0     1098 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/models/hub_solution.py
--rw-r--r--   0        0        0      606 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/models/metadata.py
--rw-r--r--   0        0        0     2162 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/models/native.py
--rw-r--r--   0        0        0     2398 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/models/pipeline.py
--rw-r--r--   0        0        0      487 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/models/secret.py
--rw-r--r--   0        0        0    11054 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/models/tests/models.json
--rw-r--r--   0        0        0     2376 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/models/tests/test_component_object_instance.py
--rw-r--r--   0        0        0     3575 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/models/tests/test_database_model.py
--rw-r--r--   0        0        0     1389 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/models/tests/test_metadata.py
--rw-r--r--   0        0        0      823 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/models/tests/test_models.py
--rw-r--r--   0        0        0      212 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/restclient/__init__.py
--rw-r--r--   0        0        0    16872 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/restclient/client.py
--rw-r--r--   0        0        0      964 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/restclient/exceptions.py
--rw-r--r--   0        0        0     1108 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/restclient/tests/test_restclient.py
--rw-r--r--   0        0        0     2386 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/restclient/types.py
--rw-r--r--   0        0        0     3586 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/settings.py
--rw-r--r--   0        0        0      427 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/stringcase.py
--rw-r--r--   0        0        0     2834 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/testing/__init__.py
--rw-r--r--   0        0        0      251 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/tests/FakeProc.py
--rw-r--r--   0        0        0     5885 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/tests/asset_geometries.json
--rw-r--r--   0        0        0     5400 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/tests/test_api_contracts.py
--rw-r--r--   0        0        0       41 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/tests/test_encryption.py
--rw-r--r--   0        0        0        0 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/utils/__init__.py
--rw-r--r--   0        0        0     2297 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/utils/custom_model.py
--rw-r--r--   0        0        0      626 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/utils/hub.py
--rw-r--r--   0        0        0       78 2024-04-11 16:55:53.710802 splight_lib-5.6.2/splight_lib/version.py
--rw-r--r--   0        0        0     2547 1970-01-01 00:00:00.000000 splight_lib-5.6.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-23 21:17:05.572489 splight_lib-5.6.3/LICENSE.txt
+-rw-r--r--   0        0        0     1108 2024-04-23 21:17:05.572489 splight_lib-5.6.3/README.md
+-rw-r--r--   0        0        0     1532 2024-04-23 21:17:05.572489 splight_lib-5.6.3/pyproject.toml
+-rw-r--r--   0        0        0      114 2024-04-23 21:17:05.572489 splight_lib-5.6.3/splight_lib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:17:05.572489 splight_lib-5.6.3/splight_lib/abstract/__init__.py
+-rw-r--r--   0        0        0     3358 2024-04-23 21:17:05.572489 splight_lib-5.6.3/splight_lib/abstract/client.py
+-rw-r--r--   0        0        0      160 2024-04-23 21:17:05.572489 splight_lib-5.6.3/splight_lib/auth/__init__.py
+-rw-r--r--   0        0        0      404 2024-04-23 21:17:05.572489 splight_lib-5.6.3/splight_lib/auth/exceptions.py
+-rw-r--r--   0        0        0     2944 2024-04-23 21:17:05.572489 splight_lib-5.6.3/splight_lib/auth/mac_auth.py
+-rw-r--r--   0        0        0      224 2024-04-23 21:17:05.572489 splight_lib-5.6.3/splight_lib/auth/token.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:17:05.572489 splight_lib-5.6.3/splight_lib/client/__init__.py
+-rw-r--r--   0        0        0      358 2024-04-23 21:17:05.572489 splight_lib-5.6.3/splight_lib/client/database/__init__.py
+-rw-r--r--   0        0        0      785 2024-04-23 21:17:05.572489 splight_lib-5.6.3/splight_lib/client/database/abstract.py
+-rw-r--r--   0        0        0      582 2024-04-23 21:17:05.572489 splight_lib-5.6.3/splight_lib/client/database/builder.py
+-rw-r--r--   0        0        0     1277 2024-04-23 21:17:05.572489 splight_lib-5.6.3/splight_lib/client/database/classmap.py
+-rw-r--r--   0        0        0     6192 2024-04-23 21:17:05.572489 splight_lib-5.6.3/splight_lib/client/database/local_client.py
+-rw-r--r--   0        0        0    12163 2024-04-23 21:17:05.572489 splight_lib-5.6.3/splight_lib/client/database/remote_client.py
+-rw-r--r--   0        0        0      474 2024-04-23 21:17:05.572489 splight_lib-5.6.3/splight_lib/client/datalake/__init__.py
+-rw-r--r--   0        0        0     1878 2024-04-23 21:17:05.572489 splight_lib-5.6.3/splight_lib/client/datalake/abstract.py
+-rw-r--r--   0        0        0     1649 2024-04-23 21:17:05.572489 splight_lib-5.6.3/splight_lib/client/datalake/buffer.py
+-rw-r--r--   0        0        0      944 2024-04-23 21:17:05.572489 splight_lib-5.6.3/splight_lib/client/datalake/builder.py
+-rw-r--r--   0        0        0      210 2024-04-23 21:17:05.572489 splight_lib-5.6.3/splight_lib/client/datalake/exceptions.py
+-rw-r--r--   0        0        0     3728 2024-04-23 21:17:05.572489 splight_lib-5.6.3/splight_lib/client/datalake/local_client.py
+-rw-r--r--   0        0        0    13636 2024-04-23 21:17:05.572489 splight_lib-5.6.3/splight_lib/client/datalake/remote_client.py
+-rw-r--r--   0        0        0     1505 2024-04-23 21:17:05.572489 splight_lib-5.6.3/splight_lib/client/datalake/schemas.py
+-rw-r--r--   0        0        0      948 2024-04-23 21:17:05.572489 splight_lib-5.6.3/splight_lib/client/exceptions.py
+-rw-r--r--   0        0        0      981 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/client/file_handler.py
+-rw-r--r--   0        0        0      595 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/client/filter.py
+-rw-r--r--   0        0        0       96 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/client/hub/__init__.py
+-rw-r--r--   0        0        0      803 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/client/hub/abstract.py
+-rw-r--r--   0        0        0     4660 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/client/hub/client.py
+-rw-r--r--   0        0        0     5218 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/client/tests/test_database.py
+-rw-r--r--   0        0        0     1623 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/client/tests/test_datalake.py
+-rw-r--r--   0        0        0      105 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/component/__init__.py
+-rw-r--r--   0        0        0     6963 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/component/abstract.py
+-rw-r--r--   0        0        0      480 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/component/exceptions.py
+-rw-r--r--   0        0        0     7844 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/component/spec.py
+-rw-r--r--   0        0        0       49 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/component/tests/test_abstract.py
+-rw-r--r--   0        0        0     4115 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/component/tests/test_spec.py
+-rw-r--r--   0        0        0      210 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/constants.py
+-rw-r--r--   0        0        0     2002 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/encryption.py
+-rw-r--r--   0        0        0      303 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/execution/__init__.py
+-rw-r--r--   0        0        0     3988 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/execution/engine.py
+-rw-r--r--   0        0        0      282 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/execution/exceptions.py
+-rw-r--r--   0        0        0     2990 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/execution/scheduling.py
+-rw-r--r--   0        0        0     1932 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/execution/task.py
+-rw-r--r--   0        0        0     1034 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/execution/tests/test_execution.py
+-rw-r--r--   0        0        0     1048 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/execution/tests/test_scheduling.py
+-rw-r--r--   0        0        0     1302 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/execution/trigger.py
+-rw-r--r--   0        0        0      192 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/logging/__init__.py
+-rw-r--r--   0        0        0     1516 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/logging/_internal.py
+-rw-r--r--   0        0        0     1426 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/logging/component.py
+-rw-r--r--   0        0        0      130 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/logging/constants.py
+-rw-r--r--   0        0        0     4881 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/logging/logging.py
+-rw-r--r--   0        0        0     4316 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/logging/tests/test_logging.py
+-rw-r--r--   0        0        0     1271 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/models/__init__.py
+-rw-r--r--   0        0        0     7791 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/models/alert.py
+-rw-r--r--   0        0        0     1600 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/models/asset.py
+-rw-r--r--   0        0        0      452 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/models/attribute.py
+-rw-r--r--   0        0        0     6362 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/models/base.py
+-rw-r--r--   0        0        0    18782 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/models/component.py
+-rw-r--r--   0        0        0     2857 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/models/dashboard.py
+-rw-r--r--   0        0        0     1024 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/models/data_address.py
+-rw-r--r--   0        0        0      634 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/models/exceptions.py
+-rw-r--r--   0        0        0     1869 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/models/file.py
+-rw-r--r--   0        0        0     6710 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/models/function.py
+-rw-r--r--   0        0        0      790 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/models/generic.py
+-rw-r--r--   0        0        0     7153 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/models/hub.py
+-rw-r--r--   0        0        0     1098 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/models/hub_solution.py
+-rw-r--r--   0        0        0      606 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/models/metadata.py
+-rw-r--r--   0        0        0     2162 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/models/native.py
+-rw-r--r--   0        0        0     2398 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/models/pipeline.py
+-rw-r--r--   0        0        0      487 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/models/secret.py
+-rw-r--r--   0        0        0    11054 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/models/tests/models.json
+-rw-r--r--   0        0        0     2376 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/models/tests/test_component_object_instance.py
+-rw-r--r--   0        0        0     3575 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/models/tests/test_database_model.py
+-rw-r--r--   0        0        0     1389 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/models/tests/test_metadata.py
+-rw-r--r--   0        0        0      823 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/models/tests/test_models.py
+-rw-r--r--   0        0        0      212 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/restclient/__init__.py
+-rw-r--r--   0        0        0    16872 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/restclient/client.py
+-rw-r--r--   0        0        0      964 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/restclient/exceptions.py
+-rw-r--r--   0        0        0     1108 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/restclient/tests/test_restclient.py
+-rw-r--r--   0        0        0     2386 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/restclient/types.py
+-rw-r--r--   0        0        0     3586 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/settings.py
+-rw-r--r--   0        0        0      427 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/stringcase.py
+-rw-r--r--   0        0        0     2834 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/testing/__init__.py
+-rw-r--r--   0        0        0      251 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/tests/FakeProc.py
+-rw-r--r--   0        0        0     5885 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/tests/asset_geometries.json
+-rw-r--r--   0        0        0     5400 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/tests/test_api_contracts.py
+-rw-r--r--   0        0        0       41 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/tests/test_encryption.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/utils/__init__.py
+-rw-r--r--   0        0        0     2297 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/utils/custom_model.py
+-rw-r--r--   0        0        0      626 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/utils/hub.py
+-rw-r--r--   0        0        0       78 2024-04-23 21:17:05.576489 splight_lib-5.6.3/splight_lib/version.py
+-rw-r--r--   0        0        0     2547 1970-01-01 00:00:00.000000 splight_lib-5.6.3/PKG-INFO
```

### Comparing `splight_lib-5.6.2/README.md` & `splight_lib-5.6.3/README.md`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/pyproject.toml` & `splight_lib-5.6.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "splight-lib"
-version = "5.6.2"
+version = "5.6.3"
 description = "Splight Library"
 authors = ["Splight Dev <dev@splight-ae.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4"
 concurrent-log-handler = "0.9.21"
```

### Comparing `splight_lib-5.6.2/splight_lib/abstract/client.py` & `splight_lib-5.6.3/splight_lib/abstract/client.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/auth/mac_auth.py` & `splight_lib-5.6.3/splight_lib/auth/mac_auth.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/client/database/abstract.py` & `splight_lib-5.6.3/splight_lib/client/database/abstract.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/client/database/builder.py` & `splight_lib-5.6.3/splight_lib/client/database/builder.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/client/database/classmap.py` & `splight_lib-5.6.3/splight_lib/client/database/classmap.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/client/database/local_client.py` & `splight_lib-5.6.3/splight_lib/client/database/local_client.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/client/database/remote_client.py` & `splight_lib-5.6.3/splight_lib/client/database/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/client/datalake/abstract.py` & `splight_lib-5.6.3/splight_lib/client/datalake/abstract.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/client/datalake/buffer.py` & `splight_lib-5.6.3/splight_lib/client/datalake/buffer.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/client/datalake/builder.py` & `splight_lib-5.6.3/splight_lib/client/datalake/builder.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/client/datalake/local_client.py` & `splight_lib-5.6.3/splight_lib/client/datalake/local_client.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/client/datalake/remote_client.py` & `splight_lib-5.6.3/splight_lib/client/datalake/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/client/datalake/schemas.py` & `splight_lib-5.6.3/splight_lib/client/datalake/schemas.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/client/exceptions.py` & `splight_lib-5.6.3/splight_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/client/file_handler.py` & `splight_lib-5.6.3/splight_lib/client/file_handler.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/client/filter.py` & `splight_lib-5.6.3/splight_lib/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/client/hub/abstract.py` & `splight_lib-5.6.3/splight_lib/client/hub/abstract.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/client/hub/client.py` & `splight_lib-5.6.3/splight_lib/client/hub/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         response = self._session.post(url, json=instance)
         response.raise_for_status()
         instance = response.json()
         return instance
 
     def _update(self, instance: Dict) -> Dict:
         instance_id = instance.get("id")
-        url = self._hub_url / "components" / f"{instance_id}/"
+        url = self._hub_url / "versions" / f"{instance_id}/"
         response = self._session.put(url, json=instance)
         response.raise_for_status()
         instance = response.json()
         return instance
 
     def build(self, id: str):
         url = self._hub_url / f"versions/{id}/build/"
```

### Comparing `splight_lib-5.6.2/splight_lib/client/tests/test_database.py` & `splight_lib-5.6.3/splight_lib/client/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/client/tests/test_datalake.py` & `splight_lib-5.6.3/splight_lib/client/tests/test_datalake.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/component/abstract.py` & `splight_lib-5.6.3/splight_lib/component/abstract.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/component/spec.py` & `splight_lib-5.6.3/splight_lib/component/spec.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/component/tests/test_spec.py` & `splight_lib-5.6.3/splight_lib/component/tests/test_spec.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/encryption.py` & `splight_lib-5.6.3/splight_lib/encryption.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/execution/engine.py` & `splight_lib-5.6.3/splight_lib/execution/engine.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/execution/scheduling.py` & `splight_lib-5.6.3/splight_lib/execution/scheduling.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/execution/task.py` & `splight_lib-5.6.3/splight_lib/execution/task.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/execution/tests/test_execution.py` & `splight_lib-5.6.3/splight_lib/execution/tests/test_execution.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/execution/tests/test_scheduling.py` & `splight_lib-5.6.3/splight_lib/execution/tests/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/execution/trigger.py` & `splight_lib-5.6.3/splight_lib/execution/trigger.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/logging/_internal.py` & `splight_lib-5.6.3/splight_lib/logging/_internal.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/logging/component.py` & `splight_lib-5.6.3/splight_lib/logging/component.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/logging/logging.py` & `splight_lib-5.6.3/splight_lib/logging/logging.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/logging/tests/test_logging.py` & `splight_lib-5.6.3/splight_lib/logging/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/models/__init__.py` & `splight_lib-5.6.3/splight_lib/models/__init__.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/models/alert.py` & `splight_lib-5.6.3/splight_lib/models/alert.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/models/asset.py` & `splight_lib-5.6.3/splight_lib/models/asset.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/models/base.py` & `splight_lib-5.6.3/splight_lib/models/base.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/models/component.py` & `splight_lib-5.6.3/splight_lib/models/component.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/models/dashboard.py` & `splight_lib-5.6.3/splight_lib/models/dashboard.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/models/data_address.py` & `splight_lib-5.6.3/splight_lib/models/data_address.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/models/exceptions.py` & `splight_lib-5.6.3/splight_lib/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/models/file.py` & `splight_lib-5.6.3/splight_lib/models/file.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/models/function.py` & `splight_lib-5.6.3/splight_lib/models/function.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/models/generic.py` & `splight_lib-5.6.3/splight_lib/models/generic.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/models/hub.py` & `splight_lib-5.6.3/splight_lib/models/hub.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/models/hub_solution.py` & `splight_lib-5.6.3/splight_lib/models/hub_solution.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/models/metadata.py` & `splight_lib-5.6.3/splight_lib/models/metadata.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/models/native.py` & `splight_lib-5.6.3/splight_lib/models/native.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/models/pipeline.py` & `splight_lib-5.6.3/splight_lib/models/pipeline.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/models/tests/models.json` & `splight_lib-5.6.3/splight_lib/models/tests/models.json`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/models/tests/test_component_object_instance.py` & `splight_lib-5.6.3/splight_lib/models/tests/test_component_object_instance.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/models/tests/test_database_model.py` & `splight_lib-5.6.3/splight_lib/models/tests/test_database_model.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/models/tests/test_metadata.py` & `splight_lib-5.6.3/splight_lib/models/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/models/tests/test_models.py` & `splight_lib-5.6.3/splight_lib/models/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/restclient/client.py` & `splight_lib-5.6.3/splight_lib/restclient/client.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/restclient/exceptions.py` & `splight_lib-5.6.3/splight_lib/restclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/restclient/tests/test_restclient.py` & `splight_lib-5.6.3/splight_lib/restclient/tests/test_restclient.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/restclient/types.py` & `splight_lib-5.6.3/splight_lib/restclient/types.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/settings.py` & `splight_lib-5.6.3/splight_lib/settings.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/testing/__init__.py` & `splight_lib-5.6.3/splight_lib/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/tests/asset_geometries.json` & `splight_lib-5.6.3/splight_lib/tests/asset_geometries.json`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/tests/test_api_contracts.py` & `splight_lib-5.6.3/splight_lib/tests/test_api_contracts.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/utils/custom_model.py` & `splight_lib-5.6.3/splight_lib/utils/custom_model.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/splight_lib/utils/hub.py` & `splight_lib-5.6.3/splight_lib/utils/hub.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.2/PKG-INFO` & `splight_lib-5.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 5.6.2
+Version: 5.6.3
 Summary: Splight Library
 Author: Splight Dev
 Author-email: dev@splight-ae.com
 Requires-Python: >=3.8.1,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

