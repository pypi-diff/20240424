# Comparing `tmp/fedn-0.9.0b2.tar.gz` & `tmp/fedn-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedn-0.9.0b2.tar", last modified: Mon Apr 15 12:06:13 2024, max compression
+gzip compressed data, was "fedn-0.9.1.tar", last modified: Wed Apr 24 08:21:12 2024, max compression
```

## Comparing `fedn-0.9.0b2.tar` & `fedn-0.9.1.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      571 2024-04-15 12:06:13.729063 fedn-0.9.0b2/PKG-INFO
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        5 2024-01-29 16:01:38.000000 fedn-0.9.0b2/README.md
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/cli/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       80 2024-01-29 16:01:38.000000 fedn-0.9.0b2/cli/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      262 2024-01-29 16:01:38.000000 fedn-0.9.0b2/cli/main.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     8980 2024-04-15 08:28:35.000000 fedn-0.9.0b2/cli/run_cmd.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/cli/tests/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.9.0b2/cli/tests/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2294 2024-01-29 16:01:38.000000 fedn-0.9.0b2/cli/tests/tests.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      453 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/common/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/common/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/common/certificate/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/common/certificate/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3140 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/common/certificate/certificate.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2131 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/common/certificate/certificatemanager.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3499 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/common/config.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       95 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/common/exceptions.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3421 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/common/log_config.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/common/net/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/common/net/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      260 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/api/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      130 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/api/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2338 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/auth.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    24093 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/client.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    38027 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/interface.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5115 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/network.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    19873 2024-04-15 12:05:57.000000 fedn-0.9.0b2/fedn/network/api/server.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    14651 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/api/tests.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/api/v1/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      614 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/v1/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    11190 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/v1/client_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    10343 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/v1/combiner_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    18235 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/v1/model_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    13598 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/v1/package_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     9335 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/v1/round_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     9284 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/v1/session_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2131 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/v1/shared.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    12614 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/v1/status_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    13391 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/api/v1/validation_routes.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/clients/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      445 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/clients/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    33231 2024-04-15 09:34:49.000000 fedn-0.9.0b2/fedn/network/clients/client.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5827 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/clients/connect.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5967 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/clients/package.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      633 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/clients/state.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1564 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/clients/test_client.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/combiner/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      147 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/combiner/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/combiner/aggregators/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      250 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/combiner/aggregators/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5323 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/combiner/aggregators/aggregator.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6744 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/combiner/aggregators/aggregatorbase.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4353 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/combiner/aggregators/fedavg.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5905 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/combiner/aggregators/fedopt.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    26190 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/combiner/combiner.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/combiner/combiner_tests.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4694 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/combiner/connect.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    10314 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/combiner/interfaces.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     7239 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/combiner/modelservice.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    14861 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/combiner/roundhandler.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      348 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/config.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/controller/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      216 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/controller/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    14347 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/controller/control.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    11363 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/controller/controlbase.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/grpc/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       40 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/grpc/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3564 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/grpc/auth.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    10980 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/grpc/fedn_pb2.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    32182 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/grpc/fedn_pb2_grpc.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2260 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/grpc/server.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/loadbalancer/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       96 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/loadbalancer/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      591 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/loadbalancer/firstavailable.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1343 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/loadbalancer/leastpacked.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      421 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/loadbalancer/loadbalancerbase.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1153 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/state.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/storage/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       95 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/storage/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/storage/models/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      322 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/storage/models/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1151 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/storage/models/memorymodelstorage.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1634 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/storage/models/modelstorage.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3220 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/models/tempmodelstorage.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/storage/s3/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      302 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/storage/s3/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1292 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/storage/s3/base.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3897 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/s3/miniorepository.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3943 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/s3/repository.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/storage/statestore/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       81 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/storage/statestore/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    30398 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/mongostatestore.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1041 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/network/storage/statestore/statestorebase.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/network/storage/statestore/stores/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/stores/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3337 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/stores/client_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4286 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/stores/combiner_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     7032 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/stores/model_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5190 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/stores/package_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3054 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/stores/round_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3552 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/stores/session_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      174 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/stores/shared.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3732 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/stores/status_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2576 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/stores/store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3792 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/network/storage/statestore/stores/validation_store.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/utils/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      442 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/utils/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      442 2024-01-29 16:01:38.000000 fedn-0.9.0b2/fedn/utils/checksum.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     9331 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/utils/dispatcher.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4067 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/utils/environment.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/utils/flowercompat/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       42 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/utils/flowercompat/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4767 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/utils/flowercompat/client_app_adapter.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/utils/helpers/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      158 2024-02-09 14:41:02.000000 fedn-0.9.0b2/fedn/utils/helpers/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1407 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/utils/helpers/helperbase.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1132 2024-02-09 14:41:02.000000 fedn-0.9.0b2/fedn/utils/helpers/helpers.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn/utils/helpers/plugins/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-02-09 14:41:02.000000 fedn-0.9.0b2/fedn/utils/helpers/plugins/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3377 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/utils/helpers/plugins/androidhelper.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4640 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/utils/helpers/plugins/numpyhelper.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    15799 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/utils/plots.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6033 2024-04-15 08:28:35.000000 fedn-0.9.0b2/fedn/utils/process.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-04-15 12:06:13.729063 fedn-0.9.0b2/fedn.egg-info/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      571 2024-04-15 12:06:13.000000 fedn-0.9.0b2/fedn.egg-info/PKG-INFO
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3841 2024-04-15 12:06:13.000000 fedn-0.9.0b2/fedn.egg-info/SOURCES.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2024-04-15 12:06:13.000000 fedn-0.9.0b2/fedn.egg-info/dependency_links.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       35 2024-04-15 12:06:13.000000 fedn-0.9.0b2/fedn.egg-info/entry_points.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2024-01-29 16:02:31.000000 fedn-0.9.0b2/fedn.egg-info/not-zip-safe
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      233 2024-04-15 12:06:13.000000 fedn-0.9.0b2/fedn.egg-info/requires.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        9 2024-04-15 12:06:13.000000 fedn-0.9.0b2/fedn.egg-info/top_level.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       38 2024-04-15 12:06:13.729063 fedn-0.9.0b2/setup.cfg
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1292 2024-04-15 12:06:06.000000 fedn-0.9.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:12.000311 fedn-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-24 08:21:12.000311 fedn-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 08:21:00.000000 fedn-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:11.980311 fedn-0.9.1/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 08:21:00.000000 fedn-0.9.1/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-24 08:21:00.000000 fedn-0.9.1/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-04-24 08:21:00.000000 fedn-0.9.1/cli/run_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:11.980311 fedn-0.9.1/cli/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:00.000000 fedn-0.9.1/cli/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-24 08:21:00.000000 fedn-0.9.1/cli/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:11.980311 fedn-0.9.1/fedn/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:11.984311 fedn-0.9.1/fedn/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:11.984311 fedn-0.9.1/fedn/common/certificate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/common/certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/common/certificate/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/common/certificate/certificatemanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/common/log_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:11.984311 fedn-0.9.1/fedn/common/net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/common/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:11.984311 fedn-0.9.1/fedn/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:11.988311 fedn-0.9.1/fedn/network/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24102 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38027 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/api/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/api/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19873 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/api/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14651 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/api/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:11.988311 fedn-0.9.1/fedn/network/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/api/v1/client_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10343 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/api/v1/combiner_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18235 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/api/v1/model_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13598 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/api/v1/package_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/api/v1/round_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/api/v1/session_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/api/v1/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/api/v1/status_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13391 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/api/v1/validation_routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:11.988311 fedn-0.9.1/fedn/network/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33231 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/clients/connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/clients/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/clients/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/clients/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:11.992311 fedn-0.9.1/fedn/network/combiner/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/combiner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:11.992311 fedn-0.9.1/fedn/network/combiner/aggregators/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/combiner/aggregators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/combiner/aggregators/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/combiner/aggregators/aggregatorbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/combiner/aggregators/fedavg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/combiner/aggregators/fedopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26190 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/combiner/combiner.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/combiner/combiner_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/combiner/connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/combiner/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/combiner/modelservice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14861 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/combiner/roundhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:11.992311 fedn-0.9.1/fedn/network/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14347 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/controller/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11363 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/controller/controlbase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:11.992311 fedn-0.9.1/fedn/network/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/grpc/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10980 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/grpc/fedn_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32182 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/grpc/fedn_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/grpc/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:11.992311 fedn-0.9.1/fedn/network/loadbalancer/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/loadbalancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/loadbalancer/firstavailable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/loadbalancer/leastpacked.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/loadbalancer/loadbalancerbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:11.992311 fedn-0.9.1/fedn/network/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:11.996311 fedn-0.9.1/fedn/network/storage/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/storage/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/storage/models/memorymodelstorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/storage/models/modelstorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/storage/models/tempmodelstorage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:11.996311 fedn-0.9.1/fedn/network/storage/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/storage/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/storage/s3/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/storage/s3/miniorepository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/storage/s3/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:11.996311 fedn-0.9.1/fedn/network/storage/statestore/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/storage/statestore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30398 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/storage/statestore/mongostatestore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/storage/statestore/statestorebase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:11.996311 fedn-0.9.1/fedn/network/storage/statestore/stores/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/storage/statestore/stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/storage/statestore/stores/client_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/storage/statestore/stores/combiner_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/storage/statestore/stores/model_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/storage/statestore/stores/package_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/storage/statestore/stores/round_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/storage/statestore/stores/session_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/storage/statestore/stores/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/storage/statestore/stores/status_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/storage/statestore/stores/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/network/storage/statestore/stores/validation_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:12.000311 fedn-0.9.1/fedn/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/utils/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/utils/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:12.000311 fedn-0.9.1/fedn/utils/flowercompat/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/utils/flowercompat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/utils/flowercompat/client_app_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:12.000311 fedn-0.9.1/fedn/utils/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/utils/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/utils/helpers/helperbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/utils/helpers/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:12.000311 fedn-0.9.1/fedn/utils/helpers/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/utils/helpers/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/utils/helpers/plugins/androidhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/utils/helpers/plugins/numpyhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15799 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/utils/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-04-24 08:21:00.000000 fedn-0.9.1/fedn/utils/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:21:12.000311 fedn-0.9.1/fedn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-24 08:21:11.000000 fedn-0.9.1/fedn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-24 08:21:11.000000 fedn-0.9.1/fedn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:21:11.000000 fedn-0.9.1/fedn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-24 08:21:11.000000 fedn-0.9.1/fedn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:21:11.000000 fedn-0.9.1/fedn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-24 08:21:11.000000 fedn-0.9.1/fedn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 08:21:11.000000 fedn-0.9.1/fedn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 08:21:12.000311 fedn-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-24 08:21:00.000000 fedn-0.9.1/setup.py
```

### Comparing `fedn-0.9.0b2/cli/run_cmd.py` & `fedn-0.9.1/cli/run_cmd.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/cli/tests/tests.py` & `fedn-0.9.1/cli/tests/tests.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/common/certificate/certificate.py` & `fedn-0.9.1/fedn/common/certificate/certificate.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/common/certificate/certificatemanager.py` & `fedn-0.9.1/fedn/common/certificate/certificatemanager.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/common/config.py` & `fedn-0.9.1/fedn/common/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 SECRET_KEY = os.environ.get('FEDN_JWT_SECRET_KEY', False)
 FEDN_JWT_CUSTOM_CLAIM_KEY = os.environ.get('FEDN_JWT_CUSTOM_CLAIM_KEY', False)
 FEDN_JWT_CUSTOM_CLAIM_VALUE = os.environ.get('FEDN_JWT_CUSTOM_CLAIM_VALUE', False)
 
 FEDN_AUTH_WHITELIST_URL_PREFIX = os.environ.get('FEDN_AUTH_WHITELIST_URL_PREFIX', False)
 FEDN_JWT_ALGORITHM = os.environ.get('FEDN_JWT_ALGORITHM', 'HS256')
-FEDN_AUTH_SCHEME = os.environ.get('FEDN_AUTH_SCHEME', 'Token')
+FEDN_AUTH_SCHEME = os.environ.get('FEDN_AUTH_SCHEME', 'Bearer')
 FEDN_AUTH_REFRESH_TOKEN_URI = os.environ.get('FEDN_AUTH_REFRESH_TOKEN_URI', False)
 FEDN_AUTH_REFRESH_TOKEN = os.environ.get('FEDN_AUTH_REFRESH_TOKEN', False)
 FEDN_CUSTOM_URL_PREFIX = os.environ.get('FEDN_CUSTOM_URL_PREFIX', '')
 
 FEDN_PACKAGE_EXTRACT_DIR = os.environ.get('FEDN_PACKAGE_EXTRACT_DIR', '')
```

### Comparing `fedn-0.9.0b2/fedn/common/log_config.py` & `fedn-0.9.1/fedn/common/log_config.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/api/auth.py` & `fedn-0.9.1/fedn/network/api/auth.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/api/client.py` & `fedn-0.9.1/fedn/network/api/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
             _params['combiner'] = combiner_id
 
         _headers = self.headers.copy()
 
         if n_max:
             _headers['X-Limit'] = str(n_max)
 
-        response = requests.get(self._get_url_api_v1('clients'), params=_params, verify=self.verify, headers=_headers)
+        response = requests.get(self._get_url_api_v1('clients/'), params=_params, verify=self.verify, headers=_headers)
 
         _json = response.json()
 
         return _json
 
     # --- Combiners --- #
 
@@ -164,15 +164,15 @@
         :rtype: dict
         """
         _headers = self.headers.copy()
 
         if n_max:
             _headers['X-Limit'] = str(n_max)
 
-        response = requests.get(self._get_url_api_v1('combiners'), verify=self.verify, headers=_headers)
+        response = requests.get(self._get_url_api_v1('combiners/'), verify=self.verify, headers=_headers)
 
         _json = response.json()
 
         return _json
 
     def get_combiners_count(self):
         """ Get the number of combiners in the statestore.
@@ -232,15 +232,15 @@
             _params['session_id'] = session_id
 
         _headers = self.headers.copy()
 
         if n_max:
             _headers['X-Limit'] = str(n_max)
 
-        response = requests.get(self._get_url_api_v1('models'), params=_params, verify=self.verify, headers=_headers)
+        response = requests.get(self._get_url_api_v1('models/'), params=_params, verify=self.verify, headers=_headers)
 
         _json = response.json()
 
         return _json
 
     def get_models_count(self):
         """ Get the number of models in the statestore.
@@ -259,15 +259,15 @@
 
         :return: The latest model.
         :rtype: dict
         """
         _headers = self.headers.copy()
         _headers['X-Limit'] = "1"
 
-        response = requests.get(self._get_url_api_v1('models'), verify=self.verify, headers=_headers)
+        response = requests.get(self._get_url_api_v1('models/'), verify=self.verify, headers=_headers)
         _json = response.json()
 
         if "result" in _json and len(_json["result"]) > 0:
             return _json["result"][0]
 
         return _json
 
@@ -358,15 +358,15 @@
         :rtype: dict
         """
         _headers = self.headers.copy()
 
         if n_max:
             _headers['X-Limit'] = str(n_max)
 
-        response = requests.get(self._get_url_api_v1('packages'), verify=self.verify, headers=_headers)
+        response = requests.get(self._get_url_api_v1('packages/'), verify=self.verify, headers=_headers)
 
         _json = response.json()
 
         return _json
 
     def get_packages_count(self):
         """ Get the number of compute packages in the statestore.
@@ -463,15 +463,15 @@
         :rtype: dict
         """
         _headers = self.headers.copy()
 
         if n_max:
             _headers['X-Limit'] = str(n_max)
 
-        response = requests.get(self._get_url_api_v1('rounds'), verify=self.verify, headers=_headers)
+        response = requests.get(self._get_url_api_v1('rounds/'), verify=self.verify, headers=_headers)
 
         _json = response.json()
 
         return _json
 
     def get_rounds_count(self):
         """ Get the number of rounds in the statestore.
@@ -511,15 +511,15 @@
         :rtype: dict
         """
         _headers = self.headers.copy()
 
         if n_max:
             _headers['X-Limit'] = str(n_max)
 
-        response = requests.get(self._get_url_api_v1('sessions'), verify=self.verify, headers=_headers)
+        response = requests.get(self._get_url_api_v1('sessions/'), verify=self.verify, headers=_headers)
 
         _json = response.json()
 
         return _json
 
     def get_sessions_count(self):
         """ Get the number of sessions in the statestore.
@@ -661,15 +661,15 @@
             _params["sender.role"] = sender_role
 
         _headers = self.headers.copy()
 
         if n_max:
             _headers['X-Limit'] = str(n_max)
 
-        response = requests.get(self._get_url_api_v1('statuses'), params=_params, verify=self.verify, headers=_headers)
+        response = requests.get(self._get_url_api_v1('statuses/'), params=_params, verify=self.verify, headers=_headers)
 
         _json = response.json()
 
         return _json
 
     def get_statuses_count(self):
         """ Get the number of statuses in the statestore.
@@ -755,15 +755,15 @@
             _params["receiver.role"] = receiver_role
 
         _headers = self.headers.copy()
 
         if n_max:
             _headers['X-Limit'] = str(n_max)
 
-        response = requests.get(self._get_url_api_v1('validations'), params=_params, verify=self.verify, headers=_headers)
+        response = requests.get(self._get_url_api_v1('validations/'), params=_params, verify=self.verify, headers=_headers)
 
         _json = response.json()
 
         return _json
 
     def get_validations_count(self):
         """ Get the number of validations in the statestore.
```

### Comparing `fedn-0.9.0b2/fedn/network/api/interface.py` & `fedn-0.9.1/fedn/network/api/interface.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/api/network.py` & `fedn-0.9.1/fedn/network/api/network.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/api/server.py` & `fedn-0.9.1/fedn/network/api/server.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/api/tests.py` & `fedn-0.9.1/fedn/network/api/tests.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/api/v1/__init__.py` & `fedn-0.9.1/fedn/network/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/api/v1/client_routes.py` & `fedn-0.9.1/fedn/network/api/v1/client_routes.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/api/v1/combiner_routes.py` & `fedn-0.9.1/fedn/network/api/v1/combiner_routes.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/api/v1/model_routes.py` & `fedn-0.9.1/fedn/network/api/v1/model_routes.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/api/v1/package_routes.py` & `fedn-0.9.1/fedn/network/api/v1/package_routes.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/api/v1/round_routes.py` & `fedn-0.9.1/fedn/network/api/v1/round_routes.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/api/v1/session_routes.py` & `fedn-0.9.1/fedn/network/api/v1/session_routes.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/api/v1/shared.py` & `fedn-0.9.1/fedn/network/api/v1/shared.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/api/v1/status_routes.py` & `fedn-0.9.1/fedn/network/api/v1/status_routes.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/api/v1/validation_routes.py` & `fedn-0.9.1/fedn/network/api/v1/validation_routes.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/clients/client.py` & `fedn-0.9.1/fedn/network/clients/client.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/clients/connect.py` & `fedn-0.9.1/fedn/network/clients/connect.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/clients/package.py` & `fedn-0.9.1/fedn/network/clients/package.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/clients/state.py` & `fedn-0.9.1/fedn/network/clients/state.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/clients/test_client.py` & `fedn-0.9.1/fedn/network/clients/test_client.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/combiner/aggregators/aggregator.py` & `fedn-0.9.1/fedn/network/combiner/aggregators/aggregator.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/combiner/aggregators/aggregatorbase.py` & `fedn-0.9.1/fedn/network/combiner/aggregators/aggregatorbase.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/combiner/aggregators/fedavg.py` & `fedn-0.9.1/fedn/network/combiner/aggregators/fedavg.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/combiner/aggregators/fedopt.py` & `fedn-0.9.1/fedn/network/combiner/aggregators/fedopt.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/combiner/combiner.py` & `fedn-0.9.1/fedn/network/combiner/combiner.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/combiner/connect.py` & `fedn-0.9.1/fedn/network/combiner/connect.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/combiner/interfaces.py` & `fedn-0.9.1/fedn/network/combiner/interfaces.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/combiner/modelservice.py` & `fedn-0.9.1/fedn/network/combiner/modelservice.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/combiner/roundhandler.py` & `fedn-0.9.1/fedn/network/combiner/roundhandler.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/controller/control.py` & `fedn-0.9.1/fedn/network/controller/control.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/controller/controlbase.py` & `fedn-0.9.1/fedn/network/controller/controlbase.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/grpc/auth.py` & `fedn-0.9.1/fedn/network/grpc/auth.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/grpc/fedn_pb2.py` & `fedn-0.9.1/fedn/network/grpc/fedn_pb2.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/grpc/fedn_pb2_grpc.py` & `fedn-0.9.1/fedn/network/grpc/fedn_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/grpc/server.py` & `fedn-0.9.1/fedn/network/grpc/server.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/loadbalancer/firstavailable.py` & `fedn-0.9.1/fedn/network/loadbalancer/firstavailable.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/loadbalancer/leastpacked.py` & `fedn-0.9.1/fedn/network/loadbalancer/leastpacked.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/state.py` & `fedn-0.9.1/fedn/network/state.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/storage/models/memorymodelstorage.py` & `fedn-0.9.1/fedn/network/storage/models/memorymodelstorage.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/storage/models/modelstorage.py` & `fedn-0.9.1/fedn/network/storage/models/modelstorage.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/storage/models/tempmodelstorage.py` & `fedn-0.9.1/fedn/network/storage/models/tempmodelstorage.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/storage/s3/base.py` & `fedn-0.9.1/fedn/network/storage/s3/base.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/storage/s3/miniorepository.py` & `fedn-0.9.1/fedn/network/storage/s3/miniorepository.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/storage/s3/repository.py` & `fedn-0.9.1/fedn/network/storage/s3/repository.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/storage/statestore/mongostatestore.py` & `fedn-0.9.1/fedn/network/storage/statestore/mongostatestore.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/storage/statestore/statestorebase.py` & `fedn-0.9.1/fedn/network/storage/statestore/statestorebase.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/storage/statestore/stores/client_store.py` & `fedn-0.9.1/fedn/network/storage/statestore/stores/client_store.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/storage/statestore/stores/combiner_store.py` & `fedn-0.9.1/fedn/network/storage/statestore/stores/combiner_store.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/storage/statestore/stores/model_store.py` & `fedn-0.9.1/fedn/network/storage/statestore/stores/model_store.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/storage/statestore/stores/package_store.py` & `fedn-0.9.1/fedn/network/storage/statestore/stores/package_store.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/storage/statestore/stores/round_store.py` & `fedn-0.9.1/fedn/network/storage/statestore/stores/round_store.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/storage/statestore/stores/session_store.py` & `fedn-0.9.1/fedn/network/storage/statestore/stores/session_store.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/storage/statestore/stores/status_store.py` & `fedn-0.9.1/fedn/network/storage/statestore/stores/status_store.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/storage/statestore/stores/store.py` & `fedn-0.9.1/fedn/network/storage/statestore/stores/store.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/network/storage/statestore/stores/validation_store.py` & `fedn-0.9.1/fedn/network/storage/statestore/stores/validation_store.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/utils/dispatcher.py` & `fedn-0.9.1/fedn/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/utils/environment.py` & `fedn-0.9.1/fedn/utils/environment.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/utils/flowercompat/client_app_adapter.py` & `fedn-0.9.1/fedn/utils/flowercompat/client_app_adapter.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/utils/helpers/helperbase.py` & `fedn-0.9.1/fedn/utils/helpers/helperbase.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/utils/helpers/helpers.py` & `fedn-0.9.1/fedn/utils/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/utils/helpers/plugins/androidhelper.py` & `fedn-0.9.1/fedn/utils/helpers/plugins/androidhelper.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/utils/helpers/plugins/numpyhelper.py` & `fedn-0.9.1/fedn/utils/helpers/plugins/numpyhelper.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/utils/plots.py` & `fedn-0.9.1/fedn/utils/plots.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn/utils/process.py` & `fedn-0.9.1/fedn/utils/process.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/fedn.egg-info/SOURCES.txt` & `fedn-0.9.1/fedn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fedn-0.9.0b2/setup.py` & `fedn-0.9.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from setuptools import find_packages, setup
 
 setup(
     name='fedn',
-    version='0.9.0b2',
+    version='0.9.1',
     description="""Scaleout Federated Learning""",
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     author='Scaleout Systems AB',
     author_email='contact@scaleoutsystems.com',
     url='https://www.scaleoutsystems.com',
     py_modules=['fedn'],
     python_requires='>=3.8,<3.12',
     install_requires=[
         "requests",
```

