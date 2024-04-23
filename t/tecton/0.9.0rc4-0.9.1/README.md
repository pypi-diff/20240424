# Comparing `tmp/tecton-0.9.0rc4.tar.gz` & `tmp/tecton-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tecton-0.9.0rc4.tar", last modified: Wed Apr  3 21:27:01 2024, max compression
+gzip compressed data, was "tecton-0.9.1.tar", last modified: Tue Apr 23 21:39:15 2024, max compression
```

## Comparing `tecton-0.9.0rc4.tar` & `tecton-0.9.1.tar`

### file list

```diff
@@ -1,670 +1,671 @@
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.425795 tecton-0.9.0rc4/
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)      206 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/MANIFEST.in
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3955 2024-04-03 21:27:01.425795 tecton-0.9.0rc4/PKG-INFO
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     3143 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/README.md
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.289783 tecton-0.9.0rc4/protoc_gen_openapiv2/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/protoc_gen_openapiv2/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.289783 tecton-0.9.0rc4/protoc_gen_openapiv2/options/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/protoc_gen_openapiv2/options/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2693 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/protoc_gen_openapiv2/options/annotations_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18717 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/protoc_gen_openapiv2/options/openapiv2_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       38 2024-04-03 21:27:01.425795 tecton-0.9.0rc4/setup.cfg
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     2503 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/setup.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.293783 tecton-0.9.0rc4/tecton/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6026 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton/_gen_version.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.301784 tecton-0.9.0rc4/tecton/_internals/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10733 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/analytics.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2279 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/athena_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1168 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/data_frame_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6558 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/delete_keys_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8122 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/display.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      930 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/env_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28683 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/errors.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      881 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/find_spark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3193 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/ingest_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2359 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/ingestion.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12345 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/materialization_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/metadata_service.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.301784 tecton-0.9.0rc4/tecton/_internals/metadata_service_impl/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton/_internals/metadata_service_impl/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      492 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/metadata_service_impl/auth_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1870 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/metadata_service_impl/request_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      615 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/metadata_service_impl/service_modules.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5408 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/mock_source_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1357 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/offline_store_credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1037 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/pandas_compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16160 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/query_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21292 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/querytree_api.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.301784 tecton-0.9.0rc4/tecton/_internals/repo/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton/_internals/repo/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11416 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/repo/function_serialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12059 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16172 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/run_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13055 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/sdk_decorators.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2059 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/secret_resolver.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7119 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/snowflake_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7034 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/spark_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2823 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/spark_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5615 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/tecton_pydantic.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7071 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/time_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3769 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/type_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14505 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4985 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_internals/validations_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      322 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/_stamp.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3067 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/aggregation_functions.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.305784 tecton-0.9.0rc4/tecton/cli/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    26054 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/access_control.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1583 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/api_key.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3083 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/auth.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5469 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/cli.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8462 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/cli_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5967 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/command.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2027 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/completion.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18539 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/engine.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1323 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/engine_renderer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    34388 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/environment.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7938 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/environment_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7691 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/error_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3759 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      515 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/pex_wrapper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1786 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/printer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5135 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/repo.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9759 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/repo_config.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7739 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/repo_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5010 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/secrets.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5824 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/service_account.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5620 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/test.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2403 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/user.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4917 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/workspace.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2711 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/cli/workspace_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2450 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/fco_listers.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.309785 tecton-0.9.0rc4/tecton/framework/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6920 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/base_tecton_object.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   119708 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/configs.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28984 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/data_frame.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    38553 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/data_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13976 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/dataset.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7683 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/entity.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    42636 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/feature_service.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   225796 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/feature_view.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3854 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/filtered_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4922 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/repo_config.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21258 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/transformation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2071 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2091 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/validation_mode.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22520 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/framework/workspace.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.309785 tecton-0.9.0rc4/tecton/identities/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/identities/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1521 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/identities/api_keys.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14640 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/identities/credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12333 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/identities/okta.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2374 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/pytest_tecton.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      381 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/run_api_consts.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      709 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/snowflake_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2747 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/tecton_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6326 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/types.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.309785 tecton-0.9.0rc4/tecton/vendor/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton/vendor/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.309785 tecton-0.9.0rc4/tecton/vendor/dill/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton/vendor/dill/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.313785 tecton-0.9.0rc4/tecton/vendor/dill/dill/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7211 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/dill/dill/__diff.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3634 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/dill/dill/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    54753 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/dill/dill/_dill.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20428 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/dill/dill/_objects.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11822 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/dill/dill/detect.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7444 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/dill/dill/info.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      755 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/dill/dill/objtypes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4467 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/dill/dill/pointers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      719 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/dill/dill/settings.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    44906 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/dill/dill/source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8238 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/dill/dill/temp.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.313785 tecton-0.9.0rc4/tecton/vendor/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.313785 tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      111 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    26941 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/clientserver.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2329 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4306 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/finalizer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18289 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/java_collections.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    96550 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/java_gateway.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14805 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/protocol.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4361 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/signals.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       23 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/version.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.321786 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4777 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2282 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/_globals.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9940 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/accumulators.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7386 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/broadcast.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.321786 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/cloudpickle/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      201 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/cloudpickle/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    30084 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29668 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      354 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/cloudpickle/compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7831 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    54613 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7619 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/daemon.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1891 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/files.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3969 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/find_spark_home.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6654 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/install.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10025 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/java_gateway.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3994 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/join.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.325786 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1530 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10846 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/base.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   126616 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/classification.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    62498 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/clustering.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4294 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    34149 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/evaluation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   212823 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/feature.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17053 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/fpm.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4603 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8092 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/image.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.325786 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/linalg/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    39791 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.325786 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/param/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18532 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/param/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9556 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22295 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/param/shared.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13656 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/pipeline.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23213 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/recommendation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    91533 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/regression.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18317 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/stat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13108 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    57402 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/tuning.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22016 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15371 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/wrapper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.329786 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28695 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/classification.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    39889 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/clustering.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4976 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20443 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/evaluation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28134 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/feature.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7028 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/fpm.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.329786 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/linalg/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    46744 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    57731 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    19517 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/random.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12101 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/recommendation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    32842 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/regression.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.329786 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/stat/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1969 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1309 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14081 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1289 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2301 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/stat/test.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    25342 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21149 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5755 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/profiler.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.333787 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/python/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/python/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.333787 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/python/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/python/pyspark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   109373 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/rdd.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4250 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/rddsampler.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.333787 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/resource/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1317 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/resource/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1590 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/resource/information.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7097 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/resource/profile.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10946 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/resource/requests.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1224 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/resultiterable.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20586 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/serializers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/shell.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27959 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/shuffle.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.337787 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2590 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.337787 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/avro/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      809 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5993 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/avro/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12110 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/catalog.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29664 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/column.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2999 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23884 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    99829 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/dataframe.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   157099 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10681 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/group.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.341787 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      959 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21163 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28130 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14683 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3806 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12308 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6324 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13225 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2745 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    77056 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/readwriter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    31188 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/session.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    69121 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/streaming.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    55203 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20068 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/udf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6976 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12863 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/window.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5149 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/statcounter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3756 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/status.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2785 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/storagelevel.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.341787 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1007 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16448 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27879 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/dstream.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5436 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/kinesis.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2333 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/listener.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5614 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9189 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/taskcontext.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2679 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/traceback_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11623 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/version.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27875 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/worker.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1334 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/vendor_dill.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/vendor/vendor_pyspark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1154 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton/version.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.293783 tecton-0.9.0rc4/tecton.egg-info/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3955 2024-04-03 21:26:58.000000 tecton-0.9.0rc4/tecton.egg-info/PKG-INFO
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22872 2024-04-03 21:26:59.000000 tecton-0.9.0rc4/tecton.egg-info/SOURCES.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        1 2024-04-03 21:26:58.000000 tecton-0.9.0rc4/tecton.egg-info/dependency_links.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       96 2024-04-03 21:26:59.000000 tecton-0.9.0rc4/tecton.egg-info/entry_points.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1044 2024-04-03 21:26:59.000000 tecton-0.9.0rc4/tecton.egg-info/requires.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      120 2024-04-03 21:26:59.000000 tecton-0.9.0rc4/tecton.egg-info/top_level.txt
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.341787 tecton-0.9.0rc4/tecton_athena/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14977 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/athena_session.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8797 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/data_catalog_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5764 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/odfv_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.341787 tecton-0.9.0rc4/tecton_athena/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2381 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/query/translate.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17721 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/sql_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.345788 tecton-0.9.0rc4/tecton_athena/templates/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/templates/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/templates/create_table.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      267 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/templates/data_source.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9544 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/templates/historical_features.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      672 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/templates/materialization_tile.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3975 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/templates/run_full_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      503 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/templates/run_partial_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1046 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/templates/time_limit.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      277 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/templates/transformation_pipeline.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      656 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_athena/templates_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.349788 tecton-0.9.0rc4/tecton_core/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/_gen_version.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13149 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/aggregation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1598 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/arrow.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/aws_credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3464 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/compute_mode.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    24781 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7234 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/data_types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3520 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/duckdb_context.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.349788 tecton-0.9.0rc4/tecton_core/embeddings/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_core/embeddings/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/embeddings/config.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7404 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/errors.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5113 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/fco_container.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27252 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/feature_definition_wrapper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9838 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/feature_set_config.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      749 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/feature_view_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/filter_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2507 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/function_deserialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      739 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/http.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      616 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/id_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      546 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/iterators.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7440 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/materialization_context.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.353788 tecton-0.9.0rc4/tecton_core/metadata_service_impl/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_core/metadata_service_impl/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      195 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/metadata_service_impl/base_stub.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2665 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/metadata_service_impl/error_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3488 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/metadata_service_impl/http_client.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      901 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/metadata_service_impl/providers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1990 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/metadata_service_impl/response.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2273 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/metadata_service_impl/service_calls.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      206 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/metadata_service_impl/trace.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20281 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/offline_store.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1427 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/online_serving_index.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7383 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/pipeline_common.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.357789 tecton-0.9.0rc4/tecton_core/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_core/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22026 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/aggregation_plans.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    56201 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/builder.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5286 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/compaction_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      179 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/dialect.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.357789 tecton-0.9.0rc4/tecton_core/query/duckdb/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_core/query/duckdb/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10669 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/duckdb/compute.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7820 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/duckdb/nodes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      714 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/duckdb/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1526 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/errors.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      746 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/executor_params.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1735 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/executor_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10749 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/node_interface.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7303 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/node_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   126328 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/nodes.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.361789 tecton-0.9.0rc4/tecton_core/query/pandas/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_core/query/pandas/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3556 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/pandas/compute.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4033 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/pandas/node.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22035 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/pandas/nodes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6169 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/pandas/pipeline_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5054 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/pandas/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      192 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/pandas/sql.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1948 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/pandas/translate.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5944 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/pipeline_sql_builder.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      786 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/prefixed_uri_resolver.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4204 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/query_tree_compute.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21774 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/query_tree_executor.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      227 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/rewrite.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.361789 tecton-0.9.0rc4/tecton_core/query/snowflake/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_core/query/snowflake/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12630 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/snowflake/compute.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20202 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query/sql_compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3294 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/query_consts.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5280 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/repo_file_handler.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      867 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/request_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3149 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/schema.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11989 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/schema_derivation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5597 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/schema_validation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1063 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/secrets.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2126 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/snowflake_context.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.361789 tecton-0.9.0rc4/tecton_core/specs/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      777 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/specs/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    44686 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/specs/data_source_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1457 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/specs/entity_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5460 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/specs/feature_service_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    43502 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/specs/feature_view_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4440 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/specs/tecton_object_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9179 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/specs/time_window_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2440 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/specs/transformation_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4952 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/specs/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9725 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/time_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.361789 tecton-0.9.0rc4/tecton_core/vendor/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_core/vendor/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9361 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/vendor/queue.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.365790 tecton-0.9.0rc4/tecton_core/vendor/treelib/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1594 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/vendor/treelib/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      943 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/vendor/treelib/exceptions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1575 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/vendor/treelib/misc.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9595 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/vendor/treelib/node.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1265 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/vendor/treelib/plugins.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    37469 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/vendor/treelib/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1275 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_core/vendor/vendor_treelib.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.369790 tecton-0.9.0rc4/tecton_materialization/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      718 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23171 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/batch_materialization.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.369790 tecton-0.9.0rc4/tecton_materialization/common/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_materialization/common/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2835 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/common/job_metadata.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5803 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/common/job_metadata_aws.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2222 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/common/job_metadata_gcp.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2693 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/common/task_params.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4811 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/consumption.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1070 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/delta_maintenance.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3731 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/entity_deletion.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5200 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/feature_export.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5090 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/ingest_materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7159 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/job_metadata.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9316 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7780 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/materialization_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.373790 tecton-0.9.0rc4/tecton_materialization/ray/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_materialization/ray/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5242 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/ray/batch_materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23853 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/ray/delta.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5973 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/ray/feature_export.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5009 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/ray/ingest_materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6869 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/ray/job_status.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10181 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/ray/materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4190 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/ray/materialization_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3172 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/ray/nodes.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.373790 tecton-0.9.0rc4/tecton_materialization/remote_host/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/remote_host/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20100 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/remote_host/pyspark_remote_host.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1996 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/secrets.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6666 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_materialization/stream_materialization.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.373790 tecton-0.9.0rc4/tecton_proto/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.373790 tecton-0.9.0rc4/tecton_proto/amplitude/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/amplitude/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4642 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/amplitude/amplitude_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3093 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/amplitude/client_logging_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.373790 tecton-0.9.0rc4/tecton_proto/api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/api/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.373790 tecton-0.9.0rc4/tecton_proto/api/featureservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/api/featureservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    81835 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/api/featureservice/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9573 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/api/featureservice/feature_service_request_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.377791 tecton-0.9.0rc4/tecton_proto/args/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/args/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2864 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/basic_info_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1897 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/data_source_config_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21470 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3996 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/diff_options_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6990 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/diff_test_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3059 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/entity_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2415 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/fco_args_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5172 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    41821 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/feature_view_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6092 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/pipeline_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1694 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/repo_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4704 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/transformation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1637 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/user_defined_function_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1893 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/version_constraints_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8163 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/args/virtual_data_source_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.381791 tecton-0.9.0rc4/tecton_proto/auditlog/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/auditlog/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2716 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/auditlog/metadata_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.381791 tecton-0.9.0rc4/tecton_proto/auth/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/auth/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1422 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/auth/acl_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29023 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/auth/authorization_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3224 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/auth/principal_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6551 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/auth/resource_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3058 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/auth/resource_role_assignments_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3058 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/auth/service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.381791 tecton-0.9.0rc4/tecton_proto/canary/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/canary/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1208 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/canary/type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2195 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/canary/update_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.381791 tecton-0.9.0rc4/tecton_proto/cli/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/cli/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3075 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/cli/repo_diff_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.385792 tecton-0.9.0rc4/tecton_proto/common/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/common/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3459 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/aggregation_function_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1717 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/analytics_options_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1823 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/aws_credentials_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1672 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/column_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1336 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/compute_mode_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1934 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/container_image_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1373 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/data_source_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2431 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/data_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1735 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/fco_locator_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1286 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/framework_version_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1725 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/id_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1150 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/pair_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1368 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/schema_container_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2819 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/schema_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1518 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/secret_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1381 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/spark_schema_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2183 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/common/time_window_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.385792 tecton-0.9.0rc4/tecton_proto/consumption/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/consumption/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5600 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/consumption/consumption_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.393792 tecton-0.9.0rc4/tecton_proto/data/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/data/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7900 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/batch_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2313 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/entity_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2848 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/fco_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2916 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/fco_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5025 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1487 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/feature_store_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20254 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/feature_view_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2121 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/freshness_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4810 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/fv_materialization_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1366 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/hive_metastore_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1975 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/internal_spark_cluster_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1683 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/materialization_roles_allowlists_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5831 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/materialization_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1752 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/odfv_compute_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2317 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/onboarding_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2614 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/principal_group_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6827 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/remote_compute_environment_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15757 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/remote_spark_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3468 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/saved_feature_data_frame_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4545 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/serving_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10895 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/state_update_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4799 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/stream_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1828 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/summary_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2349 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/tecton_api_key_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2795 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/transformation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10456 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/user_deployment_settings_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1650 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/user_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3433 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/virtual_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2355 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/data/workspace_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.397793 tecton-0.9.0rc4/tecton_proto/databricks_api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8276 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/clusters_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1889 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/dbfs_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/error_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3593 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/execution_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1501 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/instance_profiles_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8112 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/jobs_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1912 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/libraries_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2911 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/permissions_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1253 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/scim_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2391 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/secrets_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2613 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/databricks_api/workspace_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.397793 tecton-0.9.0rc4/tecton_proto/dataobs/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/dataobs/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2490 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/dataobs/config_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2553 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/dataobs/expectation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3691 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/dataobs/metric_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5748 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/dataobs/validation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3723 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/dataobs/validation_task_params_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4629 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/dataobs/validation_task_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.397793 tecton-0.9.0rc4/tecton_proto/feature_server/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/feature_server/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.397793 tecton-0.9.0rc4/tecton_proto/feature_server/configuration/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/feature_server/configuration/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    19997 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.401793 tecton-0.9.0rc4/tecton_proto/materialization/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/materialization/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9821 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/materialization/job_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2610 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/materialization/materialization_states_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14634 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/materialization/materialization_task_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8173 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/materialization/params_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2752 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/materialization/spark_cluster_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.401793 tecton-0.9.0rc4/tecton_proto/materializationjobservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/materializationjobservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16111 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/materializationjobservice/materialization_job_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.401793 tecton-0.9.0rc4/tecton_proto/metadataservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/metadataservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2776 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/metadataservice/http_over_grpc_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   121489 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/metadataservice/metadata_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.401793 tecton-0.9.0rc4/tecton_proto/offlinestore/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/offlinestore/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.401793 tecton-0.9.0rc4/tecton_proto/offlinestore/delta/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/offlinestore/delta/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1570 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/offlinestore/delta/metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6554 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/offlinestore/delta/transaction_writer_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.405794 tecton-0.9.0rc4/tecton_proto/online_store/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/online_store/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5408 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/online_store/feature_value_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1306 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/online_store/status_entry_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.405794 tecton-0.9.0rc4/tecton_proto/online_store_writer/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/online_store_writer/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2401 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/online_store_writer/config_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5522 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/online_store_writer/copier_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.405794 tecton-0.9.0rc4/tecton_proto/remoteenvironmentservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/remoteenvironmentservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13213 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.405794 tecton-0.9.0rc4/tecton_proto/secrets/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/secrets/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10485 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/secrets/secrets_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.405794 tecton-0.9.0rc4/tecton_proto/snowflake/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/snowflake/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1246 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/snowflake/location_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1392 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/snowflake/snowflake_credentials_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.405794 tecton-0.9.0rc4/tecton_proto/spark_api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/spark_api/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1195 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/spark_api/error_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7388 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/spark_api/jobs_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.405794 tecton-0.9.0rc4/tecton_proto/spark_common/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/spark_common/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7786 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/spark_common/clusters_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2386 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/spark_common/libraries_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.409794 tecton-0.9.0rc4/tecton_proto/testhelperservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/testhelperservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3516 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/testhelperservice/test_helper_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.409794 tecton-0.9.0rc4/tecton_proto/validation/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:54.000000 tecton-0.9.0rc4/tecton_proto/validation/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4609 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_proto/validation/validator_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.409794 tecton-0.9.0rc4/tecton_snowflake/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    30085 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/pipeline_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.413794 tecton-0.9.0rc4/tecton_snowflake/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10160 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/query/aggregation_plans.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/query/dataframe_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13673 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/query/nodes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6314 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/query/queries.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      741 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/query/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3704 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/query/translate.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8392 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/schema_derivation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2246 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/snowflake_type_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    33728 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/sql_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.417795 tecton-0.9.0rc4/tecton_snowflake/templates/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1025 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/copier_macro.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      396 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/create_temp_table_for_bfv.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      363 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/create_temp_table_for_bwafv.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      255 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/data_source.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1248 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/delete_orphaned_schemas.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      698 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/delete_staged_files.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3069 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/historical_features.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7892 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/historical_features_macros.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1795 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/materialization_tile.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2575 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/materialized_feature_view.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      937 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/offline_materialization_macros.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      126 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/online_store_copier.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6777 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/run_full_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      583 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/run_partial_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      569 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/time_limit.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      213 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates/transformation_pipeline.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/templates_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      249 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_snowflake/utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.421795 tecton-0.9.0rc4/tecton_spark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      808 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    30278 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/aggregation_plans.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2263 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/data_observability.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      926 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/data_source_credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    35476 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/data_source_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      425 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/errors_spark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6470 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/feature_view_spark_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.421795 tecton-0.9.0rc4/tecton_spark/jars/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/jars/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2633 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/jars/class_loader.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)  1794322 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/jars/tecton-udfs-spark-3.jar
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7188 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/materialization_plan.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27440 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/offline_store.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15491 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/partial_aggregations.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    33278 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/pipeline_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:27:01.425795 tecton-0.9.0rc4/tecton_spark/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3356 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/query/data_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10751 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/query/filter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    37167 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/query/join.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1515 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/query/node.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7583 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/query/pipeline.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14752 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/query/projection.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10712 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/query/translate.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17887 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/schema_derivation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5434 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/schema_spark_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2317 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/spark_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1697 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/spark_schema_wrapper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4858 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/time_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      393 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/udf_jar.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3257 2024-04-03 21:26:55.000000 tecton-0.9.0rc4/tecton_spark/udfs.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.939819 tecton-0.9.1/
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)      206 2024-04-23 21:39:10.000000 tecton-0.9.1/MANIFEST.in
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3952 2024-04-23 21:39:15.939819 tecton-0.9.1/PKG-INFO
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     3143 2024-04-23 21:39:10.000000 tecton-0.9.1/README.md
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.859812 tecton-0.9.1/protoc_gen_openapiv2/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/protoc_gen_openapiv2/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.859812 tecton-0.9.1/protoc_gen_openapiv2/options/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/protoc_gen_openapiv2/options/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2693 2024-04-23 21:39:11.000000 tecton-0.9.1/protoc_gen_openapiv2/options/annotations_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18717 2024-04-23 21:39:11.000000 tecton-0.9.1/protoc_gen_openapiv2/options/openapiv2_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       38 2024-04-23 21:39:15.939819 tecton-0.9.1/setup.cfg
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     2590 2024-04-23 21:39:10.000000 tecton-0.9.1/setup.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.859812 tecton-0.9.1/tecton/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6026 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       17 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton/_gen_version.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.867813 tecton-0.9.1/tecton/_internals/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10733 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/analytics.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2279 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/athena_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1168 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/data_frame_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6558 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/delete_keys_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8122 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/display.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      930 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/env_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29109 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/errors.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      881 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/find_spark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3193 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/ingest_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2359 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/ingestion.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12345 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/materialization_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/metadata_service.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.867813 tecton-0.9.1/tecton/_internals/metadata_service_impl/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton/_internals/metadata_service_impl/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      492 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/metadata_service_impl/auth_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1870 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/metadata_service_impl/request_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      615 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/metadata_service_impl/service_modules.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5408 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/mock_source_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1357 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/offline_store_credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1037 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/pandas_compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16160 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/query_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21223 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/querytree_api.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.867813 tecton-0.9.1/tecton/_internals/repo/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton/_internals/repo/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11416 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/repo/function_serialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12059 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16298 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/run_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13055 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/sdk_decorators.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2059 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/secret_resolver.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7119 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/snowflake_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7034 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/spark_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2823 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/spark_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5615 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/tecton_pydantic.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7071 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/time_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3769 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/type_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14505 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4985 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_internals/validations_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      322 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/_stamp.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3067 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/aggregation_functions.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.871813 tecton-0.9.1/tecton/cli/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    26054 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/access_control.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1583 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/api_key.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3083 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/auth.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5469 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/cli.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8462 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/cli_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5967 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/command.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2027 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/completion.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18539 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/engine.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1323 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/engine_renderer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    32012 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/environment.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8982 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/environment_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7691 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/error_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3759 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      515 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/pex_wrapper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1786 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/printer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5135 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/repo.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9759 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/repo_config.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7739 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/repo_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5011 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/secrets.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5824 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/service_account.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5620 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/test.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2403 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/user.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4917 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/workspace.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2711 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/cli/workspace_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2450 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/fco_listers.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.875814 tecton-0.9.1/tecton/framework/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/framework/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6920 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/framework/base_tecton_object.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   119684 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/framework/configs.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28984 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/framework/data_frame.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    40690 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/framework/data_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13976 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/framework/dataset.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7683 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/framework/entity.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2641 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/framework/feature.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    42636 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/framework/feature_service.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   228559 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/framework/feature_view.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3854 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/framework/filtered_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4922 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/framework/repo_config.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21258 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/framework/transformation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2071 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/framework/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2091 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/framework/validation_mode.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22520 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/framework/workspace.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.875814 tecton-0.9.1/tecton/identities/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/identities/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1521 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/identities/api_keys.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14640 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/identities/credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12333 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/identities/okta.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2374 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/pytest_tecton.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      381 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/run_api_consts.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      709 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/snowflake_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2747 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/tecton_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6326 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/types.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.875814 tecton-0.9.1/tecton/vendor/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton/vendor/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.875814 tecton-0.9.1/tecton/vendor/dill/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton/vendor/dill/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.875814 tecton-0.9.1/tecton/vendor/dill/dill/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7211 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/dill/dill/__diff.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3634 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/dill/dill/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    54753 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/dill/dill/_dill.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20428 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/dill/dill/_objects.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11822 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/dill/dill/detect.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7444 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/dill/dill/info.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      755 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/dill/dill/objtypes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4467 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/dill/dill/pointers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      719 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/dill/dill/settings.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    44906 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/dill/dill/source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8238 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/dill/dill/temp.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.875814 tecton-0.9.1/tecton/vendor/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton/vendor/pyspark/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.879814 tecton-0.9.1/tecton/vendor/pyspark/py4j/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      111 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/py4j/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    26941 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/py4j/clientserver.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2329 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/py4j/compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4306 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/py4j/finalizer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18289 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/py4j/java_collections.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    96550 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/py4j/java_gateway.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14805 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/py4j/protocol.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4361 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/py4j/signals.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       23 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/py4j/version.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.883814 tecton-0.9.1/tecton/vendor/pyspark/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4777 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2282 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/_globals.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9940 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/accumulators.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7386 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/broadcast.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.883814 tecton-0.9.1/tecton/vendor/pyspark/pyspark/cloudpickle/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      201 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/cloudpickle/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    30084 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29668 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      354 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/cloudpickle/compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7831 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    54613 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7619 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/daemon.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1891 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/files.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3969 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/find_spark_home.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6654 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/install.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10025 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/java_gateway.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3994 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/join.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.883814 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1530 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10846 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/base.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   126616 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/classification.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    62498 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/clustering.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4294 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    34149 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/evaluation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   212823 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/feature.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17053 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/fpm.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4603 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8092 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/image.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.883814 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/linalg/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    39791 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.887815 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/param/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18532 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/param/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9556 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22295 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/param/shared.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13656 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/pipeline.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23213 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/recommendation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    91533 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/regression.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18317 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/stat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13108 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    57402 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/tuning.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22016 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15371 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/wrapper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.887815 tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28695 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/classification.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    39889 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/clustering.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4976 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20443 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/evaluation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28134 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/feature.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7028 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/fpm.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.887815 tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/linalg/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    46744 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    57731 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    19517 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/random.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12101 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/recommendation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    32842 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/regression.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.887815 tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/stat/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1969 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1309 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14081 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1289 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2301 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/stat/test.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    25342 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21149 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5755 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/profiler.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.887815 tecton-0.9.1/tecton/vendor/pyspark/pyspark/python/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/python/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.887815 tecton-0.9.1/tecton/vendor/pyspark/pyspark/python/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/python/pyspark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   109373 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/rdd.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4250 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/rddsampler.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.887815 tecton-0.9.1/tecton/vendor/pyspark/pyspark/resource/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1317 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/resource/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1590 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/resource/information.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7097 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/resource/profile.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10946 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/resource/requests.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1224 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/resultiterable.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20586 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/serializers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/shell.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27959 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/shuffle.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.891815 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2590 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.891815 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/avro/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      809 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5993 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/avro/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12110 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/catalog.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29664 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/column.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2999 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23884 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    99829 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/dataframe.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   157099 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10681 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/group.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.891815 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/pandas/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      959 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21163 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28130 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14683 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3806 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12308 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6324 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13225 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/pandas/types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2745 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    77056 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/readwriter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    31188 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/session.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    69121 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/streaming.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    55203 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20068 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/udf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6976 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12863 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/window.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5149 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/statcounter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3756 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/status.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2785 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/storagelevel.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.895815 tecton-0.9.1/tecton/vendor/pyspark/pyspark/streaming/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1007 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/streaming/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16448 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/streaming/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27879 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/streaming/dstream.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5436 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/streaming/kinesis.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2333 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/streaming/listener.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5614 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/streaming/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9189 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/taskcontext.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2679 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/traceback_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11623 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/version.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27875 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/pyspark/pyspark/worker.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1334 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/vendor_dill.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/vendor/vendor_pyspark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1154 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton/version.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.863812 tecton-0.9.1/tecton.egg-info/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3952 2024-04-23 21:39:13.000000 tecton-0.9.1/tecton.egg-info/PKG-INFO
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22900 2024-04-23 21:39:14.000000 tecton-0.9.1/tecton.egg-info/SOURCES.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        1 2024-04-23 21:39:13.000000 tecton-0.9.1/tecton.egg-info/dependency_links.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       96 2024-04-23 21:39:14.000000 tecton-0.9.1/tecton.egg-info/entry_points.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1128 2024-04-23 21:39:14.000000 tecton-0.9.1/tecton.egg-info/requires.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      120 2024-04-23 21:39:14.000000 tecton-0.9.1/tecton.egg-info/top_level.txt
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.895815 tecton-0.9.1/tecton_athena/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_athena/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14977 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_athena/athena_session.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8797 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_athena/data_catalog_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5764 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_athena/odfv_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.895815 tecton-0.9.1/tecton_athena/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_athena/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2381 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_athena/query/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17721 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_athena/sql_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.895815 tecton-0.9.1/tecton_athena/templates/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_athena/templates/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_athena/templates/create_table.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      267 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_athena/templates/data_source.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9544 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_athena/templates/historical_features.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      672 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_athena/templates/materialization_tile.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3975 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_athena/templates/run_full_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      503 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_athena/templates/run_partial_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1046 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_athena/templates/time_limit.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      277 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_athena/templates/transformation_pipeline.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      656 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_athena/templates_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.899816 tecton-0.9.1/tecton_core/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       17 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/_gen_version.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13149 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/aggregation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1598 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/arrow.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/aws_credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3464 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/compute_mode.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    24797 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7234 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/data_types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3981 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/duckdb_context.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.899816 tecton-0.9.1/tecton_core/embeddings/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_core/embeddings/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/embeddings/config.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7404 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/errors.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5113 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/fco_container.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27206 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/feature_definition_wrapper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9838 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/feature_set_config.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      749 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/feature_view_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/filter_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2507 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/function_deserialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      739 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/http.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      616 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/id_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      546 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/iterators.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7440 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/materialization_context.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.899816 tecton-0.9.1/tecton_core/metadata_service_impl/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_core/metadata_service_impl/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      195 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/metadata_service_impl/base_stub.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2665 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/metadata_service_impl/error_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3488 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/metadata_service_impl/http_client.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      901 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/metadata_service_impl/providers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1990 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/metadata_service_impl/response.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2273 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/metadata_service_impl/service_calls.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      206 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/metadata_service_impl/trace.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20281 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/offline_store.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1427 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/online_serving_index.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7383 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/pipeline_common.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.903816 tecton-0.9.1/tecton_core/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_core/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22026 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/aggregation_plans.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    56183 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/builder.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5286 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/compaction_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      179 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/dialect.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.903816 tecton-0.9.1/tecton_core/query/duckdb/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_core/query/duckdb/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10983 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/duckdb/compute.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7820 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/duckdb/nodes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      714 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/duckdb/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1526 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/errors.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      746 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/executor_params.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1735 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/executor_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10749 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/node_interface.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7303 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/node_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   126322 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/nodes.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.903816 tecton-0.9.1/tecton_core/query/pandas/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_core/query/pandas/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3556 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/pandas/compute.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4033 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/pandas/node.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22035 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/pandas/nodes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6169 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/pandas/pipeline_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5054 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/pandas/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      192 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/pandas/sql.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1948 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/pandas/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5944 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/pipeline_sql_builder.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      786 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/prefixed_uri_resolver.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4204 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/query_tree_compute.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21774 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/query_tree_executor.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      227 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/rewrite.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.903816 tecton-0.9.1/tecton_core/query/snowflake/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_core/query/snowflake/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12630 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/snowflake/compute.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20202 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query/sql_compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3294 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/query_consts.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5280 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/repo_file_handler.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      867 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/request_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3149 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/schema.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11989 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/schema_derivation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5597 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/schema_validation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1063 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/secrets.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2126 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/snowflake_context.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.907817 tecton-0.9.1/tecton_core/specs/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      777 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/specs/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    44686 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/specs/data_source_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1457 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/specs/entity_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5460 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/specs/feature_service_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    43407 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/specs/feature_view_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4440 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/specs/tecton_object_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9179 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/specs/time_window_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2440 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/specs/transformation_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4952 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/specs/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9725 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/time_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.907817 tecton-0.9.1/tecton_core/vendor/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_core/vendor/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9361 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/vendor/queue.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.907817 tecton-0.9.1/tecton_core/vendor/treelib/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1594 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/vendor/treelib/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      943 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/vendor/treelib/exceptions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1575 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/vendor/treelib/misc.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9595 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/vendor/treelib/node.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1265 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/vendor/treelib/plugins.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    37469 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/vendor/treelib/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1275 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_core/vendor/vendor_treelib.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.907817 tecton-0.9.1/tecton_materialization/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      718 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23147 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/batch_materialization.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.907817 tecton-0.9.1/tecton_materialization/common/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_materialization/common/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2835 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/common/job_metadata.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5803 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/common/job_metadata_aws.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2222 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/common/job_metadata_gcp.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2693 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/common/task_params.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4811 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/consumption.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1070 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/delta_maintenance.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3731 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/entity_deletion.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5200 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/feature_export.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5090 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/ingest_materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7159 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/job_metadata.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9316 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7780 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/materialization_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.911817 tecton-0.9.1/tecton_materialization/ray/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_materialization/ray/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5242 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/ray/batch_materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23853 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/ray/delta.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5973 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/ray/feature_export.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5009 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/ray/ingest_materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6869 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/ray/job_status.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10181 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/ray/materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4190 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/ray/materialization_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3172 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/ray/nodes.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.911817 tecton-0.9.1/tecton_materialization/remote_host/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/remote_host/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20100 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/remote_host/pyspark_remote_host.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1996 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/secrets.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6666 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_materialization/stream_materialization.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.911817 tecton-0.9.1/tecton_proto/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.911817 tecton-0.9.1/tecton_proto/amplitude/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/amplitude/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4642 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/amplitude/amplitude_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3093 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/amplitude/client_logging_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.911817 tecton-0.9.1/tecton_proto/api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/api/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.911817 tecton-0.9.1/tecton_proto/api/featureservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/api/featureservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    81835 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/api/featureservice/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9573 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/api/featureservice/feature_service_request_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.911817 tecton-0.9.1/tecton_proto/args/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/args/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2864 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/args/basic_info_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1897 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/args/data_source_config_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21470 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/args/data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3996 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/args/diff_options_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6990 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/args/diff_test_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3059 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/args/entity_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2415 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/args/fco_args_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5172 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/args/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    41778 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/args/feature_view_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6092 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/args/pipeline_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1694 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/args/repo_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4704 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/args/transformation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1637 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/args/user_defined_function_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1893 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/args/version_constraints_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8163 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/args/virtual_data_source_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.911817 tecton-0.9.1/tecton_proto/auditlog/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/auditlog/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2716 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/auditlog/metadata_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.915817 tecton-0.9.1/tecton_proto/auth/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/auth/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1422 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/auth/acl_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29023 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/auth/authorization_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3224 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/auth/principal_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6551 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/auth/resource_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3058 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/auth/resource_role_assignments_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3058 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/auth/service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.915817 tecton-0.9.1/tecton_proto/canary/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/canary/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1208 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/canary/type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2195 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/canary/update_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.915817 tecton-0.9.1/tecton_proto/cli/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/cli/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3075 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/cli/repo_diff_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.915817 tecton-0.9.1/tecton_proto/common/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/common/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3459 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/common/aggregation_function_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1717 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/common/analytics_options_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1823 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/common/aws_credentials_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1672 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/common/column_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1336 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/common/compute_mode_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1934 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/common/container_image_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1373 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/common/data_source_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2431 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/common/data_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1735 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/common/fco_locator_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1286 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/common/framework_version_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1725 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/common/id_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1150 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/common/pair_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1368 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/common/schema_container_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2819 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/common/schema_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1518 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/common/secret_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1381 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/common/spark_schema_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2183 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/common/time_window_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.915817 tecton-0.9.1/tecton_proto/consumption/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/consumption/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5600 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/consumption/consumption_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.919818 tecton-0.9.1/tecton_proto/data/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/data/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7900 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/batch_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2313 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/entity_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2848 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/fco_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2916 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/fco_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5025 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1487 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/feature_store_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20207 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/feature_view_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2121 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/freshness_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4810 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/fv_materialization_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1366 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/hive_metastore_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1975 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/internal_spark_cluster_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1683 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/materialization_roles_allowlists_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5831 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/materialization_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1752 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/odfv_compute_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2317 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/onboarding_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2614 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/principal_group_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6827 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/remote_compute_environment_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15757 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/remote_spark_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3468 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/saved_feature_data_frame_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4545 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/serving_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10895 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/state_update_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4799 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/stream_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1828 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/summary_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2349 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/tecton_api_key_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2795 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/transformation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10456 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/user_deployment_settings_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1650 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/user_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3433 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/virtual_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2355 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/data/workspace_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.923818 tecton-0.9.1/tecton_proto/databricks_api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/databricks_api/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8276 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/databricks_api/clusters_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1889 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/databricks_api/dbfs_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/databricks_api/error_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3593 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/databricks_api/execution_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1501 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/databricks_api/instance_profiles_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8112 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/databricks_api/jobs_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1912 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/databricks_api/libraries_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2911 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/databricks_api/permissions_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1253 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/databricks_api/scim_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2391 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/databricks_api/secrets_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2613 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/databricks_api/workspace_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.923818 tecton-0.9.1/tecton_proto/dataobs/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/dataobs/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2490 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/dataobs/config_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2553 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/dataobs/expectation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3691 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/dataobs/metric_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5748 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/dataobs/validation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3723 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/dataobs/validation_task_params_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4629 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/dataobs/validation_task_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.923818 tecton-0.9.1/tecton_proto/feature_server/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/feature_server/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.923818 tecton-0.9.1/tecton_proto/feature_server/configuration/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/feature_server/configuration/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    19997 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.923818 tecton-0.9.1/tecton_proto/materialization/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/materialization/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9821 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/materialization/job_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2610 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/materialization/materialization_states_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14634 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/materialization/materialization_task_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8173 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/materialization/params_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2752 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/materialization/spark_cluster_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.923818 tecton-0.9.1/tecton_proto/materializationjobservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/materializationjobservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16111 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/materializationjobservice/materialization_job_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.923818 tecton-0.9.1/tecton_proto/metadataservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/metadataservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2776 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/metadataservice/http_over_grpc_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   121489 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/metadataservice/metadata_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.923818 tecton-0.9.1/tecton_proto/offlinestore/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/offlinestore/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.923818 tecton-0.9.1/tecton_proto/offlinestore/delta/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/offlinestore/delta/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1570 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/offlinestore/delta/metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6554 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/offlinestore/delta/transaction_writer_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.923818 tecton-0.9.1/tecton_proto/online_store/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/online_store/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5408 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/online_store/feature_value_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1306 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/online_store/status_entry_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.927818 tecton-0.9.1/tecton_proto/online_store_writer/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/online_store_writer/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2401 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/online_store_writer/config_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5522 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/online_store_writer/copier_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.927818 tecton-0.9.1/tecton_proto/remoteenvironmentservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/remoteenvironmentservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13213 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.927818 tecton-0.9.1/tecton_proto/secrets/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/secrets/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10485 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/secrets/secrets_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.927818 tecton-0.9.1/tecton_proto/snowflake/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/snowflake/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1246 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/snowflake/location_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1392 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/snowflake/snowflake_credentials_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.927818 tecton-0.9.1/tecton_proto/spark_api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/spark_api/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1195 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/spark_api/error_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7388 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/spark_api/jobs_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.927818 tecton-0.9.1/tecton_proto/spark_common/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/spark_common/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7786 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/spark_common/clusters_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2386 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/spark_common/libraries_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.927818 tecton-0.9.1/tecton_proto/testhelperservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/testhelperservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3516 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/testhelperservice/test_helper_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.927818 tecton-0.9.1/tecton_proto/validation/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:10.000000 tecton-0.9.1/tecton_proto/validation/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4609 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_proto/validation/validator_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.927818 tecton-0.9.1/tecton_snowflake/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    30085 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/pipeline_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.931819 tecton-0.9.1/tecton_snowflake/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10160 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/query/aggregation_plans.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/query/dataframe_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13676 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/query/nodes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6314 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/query/queries.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      741 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/query/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3704 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/query/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8392 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/schema_derivation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2246 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/snowflake_type_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    33728 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/sql_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.935819 tecton-0.9.1/tecton_snowflake/templates/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/templates/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1025 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/templates/copier_macro.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      396 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/templates/create_temp_table_for_bfv.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      363 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/templates/create_temp_table_for_bwafv.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      255 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/templates/data_source.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1248 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/templates/delete_orphaned_schemas.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      698 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/templates/delete_staged_files.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3069 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/templates/historical_features.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7892 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/templates/historical_features_macros.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1795 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/templates/materialization_tile.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2575 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/templates/materialized_feature_view.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      937 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/templates/offline_materialization_macros.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      126 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/templates/online_store_copier.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6777 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/templates/run_full_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      583 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/templates/run_partial_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      569 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/templates/time_limit.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      213 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/templates/transformation_pipeline.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/templates_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      249 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_snowflake/utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.935819 tecton-0.9.1/tecton_spark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      808 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    30278 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/aggregation_plans.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2263 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/data_observability.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      926 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/data_source_credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    35476 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/data_source_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      425 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/errors_spark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6470 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/feature_view_spark_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.935819 tecton-0.9.1/tecton_spark/jars/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/jars/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2633 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/jars/class_loader.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)  1794322 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/jars/tecton-udfs-spark-3.jar
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7182 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/materialization_plan.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27440 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/offline_store.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15491 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/partial_aggregations.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    33278 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/pipeline_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:15.939819 tecton-0.9.1/tecton_spark/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3356 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/query/data_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10751 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/query/filter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    37167 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/query/join.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1515 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/query/node.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7583 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/query/pipeline.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14752 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/query/projection.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10712 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/query/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17887 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/schema_derivation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5434 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/schema_spark_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2317 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/spark_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1697 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/spark_schema_wrapper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4858 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/time_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      393 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/udf_jar.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3257 2024-04-23 21:39:11.000000 tecton-0.9.1/tecton_spark/udfs.py
```

### Comparing `tecton-0.9.0rc4/PKG-INFO` & `tecton-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tecton
-Version: 0.9.0rc4
+Version: 0.9.1
 Summary: Tecton Python SDK
 Home-page: https://tecton.ai
 Author: Tecton, Inc.
 Author-email: support@tecton.ai
 License: Tecton Proprietary
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `tecton-0.9.0rc4/README.md` & `tecton-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/protoc_gen_openapiv2/options/annotations_pb2.py` & `tecton-0.9.1/protoc_gen_openapiv2/options/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/protoc_gen_openapiv2/options/openapiv2_pb2.py` & `tecton-0.9.1/protoc_gen_openapiv2/options/openapiv2_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/setup.py` & `tecton-0.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,14 @@
     author_email='support@tecton.ai',
     url='https://tecton.ai',
     license='Tecton Proprietary',
     include_package_data=True,
     description='Tecton Python SDK',
     entry_points={'console_scripts': ['tecton=tecton.cli.cli:main'], 'pytest11': ['pytest_tecton=tecton.pytest_tecton']},
     name='tecton',
-    version='0.9.0rc4',
+    version='0.9.1',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    install_requires=['attrs>=21.3.0', 'boto3', 'googleapis-common-protos~=1.52', 'jinja2~=3.0', 'numpy~=1.16', 'pathspec', 'pendulum~=2.1', 'protobuf>=3.20.0', 'pypika~=0.48.9', 'pytimeparse', 'pandas>=1.0', 'texttable', 'requests', 'colorama~=0.4', 'tqdm~=4.41', 'yaspin<3,>=0.16', 'typing-extensions~=4.1', 'pygments>=2.7.4', 'pytest', 'click~=8.0', 'typeguard~=2.0', 'sqlparse', 'semantic_version', 'pyarrow<15,>=8', 'pydantic<3,>=1.10.13', 'pyyaml', 'setuptools', 'pip', 'pex~=2.1'],
-    extras_require={'databricks-connect': ['databricks-connect[sql]~=10.4.12'], 'databricks-connect9': ['databricks-connect[sql]~=9.1.23'], 'databricks-connect10': ['databricks-connect[sql]~=10.4.12'], 'databricks-connect11': ['databricks-connect[sql]~=11.3.12'], 'pyspark': ['pyspark[sql]~=3.2.1'], 'pyspark3': ['pyspark[sql]~=3.2.1'], 'pyspark3.1': ['pyspark[sql]~=3.1.2'], 'pyspark3.2': ['pyspark[sql]~=3.2.1'], 'pyspark3.3': ['pyspark[sql]~=3.3.2'], 'rift': ['duckdb==0.10.0', 'deltalake~=0.15', 'pyarrow>=11.0.0'], 'rift-materialization': ['duckdb==0.10.0', 'deltalake~=0.15', 'pyarrow>=11.0.0', 'pydantic<2', 'urllib3<1.27'], 'snowflake': ['snowflake-snowpark-python[pandas]~=1.0'], 'athena': ['awswrangler~=3.0'], 'materialization': ['statsd==3.3.0', 'urllib3<2.0.0']},
+    install_requires=['attrs>=21.3.0', 'boto3', 'googleapis-common-protos<2,>=1.57.0', 'jinja2~=3.0', 'numpy~=1.16', 'pathspec', 'pendulum~=2.1', 'protobuf>=3.20.0', 'pypika~=0.48.9', 'pytimeparse', 'pandas>=1.0', 'texttable', 'requests', 'colorama~=0.4', 'tqdm~=4.41', 'yaspin<3,>=0.16', 'typing-extensions~=4.1', 'pygments>=2.7.4', 'pytest', 'click~=8.0', 'typeguard~=2.0', 'sqlparse', 'semantic_version', 'pyarrow<15,>=8', 'pydantic<3,>=1.10.13', 'pyyaml', 'setuptools', 'pip', 'pex~=2.1'],
+    extras_require={'databricks-connect': ['databricks-connect[sql]~=10.4.12'], 'databricks-connect9': ['databricks-connect[sql]~=9.1.23'], 'databricks-connect10': ['databricks-connect[sql]~=10.4.12'], 'databricks-connect11': ['databricks-connect[sql]~=11.3.12'], 'pyspark': ['pyspark[sql]~=3.2.1'], 'pyspark3': ['pyspark[sql]~=3.2.1'], 'pyspark3.1': ['pyspark[sql]~=3.1.2'], 'pyspark3.2': ['pyspark[sql]~=3.2.1'], 'pyspark3.3': ['pyspark[sql]~=3.3.2'], 'rift': ['duckdb==0.10.0', 'deltalake~=0.15', 'pyarrow>=11.0.0'], 'rift-materialization': ['duckdb==0.10.0', 'deltalake~=0.15', 'pyarrow>=11.0.0', 'snowflake-connector-python[pandas]~=3.6', 'snowflake-snowpark-python[pandas]~=1.0', 'pydantic<2', 'urllib3<1.27'], 'snowflake': ['snowflake-snowpark-python[pandas]~=1.0'], 'athena': ['awswrangler~=3.0'], 'materialization': ['statsd==3.3.0', 'urllib3<2.0.0']},
     packages=packages,
 )
```

### Comparing `tecton-0.9.0rc4/tecton/__init__.py` & `tecton-0.9.1/tecton/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/analytics.py` & `tecton-0.9.1/tecton/_internals/analytics.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/athena_api.py` & `tecton-0.9.1/tecton/_internals/athena_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/data_frame_helper.py` & `tecton-0.9.1/tecton/_internals/data_frame_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/delete_keys_api.py` & `tecton-0.9.1/tecton/_internals/delete_keys_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/display.py` & `tecton-0.9.1/tecton/_internals/display.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/env_utils.py` & `tecton-0.9.1/tecton/_internals/env_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/errors.py` & `tecton-0.9.1/tecton/_internals/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,20 @@
 
 def FEATURE_TABLE_GET_ONLINE_FEATURES_FROM_DEVELOPMENT_WORKSPACE(ft_name, workspace):
     return TectonValidationError(
         f"Feature Table {ft_name} is in workspace {workspace}, which is a development workspace (does not have materialization enabled). Please apply this Feature Table to a live workspace and ingest some features before using with get_online_features()."
     )
 
 
+def STREAM_COMPACTION_ENABLED_DEPRECATED():
+    return TectonValidationError(
+        "FeatureView.stream_compaction_enabled is deprecated. Please use stream_tiling_enabled instead. stream_tiling_enabled has the same semantics and is just a new name."
+    )
+
+
 def FEATURE_TABLE_GET_MATERIALIZED_FEATURES_OFFLINE_FALSE(ft_name):
     return TectonValidationError(
         f"Feature Table {ft_name} does not have offline materialization enabled, i.e. offline=True. Cannot retrieve offline feature if offline materializaiton is not enabled."
     )
 
 
 def FD_GET_MATERIALIZED_FEATURES_FROM_LOCAL_OBJECT(fv_name, fco_name):
@@ -567,15 +573,15 @@
 
 def AGGREGATION_INTERVAL_SET_COMPACTION():
     return TectonValidationError("Feature views with stream compaction enabled cannot have `aggregation_interval` set.")
 
 
 def COMPACTION_TIME_WINDOW_SERIES_UNSUPPORTED():
     return TectonValidationError(
-        "Aggregations using a TimeWindowSeries window are not supported when `stream_compaction_enabled=True`."
+        "Aggregations using a TimeWindowSeries window are not supported when `compaction_enabled=True`."
     )
 
 
 # New Read API
 GET_FEATURES_FOR_EVENTS_UNSUPPORTED = TectonValidationError(
     "get_features_for_events() is only supported for SPARK or RIFT Compute Modes."
 )
@@ -588,14 +594,18 @@
     "get_partial_aggregates() is only supported for Feature Views with Tecton Managed Aggregations."
 )
 
 GET_PARTIAL_AGGREGATES_UNSUPPORTED_COMPACTED = TectonValidationError(
     "get_partial_aggregates() is only supported for Aggregate Feature Views with Compaction Disabled."
 )
 
+RUN_TRANSFORMATION_UNSUPPORTED = TectonValidationError(
+    "run_transformation() for Batch and Stream Feature Views is only supported for SPARK and RIFT Compute Modes."
+)
+
 
 def READ_API_DEPRECATION_TEMPLATE(old_method, new_method):
     return f"{old_method}() has been deprecated in Tecton 0.9 and will be fully removed in the next major SDK release. Please use {new_method}() instead. See https://docs.tecton.ai/docs/reading-feature-data/reading-feature-data-for-training/offline-retrieval-methods for more information."
 
 
 GET_HISTORICAL_FEATURES_DEPRECATED_SPINE = READ_API_DEPRECATION_TEMPLATE(
     "get_historical_features", "get_features_for_events"
```

### Comparing `tecton-0.9.0rc4/tecton/_internals/find_spark.py` & `tecton-0.9.1/tecton/_internals/find_spark.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/ingest_utils.py` & `tecton-0.9.1/tecton/_internals/ingest_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/ingestion.py` & `tecton-0.9.1/tecton/_internals/ingestion.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/materialization_api.py` & `tecton-0.9.1/tecton/_internals/materialization_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/metadata_service.py` & `tecton-0.9.1/tecton/_internals/metadata_service.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/metadata_service_impl/request_lib.py` & `tecton-0.9.1/tecton/_internals/metadata_service_impl/request_lib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/metadata_service_impl/service_modules.py` & `tecton-0.9.1/tecton/_internals/metadata_service_impl/service_modules.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/mock_source_utils.py` & `tecton-0.9.1/tecton/_internals/mock_source_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/offline_store_credentials.py` & `tecton-0.9.1/tecton/_internals/offline_store_credentials.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/pandas_compat.py` & `tecton-0.9.1/tecton/_internals/pandas_compat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/query_helper.py` & `tecton-0.9.1/tecton/_internals/query_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/querytree_api.py` & `tecton-0.9.1/tecton/_internals/querytree_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,14 @@
     feature_set_config: feature_set_config.FeatureSetConfig,
     spine: Union[pyspark_sql.DataFrame, pd.DataFrame, TectonDataFrame, str],
     timestamp_key: Optional[str],
     from_source: Optional[bool],
     save: bool,
     save_as: Optional[str],
 ) -> TectonDataFrame:
-    logger.warning(errors.GET_HISTORICAL_FEATURES_DEPRECATED_SPINE)
-
     timestamp_required = spine is not None and any(
         _should_infer_timestamp_of_spine(fd, timestamp_key) for fd in feature_set_config.feature_definitions
     )
 
     _validate_sql_string_support(dialect, spine)
 
     if timestamp_required:
```

### Comparing `tecton-0.9.0rc4/tecton/_internals/repo/function_serialization.py` & `tecton-0.9.1/tecton/_internals/repo/function_serialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/rewrite.py` & `tecton-0.9.1/tecton/_internals/rewrite.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/run_api.py` & `tecton-0.9.1/tecton/_internals/run_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,16 @@
     compute_mode: ComputeMode,
     fd: FeatureDefinitionWrapper,
     feature_start_time: datetime,
     feature_end_time: datetime,
     mock_data_sources: Dict[str, NodeRef],
     aggregation_level: Optional[str],
 ) -> "tecton.framework.data_frame.TectonDataFrame":
+    _print_run_deprecation_message(aggregation_level)
+
     if not fd.is_on_demand:
         check_spark_version(fd.fv_spec.batch_cluster_config)
 
     return _querytree_run_batch(
         dialect=dialect,
         compute_mode=compute_mode,
         fd=fd,
@@ -255,23 +257,25 @@
         else:
             aggregation_level = AGGREGATION_LEVEL_DISABLED
 
     if aggregation_level not in SUPPORTED_AGGREGATION_LEVEL_VALUES:
         msg = "aggregation_level"
         raise errors.FV_INVALID_ARG_VALUE(msg, str(aggregation_level), str(SUPPORTED_AGGREGATION_LEVEL_VALUES))
 
+    return aggregation_level
+
+
+def _print_run_deprecation_message(aggregation_level: Optional[str]):
     if aggregation_level == AGGREGATION_LEVEL_FULL:
         logger.warning(errors.RUN_DEPRECATED_FULL_AGG)
     elif aggregation_level == AGGREGATION_LEVEL_DISABLED:
         logger.warning(errors.RUN_DEPRECATED_TRANSFORMATION)
     elif aggregation_level == AGGREGATION_LEVEL_PARTIAL:
         logger.warning(errors.RUN_DEPRECATED_PARTIAL_AGGS)
 
-    return aggregation_level
-
 
 # Validate that mock_inputs keys are exact match with expected inputs.
 def validate_ondemand_mock_inputs(
     mock_inputs: Dict[str, Union[Dict[str, Any], pandas.DataFrame]],
     pipeline: pipeline_pb2.Pipeline,
     odfv_fd: Optional[FeatureDefinitionWrapper] = None,
 ):
```

### Comparing `tecton-0.9.0rc4/tecton/_internals/sdk_decorators.py` & `tecton-0.9.1/tecton/_internals/sdk_decorators.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/secret_resolver.py` & `tecton-0.9.1/tecton/_internals/secret_resolver.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/snowflake_api.py` & `tecton-0.9.1/tecton/_internals/snowflake_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/spark_api.py` & `tecton-0.9.1/tecton/_internals/spark_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/spark_utils.py` & `tecton-0.9.1/tecton/_internals/spark_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/tecton_pydantic.py` & `tecton-0.9.1/tecton/_internals/tecton_pydantic.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/time_utils.py` & `tecton-0.9.1/tecton/_internals/time_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/type_utils.py` & `tecton-0.9.1/tecton/_internals/type_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/utils.py` & `tecton-0.9.1/tecton/_internals/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/_internals/validations_api.py` & `tecton-0.9.1/tecton/_internals/validations_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/aggregation_functions.py` & `tecton-0.9.1/tecton/aggregation_functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/cli/access_control.py` & `tecton-0.9.1/tecton/cli/access_control.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/cli/api_key.py` & `tecton-0.9.1/tecton/cli/api_key.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/cli/auth.py` & `tecton-0.9.1/tecton/cli/auth.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/cli/cli.py` & `tecton-0.9.1/tecton/cli/cli.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/cli/cli_utils.py` & `tecton-0.9.1/tecton/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/cli/command.py` & `tecton-0.9.1/tecton/cli/command.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/cli/completion.py` & `tecton-0.9.1/tecton/cli/completion.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/cli/engine.py` & `tecton-0.9.1/tecton/cli/engine.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/cli/engine_renderer.py` & `tecton-0.9.1/tecton/cli/engine_renderer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/cli/environment.py` & `tecton-0.9.1/tecton/cli/environment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+import json
 import math
-import re
 import shutil
 import sys
 import tempfile
 from concurrent.futures import ThreadPoolExecutor
 from concurrent.futures import as_completed
 from dataclasses import dataclass
 from datetime import datetime
@@ -11,25 +11,24 @@
 from pathlib import Path
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 import click
 from google.protobuf import timestamp_pb2
-from pkg_resources.extern.packaging.requirements import InvalidRequirement
 from tqdm import tqdm
 
 from tecton import version
 from tecton._internals import metadata_service
 from tecton.cli import printer
 from tecton.cli.cli_utils import display_table
 from tecton.cli.command import TectonGroup
+from tecton.cli.environment_utils import EnvironmentDependencies
 from tecton.cli.environment_utils import create_requirements_from_lock_file
 from tecton.cli.environment_utils import download_dependencies
-from tecton.cli.environment_utils import get_requirement
 from tecton.cli.environment_utils import is_valid_environment_name
 from tecton.cli.environment_utils import resolve_dependencies
 from tecton_core import http
 from tecton_core import id_helper
 from tecton_proto.common.container_image_pb2 import ContainerImage
 from tecton_proto.data.remote_compute_environment_pb2 import ObjectStoreUploadPart
 from tecton_proto.data.remote_compute_environment_pb2 import RemoteComputeType
@@ -160,38 +159,28 @@
     requirements: str,
     output_file: Optional[str] = None,
     python_version: Optional[str] = None,
     verbose: Optional[bool] = False,
 ):
     """Resolve dependencies and return a fully resolved set of requirements for a given requirements.txt"""
     _python_version = python_version or DEFAULT_PYTHON_VERSION
-    on_demand_transform_runtime_version = _on_demand_transform_runtime_version(requirements)
-    rift_runtime_version = _rift_materialization_runtime_version(requirements)
-    if not on_demand_transform_runtime_version and not rift_runtime_version:
-        printer.safe_print(
-            f"{ERROR_MESSAGE_PREFIX} Please include these Tecton supporting libraries:\n"
-            f"💡  `tecton-runtime` package (https://pypi.org/project/tecton-runtime) to support On Demand Feature Views.\n"
-            f"💡  `tecton[rift-materialization]` package (https://pypi.org/project/tecton) to support Rift Batch Feature Views.\n",
-            "💡  `tecton[rift-materialization]` and `tecton-runtime` package to support OnDemand Feature Views, Rift Batch Feature Views and Rift Stream Feature Views.\n",
-            file=sys.stderr,
-        )
-        sys.exit(1)
 
     with tempfile.TemporaryDirectory() as tmpdir:
         try:
-            resolved_requirements_path, _ = _run_dependency_resolution(
+            resolved_requirements_path, lock_output_path = _run_dependency_resolution(
                 requirements_path=Path(requirements),
                 resolved_requirements_directory=Path(tmpdir),
                 python_version=_python_version,
                 verbose=verbose,
             )
         except ValueError as e:
             printer.safe_print(f"{ERROR_MESSAGE_PREFIX} {e}", file=sys.stderr)
             sys.exit(1)
 
+        _validate_and_get_dependencies(lock_output_path)
         printer.safe_print("✅ Successfully resolved dependencies")
 
         if output_file is not None:
             output_path = Path(output_file)
             resolved_requirements_str = resolved_requirements_path.read_bytes()
             output_path.write_bytes(resolved_requirements_str)
         else:
@@ -240,40 +229,19 @@
     if name in environment_names:
         printer.safe_print(
             f"{ERROR_MESSAGE_PREFIX} An environment with the name `{name}` already exists in Tecton!",
             file=sys.stderr,
         )
         sys.exit(1)
 
-    on_demand_transform_runtime_version = _on_demand_transform_runtime_version(requirements)
-    rift_runtime_version = _rift_materialization_runtime_version(requirements)
-    if not on_demand_transform_runtime_version and not rift_runtime_version:
-        # TODO (vitaly): update the doc link for more information on custom Rift materialization envs
-        printer.safe_print(
-            f"{ERROR_MESSAGE_PREFIX} Please include at least one of the supporting Tecton libraries:\n"
-            f"💡  `tecton-runtime` package (https://pypi.org/project/tecton-runtime) to support On Demand environments\n"
-            f"💡  `tecton[rift-materialization]` package (https://pypi.org/project/tecton) to support Rift materialization environments",
-            "\nFor more information, please see: https://docs.tecton.ai/docs/defining-features/feature-views/on-demand-feature-view/on-demand-feature-view-environments/custom-on-demand-feature-view-environments",
-            file=sys.stderr,
-        )
-        sys.exit(1)
-    else:
-        printer.safe_print(
-            f"\n💡 Creating environment '{name}' for job types:\n"
-            f"{CHECK_MARK if on_demand_transform_runtime_version else ERROR_SIGN} On Demand\n"
-            f"{CHECK_MARK if rift_runtime_version else ERROR_SIGN} Rift Batch\n"
-            f"{CHECK_MARK if rift_runtime_version and on_demand_transform_runtime_version else ERROR_SIGN} Rift Stream Ingest\n"
-        )
     resp = _create_environment_with_requirements(
         name,
         description,
         Path(requirements),
         _python_version,
-        on_demand_transform_runtime_version=on_demand_transform_runtime_version,
-        rift_runtime_version=rift_runtime_version,
         verbose=verbose,
     )
     if resp:
         _display_environments([resp.remote_environment])
         printer.safe_print(
             f"\n🎉 Successfully created environment {name} with Status=PENDING. Please run `tecton environment get --name <environment-name>` to monitor the status of the environment"
         )
@@ -367,15 +335,15 @@
             (
                 i.id,
                 i.name,
                 i.description,
                 RemoteComputeType.Name(i.type).split("_")[-1],
                 RemoteEnvironmentStatus.Name(i.status).split("_")[-1],
                 i.rift_batch_job_environment.tecton_materialization_runtime_version or "N/A",
-                i.on_demand_job_environment.tecton_transform_runtime_version or "N/A",
+                i.realtime_job_environment.tecton_transform_runtime_version or "N/A",
                 _timestamp_to_string(i.created_at),
             )
             for i in environments
         ],
     )
 
 
@@ -418,16 +386,14 @@
 
 
 def _create_environment_with_requirements(
     name: str,
     description: str,
     requirements_path: Path,
     python_version: str,
-    on_demand_transform_runtime_version: str,
-    rift_runtime_version: str,
     verbose: bool,
 ):
     """Create a custom environment by resolving dependencies, downloading wheels and updating MDS
     Parameters:
         name(str): Name of the custom environment
         description(str): Description of the custom environment
         requirements_path(str): Path to the `requirements.txt` file
@@ -442,15 +408,26 @@
                 python_version=python_version,
                 verbose=verbose,
             )
         except ValueError as e:
             printer.safe_print(f"{ERROR_MESSAGE_PREFIX} {e}", file=sys.stderr)
             sys.exit(1)
 
+        dependencies = _validate_and_get_dependencies(lock_output_path)
+
         printer.safe_print("✅ Successfully resolved dependencies")
+        tecton_runtime_version = dependencies.get_version(dependency_name=TECTON_TRANSFORM_RUNTIME_PACKAGE)
+        tecton_rift_version = dependencies.get_version(dependency_name=TECTON_RIFT_MATERIALIZATION_RUNTIME_PACKAGE)
+
+        printer.safe_print(
+            f"\n💡 Creating environment '{name}' for job types:\n"
+            f"{CHECK_MARK if tecton_runtime_version else ERROR_SIGN} On Demand\n"
+            f"{CHECK_MARK if tecton_rift_version else ERROR_SIGN} Rift Batch\n"
+            f"{CHECK_MARK if tecton_rift_version and tecton_runtime_version else ERROR_SIGN} Rift Stream Ingest\n"
+        )
 
         url_requirements_path = Path(tmpdir) / "url_requirements.txt"
 
         # doing this to use the url because some wheels maybe coming from different sources
         create_requirements_from_lock_file(lock_output_path, url_requirements_path)
 
         download_wheels_dir = Path(tmpdir) / "wheels"
@@ -486,21 +463,50 @@
             name=name,
             id=environment_id,
             description=description,
             python_version=python_version,
             s3_wheels_location=location,
             requirements=requirements_path.read_text(),
             resolved_requirements=resolved_requirements_path.read_text(),
-            transform_runtime_version=on_demand_transform_runtime_version,
-            rift_materialization_runtime_version=rift_runtime_version,
+            transform_runtime_version=tecton_runtime_version,
+            rift_materialization_runtime_version=tecton_rift_version,
             sdk_version=version.get_semantic_version(),
         )
         return metadata_service.instance().CreateRemoteEnvironment(req)
 
 
+def _validate_and_get_dependencies(lock_file_path: Path) -> EnvironmentDependencies:
+    with open(lock_file_path, "r") as lock_file:
+        dependencies_data = json.load(lock_file)
+    dependencies = EnvironmentDependencies(dependencies_data)
+    tecton_runtime_version = dependencies.get_version(dependency_name=TECTON_TRANSFORM_RUNTIME_PACKAGE)
+    tecton_rift_version = dependencies.get_version(dependency_name=TECTON_RIFT_MATERIALIZATION_RUNTIME_PACKAGE)
+
+    if tecton_rift_version is not None:
+        rift_extras = dependencies.get_dependency_extras(TECTON_RIFT_MATERIALIZATION_RUNTIME_PACKAGE)
+        if "rift-materialization" not in rift_extras:
+            printer.safe_print(
+                f"{ERROR_MESSAGE_PREFIX} `rift-materialization` extra must be included for package `tecton` to support Rift materialization (tecton[rift-materialization]==x.x.x)",
+                file=sys.stderr,
+            )
+            sys.exit(1)
+
+    if not tecton_runtime_version and not tecton_rift_version:
+        # TODO (vitaly): update the doc link for more information on custom Rift materialization envs
+        printer.safe_print(
+            f"{ERROR_MESSAGE_PREFIX} Please include at least one of the supporting Tecton libraries:\n"
+            f"💡  `tecton-runtime` package (https://pypi.org/project/tecton-runtime) to support On Demand environments\n"
+            f"💡  `tecton[rift-materialization]` package (https://pypi.org/project/tecton) to support Rift materialization environments",
+            "\nFor more information, please see: https://docs.tecton.ai/docs/defining-features/feature-views/on-demand-feature-view/on-demand-feature-view-environments/custom-on-demand-feature-view-environments",
+            file=sys.stderr,
+        )
+        sys.exit(1)
+    return dependencies
+
+
 def _run_dependency_resolution(
     requirements_path: Path, resolved_requirements_directory: Path, python_version: str, verbose: bool = False
 ) -> Tuple[Path, Path]:
     printer.safe_print(
         f"\n⏳ Resolving dependencies for Python {python_version} and architecture {DEFAULT_ARCHITECTURE}. This may take a few seconds....."
     )
     lock_output_path = resolved_requirements_directory / "lock.json"
@@ -564,64 +570,14 @@
 
 
 def _timestamp_to_string(value: timestamp_pb2.Timestamp) -> str:
     t = datetime.fromtimestamp(value.ToSeconds())
     return t.astimezone(timezone.utc).strftime("%Y-%m-%d %H:%M:%S %Z")
 
 
-def _on_demand_transform_runtime_version(requirements_path_str: str) -> Optional[str]:
-    requirements_path = Path(requirements_path_str)
-    try:
-        req = get_requirement(requirements_path=requirements_path, package_name=TECTON_TRANSFORM_RUNTIME_PACKAGE)
-        if req is None:
-            return
-        if not req.specs or req.specs[0][0] != "==":
-            printer.safe_print(
-                f"{ERROR_MESSAGE_PREFIX} `tecton-runtime` package (https://pypi.org/project/tecton-runtime) must be pinned to a version (tecton-runtime==x.x.x)",
-                file=sys.stderr,
-            )
-            sys.exit(1)
-        return re.sub(r"\s*--hash=[^ ]+", "", req.specs[0][1])
-    except InvalidRequirement as e:
-        printer.safe_print(
-            f"{ERROR_MESSAGE_PREFIX} Invalid `requirements` file: {e}.\n Please pass a valid Requirements file formatted according to https://pip.pypa.io/en/stable/reference/requirements-file-format/",
-            file=sys.stderr,
-        )
-        sys.exit(1)
-
-
-def _rift_materialization_runtime_version(requirements_path_str: str) -> Optional[str]:
-    requirements_path = Path(requirements_path_str)
-    try:
-        req = get_requirement(
-            requirements_path=requirements_path, package_name=TECTON_RIFT_MATERIALIZATION_RUNTIME_PACKAGE
-        )
-        if req is None:
-            return
-        if "rift-materialization" not in req.extras:
-            printer.safe_print(
-                f"{ERROR_MESSAGE_PREFIX} `rift-materialization` extra must be included to support Rift materialization (tecton[rift-materialization]==x.x.x)",
-                file=sys.stderr,
-            )
-            sys.exit(1)
-        if not req.specs or req.specs[0][0] != "==":
-            printer.safe_print(
-                f"{ERROR_MESSAGE_PREFIX} `tecton[rift-materialization]` must be pinned to a version (tecton[rift-materialization]==x.x.x)",
-                file=sys.stderr,
-            )
-            sys.exit(1)
-        return re.sub(r"\s*--hash=[^ ]+", "", req.specs[0][1])
-    except InvalidRequirement:
-        printer.safe_print(
-            f"{ERROR_MESSAGE_PREFIX} Invalid `requirements` file. Please pass a valid Requirements file formatted according to https://pip.pypa.io/en/stable/reference/requirements-file-format/",
-            file=sys.stderr,
-        )
-        sys.exit(1)
-
-
 def _upload_dependencies(source_path: Path, environment_id: str, verbose: bool) -> str:
     """Upload dependencies from the specified source path to S3.
     Args:
         source_path (str): The path to the dependencies to upload.
         environment_id (str): The ID of the environment.
         verbose (bool): Activates verbose logging
     """
```

### Comparing `tecton-0.9.0rc4/tecton/cli/environment_utils.py` & `tecton-0.9.1/tecton/cli/environment_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import json
 import re
 import subprocess
 import sys
 from pathlib import Path
 from typing import List
-from typing import Optional
-
-from pkg_resources import Requirement
-from pkg_resources import parse_requirements
 
 from tecton.cli import printer
 from tecton_core.errors import FailedDependencyDownloadError
 
 
 PLATFORM = "linux_x86_64"
 
@@ -39,17 +35,19 @@
     python_version: str,
     timeout_seconds: int,
     verbose: bool,
 ):
     """Resolve dependencies using `pex`
     Parameters:
         requirements_path(Path): Path to the `requirements.txt` file
+        lock_output_path(Path): Path to store the output lock.json
         resolved_requirements_path(Path): The target path for generating the fully resolved and pinned `resolved-requirements.txt` file
         python_version(str): The python version to resolve dependencies for
         timeout_seconds(int): The timeout in seconds for the dependency resolution
+        verbose(bool): Run in verbose mode and print additional information for debugging
     """
     major_minor_version = _get_major_minor_version(python_version)
     if major_minor_version not in PYTHON_VERSION_TO_PLATFORM:
         msg = f"Invalid `python_version` {python_version}. Expected one of: {list(PYTHON_VERSION_TO_PLATFORM.keys())}"
         raise ValueError(msg)
     platform = PYTHON_VERSION_TO_PLATFORM[major_minor_version]
     if verbose:
@@ -181,24 +179,50 @@
         error_string = error_string[start_index + 6 :].replace("\n", " ")
     # The pex error message does not clarify that wheels must be present and so we append it to the original error message
     if MISSING_REQUIREMENTS_ERROR in error_string:
         error_string = f"{error_string}\n\n💡 {ENSURE_WHEELS_EXIST_WARNING}"
     return error_string
 
 
-def is_requirement_present(requirements_path: Path, package_name: str) -> bool:
-    requirements = parse_requirements(requirements_path.read_text())
-    package_names = [requirement.project_name for requirement in requirements]
-    return package_name in package_names
-
-
-def get_requirement(requirements_path: Path, package_name: str) -> Optional[Requirement]:
-    requirements = parse_requirements(requirements_path.read_text())
-    for requirement in requirements:
-        if requirement.project_name == package_name:
-            return requirement
-
-
 def is_valid_environment_name(name: str) -> bool:
     # Only letters, numbers, hyphens, or underscores allowed in an environment name
     pattern = r"^[a-zA-Z0-9_-]+$"
     return bool(re.match(pattern, name))
+
+
+class EnvironmentDependencies:
+    def __init__(self, data):
+        self.data = data
+        self.locked_dependencies = {
+            item["project_name"]: item for item in data["locked_resolves"][0]["locked_requirements"]
+        }
+        self.input_requirements = data["requirements"]
+
+    def get_version(self, dependency_name):
+        """Retrieve the version of the specified dependency"""
+        package = self.locked_dependencies.get(dependency_name)
+        if package:
+            return package["version"]
+        return None
+
+    def is_dependency_present(self, dependency_name):
+        """Check if the specified dependency is present in the requirements."""
+        return dependency_name in self.locked_dependencies
+
+    def get_dependency_extras(self, dependency_name):
+        """Retrieve a list of extras available for the specified dependency."""
+        package = self.locked_dependencies.get(dependency_name)
+        if package:
+            extras = set()
+            for dist in package["requires_dists"]:
+                if "; extra ==" in dist:
+                    extracted_extra = dist.split("; extra ==")[1].strip(' "').replace("'", "")
+                    extras.add(extracted_extra)
+            return list(extras)
+        return []
+
+    def is_version_pinned(self, package_name):
+        """Check if the dependency version is explicitly pinned in the input requirements"""
+        for req in self.input_requirements:
+            if package_name in req and "==" in req:
+                return True
+        return False
```

### Comparing `tecton-0.9.0rc4/tecton/cli/error_utils.py` & `tecton-0.9.1/tecton/cli/error_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/cli/materialization.py` & `tecton-0.9.1/tecton/cli/materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/cli/pex_wrapper.py` & `tecton-0.9.1/tecton/cli/pex_wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/cli/printer.py` & `tecton-0.9.1/tecton/cli/printer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/cli/repo.py` & `tecton-0.9.1/tecton/cli/repo.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/cli/repo_config.py` & `tecton-0.9.1/tecton/cli/repo_config.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/cli/repo_utils.py` & `tecton-0.9.1/tecton/cli/repo_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/cli/secrets.py` & `tecton-0.9.1/tecton/cli/secrets.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 @secrets.command("create-scope", requires_auth=True, cls=TectonCommand)
 @click.option("-s", "--scope", default=None, required=True, help="Secret scope name")
 @click_exception_wrapper
 def create_scope(scope):
     """Create a new secret scope."""
     request = CreateSecretScopeRequest(scope=scope)
     response = metadata_service.instance().CreateSecretScope(request)
-    printer.safe_print('Created secret scope "{scope}"')
+    printer.safe_print(f'Created secret scope "{scope}"')
 
 
 @secrets.command("list-scopes", requires_auth=True, cls=TectonCommand)
 @click_exception_wrapper
 def list_scopes():
     """List secret scopes."""
     request = ListSecretScopesRequest()
```

### Comparing `tecton-0.9.0rc4/tecton/cli/service_account.py` & `tecton-0.9.1/tecton/cli/service_account.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/cli/test.py` & `tecton-0.9.1/tecton/cli/test.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/cli/user.py` & `tecton-0.9.1/tecton/cli/user.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/cli/workspace.py` & `tecton-0.9.1/tecton/cli/workspace.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/cli/workspace_utils.py` & `tecton-0.9.1/tecton/cli/workspace_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/fco_listers.py` & `tecton-0.9.1/tecton/fco_listers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/framework/base_tecton_object.py` & `tecton-0.9.1/tecton/framework/base_tecton_object.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/framework/configs.py` & `tecton-0.9.1/tecton/framework/configs.py`

 * *Files 0% similar despite different names*

```diff
@@ -7319,164 +7319,163 @@
 0001c960: 6f77 2c20 6e61 6d65 3d6e 616d 6529 0a0a  ow, name=name)..
 0001c970: 2020 2020 6465 6620 5f74 6f5f 7072 6f74      def _to_prot
 0001c980: 6f28 0a20 2020 2020 2020 2073 656c 662c  o(.        self,
 0001c990: 2061 6767 7265 6761 7469 6f6e 5f69 6e74   aggregation_int
 0001c9a0: 6572 7661 6c3a 2064 6174 6574 696d 652e  erval: datetime.
 0001c9b0: 7469 6d65 6465 6c74 612c 2069 735f 636f  timedelta, is_co
 0001c9c0: 6e74 696e 756f 7573 3a20 626f 6f6c 2c20  ntinuous: bool, 
-0001c9d0: 6261 7463 685f 636f 6d70 6163 7469 6f6e  batch_compaction
-0001c9e0: 5f65 6e61 626c 6564 3a20 626f 6f6c 203d  _enabled: bool =
-0001c9f0: 2046 616c 7365 0a20 2020 2029 3a0a 2020   False.    ):.  
-0001ca00: 2020 2020 2020 7072 6f74 6f20 3d20 6665        proto = fe
-0001ca10: 6174 7572 655f 7669 6577 5f70 6232 2e46  ature_view_pb2.F
-0001ca20: 6561 7475 7265 4167 6772 6567 6174 696f  eatureAggregatio
-0001ca30: 6e28 0a20 2020 2020 2020 2020 2020 206e  n(.            n
-0001ca40: 616d 653d 7365 6c66 2e6e 616d 650a 2020  ame=self.name.  
-0001ca50: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0001ca60: 662e 6e61 6d65 0a20 2020 2020 2020 2020  f.name.         
-0001ca70: 2020 2065 6c73 6520 7365 6c66 2e5f 6465     else self._de
-0001ca80: 6661 756c 745f 6e61 6d65 2861 6767 7265  fault_name(aggre
-0001ca90: 6761 7469 6f6e 5f69 6e74 6572 7661 6c2c  gation_interval,
-0001caa0: 2069 735f 636f 6e74 696e 756f 7573 2c20   is_continuous, 
-0001cab0: 6261 7463 685f 636f 6d70 6163 7469 6f6e  batch_compaction
-0001cac0: 5f65 6e61 626c 6564 292c 0a20 2020 2020  _enabled),.     
-0001cad0: 2020 2020 2020 2063 6f6c 756d 6e3d 7365         column=se
-0001cae0: 6c66 2e63 6f6c 756d 6e2c 0a20 2020 2020  lf.column,.     
-0001caf0: 2020 2020 2020 2066 756e 6374 696f 6e3d         function=
-0001cb00: 7365 6c66 2e66 756e 6374 696f 6e2e 6261  self.function.ba
-0001cb10: 7365 5f6e 616d 652c 0a20 2020 2020 2020  se_name,.       
-0001cb20: 2029 0a0a 2020 2020 2020 2020 666f 7220   )..        for 
-0001cb30: 6b2c 2076 2069 6e20 7365 6c66 2e66 756e  k, v in self.fun
-0001cb40: 6374 696f 6e2e 7061 7261 6d73 2e69 7465  ction.params.ite
-0001cb50: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
-0001cb60: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-0001cb70: 762c 2069 6e74 293a 0a20 2020 2020 2020  v, int):.       
-0001cb80: 2020 2020 2020 2020 2070 726f 746f 2e66           proto.f
-0001cb90: 756e 6374 696f 6e5f 7061 7261 6d73 5b6b  unction_params[k
-0001cba0: 5d2e 436f 7079 4672 6f6d 2866 6561 7475  ].CopyFrom(featu
-0001cbb0: 7265 5f76 6965 775f 7062 322e 5061 7261  re_view_pb2.Para
-0001cbc0: 6d56 616c 7565 2869 6e74 3634 5f76 616c  mValue(int64_val
-0001cbd0: 7565 3d76 2929 0a20 2020 2020 2020 2020  ue=v)).         
-0001cbe0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0001cbf0: 2020 2020 2020 2020 2070 726f 746f 2e66           proto.f
-0001cc00: 756e 6374 696f 6e5f 7061 7261 6d73 5b6b  unction_params[k
-0001cc10: 5d2e 436f 7079 4672 6f6d 2866 6561 7475  ].CopyFrom(featu
-0001cc20: 7265 5f76 6965 775f 7062 322e 5061 7261  re_view_pb2.Para
-0001cc30: 6d56 616c 7565 2864 6f75 626c 655f 7661  mValue(double_va
-0001cc40: 6c75 653d 7629 290a 0a20 2020 2020 2020  lue=v))..       
-0001cc50: 2069 6620 6973 696e 7374 616e 6365 2873   if isinstance(s
-0001cc60: 656c 662e 7469 6d65 5f77 696e 646f 772c  elf.time_window,
-0001cc70: 2054 696d 6557 696e 646f 7729 3a0a 2020   TimeWindow):.  
-0001cc80: 2020 2020 2020 2020 2020 7072 6f74 6f2e            proto.
-0001cc90: 7469 6d65 5f77 696e 646f 772e 436f 7079  time_window.Copy
-0001cca0: 4672 6f6d 2873 656c 662e 7469 6d65 5f77  From(self.time_w
-0001ccb0: 696e 646f 772e 5f74 6f5f 7072 6f74 6f28  indow._to_proto(
-0001ccc0: 2929 0a20 2020 2020 2020 2065 6c69 6620  )).        elif 
-0001ccd0: 6973 696e 7374 616e 6365 2873 656c 662e  isinstance(self.
-0001cce0: 7469 6d65 5f77 696e 646f 772c 204c 6966  time_window, Lif
-0001ccf0: 6574 696d 6557 696e 646f 7729 3a0a 2020  etimeWindow):.  
-0001cd00: 2020 2020 2020 2020 2020 7072 6f74 6f2e            proto.
-0001cd10: 6c69 6665 7469 6d65 5f77 696e 646f 772e  lifetime_window.
-0001cd20: 436f 7079 4672 6f6d 2873 656c 662e 7469  CopyFrom(self.ti
-0001cd30: 6d65 5f77 696e 646f 772e 5f74 6f5f 7072  me_window._to_pr
-0001cd40: 6f74 6f28 2929 0a20 2020 2020 2020 2065  oto()).        e
-0001cd50: 6c69 6620 6973 696e 7374 616e 6365 2873  lif isinstance(s
-0001cd60: 656c 662e 7469 6d65 5f77 696e 646f 772c  elf.time_window,
-0001cd70: 2054 696d 6557 696e 646f 7753 6572 6965   TimeWindowSerie
-0001cd80: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-0001cd90: 7072 6f74 6f2e 7469 6d65 5f77 696e 646f  proto.time_windo
-0001cda0: 775f 7365 7269 6573 2e43 6f70 7946 726f  w_series.CopyFro
-0001cdb0: 6d28 7365 6c66 2e74 696d 655f 7769 6e64  m(self.time_wind
-0001cdc0: 6f77 2e5f 746f 5f70 726f 746f 2829 290a  ow._to_proto()).
-0001cdd0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0001cde0: 2020 2020 2020 2020 2020 6d73 6720 3d20            msg = 
-0001cdf0: 6622 496e 7661 6c69 6420 7469 6d65 5f77  f"Invalid time_w
-0001ce00: 696e 646f 7720 7479 7065 3a20 7b74 7970  indow type: {typ
-0001ce10: 6528 7365 6c66 2e74 696d 655f 7769 6e64  e(self.time_wind
-0001ce20: 6f77 297d 220a 2020 2020 2020 2020 2020  ow)}".          
-0001ce30: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
-0001ce40: 7228 6d73 6729 0a0a 2020 2020 2020 2020  r(msg)..        
-0001ce50: 7265 7475 726e 2070 726f 746f 0a0a 2020  return proto..  
-0001ce60: 2020 6465 6620 5f64 6566 6175 6c74 5f6e    def _default_n
-0001ce70: 616d 6528 0a20 2020 2020 2020 2073 656c  ame(.        sel
-0001ce80: 662c 2061 6767 7265 6761 7469 6f6e 5f69  f, aggregation_i
-0001ce90: 6e74 6572 7661 6c3a 2064 6174 6574 696d  nterval: datetim
-0001cea0: 652e 7469 6d65 6465 6c74 612c 2069 735f  e.timedelta, is_
-0001ceb0: 636f 6e74 696e 756f 7573 3a20 626f 6f6c  continuous: bool
-0001cec0: 2c20 6261 7463 685f 636f 6d70 6163 7469  , batch_compacti
-0001ced0: 6f6e 5f65 6e61 626c 6564 3a20 626f 6f6c  on_enabled: bool
-0001cee0: 0a20 2020 2029 202d 3e20 7374 723a 0a20  .    ) -> str:. 
-0001cef0: 2020 2020 2020 2077 696e 646f 775f 7370         window_sp
-0001cf00: 6563 203d 2073 656c 662e 7469 6d65 5f77  ec = self.time_w
-0001cf10: 696e 646f 772e 5f74 6f5f 7370 6563 2829  indow._to_spec()
-0001cf20: 0a20 2020 2020 2020 2063 6f6c 756d 6e5f  .        column_
-0001cf30: 6e61 6d65 203d 2066 227b 7365 6c66 2e63  name = f"{self.c
-0001cf40: 6f6c 756d 6e7d 5f7b 7365 6c66 2e66 756e  olumn}_{self.fun
-0001cf50: 6374 696f 6e2e 7265 736f 6c76 6564 5f6e  ction.resolved_n
-0001cf60: 616d 657d 5f7b 7769 6e64 6f77 5f73 7065  ame}_{window_spe
-0001cf70: 632e 7769 6e64 6f77 5f64 7572 6174 696f  c.window_duratio
-0001cf80: 6e5f 7374 7269 6e67 2829 7d22 0a0a 2020  n_string()}"..  
-0001cf90: 2020 2020 2020 6966 206e 6f74 2062 6174        if not bat
-0001cfa0: 6368 5f63 6f6d 7061 6374 696f 6e5f 656e  ch_compaction_en
-0001cfb0: 6162 6c65 643a 0a20 2020 2020 2020 2020  abled:.         
-0001cfc0: 2020 2061 6767 5f69 6e74 6572 7661 6c5f     agg_interval_
-0001cfd0: 6e61 6d65 203d 2066 6561 7475 7265 5f76  name = feature_v
-0001cfe0: 6965 775f 7574 696c 732e 636f 6e73 7472  iew_utils.constr
-0001cff0: 7563 745f 6167 6772 6567 6174 696f 6e5f  uct_aggregation_
-0001d000: 696e 7465 7276 616c 5f6e 616d 6528 0a20  interval_name(. 
-0001d010: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0001d020: 696d 655f 7574 696c 732e 7469 6d65 6465  ime_utils.timede
-0001d030: 6c74 615f 746f 5f70 726f 746f 2861 6767  lta_to_proto(agg
-0001d040: 7265 6761 7469 6f6e 5f69 6e74 6572 7661  regation_interva
-0001d050: 6c29 2c20 6973 5f63 6f6e 7469 6e75 6f75  l), is_continuou
-0001d060: 730a 2020 2020 2020 2020 2020 2020 290a  s.            ).
-0001d070: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
-0001d080: 6d6e 5f6e 616d 6520 3d20 6622 7b63 6f6c  mn_name = f"{col
-0001d090: 756d 6e5f 6e61 6d65 7d5f 7b61 6767 5f69  umn_name}_{agg_i
-0001d0a0: 6e74 6572 7661 6c5f 6e61 6d65 7d22 0a0a  nterval_name}"..
-0001d0b0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-0001d0c0: 7461 6e63 6528 7365 6c66 2e74 696d 655f  tance(self.time_
-0001d0d0: 7769 6e64 6f77 2c20 5469 6d65 5769 6e64  window, TimeWind
-0001d0e0: 6f77 5365 7269 6573 293a 0a20 2020 2020  owSeries):.     
-0001d0f0: 2020 2020 2020 2063 6f6c 756d 6e5f 6e61         column_na
-0001d100: 6d65 203d 2066 227b 636f 6c75 6d6e 5f6e  me = f"{column_n
-0001d110: 616d 657d 5f73 6572 6965 735f 7b77 696e  ame}_series_{win
-0001d120: 646f 775f 7370 6563 2e77 696e 646f 775f  dow_spec.window_
-0001d130: 7365 7269 6573 5f73 7461 7274 5f73 7472  series_start_str
-0001d140: 696e 6728 297d 5f7b 7769 6e64 6f77 5f73  ing()}_{window_s
-0001d150: 7065 632e 7769 6e64 6f77 5f73 6572 6965  pec.window_serie
-0001d160: 735f 656e 645f 7374 7269 6e67 2829 7d5f  s_end_string()}_
-0001d170: 7b77 696e 646f 775f 7370 6563 2e73 7465  {window_spec.ste
-0001d180: 705f 7369 7a65 5f73 7472 696e 6728 297d  p_size_string()}
-0001d190: 220a 2020 2020 2020 2020 656c 7365 3a0a  ".        else:.
-0001d1a0: 2020 2020 2020 2020 2020 2020 6966 2077              if w
-0001d1b0: 696e 646f 775f 7370 6563 2e6f 6666 7365  indow_spec.offse
-0001d1c0: 745f 7374 7269 6e67 2829 3a0a 2020 2020  t_string():.    
-0001d1d0: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
-0001d1e0: 6d6e 5f6e 616d 6520 3d20 6622 7b63 6f6c  mn_name = f"{col
-0001d1f0: 756d 6e5f 6e61 6d65 7d5f 7b77 696e 646f  umn_name}_{windo
-0001d200: 775f 7370 6563 2e6f 6666 7365 745f 7374  w_spec.offset_st
-0001d210: 7269 6e67 2829 7d22 0a20 2020 2020 2020  ring()}".       
-0001d220: 2063 6f6c 756d 6e5f 6e61 6d65 203d 2063   column_name = c
-0001d230: 6f6c 756d 6e5f 6e61 6d65 2e72 6570 6c61  olumn_name.repla
-0001d240: 6365 2822 2022 2c20 2222 290a 0a20 2020  ce(" ", "")..   
-0001d250: 2020 2020 2072 6574 7572 6e20 636f 6c75       return colu
-0001d260: 6d6e 5f6e 616d 650a 0a0a 2320 436f 6d70  mn_name...# Comp
-0001d270: 6f73 6974 6520 7479 7065 732e 0a4f 6e6c  osite types..Onl
-0001d280: 696e 6553 746f 7265 5479 7065 7320 3d20  ineStoreTypes = 
-0001d290: 556e 696f 6e5b 4479 6e61 6d6f 436f 6e66  Union[DynamoConf
-0001d2a0: 6967 2c20 5265 6469 7343 6f6e 6669 672c  ig, RedisConfig,
-0001d2b0: 2042 6967 7461 626c 6543 6f6e 6669 675d   BigtableConfig]
-0001d2c0: 0a43 6f6d 7075 7465 436f 6e66 6967 5479  .ComputeConfigTy
-0001d2d0: 7065 7320 3d20 556e 696f 6e5b 0a20 2020  pes = Union[.   
-0001d2e0: 205f 4465 6661 756c 7443 6c75 7374 6572   _DefaultCluster
-0001d2f0: 436f 6e66 6967 2c0a 2020 2020 4461 7461  Config,.    Data
-0001d300: 6272 6963 6b73 436c 7573 7465 7243 6f6e  bricksClusterCon
-0001d310: 6669 672c 0a20 2020 2045 4d52 436c 7573  fig,.    EMRClus
-0001d320: 7465 7243 6f6e 6669 672c 0a20 2020 2044  terConfig,.    D
-0001d330: 6174 6162 7269 636b 734a 736f 6e43 6c75  atabricksJsonClu
-0001d340: 7374 6572 436f 6e66 6967 2c0a 2020 2020  sterConfig,.    
-0001d350: 4461 7461 7072 6f63 4a73 6f6e 436c 7573  DataprocJsonClus
-0001d360: 7465 7243 6f6e 6669 672c 0a20 2020 2045  terConfig,.    E
-0001d370: 4d52 4a73 6f6e 436c 7573 7465 7243 6f6e  MRJsonClusterCon
-0001d380: 6669 672c 0a20 2020 2052 6966 7442 6174  fig,.    RiftBat
-0001d390: 6368 436f 6e66 6967 2c0a 5d0a            chConfig,.].
+0001c9d0: 636f 6d70 6163 7469 6f6e 5f65 6e61 626c  compaction_enabl
+0001c9e0: 6564 3a20 626f 6f6c 203d 2046 616c 7365  ed: bool = False
+0001c9f0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+0001ca00: 7072 6f74 6f20 3d20 6665 6174 7572 655f  proto = feature_
+0001ca10: 7669 6577 5f70 6232 2e46 6561 7475 7265  view_pb2.Feature
+0001ca20: 4167 6772 6567 6174 696f 6e28 0a20 2020  Aggregation(.   
+0001ca30: 2020 2020 2020 2020 206e 616d 653d 7365           name=se
+0001ca40: 6c66 2e6e 616d 650a 2020 2020 2020 2020  lf.name.        
+0001ca50: 2020 2020 6966 2073 656c 662e 6e61 6d65      if self.name
+0001ca60: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0001ca70: 6520 7365 6c66 2e5f 6465 6661 756c 745f  e self._default_
+0001ca80: 6e61 6d65 2861 6767 7265 6761 7469 6f6e  name(aggregation
+0001ca90: 5f69 6e74 6572 7661 6c2c 2069 735f 636f  _interval, is_co
+0001caa0: 6e74 696e 756f 7573 2c20 636f 6d70 6163  ntinuous, compac
+0001cab0: 7469 6f6e 5f65 6e61 626c 6564 292c 0a20  tion_enabled),. 
+0001cac0: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
+0001cad0: 6e3d 7365 6c66 2e63 6f6c 756d 6e2c 0a20  n=self.column,. 
+0001cae0: 2020 2020 2020 2020 2020 2066 756e 6374             funct
+0001caf0: 696f 6e3d 7365 6c66 2e66 756e 6374 696f  ion=self.functio
+0001cb00: 6e2e 6261 7365 5f6e 616d 652c 0a20 2020  n.base_name,.   
+0001cb10: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0001cb20: 666f 7220 6b2c 2076 2069 6e20 7365 6c66  for k, v in self
+0001cb30: 2e66 756e 6374 696f 6e2e 7061 7261 6d73  .function.params
+0001cb40: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+0001cb50: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+0001cb60: 6e63 6528 762c 2069 6e74 293a 0a20 2020  nce(v, int):.   
+0001cb70: 2020 2020 2020 2020 2020 2020 2070 726f               pro
+0001cb80: 746f 2e66 756e 6374 696f 6e5f 7061 7261  to.function_para
+0001cb90: 6d73 5b6b 5d2e 436f 7079 4672 6f6d 2866  ms[k].CopyFrom(f
+0001cba0: 6561 7475 7265 5f76 6965 775f 7062 322e  eature_view_pb2.
+0001cbb0: 5061 7261 6d56 616c 7565 2869 6e74 3634  ParamValue(int64
+0001cbc0: 5f76 616c 7565 3d76 2929 0a20 2020 2020  _value=v)).     
+0001cbd0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0001cbe0: 2020 2020 2020 2020 2020 2020 2070 726f               pro
+0001cbf0: 746f 2e66 756e 6374 696f 6e5f 7061 7261  to.function_para
+0001cc00: 6d73 5b6b 5d2e 436f 7079 4672 6f6d 2866  ms[k].CopyFrom(f
+0001cc10: 6561 7475 7265 5f76 6965 775f 7062 322e  eature_view_pb2.
+0001cc20: 5061 7261 6d56 616c 7565 2864 6f75 626c  ParamValue(doubl
+0001cc30: 655f 7661 6c75 653d 7629 290a 0a20 2020  e_value=v))..   
+0001cc40: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+0001cc50: 6365 2873 656c 662e 7469 6d65 5f77 696e  ce(self.time_win
+0001cc60: 646f 772c 2054 696d 6557 696e 646f 7729  dow, TimeWindow)
+0001cc70: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+0001cc80: 6f74 6f2e 7469 6d65 5f77 696e 646f 772e  oto.time_window.
+0001cc90: 436f 7079 4672 6f6d 2873 656c 662e 7469  CopyFrom(self.ti
+0001cca0: 6d65 5f77 696e 646f 772e 5f74 6f5f 7072  me_window._to_pr
+0001ccb0: 6f74 6f28 2929 0a20 2020 2020 2020 2065  oto()).        e
+0001ccc0: 6c69 6620 6973 696e 7374 616e 6365 2873  lif isinstance(s
+0001ccd0: 656c 662e 7469 6d65 5f77 696e 646f 772c  elf.time_window,
+0001cce0: 204c 6966 6574 696d 6557 696e 646f 7729   LifetimeWindow)
+0001ccf0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+0001cd00: 6f74 6f2e 6c69 6665 7469 6d65 5f77 696e  oto.lifetime_win
+0001cd10: 646f 772e 436f 7079 4672 6f6d 2873 656c  dow.CopyFrom(sel
+0001cd20: 662e 7469 6d65 5f77 696e 646f 772e 5f74  f.time_window._t
+0001cd30: 6f5f 7072 6f74 6f28 2929 0a20 2020 2020  o_proto()).     
+0001cd40: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
+0001cd50: 6365 2873 656c 662e 7469 6d65 5f77 696e  ce(self.time_win
+0001cd60: 646f 772c 2054 696d 6557 696e 646f 7753  dow, TimeWindowS
+0001cd70: 6572 6965 7329 3a0a 2020 2020 2020 2020  eries):.        
+0001cd80: 2020 2020 7072 6f74 6f2e 7469 6d65 5f77      proto.time_w
+0001cd90: 696e 646f 775f 7365 7269 6573 2e43 6f70  indow_series.Cop
+0001cda0: 7946 726f 6d28 7365 6c66 2e74 696d 655f  yFrom(self.time_
+0001cdb0: 7769 6e64 6f77 2e5f 746f 5f70 726f 746f  window._to_proto
+0001cdc0: 2829 290a 2020 2020 2020 2020 656c 7365  ()).        else
+0001cdd0: 3a0a 2020 2020 2020 2020 2020 2020 6d73  :.            ms
+0001cde0: 6720 3d20 6622 496e 7661 6c69 6420 7469  g = f"Invalid ti
+0001cdf0: 6d65 5f77 696e 646f 7720 7479 7065 3a20  me_window type: 
+0001ce00: 7b74 7970 6528 7365 6c66 2e74 696d 655f  {type(self.time_
+0001ce10: 7769 6e64 6f77 297d 220a 2020 2020 2020  window)}".      
+0001ce20: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
+0001ce30: 4572 726f 7228 6d73 6729 0a0a 2020 2020  Error(msg)..    
+0001ce40: 2020 2020 7265 7475 726e 2070 726f 746f      return proto
+0001ce50: 0a0a 2020 2020 6465 6620 5f64 6566 6175  ..    def _defau
+0001ce60: 6c74 5f6e 616d 6528 0a20 2020 2020 2020  lt_name(.       
+0001ce70: 2073 656c 662c 2061 6767 7265 6761 7469   self, aggregati
+0001ce80: 6f6e 5f69 6e74 6572 7661 6c3a 2064 6174  on_interval: dat
+0001ce90: 6574 696d 652e 7469 6d65 6465 6c74 612c  etime.timedelta,
+0001cea0: 2069 735f 636f 6e74 696e 756f 7573 3a20   is_continuous: 
+0001ceb0: 626f 6f6c 2c20 636f 6d70 6163 7469 6f6e  bool, compaction
+0001cec0: 5f65 6e61 626c 6564 3a20 626f 6f6c 0a20  _enabled: bool. 
+0001ced0: 2020 2029 202d 3e20 7374 723a 0a20 2020     ) -> str:.   
+0001cee0: 2020 2020 2077 696e 646f 775f 7370 6563       window_spec
+0001cef0: 203d 2073 656c 662e 7469 6d65 5f77 696e   = self.time_win
+0001cf00: 646f 772e 5f74 6f5f 7370 6563 2829 0a20  dow._to_spec(). 
+0001cf10: 2020 2020 2020 2063 6f6c 756d 6e5f 6e61         column_na
+0001cf20: 6d65 203d 2066 227b 7365 6c66 2e63 6f6c  me = f"{self.col
+0001cf30: 756d 6e7d 5f7b 7365 6c66 2e66 756e 6374  umn}_{self.funct
+0001cf40: 696f 6e2e 7265 736f 6c76 6564 5f6e 616d  ion.resolved_nam
+0001cf50: 657d 5f7b 7769 6e64 6f77 5f73 7065 632e  e}_{window_spec.
+0001cf60: 7769 6e64 6f77 5f64 7572 6174 696f 6e5f  window_duration_
+0001cf70: 7374 7269 6e67 2829 7d22 0a0a 2020 2020  string()}"..    
+0001cf80: 2020 2020 6966 206e 6f74 2063 6f6d 7061      if not compa
+0001cf90: 6374 696f 6e5f 656e 6162 6c65 643a 0a20  ction_enabled:. 
+0001cfa0: 2020 2020 2020 2020 2020 2061 6767 5f69             agg_i
+0001cfb0: 6e74 6572 7661 6c5f 6e61 6d65 203d 2066  nterval_name = f
+0001cfc0: 6561 7475 7265 5f76 6965 775f 7574 696c  eature_view_util
+0001cfd0: 732e 636f 6e73 7472 7563 745f 6167 6772  s.construct_aggr
+0001cfe0: 6567 6174 696f 6e5f 696e 7465 7276 616c  egation_interval
+0001cff0: 5f6e 616d 6528 0a20 2020 2020 2020 2020  _name(.         
+0001d000: 2020 2020 2020 2074 696d 655f 7574 696c         time_util
+0001d010: 732e 7469 6d65 6465 6c74 615f 746f 5f70  s.timedelta_to_p
+0001d020: 726f 746f 2861 6767 7265 6761 7469 6f6e  roto(aggregation
+0001d030: 5f69 6e74 6572 7661 6c29 2c20 6973 5f63  _interval), is_c
+0001d040: 6f6e 7469 6e75 6f75 730a 2020 2020 2020  ontinuous.      
+0001d050: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001d060: 2020 2020 636f 6c75 6d6e 5f6e 616d 6520      column_name 
+0001d070: 3d20 6622 7b63 6f6c 756d 6e5f 6e61 6d65  = f"{column_name
+0001d080: 7d5f 7b61 6767 5f69 6e74 6572 7661 6c5f  }_{agg_interval_
+0001d090: 6e61 6d65 7d22 0a0a 2020 2020 2020 2020  name}"..        
+0001d0a0: 6966 2069 7369 6e73 7461 6e63 6528 7365  if isinstance(se
+0001d0b0: 6c66 2e74 696d 655f 7769 6e64 6f77 2c20  lf.time_window, 
+0001d0c0: 5469 6d65 5769 6e64 6f77 5365 7269 6573  TimeWindowSeries
+0001d0d0: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+0001d0e0: 6f6c 756d 6e5f 6e61 6d65 203d 2066 227b  olumn_name = f"{
+0001d0f0: 636f 6c75 6d6e 5f6e 616d 657d 5f73 6572  column_name}_ser
+0001d100: 6965 735f 7b77 696e 646f 775f 7370 6563  ies_{window_spec
+0001d110: 2e77 696e 646f 775f 7365 7269 6573 5f73  .window_series_s
+0001d120: 7461 7274 5f73 7472 696e 6728 297d 5f7b  tart_string()}_{
+0001d130: 7769 6e64 6f77 5f73 7065 632e 7769 6e64  window_spec.wind
+0001d140: 6f77 5f73 6572 6965 735f 656e 645f 7374  ow_series_end_st
+0001d150: 7269 6e67 2829 7d5f 7b77 696e 646f 775f  ring()}_{window_
+0001d160: 7370 6563 2e73 7465 705f 7369 7a65 5f73  spec.step_size_s
+0001d170: 7472 696e 6728 297d 220a 2020 2020 2020  tring()}".      
+0001d180: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0001d190: 2020 2020 6966 2077 696e 646f 775f 7370      if window_sp
+0001d1a0: 6563 2e6f 6666 7365 745f 7374 7269 6e67  ec.offset_string
+0001d1b0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+0001d1c0: 2020 2020 636f 6c75 6d6e 5f6e 616d 6520      column_name 
+0001d1d0: 3d20 6622 7b63 6f6c 756d 6e5f 6e61 6d65  = f"{column_name
+0001d1e0: 7d5f 7b77 696e 646f 775f 7370 6563 2e6f  }_{window_spec.o
+0001d1f0: 6666 7365 745f 7374 7269 6e67 2829 7d22  ffset_string()}"
+0001d200: 0a20 2020 2020 2020 2063 6f6c 756d 6e5f  .        column_
+0001d210: 6e61 6d65 203d 2063 6f6c 756d 6e5f 6e61  name = column_na
+0001d220: 6d65 2e72 6570 6c61 6365 2822 2022 2c20  me.replace(" ", 
+0001d230: 2222 290a 0a20 2020 2020 2020 2072 6574  "")..        ret
+0001d240: 7572 6e20 636f 6c75 6d6e 5f6e 616d 650a  urn column_name.
+0001d250: 0a0a 2320 436f 6d70 6f73 6974 6520 7479  ..# Composite ty
+0001d260: 7065 732e 0a4f 6e6c 696e 6553 746f 7265  pes..OnlineStore
+0001d270: 5479 7065 7320 3d20 556e 696f 6e5b 4479  Types = Union[Dy
+0001d280: 6e61 6d6f 436f 6e66 6967 2c20 5265 6469  namoConfig, Redi
+0001d290: 7343 6f6e 6669 672c 2042 6967 7461 626c  sConfig, Bigtabl
+0001d2a0: 6543 6f6e 6669 675d 0a43 6f6d 7075 7465  eConfig].Compute
+0001d2b0: 436f 6e66 6967 5479 7065 7320 3d20 556e  ConfigTypes = Un
+0001d2c0: 696f 6e5b 0a20 2020 205f 4465 6661 756c  ion[.    _Defaul
+0001d2d0: 7443 6c75 7374 6572 436f 6e66 6967 2c0a  tClusterConfig,.
+0001d2e0: 2020 2020 4461 7461 6272 6963 6b73 436c      DatabricksCl
+0001d2f0: 7573 7465 7243 6f6e 6669 672c 0a20 2020  usterConfig,.   
+0001d300: 2045 4d52 436c 7573 7465 7243 6f6e 6669   EMRClusterConfi
+0001d310: 672c 0a20 2020 2044 6174 6162 7269 636b  g,.    Databrick
+0001d320: 734a 736f 6e43 6c75 7374 6572 436f 6e66  sJsonClusterConf
+0001d330: 6967 2c0a 2020 2020 4461 7461 7072 6f63  ig,.    Dataproc
+0001d340: 4a73 6f6e 436c 7573 7465 7243 6f6e 6669  JsonClusterConfi
+0001d350: 672c 0a20 2020 2045 4d52 4a73 6f6e 436c  g,.    EMRJsonCl
+0001d360: 7573 7465 7243 6f6e 6669 672c 0a20 2020  usterConfig,.   
+0001d370: 2052 6966 7442 6174 6368 436f 6e66 6967   RiftBatchConfig
+0001d380: 2c0a 5d0a                                ,.].
```

### Comparing `tecton-0.9.0rc4/tecton/framework/data_frame.py` & `tecton-0.9.1/tecton/framework/data_frame.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/framework/data_source.py` & `tecton-0.9.1/tecton/framework/data_source.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from tecton_core import conf
 from tecton_core import id_helper
 from tecton_core import specs
 from tecton_core.compute_mode import BatchComputeMode
 from tecton_core.compute_mode import ComputeMode
 from tecton_core.compute_mode import default_batch_compute_mode
 from tecton_core.compute_mode import offline_retrieval_compute_mode
+from tecton_core.specs.utils import get_field_or_none
 from tecton_proto.args import basic_info_pb2
 from tecton_proto.args import fco_args_pb2
 from tecton_proto.args import virtual_data_source_pb2 as virtual_data_source__args_pb2
 from tecton_proto.common import data_source_type_pb2
 from tecton_proto.common import fco_locator_pb2
 from tecton_proto.common import framework_version_pb2
 from tecton_proto.common import schema_container_pb2
@@ -235,14 +236,60 @@
             return self._args.file_ds_config.common_args.data_delay.ToTimedelta()
         elif self._args.type == data_source_type_pb2.DataSourceType.PUSH_NO_BATCH:
             return None
         else:
             msg = f"Invalid batch source args: {self._args}"
             raise ValueError(msg)
 
+    def _rebuild_spec_with_schema(self) -> specs.DataSourceSpec:
+        # This should only ever be called on a remote DS which is missing schema!
+        def _raise_internal_validation_error(msg: str):
+            full_message = f"Error rebuilding spec schema: {msg}"
+            raise errors.TectonInternalError(full_message)
+
+        if not self._is_valid:
+            _raise_internal_validation_error("Object is not validated")
+        if self._spec.schema is not None:
+            _raise_internal_validation_error("Schema is already defined")
+        if self._is_local_object:
+            _raise_internal_validation_error("Refusing to rebuild schema for a local object")
+
+        fco_validation_args = self._build_fco_validation_args()
+        validation_args = fco_validation_args.virtual_data_source
+        virtual_data_source_args = get_field_or_none(validation_args, "args")
+        if virtual_data_source_args is None:
+            _raise_internal_validation_error("Missing virtual data source args")
+
+        batch_schema = None
+        stream_schema = None
+        if self._spec.batch_source:
+            post_processor = getattr(self._spec.batch_source, "post_processor", None)
+            function = getattr(self._spec.batch_source, "function", None)
+            batch_schema = spark_api.derive_batch_schema(
+                virtual_data_source_args,
+                post_processor,
+                function,
+            )
+        if self._spec.stream_source:
+            post_processor = getattr(self._spec.stream_source, "post_processor", None)
+            function = getattr(self._spec.stream_source, "function", None)
+            stream_schema = spark_api.derive_stream_schema(
+                virtual_data_source_args,
+                post_processor,
+                function,
+            )
+        supplement = specs.DataSourceSpecArgsSupplement(
+            batch_schema=batch_schema,
+            stream_schema=stream_schema,
+        )
+        return specs.DataSourceSpec.from_args_proto(
+            virtual_data_source_args,
+            supplement,
+        )
+
 
 @attrs.define(eq=False)
 class BatchSource(DataSource):
     """A Tecton BatchSource, used to read batch data into Tecton for use in a BatchFeatureView.
 
     Example of a BatchSource declaration:
```

### Comparing `tecton-0.9.0rc4/tecton/framework/dataset.py` & `tecton-0.9.1/tecton/framework/dataset.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/framework/entity.py` & `tecton-0.9.1/tecton/framework/entity.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/framework/feature_service.py` & `tecton-0.9.1/tecton/framework/feature_service.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/framework/feature_view.py` & `tecton-0.9.1/tecton/framework/feature_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -560,21 +560,36 @@
         )
 
         return obj
 
     def _get_dependent_objects(self, include_indirect_dependencies: bool) -> List[base_tecton_object.BaseTectonObject]:
         return list(self.sources) + list(self.entities) + list(self.transformations)
 
+    def _build_ds_specs_with_derived_schema(self) -> List[specs.DataSourceSpec]:
+        specs_with_schema = []
+        for ds in self.sources:
+            ds_spec = ds._spec
+            ds_spec_requires_schema = ds._is_valid and not ds._is_local_object and not ds_spec.schema
+            if self._batch_compute_mode == BatchComputeMode.SPARK and ds_spec_requires_schema:
+                # A DataSource may not have derived schema IFF it was applied without a FeatureView
+                # In those cases, NDD FeatureView definitions will fail unless we force the schema derivation here.
+                #
+                # See https://tecton.atlassian.net/browse/TEC-18736 for additional context
+                specs_with_schema.append(ds._rebuild_spec_with_schema())
+            else:
+                specs_with_schema.append(ds._spec)
+        return specs_with_schema
+
     def _derive_schemas(self) -> _Schemas:
         assert all(
             obj._is_valid for obj in self.transformations + self.sources
         ), "_derive_schemas expects that dependent objects have been validated."
         return self._derive_schemas_with_specs(
             transformation_specs=[transformation._spec for transformation in self.transformations],
-            data_source_specs=[source._spec for source in self.sources],
+            data_source_specs=self._build_ds_specs_with_derived_schema(),
         )
 
     def _derive_schemas_with_specs(
         self,
         transformation_specs: Optional[List[specs.TransformationSpec]],
         data_source_specs: Optional[List[specs.DataSourceSpec]],
     ) -> _Schemas:
@@ -598,15 +613,15 @@
         )
 
         if has_legacy_snowflake_hacks:
             for column in materialization_schema.columns:
                 column.name = column.name.upper()
 
         online_batch_table_format = None
-        if self._args.materialized_feature_view_args.batch_compaction_enabled:
+        if self._args.materialized_feature_view_args.compaction_enabled:
             online_batch_table_format = schema_derivation_utils.compute_batch_table_format(self._args, view_schema)
 
         return _Schemas(
             view_schema=view_schema,
             materialization_schema=materialization_schema,
             online_batch_table_format=online_batch_table_format,
         )
@@ -1132,15 +1147,15 @@
                 raise errors.FV_WITH_INC_BACKFILLS_GET_MATERIALIZED_FEATURES_MOCK_DATA(
                     self.name, self.get_partial_aggregates.__name__
                 )
 
         if not self._feature_definition.is_temporal_aggregate:
             raise errors.GET_PARTIAL_AGGREGATES_UNSUPPORTED_NON_AGGREGATE()
 
-        if self._feature_definition.batch_compaction_enabled:
+        if self._feature_definition.compaction_enabled:
             raise errors.GET_PARTIAL_AGGREGATES_UNSUPPORTED_COMPACTED()
 
         if any(ds._data_source_type == DataSourceType.PUSH_NO_BATCH for ds in self.sources):
             msg = "The `get_partial_aggregates()` method is currently unsupported for Feature Views that are backed by a PushSource without a batch_config."
             raise TectonValidationError(msg)
 
         if entities is not None:
@@ -1234,14 +1249,19 @@
         else:
             feature_definition = self._feature_definition
 
         if any(ds._data_source_type == DataSourceType.PUSH_NO_BATCH for ds in self.sources) and len(mock_inputs) == 0:
             msg = "The `run_transformation()` method is currently unsupported for Feature Views backed by a StreamSource without a batch_config unless mock_inputs are provided."
             raise TectonValidationError(msg)
 
+        compute_mode = offline_retrieval_compute_mode(compute_mode)
+
+        if compute_mode != ComputeMode.SPARK and compute_mode != ComputeMode.RIFT:
+            raise errors.RUN_TRANSFORMATION_UNSUPPORTED
+
         if start_time is None or end_time is None:
             msg = "run_transformation() requires start_time and end_time to be set."
             raise TypeError(msg)
 
         if start_time >= end_time:
             raise core_errors.START_TIME_NOT_BEFORE_END_TIME(start_time, end_time)
 
@@ -1250,16 +1270,14 @@
             feature_definition.is_incremental_backfill
             and time_range != feature_definition.batch_materialization_schedule
         ):
             logger.warning(
                 f"run_transformation() time range ({start_time}, {end_time}) is not equivalent to the batch_schedule: {feature_definition.batch_materialization_schedule}. This may lead to incorrect feature values since feature views with incremental_backfills typically implicitly rely on the materialization range being equivalent to the batch_schedule."
             )
 
-        compute_mode = offline_retrieval_compute_mode(compute_mode)
-
         dialect = compute_mode.default_dialect()
 
         mock_data_sources = {}
         if mock_inputs:
             mock_data_sources = mock_source_utils.convert_mock_inputs_to_mock_sources(
                 dialect, compute_mode, feature_definition, mock_inputs
             )
@@ -1376,18 +1394,15 @@
             feature_definition = self._create_unvalidated_feature_definition(resolved_mock_inputs)
         else:
             feature_definition = self._feature_definition
 
         if feature_definition.is_temporal and aggregation_level is not None:
             raise errors.FV_UNSUPPORTED_AGGREGATION
 
-        if (
-            feature_definition.batch_compaction_enabled
-            and aggregation_level == run_api_consts.AGGREGATION_LEVEL_PARTIAL
-        ):
+        if feature_definition.compaction_enabled and aggregation_level == run_api_consts.AGGREGATION_LEVEL_PARTIAL:
             raise errors.RUN_API_PARTIAL_LEVEL_UNSUPPORTED_FOR_COMPACTION
 
         aggregation_level = run_api.validate_and_get_aggregation_level(feature_definition, aggregation_level)
 
         run_api.maybe_warn_incorrect_time_range_size(feature_definition, start_time, end_time, aggregation_level)
 
         compute_mode = offline_retrieval_compute_mode(compute_mode)
@@ -1819,15 +1834,15 @@
         max_backfill_interval: Optional[datetime.timedelta] = None,
         incremental_backfills: bool = False,
         schema: Optional[List[types.Field]] = None,
         run_transformation_validation: Optional[bool] = None,
         options: Optional[Dict[str, str]] = None,
         tecton_materialization_runtime: Optional[str] = None,
         cache_config: Optional[configs.CacheConfig] = None,
-        batch_compaction_enabled: bool = False,
+        compaction_enabled: bool = False,
         environment: Optional[str] = None,
     ):
         from tecton.cli import repo_utils as cli_common
 
         if online_store is None:
             online_store = repo_config.get_batch_feature_view_defaults().online_store
 
@@ -1912,15 +1927,15 @@
             output_stream=None,
             incremental_backfills=incremental_backfills,
             schema=schema,
             run_transformation_validation=run_transformation_validation,
             options=options,
             tecton_materialization_runtime=tecton_materialization_runtime,
             cache_config=cache_config,
-            batch_compaction_enabled=batch_compaction_enabled,
+            compaction_enabled=compaction_enabled,
             environment=environment,
         )
 
         info = base_tecton_object.TectonObjectInfo.from_args_proto(args.info, args.feature_view_id)
 
         data_sources = tuple(
             source.source if isinstance(source, filtered_source.FilteredSource) else source for source in sources
@@ -1976,15 +1991,16 @@
     max_batch_aggregation_interval: Optional[datetime.timedelta] = None,
     incremental_backfills: bool = False,
     schema: Optional[List[types.Field]] = None,
     run_transformation_validation: Optional[bool] = None,
     options: Optional[Dict[str, str]] = None,
     tecton_materialization_runtime: Optional[str] = None,
     cache_config: Optional[configs.CacheConfig] = None,
-    batch_compaction_enabled: bool = False,
+    batch_compaction_enabled: Optional[bool] = None,
+    compaction_enabled: Optional[bool] = None,
     environment: Optional[str] = None,
 ):
     """Declare a Batch Feature View.
 
     :param mode: Whether the annotated function is a pipeline function ("pipeline" mode) or a transformation mode
         ("spark_sql", "pyspark", "snowflake_sql", "snowpark", "python", or "pandas"). For the non-pipeline mode, an
         inferred transformation will also be registered.
@@ -2050,17 +2066,18 @@
         set. Skipping query validation can be useful to speed up tecton plan/apply or for Feature Views that have issues
         with Tecton's validation (e.g. some pip dependencies). Default is True for Spark and Snowflake Feature Views and
         False for Python and Pandas Feature Views.
     :param tecton_materialization_runtime: Version of `tecton` package used by your job cluster.
     :param cache_config: Cache config for the Feature View. Including this option enables the feature server to use the cache
         when retrieving features for this feature view. Will only be respected if the feature service containing this feature
         view has `enable_online_caching` set to `True`.
-    :param batch_compaction_enabled: (Private preview) If `True`, Tecton will run a compaction job after each batch
+    :param batch_compaction_enabled: Deprecated: Please use `compaction_enabled` instead which has the exact same usage.
+     :param compaction_enabled: (Private preview) If `True`, Tecton will run a compaction job after each batch
         materialization job to write to the online store. This requires the use of Dynamo and uses the ImportTable API.
-        Becuase each batch job overwrites the online store, a larger compute cluster may be required.
+        Because each batch job overwrites the online store, a larger compute cluster may be required.
     :param environment: The custom environment in which materialization jobs will be run. Defaults to `None`, which means
         jobs will execute in the default Tecton environment.
 
     :return: An object of type :class:`tecton.BatchFeatureView`.
 
     Example BatchFeatureView declaration:
 
@@ -2136,14 +2153,20 @@
     """
 
     # TODO(deprecate_after=0.8): This warning can be completely removed in 0.9, so it can be deleted once the 0.8 branch is cut.
     if max_batch_aggregation_interval is not None:
         msg = "FeatureView.max_batch_aggregation_interval is deprecated and is no longer supported in 0.8. Please use max_backfill_interval instead. max_backfill_interval has the same semantics and is just a new name."
         raise ValueError(msg)
 
+    if batch_compaction_enabled is not None and compaction_enabled is not None:
+        msg = "FeatureView.batch_compaction_enabled is deprecated. Please use compaction_enabled instead. compaction_enabled has the same semantics and is just a new name."
+        raise TectonValidationError(msg)
+
+    compaction_enabled = compaction_enabled or batch_compaction_enabled or False
+
     def decorator(feature_view_function):
         return BatchFeatureView(
             name=name or feature_view_function.__name__,
             description=description,
             owner=owner,
             tags=tags,
             prevent_destroy=prevent_destroy,
@@ -2175,15 +2198,15 @@
             max_backfill_interval=max_backfill_interval,
             incremental_backfills=incremental_backfills,
             schema=schema,
             run_transformation_validation=run_transformation_validation,
             options=options,
             tecton_materialization_runtime=tecton_materialization_runtime,
             cache_config=cache_config,
-            batch_compaction_enabled=batch_compaction_enabled,
+            compaction_enabled=compaction_enabled,
             environment=environment,
         )
 
     return decorator
 
 
 @attrs.define(eq=False)
@@ -2240,16 +2263,16 @@
         max_backfill_interval: Optional[datetime.timedelta] = None,
         output_stream: Optional[configs.OutputStream] = None,
         schema: Optional[List[types.Field]] = None,
         run_transformation_validation: Optional[bool] = None,
         options: Optional[Dict[str, str]] = None,
         tecton_materialization_runtime: Optional[str] = None,
         cache_config: Optional[configs.CacheConfig] = None,
-        stream_compaction_enabled: bool = False,
-        batch_compaction_enabled: bool = False,
+        compaction_enabled: bool = False,
+        stream_tiling_enabled: bool = False,
         environment: Optional[str] = None,
     ):
         """Construct a StreamFeatureView.
 
         `init` should not be used directly, and instead :py:func:`tecton.stream_feature_view` decorator is recommended.
         """
         from tecton.cli import repo_utils as cli_common
@@ -2281,26 +2304,21 @@
         if stream_compute is None and not has_push_source:
             # The stream compute default should not be applied for Stream Feature Views with Push Sources, since they
             # don't have any stream compute.
             stream_compute = repo_config.get_stream_feature_view_defaults().stream_compute
 
         _validate_fv_input_count([source], feature_view_function)
 
-        if has_push_source:
-            # Stream Feature Views with Push Sources are mandatorily continuous-mode only.
-            stream_processing_mode_ = StreamProcessingMode.CONTINUOUS
-        elif batch_compaction_enabled:
-            # This is a Compacted stream feature view. We set defaults here for compacted feature views. The actual validations
-            # will be in the validation server.
-            if not stream_compaction_enabled:
-                stream_processing_mode_ = (
-                    stream_processing_mode or StreamProcessingMode.CONTINUOUS
-                )  # Default to continuous
-            else:
-                stream_processing_mode_ = stream_processing_mode or None
+        if stream_processing_mode is None:
+            stream_processing_mode_ = _compute_default_stream_processing_mode(
+                has_push_source,
+                aggregations,
+                compaction_enabled,
+                stream_tiling_enabled,
+            )
         else:
             if aggregations:
                 stream_processing_mode_ = stream_processing_mode or StreamProcessingMode.TIME_INTERVAL
             else:
                 stream_processing_mode_ = stream_processing_mode
 
         if feature_view_function:
@@ -2374,16 +2392,16 @@
             output_stream=output_stream,
             incremental_backfills=False,
             schema=schema,
             run_transformation_validation=run_transformation_validation,
             options=options,
             tecton_materialization_runtime=tecton_materialization_runtime,
             cache_config=cache_config,
-            stream_compaction_enabled=stream_compaction_enabled,
-            batch_compaction_enabled=batch_compaction_enabled,
+            stream_tiling_enabled=stream_tiling_enabled,
+            compaction_enabled=compaction_enabled,
             environment=environment,
         )
 
         info = base_tecton_object.TectonObjectInfo.from_args_proto(args.info, args.feature_view_id)
 
         data_sources = (source.source if isinstance(source, filtered_source.FilteredSource) else source,)
 
@@ -2460,16 +2478,18 @@
     max_batch_aggregation_interval: Optional[datetime.timedelta] = None,
     output_stream: Optional[configs.OutputStream] = None,
     schema: Optional[List[types.Field]] = None,
     options: Optional[Dict[str, str]] = None,
     run_transformation_validation: Optional[bool] = None,
     tecton_materialization_runtime: Optional[str] = None,
     cache_config: Optional[configs.CacheConfig] = None,
-    stream_compaction_enabled: bool = False,
-    batch_compaction_enabled: bool = False,
+    stream_compaction_enabled: Optional[bool] = None,
+    batch_compaction_enabled: Optional[bool] = None,
+    compaction_enabled: Optional[bool] = None,
+    stream_tiling_enabled: Optional[bool] = None,
     environment: Optional[str] = None,
 ):
     """Declare a Stream Feature View.
 
     :param mode: Whether the annotated function is a pipeline function ("pipeline" mode) or a transformation function ("spark_sql" or "pyspark" mode).
         For the non-pipeline mode, an inferred transformation will also be registered.
     :param source: The data source input to the feature view.
@@ -2530,16 +2550,18 @@
         set. Skipping query validation can be useful to speed up tecton plan/apply or for Feature Views that have issues
         with Tecton's validation (e.g. some pip dependencies). Default is True for Spark and Snowflake Feature Views and
         False for Python and Pandas Feature Views or Feature Views with Push Sources.
     :param tecton_materialization_runtime: Version of `tecton` package used by your job cluster.
     :param cache_config: Cache config for the Feature View. Including this option enables the feature server to use the cache
         when retrieving features for this feature view. Will only be respected if the feature service containing this feature
         view has `enable_online_caching` set to `True`.
-    :param stream_compaction_enabled: (Private preview) If `False`, Tecton transforms and writes all events from the stream to the online store (same as stream_processing_mode=``StreamProcessingMode.CONTINUOUS``) . If `True`, Tecton will store the partial aggregations of the events in the online store. Defaults to ``False``.
-    :param batch_compaction_enabled: (Private preview) If `True`, Tecton will run a compaction job after each batch
+    :param stream_compaction_enabled: Deprecated: Please use `stream_tiling_enabled` instead which has the exact same usage.
+    :param batch_compaction_enabled: Deprecated: Please use `compaction_enabled` instead which has the exact same usage.
+    :param stream_tiling_enabled: (Private preview) If `False`, Tecton transforms and writes all events from the stream to the online store (same as stream_processing_mode=``StreamProcessingMode.CONTINUOUS``) . If `True`, Tecton will store the partial aggregations of the events in the online store. Defaults to ``False``.
+    :param compaction_enabled: (Private preview) If `True`, Tecton will run a compaction job after each batch
         materialization job to write to the online store. This requires the use of Dynamo and uses the ImportTable API.
         Becuase each batch job overwrites the online store, a larger compute cluster may be required. This is required to be True if `stream_compaction_enabled` is True. Defaults to ``False``.
     :param environment: The custom environment in which materialization jobs will be run. Defaults to `None`, which means
         jobs will execute in the default Tecton environment.
 
     :return: An object of type :class:`tecton.StreamFeatureView`.
 
@@ -2616,14 +2638,26 @@
     """
 
     # TODO(deprecate_after=0.8): This warning can be completely removed in 0.9, so it can be deleted once the 0.8 branch is cut.
     if max_batch_aggregation_interval is not None:
         msg = "FeatureView.max_batch_aggregation_interval is deprecated and is no longer supported in 0.8. Please use max_backfill_interval instead. max_backfill_interval has the same semantics and is just a new name."
         raise ValueError(msg)
 
+    if batch_compaction_enabled is not None and compaction_enabled is not None:
+        msg = "FeatureView.batch_compaction_enabled is deprecated. Please use compaction_enabled instead. compaction_enabled has the same semantics and is just a new name."
+        raise TectonValidationError(msg)
+
+    compaction_enabled = compaction_enabled or batch_compaction_enabled or False
+
+    if stream_compaction_enabled is not None and stream_tiling_enabled is not None:
+        msg = "FeatureView.stream_compaction_enabled is deprecated. Please use stream_tiling_enabled instead. stream_tiling_enabled has the same semantics and is just a new name."
+        raise TectonValidationError(msg)
+
+    stream_tiling_enabled = stream_tiling_enabled or stream_compaction_enabled or False
+
     def decorator(feature_view_function):
         return StreamFeatureView(
             name=name or feature_view_function.__name__,
             description=description,
             owner=owner,
             tags=tags,
             prevent_destroy=prevent_destroy,
@@ -2657,16 +2691,16 @@
             max_backfill_interval=max_backfill_interval,
             output_stream=output_stream,
             schema=schema,
             options=options,
             run_transformation_validation=run_transformation_validation,
             tecton_materialization_runtime=tecton_materialization_runtime,
             cache_config=cache_config,
-            stream_compaction_enabled=stream_compaction_enabled,
-            batch_compaction_enabled=batch_compaction_enabled,
+            compaction_enabled=compaction_enabled,
+            stream_tiling_enabled=stream_tiling_enabled,
             environment=environment,
         )
 
     return decorator
 
 
 @attrs.define(eq=False)
@@ -4352,33 +4386,33 @@
     max_backfill_interval: Optional[datetime.timedelta] = None,
     output_stream: Optional[configs.OutputStream] = None,
     batch_trigger: Optional[BatchTriggerType] = None,
     schema: Optional[List[types.Field]] = None,
     options: Optional[Dict[str, str]] = None,
     tecton_materialization_runtime: Optional[str] = None,
     cache_config: Optional[configs.CacheConfig] = None,
-    stream_compaction_enabled: bool = False,
-    batch_compaction_enabled: bool = False,
+    compaction_enabled: bool = False,
+    stream_tiling_enabled: bool = False,
     environment: Optional[str] = None,
 ) -> feature_view__args_pb2.FeatureViewArgs:
     """Build feature view args proto for materialized feature views (i.e. batch and stream feature views)."""
     monitoring = configs.MonitoringConfig(
         monitor_freshness=monitor_freshness, expected_freshness=expected_feature_freshness, alert_email=alert_email
     )
 
     aggregation_protos = None
     if aggregations:
         is_continuous = stream_processing_mode == StreamProcessingMode.CONTINUOUS
-        if batch_compaction_enabled and stream_compaction_enabled and aggregation_interval:
+        if compaction_enabled and stream_tiling_enabled and aggregation_interval:
             raise errors.AGGREGATION_INTERVAL_SET_COMPACTION()
         else:
             if aggregation_interval is None:
                 aggregation_interval = datetime.timedelta(seconds=0)
         aggregation_protos = [
-            agg._to_proto(aggregation_interval, is_continuous, batch_compaction_enabled) for agg in aggregations
+            agg._to_proto(aggregation_interval, is_continuous, compaction_enabled) for agg in aggregations
         ]
 
     secondary_key_output_columns = (
         _create_secondary_key_output_columns(aggregations, aggregation_secondary_key)
         if aggregation_secondary_key
         else None
     )
@@ -4427,19 +4461,17 @@
             stream_processing_mode=stream_processing_mode.value if stream_processing_mode else None,
             aggregations=aggregation_protos,
             aggregation_interval=time_utils.timedelta_to_proto(aggregation_interval),
             schema=schema_proto,
             run_transformation_validation=run_transformation_validation,
             tecton_materialization_runtime=tecton_materialization_runtime,
             offline_store=offline_store._to_proto(),
-            stream_compaction_enabled=stream_compaction_enabled,
-            stream_compaction_tile_size=_compute_stream_compaction_tile_size(aggregations)
-            if stream_compaction_enabled
-            else None,
-            batch_compaction_enabled=batch_compaction_enabled,
+            stream_tiling_enabled=stream_tiling_enabled,
+            stream_tile_size=_compute_compacted_fv_stream_tile_size(aggregations) if stream_tiling_enabled else None,
+            compaction_enabled=compaction_enabled,
             environment=environment,
         ),
         options=options,
         cache_config=cache_config._to_proto() if cache_config else None,
     )
 
 
@@ -4474,22 +4506,22 @@
         else:
             msg = f"Unexpected time window type in agg args proto: {type(window)}"
             raise ValueError(msg)
         secondary_key_output_columns.append(output_col)
     return secondary_key_output_columns
 
 
-def _compute_stream_compaction_tile_size(
+def _compute_compacted_fv_stream_tile_size(
     aggregations: Optional[Sequence[configs.Aggregation]],
 ) -> Optional[duration_pb2.Duration]:
-    """Calculate stream compaction tile size.
+    """Calculate the compacted fv stream tile size.
 
-    Only applicable for fvs with stream_comapction_enabled=True. This calculates the tile sized used for the online stream table. Currently, this cannot be set by the user."""
+    Only applicable for fvs with stream_tiling_enabled=True. This calculates the tile size used for the online stream table. Currently, this cannot be set by the user."""
     if aggregations is None or len(aggregations) == 0:
-        msg = "Only feature views with aggregations can set a stream compaction tile size."
+        msg = "Only feature views with aggregations can set `stream_tiling_enabled`=True"
         raise ValueError(msg)
 
     relative_time_windows = []
     for agg in aggregations:
         if isinstance(agg.time_window, configs.TimeWindow):
             relative_time_windows.append(agg.time_window)
         elif isinstance(agg.time_window, configs.TimeWindowSeries):
@@ -4499,7 +4531,25 @@
         min_time_window = min([window.window_size for window in relative_time_windows])
         if min_time_window < timedelta(hours=1):
             return time_utils.timedelta_to_proto(timedelta(minutes=1))
         elif min_time_window < timedelta(hours=10):
             return time_utils.timedelta_to_proto(timedelta(minutes=5))
 
     return time_utils.timedelta_to_proto(timedelta(hours=1))
+
+
+def _compute_default_stream_processing_mode(
+    has_push_source: bool,
+    aggregations: Optional[Sequence[configs.Aggregation]],
+    compaction_enabled: bool,
+    stream_tiling_enabled: Optional[bool] = None,
+):
+    if has_push_source:
+        # Stream Feature Views with Push Sources default to continuous-mode only.
+        return StreamProcessingMode.CONTINUOUS
+    elif compaction_enabled and not stream_tiling_enabled:
+        # This is a Compacted stream feature view. We set defaults here for compacted feature views. The actual validations
+        # will be in the validation server.
+        return StreamProcessingMode.CONTINUOUS
+    elif aggregations:
+        StreamProcessingMode.TIME_INTERVAL
+    return None
```

### Comparing `tecton-0.9.0rc4/tecton/framework/filtered_source.py` & `tecton-0.9.1/tecton/framework/filtered_source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/framework/repo_config.py` & `tecton-0.9.1/tecton/framework/repo_config.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/framework/transformation.py` & `tecton-0.9.1/tecton/framework/transformation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/framework/utils.py` & `tecton-0.9.1/tecton/framework/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/framework/validation_mode.py` & `tecton-0.9.1/tecton/framework/validation_mode.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/framework/workspace.py` & `tecton-0.9.1/tecton/framework/workspace.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/identities/api_keys.py` & `tecton-0.9.1/tecton/identities/api_keys.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/identities/credentials.py` & `tecton-0.9.1/tecton/identities/credentials.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/identities/okta.py` & `tecton-0.9.1/tecton/identities/okta.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/pytest_tecton.py` & `tecton-0.9.1/tecton/pytest_tecton.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/snowflake_context.py` & `tecton-0.9.1/tecton/snowflake_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/tecton_context.py` & `tecton-0.9.1/tecton/tecton_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/types.py` & `tecton-0.9.1/tecton/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/dill/dill/__diff.py` & `tecton-0.9.1/tecton/vendor/dill/dill/__diff.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/dill/dill/__init__.py` & `tecton-0.9.1/tecton/vendor/dill/dill/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/dill/dill/_dill.py` & `tecton-0.9.1/tecton/vendor/dill/dill/_dill.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/dill/dill/_objects.py` & `tecton-0.9.1/tecton/vendor/dill/dill/_objects.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/dill/dill/detect.py` & `tecton-0.9.1/tecton/vendor/dill/dill/detect.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/dill/dill/info.py` & `tecton-0.9.1/tecton/vendor/dill/dill/info.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/dill/dill/objtypes.py` & `tecton-0.9.1/tecton/vendor/dill/dill/objtypes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/dill/dill/pointers.py` & `tecton-0.9.1/tecton/vendor/dill/dill/pointers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/dill/dill/settings.py` & `tecton-0.9.1/tecton/vendor/dill/dill/settings.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/dill/dill/source.py` & `tecton-0.9.1/tecton/vendor/dill/dill/source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/dill/dill/temp.py` & `tecton-0.9.1/tecton/vendor/dill/dill/temp.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/clientserver.py` & `tecton-0.9.1/tecton/vendor/pyspark/py4j/clientserver.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/compat.py` & `tecton-0.9.1/tecton/vendor/pyspark/py4j/compat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/finalizer.py` & `tecton-0.9.1/tecton/vendor/pyspark/py4j/finalizer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/java_collections.py` & `tecton-0.9.1/tecton/vendor/pyspark/py4j/java_collections.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/java_gateway.py` & `tecton-0.9.1/tecton/vendor/pyspark/py4j/java_gateway.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/protocol.py` & `tecton-0.9.1/tecton/vendor/pyspark/py4j/protocol.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/py4j/signals.py` & `tecton-0.9.1/tecton/vendor/pyspark/py4j/signals.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/__init__.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/_globals.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/_globals.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/accumulators.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/accumulators.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/broadcast.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/broadcast.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/conf.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/conf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/context.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/daemon.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/daemon.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/files.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/files.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/find_spark_home.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/find_spark_home.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/install.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/install.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/java_gateway.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/java_gateway.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/join.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/join.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/__init__.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/base.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/base.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/classification.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/classification.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/clustering.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/clustering.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/common.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/evaluation.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/evaluation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/feature.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/feature.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/fpm.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/fpm.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/functions.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/image.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/image.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/param/__init__.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/param/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/param/shared.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/param/shared.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/pipeline.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/pipeline.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/recommendation.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/recommendation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/regression.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/regression.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/stat.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/stat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/tree.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/tuning.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/tuning.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/util.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/ml/wrapper.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/ml/wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/__init__.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/classification.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/classification.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/clustering.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/clustering.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/common.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/evaluation.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/evaluation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/feature.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/feature.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/fpm.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/fpm.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/random.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/random.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/recommendation.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/recommendation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/regression.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/regression.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/stat/test.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/stat/test.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/tree.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/mllib/util.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/mllib/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/profiler.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/profiler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/rdd.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/rdd.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/rddsampler.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/rddsampler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/resource/__init__.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/resource/information.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/resource/information.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/resource/profile.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/resource/profile.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/resource/requests.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/resource/requests.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/resultiterable.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/resultiterable.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/serializers.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/serializers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/shell.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/shell.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/shuffle.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/shuffle.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/__init__.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/avro/functions.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/avro/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/catalog.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/catalog.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/column.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/column.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/conf.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/conf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/context.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/dataframe.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/dataframe.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/functions.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/group.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/group.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/types.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/pandas/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/readwriter.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/readwriter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/session.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/session.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/streaming.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/streaming.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/types.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/udf.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/udf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/utils.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/sql/window.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/sql/window.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/statcounter.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/statcounter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/status.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/status.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/storagelevel.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/storagelevel.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/__init__.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/context.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/streaming/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/dstream.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/streaming/dstream.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/kinesis.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/streaming/kinesis.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/listener.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/streaming/listener.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/streaming/util.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/streaming/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/taskcontext.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/taskcontext.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/traceback_utils.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/util.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/pyspark/pyspark/worker.py` & `tecton-0.9.1/tecton/vendor/pyspark/pyspark/worker.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/vendor_dill.py` & `tecton-0.9.1/tecton/vendor/vendor_dill.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/vendor/vendor_pyspark.py` & `tecton-0.9.1/tecton/vendor/vendor_pyspark.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton/version.py` & `tecton-0.9.1/tecton/version.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton.egg-info/PKG-INFO` & `tecton-0.9.1/tecton.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tecton
-Version: 0.9.0rc4
+Version: 0.9.1
 Summary: Tecton Python SDK
 Home-page: https://tecton.ai
 Author: Tecton, Inc.
 Author-email: support@tecton.ai
 License: Tecton Proprietary
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `tecton-0.9.0rc4/tecton.egg-info/SOURCES.txt` & `tecton-0.9.1/tecton.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 tecton/framework/__init__.py
 tecton/framework/base_tecton_object.py
 tecton/framework/configs.py
 tecton/framework/data_frame.py
 tecton/framework/data_source.py
 tecton/framework/dataset.py
 tecton/framework/entity.py
+tecton/framework/feature.py
 tecton/framework/feature_service.py
 tecton/framework/feature_view.py
 tecton/framework/filtered_source.py
 tecton/framework/repo_config.py
 tecton/framework/transformation.py
 tecton/framework/utils.py
 tecton/framework/validation_mode.py
```

### Comparing `tecton-0.9.0rc4/tecton.egg-info/requires.txt` & `tecton-0.9.1/tecton.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 attrs>=21.3.0
 boto3
-googleapis-common-protos~=1.52
+googleapis-common-protos<2,>=1.57.0
 jinja2~=3.0
 numpy~=1.16
 pathspec
 pendulum~=2.1
 protobuf>=3.20.0
 pypika~=0.48.9
 pytimeparse
@@ -67,12 +67,14 @@
 deltalake~=0.15
 pyarrow>=11.0.0
 
 [rift-materialization]
 duckdb==0.10.0
 deltalake~=0.15
 pyarrow>=11.0.0
+snowflake-connector-python[pandas]~=3.6
+snowflake-snowpark-python[pandas]~=1.0
 pydantic<2
 urllib3<1.27
 
 [snowflake]
 snowflake-snowpark-python[pandas]~=1.0
```

### Comparing `tecton-0.9.0rc4/tecton_athena/athena_session.py` & `tecton-0.9.1/tecton_athena/athena_session.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_athena/data_catalog_helper.py` & `tecton-0.9.1/tecton_athena/data_catalog_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_athena/odfv_helper.py` & `tecton-0.9.1/tecton_athena/odfv_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_athena/query/translate.py` & `tecton-0.9.1/tecton_athena/query/translate.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_athena/sql_helper.py` & `tecton-0.9.1/tecton_athena/sql_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_athena/templates/create_table.sql` & `tecton-0.9.1/tecton_athena/templates/create_table.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_athena/templates/historical_features.sql` & `tecton-0.9.1/tecton_athena/templates/historical_features.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_athena/templates/materialization_tile.sql` & `tecton-0.9.1/tecton_athena/templates/materialization_tile.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_athena/templates/run_full_aggregation.sql` & `tecton-0.9.1/tecton_athena/templates/run_full_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_athena/templates/time_limit.sql` & `tecton-0.9.1/tecton_athena/templates/time_limit.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_athena/templates_utils.py` & `tecton-0.9.1/tecton_athena/templates_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/aggregation_utils.py` & `tecton-0.9.1/tecton_core/aggregation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/arrow.py` & `tecton-0.9.1/tecton_core/arrow.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/aws_credentials.py` & `tecton-0.9.1/tecton_core/aws_credentials.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/compute_mode.py` & `tecton-0.9.1/tecton_core/compute_mode.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/conf.py` & `tecton-0.9.1/tecton_core/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,15 +360,15 @@
     # Instead of the querytree code path, use the old snowflake ghf implementation
     "REDIS_AUTH_TOKEN": DEFAULT_ALLOWED_SOURCES,
     "TECTON_PYTHON_ODFV_OUTPUT_SCHEMA_CHECK_ENABLED": RUNTIME_ALLOWED_SOURCES,
     "USE_LOCAL_OFFLINE_STORE_CREDENTIALS": DEFAULT_ALLOWED_SOURCES,
     "SKIP_REPO_CONFIG_INIT": DEFAULT_ALLOWED_SOURCES,  # Used by itests only
     "ARROW_BATCH_READ_AHEAD": DEFAULT_ALLOWED_SOURCES,
     "ARROW_FRAGMENT_READ_AHEAD": DEFAULT_ALLOWED_SOURCES,
-    "DUCKDB_DISK_SPILLING": DEFAULT_ALLOWED_SOURCES,
+    "DUCKDB_DISK_SPILLING_ENABLED": DEFAULT_ALLOWED_SOURCES,
     "MODEL_CACHE_DIRECTORY": RUNTIME_ALLOWED_SOURCES,
 }
 
 _VALID_KEY_PREFIXES = ["SECRET_"]
 
 _DEFAULTS = {
     "TECTON_WORKSPACE": (lambda: "prod"),
@@ -381,15 +381,15 @@
     "DUCKDB_EXTENSION_REPO": (
         lambda: "http://s3.us-west-2.amazonaws.com/tecton.ai.public/duckdb/tecton-extension/{version}"
     ),
     "USE_DEPRECATED_SNOWFLAKE_RETRIEVAL": (lambda: "false"),
     "TECTON_PYTHON_ODFV_OUTPUT_SCHEMA_CHECK_ENABLED": (lambda: "true"),
     "ARROW_BATCH_READ_AHEAD": (lambda: "64"),
     "ARROW_FRAGMENT_READ_AHEAD": (lambda: "16"),
-    "DUCKDB_DISK_SPILLING": (lambda: "true"),
+    "DUCKDB_DISK_SPILLING_ENABLED": (lambda: "true"),
     "MODEL_CACHE_DIRECTORY": (lambda: _model_cache_directory()),
 }
 
 _mds_config_lock = threading.Lock()
 _remote_mds_configs: _ConfigSettings = {}
 
 _is_interactive_notebook = None
```

### Comparing `tecton-0.9.0rc4/tecton_core/data_types.py` & `tecton-0.9.1/tecton_core/data_types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/duckdb_context.py` & `tecton-0.9.1/tecton_core/duckdb_context.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import tempfile
 from typing import TYPE_CHECKING
 from typing import Optional
 
 from tecton_core import _gen_version
 from tecton_core import conf
 
 
@@ -17,24 +18,29 @@
 
 class DuckDBContext:
     """
     Singleton holder of DuckDB connection.
     """
 
     _current_context_instance = None
-    _connection = None
 
     def __init__(self, connection: "DuckDBPyConnection", home_dir_override: Optional[str] = None) -> None:
         self._connection = connection
         # Needed to export to S3
         if home_dir_override:
             connection.sql(f"SET home_directory='{home_dir_override}'")
         connection.sql("INSTALL httpfs;")
-        if conf.get_bool("DUCKDB_DISK_SPILLING"):
-            connection.sql("SET temp_directory = '/temp_dir.tmp'")
+        if conf.get_bool("DUCKDB_DISK_SPILLING_ENABLED"):
+            # The directory will be deleted when the TemporaryDirectory object is destroyed even if we don't call
+            # __enter__. This means as long as we store the object somewhere the directory will live as the context and
+            # will be cleaned up at interpreter exit.
+            self._temporary_directory = tempfile.TemporaryDirectory(suffix=".tecton_duckdb")
+            connection.sql(f"SET temp_directory = '{self._temporary_directory.name}'")
+        else:
+            self._temporary_directory = None
         duckdb_memory_limit = conf.get_or_none("DUCKDB_MEMORY_LIMIT")
         if duckdb_memory_limit:
             if conf.get_bool("DUCKDB_DEBUG"):
                 print(f"Setting duckdb memory limit to {duckdb_memory_limit}")
 
             connection.sql(f"SET memory_limit='{duckdb_memory_limit}'")
```

### Comparing `tecton-0.9.0rc4/tecton_core/errors.py` & `tecton-0.9.1/tecton_core/errors.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/fco_container.py` & `tecton-0.9.1/tecton_core/fco_container.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/feature_definition_wrapper.py` & `tecton-0.9.1/tecton_core/feature_definition_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -419,17 +419,17 @@
         msg = "Invalid invocation on unsupported FeatureView type"
         raise TypeError(msg)
 
     @property
     def get_tile_interval_duration_for_offline_store(self) -> pendulum.Duration:
         """The tile interval to be used for offline retrieval.
 
-        For most cases this will be the aggregation interval. For fvs with stream_compaction_enabled=True, the online store is tiled, but offline retrieval should not be using tiles (like continuous mode).
+        For most cases this will be the aggregation interval. For fvs with stream_tiling_enabled=True, the online store is tiled, but offline retrieval should not be using tiles (like continuous mode).
         """
-        if self.is_temporal_aggregate and self.fv_spec.stream_compaction_enabled:
+        if self.is_temporal_aggregate and self.fv_spec.stream_tiling_enabled:
             return pendulum.Duration(seconds=0)
         return self.get_tile_interval
 
     @property
     def get_tile_interval_seconds_for_offline_store(self) -> int:
         return time_utils.convert_timedelta_for_version(
             self.get_tile_interval_duration_for_offline_store, self.get_feature_store_format_version
@@ -613,28 +613,28 @@
     def time_range_for_relative_time_window(self, time_window: RelativeTimeWindowSpec) -> Tuple[int, int]:
         start = self.earliest_anchor_time_from_window_start(time_window.window_start)
         end = convert_timedelta_for_version(time_window.window_end, self.get_feature_store_format_version)
         assert start <= end
         return start, end
 
     @property
-    def batch_compaction_enabled(self):
-        """Whether a feature view has batch_compaction_enabled set to True."""
+    def compaction_enabled(self):
+        """Whether a feature view has `compaction_enabled` set to True."""
         if not isinstance(self.fv_spec, specs.MaterializedFeatureViewSpec):
             return False
-        return self.fv_spec.batch_compaction_enabled
+        return self.fv_spec.compaction_enabled
 
     @property
-    def stream_compaction_enabled(self):
-        """Whether a stream feature view has stream_compaction_enabled set to True.
+    def stream_tiling_enabled(self):
+        """Whether a stream feature view has stream_tiling_enabled set to True.
 
-        stream_compaction_enabled is only applicable to stream feature views with batch_compaction_enabled=True."""
+        stream_tiling_enabled is only applicable to stream feature views with compaction_enabled=True."""
         if not isinstance(self.fv_spec, specs.MaterializedFeatureViewSpec):
             return False
-        return self.fv_spec.stream_compaction_enabled
+        return self.fv_spec.stream_tiling_enabled
 
 
 def pipeline_to_ds_inputs(pipeline: Pipeline) -> Dict[str, DataSourceNode]:
     ds_nodes: Dict[str, DataSourceNode] = {}
 
     def _recurse_pipeline_to_ds_nodes(pipeline_node: PipelineNode, ds_nodes_: Dict[str, DataSourceNode]) -> None:
         if pipeline_node.HasField("data_source_node"):
```

### Comparing `tecton-0.9.0rc4/tecton_core/feature_set_config.py` & `tecton-0.9.1/tecton_core/feature_set_config.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/feature_view_utils.py` & `tecton-0.9.1/tecton_core/feature_view_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/function_deserialization.py` & `tecton-0.9.1/tecton_core/function_deserialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/http.py` & `tecton-0.9.1/tecton_core/http.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/id_helper.py` & `tecton-0.9.1/tecton_core/id_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/iterators.py` & `tecton-0.9.1/tecton_core/iterators.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/materialization_context.py` & `tecton-0.9.1/tecton_core/materialization_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/metadata_service_impl/error_lib.py` & `tecton-0.9.1/tecton_core/metadata_service_impl/error_lib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/metadata_service_impl/http_client.py` & `tecton-0.9.1/tecton_core/metadata_service_impl/http_client.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/metadata_service_impl/providers.py` & `tecton-0.9.1/tecton_core/metadata_service_impl/providers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/metadata_service_impl/response.py` & `tecton-0.9.1/tecton_core/metadata_service_impl/response.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/metadata_service_impl/service_calls.py` & `tecton-0.9.1/tecton_core/metadata_service_impl/service_calls.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/offline_store.py` & `tecton-0.9.1/tecton_core/offline_store.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/online_serving_index.py` & `tecton-0.9.1/tecton_core/online_serving_index.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/pipeline_common.py` & `tecton-0.9.1/tecton_core/pipeline_common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/query/aggregation_plans.py` & `tecton-0.9.1/tecton_core/query/aggregation_plans.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/query/builder.py` & `tecton-0.9.1/tecton_core/query/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,15 @@
     if for_stream:
         watermark = _get_stream_watermark(fdw)
         if watermark:
             tree = StreamWatermarkNode(dialect, compute_mode, tree, fdw.time_key, watermark).as_ref()
     if enable_feature_metrics:
         tree = MetricsCollectorNode(dialect, compute_mode, tree).as_ref()
 
-    if fdw.batch_compaction_enabled and not for_stream:
+    if fdw.compaction_enabled and not for_stream:
         return _build_compaction_materialization_querytree(
             dialect=dialect,
             compute_mode=compute_mode,
             fdw=fdw,
             pipeline_tree=tree,
         )
 
@@ -351,15 +351,15 @@
 
 def _build_compaction_materialization_querytree(
     dialect: Dialect,
     compute_mode: ComputeMode,
     fdw: feature_definition_wrapper.FeatureDefinitionWrapper,
     pipeline_tree: NodeRef,
 ) -> NodeRef:
-    # Offline materialization query for fvs with batch_compaction_enabled=True
+    # Offline materialization query for fvs with compaction_enabled=True
     tree = StagingNode(
         dialect=dialect,
         compute_mode=compute_mode,
         input_node=pipeline_tree,
         staging_table_name=f"{fdw.name}",
         query_tree_step=QueryTreeStep.PIPELINE,
     ).as_ref()
@@ -456,15 +456,15 @@
             fdw,
             for_stream=False,
             feature_data_time_limits=feature_data_time_limits,
             aggregation_anchor_time=aggregation_anchor_time,
             include_window_end_time=include_window_end_time,
         )
 
-    if fdw.batch_compaction_enabled and fdw.is_temporal_aggregate:
+    if fdw.compaction_enabled and fdw.is_temporal_aggregate:
         end_column_name = window_end_column_name() if include_window_end_time else None
         tree = PartialAggNode(
             dialect=dialect,
             compute_mode=compute_mode,
             input_node=tree,
             fdw=fdw,
             window_start_column_name=anchor_time(),
```

### Comparing `tecton-0.9.0rc4/tecton_core/query/compaction_utils.py` & `tecton-0.9.1/tecton_core/query/compaction_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/query/duckdb/compute.py` & `tecton-0.9.1/tecton_core/query/duckdb/compute.py`

 * *Files 6% similar despite different names*

```diff
@@ -182,14 +182,18 @@
         if isinstance(fs, pyarrow.fs.S3FileSystem):
             options = BotoOfflineStoreOptionsProvider.static_options()
             if options is not None:
                 fs = pyarrow.fs.S3FileSystem(
                     access_key=options.access_key_id,
                     secret_key=options.secret_access_key,
                     session_token=options.session_token,
+                    # When created via Filesystem.from_uri, the bucket region will be autodetected. This constructor
+                    # does not have a bucket from which it can detect the region, so we need to copy it over from the
+                    # previous instance.
+                    region=fs.region,
                 )
 
         # There seems to be a bug in Arrow related to the explicit schema:
         # when we pass an explicit schema to `dataset` and both resolution and timezone in the timestamp column
         # don't match the schema in parquet files - filters that are pushed down by DuckDB will not work.
         # It is very likely that we will not guess both resolution and timezone correctly.
         # So we won't pass schema for now.
```

### Comparing `tecton-0.9.0rc4/tecton_core/query/duckdb/nodes.py` & `tecton-0.9.1/tecton_core/query/duckdb/nodes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/query/duckdb/rewrite.py` & `tecton-0.9.1/tecton_core/query/duckdb/rewrite.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/query/errors.py` & `tecton-0.9.1/tecton_core/query/errors.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/query/executor_params.py` & `tecton-0.9.1/tecton_core/query/executor_params.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/query/executor_utils.py` & `tecton-0.9.1/tecton_core/query/executor_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/query/node_interface.py` & `tecton-0.9.1/tecton_core/query/node_interface.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/query/node_utils.py` & `tecton-0.9.1/tecton_core/query/node_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/query/nodes.py` & `tecton-0.9.1/tecton_core/query/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,15 +403,15 @@
     """
 
     feature_definition_wrapper: FeatureDefinitionWrapper
     partition_time_filter: Optional[pendulum.Period] = None
 
     @property
     def columns(self) -> Sequence[str]:
-        if self.feature_definition_wrapper.batch_compaction_enabled:
+        if self.feature_definition_wrapper.compaction_enabled:
             return self.feature_definition_wrapper.view_schema.column_names()
 
         store_type = get_offline_store_type(self.feature_definition_wrapper)
         cols = self.feature_definition_wrapper.materialization_schema.column_names()
         if store_type == OfflineStoreType.SNOWFLAKE:
             if self.feature_definition_wrapper.is_temporal_aggregate:
                 # Snowflake stores the timestamp_key instead of _anchor_time in offline store, but it's not used in QT for aggregates
```

### Comparing `tecton-0.9.0rc4/tecton_core/query/pandas/compute.py` & `tecton-0.9.1/tecton_core/query/pandas/compute.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/query/pandas/node.py` & `tecton-0.9.1/tecton_core/query/pandas/node.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/query/pandas/nodes.py` & `tecton-0.9.1/tecton_core/query/pandas/nodes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/query/pandas/pipeline_helper.py` & `tecton-0.9.1/tecton_core/query/pandas/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/query/pandas/rewrite.py` & `tecton-0.9.1/tecton_core/query/pandas/rewrite.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/query/pandas/translate.py` & `tecton-0.9.1/tecton_core/query/pandas/translate.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/query/pipeline_sql_builder.py` & `tecton-0.9.1/tecton_core/query/pipeline_sql_builder.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/query/prefixed_uri_resolver.py` & `tecton-0.9.1/tecton_core/query/prefixed_uri_resolver.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/query/query_tree_compute.py` & `tecton-0.9.1/tecton_core/query/query_tree_compute.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/query/query_tree_executor.py` & `tecton-0.9.1/tecton_core/query/query_tree_executor.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/query/snowflake/compute.py` & `tecton-0.9.1/tecton_core/query/snowflake/compute.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/query/sql_compat.py` & `tecton-0.9.1/tecton_core/query/sql_compat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/query_consts.py` & `tecton-0.9.1/tecton_core/query_consts.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/repo_file_handler.py` & `tecton-0.9.1/tecton_core/repo_file_handler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/request_context.py` & `tecton-0.9.1/tecton_core/request_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/schema.py` & `tecton-0.9.1/tecton_core/schema.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/schema_derivation_utils.py` & `tecton-0.9.1/tecton_core/schema_derivation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/schema_validation.py` & `tecton-0.9.1/tecton_core/schema_validation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/secrets.py` & `tecton-0.9.1/tecton_core/secrets.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/snowflake_context.py` & `tecton-0.9.1/tecton_core/snowflake_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/specs/__init__.py` & `tecton-0.9.1/tecton_core/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/specs/data_source_spec.py` & `tecton-0.9.1/tecton_core/specs/data_source_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/specs/entity_spec.py` & `tecton-0.9.1/tecton_core/specs/entity_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/specs/feature_service_spec.py` & `tecton-0.9.1/tecton_core/specs/feature_service_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/specs/feature_view_spec.py` & `tecton-0.9.1/tecton_core/specs/feature_view_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,16 +210,16 @@
 
     # TODO(TEC-12321): Audit and fix feature view spec fields that should be required.
     # See failure: https://tectonworkspace.slack.com/archives/C04L8M14XGX/p1675279851469019
     batch_trigger: Optional[feature_view__args_pb2.BatchTriggerType.ValueType]
     manual_trigger_backfill_end_time: Optional[pendulum.DateTime]
 
     online_batch_table_format: Optional[OnlineBatchTableFormat]
-    batch_compaction_enabled: bool
-    stream_compaction_enabled: bool
+    compaction_enabled: bool
+    stream_tiling_enabled: bool
 
     has_explicit_view_schema: bool
 
     @classmethod
     @typechecked
     def from_data_proto(cls, proto: feature_view__data_pb2.FeatureView) -> "MaterializedFeatureViewSpec":
         if proto.HasField("temporal_aggregate"):
@@ -314,29 +314,29 @@
                 proto.materialization_params, "manual_trigger_backfill_end_timestamp"
             ),
             url=utils.get_field_or_none(proto, "web_url"),
             online_batch_table_format=_get_online_batch_table_format(proto.schemas),
             batch_compute_mode=BatchComputeMode(proto.batch_compute_mode)
             if proto.HasField("batch_compute_mode")
             else None,
-            batch_compaction_enabled=proto.materialization_params.batch_compaction_enabled,
-            stream_compaction_enabled=proto.materialization_params.stream_compaction_enabled,
+            compaction_enabled=proto.materialization_params.compaction_enabled,
+            stream_tiling_enabled=proto.materialization_params.stream_tiling_enabled,
             options=MappingProxyType(proto.options),
         )
 
     @classmethod
     @typechecked
     def from_args_proto(
         cls, proto: feature_view__args_pb2.FeatureViewArgs, supplement: FeatureViewSpecArgsSupplement
     ) -> "MaterializedFeatureViewSpec":
         feature_start_time = utils.get_timestamp_field_or_none(
             proto.materialized_feature_view_args, "feature_start_time"
         )
 
-        batch_compaction_enabled = proto.materialized_feature_view_args.batch_compaction_enabled
+        compaction_enabled = proto.materialized_feature_view_args.compaction_enabled
         is_continuous = get_is_continuous_from_feature_view_args(proto)
         data_source_type = utils.get_field_or_none(proto.materialized_feature_view_args, "data_source_type")
         aggregate_features = get_aggregate_features_from_feature_view_args(proto)
 
         is_aggregate = len(proto.materialized_feature_view_args.aggregations) > 0
         if is_aggregate:
             fv_type = MaterializedFeatureViewType.TEMPORAL_AGGREGATE
@@ -438,16 +438,16 @@
             url=None,
             online_batch_table_format=OnlineBatchTableFormat.from_proto(supplement.online_batch_table_format)
             if supplement.online_batch_table_format
             else None,
             batch_compute_mode=BatchComputeMode(proto.batch_compute_mode)
             if proto.HasField("batch_compute_mode")
             else None,
-            batch_compaction_enabled=batch_compaction_enabled,
-            stream_compaction_enabled=proto.materialized_feature_view_args.stream_compaction_enabled,
+            compaction_enabled=compaction_enabled,
+            stream_tiling_enabled=proto.materialized_feature_view_args.stream_tiling_enabled,
             options=MappingProxyType(proto.options),
         )
 
     @property
     def features(self) -> List[str]:
         if len(self.aggregate_features) > 0:
             # Temporal aggregate feature view.
@@ -787,38 +787,38 @@
 
 @typechecked
 def _get_aggregation_interval_from_feature_view_args(
     proto: feature_view__args_pb2.FeatureViewArgs,
     is_continuous: bool,
     data_source_type: Optional[data_source_type_pb2.DataSourceType.ValueType],
 ) -> Optional[duration_pb2.Duration]:
-    if proto.materialized_feature_view_args.batch_compaction_enabled:
+    if proto.materialized_feature_view_args.compaction_enabled:
         is_stream = (
             data_source_type == data_source_type_pb2.DataSourceType.STREAM_WITH_BATCH if data_source_type else False
         )
-        # Default set in Kotlin for batch fvs with compaction is the batch schedule. Batch schedule is required for fvs with batch_compaction_enabled=True
+        # Default set in Kotlin for batch fvs with compaction is the batch schedule. Batch schedule is required for fvs with compaction_enabled=True
         # Default set in Kotlin for non-continuous stream fvs with compaction is the stream compaction tile size.
         if not is_stream:
             return utils.get_field_or_none(proto.materialized_feature_view_args, "batch_schedule")
         elif not is_continuous:
-            return utils.get_field_or_none(proto.materialized_feature_view_args, "stream_compaction_tile_size")
+            return utils.get_field_or_none(proto.materialized_feature_view_args, "stream_tile_size")
 
     return utils.get_field_or_none(proto.materialized_feature_view_args, "aggregation_interval")
 
 
 @typechecked
 def get_is_continuous_from_feature_view_args(
     proto: feature_view__args_pb2.FeatureViewArgs,
 ) -> bool:
     data_source_type = utils.get_field_or_none(proto.materialized_feature_view_args, "data_source_type")
     if not data_source_type or data_source_type == data_source_type_pb2.DataSourceType.BATCH:
         return False
 
-    if proto.materialized_feature_view_args.batch_compaction_enabled:
-        return proto.materialized_feature_view_args.stream_compaction_enabled == False
+    if proto.materialized_feature_view_args.compaction_enabled:
+        return proto.materialized_feature_view_args.stream_tiling_enabled == False
 
     return (
         proto.materialized_feature_view_args.stream_processing_mode
         == feature_view__args_pb2.StreamProcessingMode.STREAM_PROCESSING_MODE_CONTINUOUS
     )
```

### Comparing `tecton-0.9.0rc4/tecton_core/specs/tecton_object_spec.py` & `tecton-0.9.1/tecton_core/specs/tecton_object_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/specs/time_window_spec.py` & `tecton-0.9.1/tecton_core/specs/time_window_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/specs/transformation_spec.py` & `tecton-0.9.1/tecton_core/specs/transformation_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/specs/utils.py` & `tecton-0.9.1/tecton_core/specs/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/time_utils.py` & `tecton-0.9.1/tecton_core/time_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/vendor/queue.py` & `tecton-0.9.1/tecton_core/vendor/queue.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/vendor/treelib/__init__.py` & `tecton-0.9.1/tecton_core/vendor/treelib/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/vendor/treelib/exceptions.py` & `tecton-0.9.1/tecton_core/vendor/treelib/exceptions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/vendor/treelib/misc.py` & `tecton-0.9.1/tecton_core/vendor/treelib/misc.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/vendor/treelib/node.py` & `tecton-0.9.1/tecton_core/vendor/treelib/node.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/vendor/treelib/plugins.py` & `tecton-0.9.1/tecton_core/vendor/treelib/plugins.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/vendor/treelib/tree.py` & `tecton-0.9.1/tecton_core/vendor/treelib/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_core/vendor/vendor_treelib.py` & `tecton-0.9.1/tecton_core/vendor/vendor_treelib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/__init__.py` & `tecton-0.9.1/tecton_materialization/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/batch_materialization.py` & `tecton-0.9.1/tecton_materialization/batch_materialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,18 +120,18 @@
 ) -> DataFrame:
     df = df_to_online_store_msg(
         df,
         fd.id,
         is_batch=True,
         is_status=False,
         canary_id=None,
-        is_compaction_job=fd.batch_compaction_enabled,
+        is_compaction_job=fd.compaction_enabled,
     )
     udf_name = f"to_dynamodb_json_{fd.id}"
-    if fd.batch_compaction_enabled:
+    if fd.compaction_enabled:
         # UDF used for compaction jobs. Compatible with TableFormatVersionV3
         spark._jvm.com.tecton.onlinestorewriter.RegisterFeatureToDynamoDbJsonUDFV2().register(
             udf_name, materialization_task_params.SerializeToString()
         )
         udf_column_name = "dynamodb_json"
         df = df.select(expr(f"{udf_name}(value) as {udf_column_name}"))
         return df.select(explode(udf_column_name))
@@ -327,15 +327,15 @@
             materialization_task_params,
             store_type="online",
             online_store_type=OnlineStoreType.ONLINE_STORE_TYPE_DYNAMO,
             job_metadata_client=job_metadata_client,
         )
         logger.info(f"Wrote {dynamo_import_row_count} rows to bulk load intermediate storage")
     else:
-        assert not fv_spec.batch_compaction_enabled, "Batch compaction must use create_online_table"
+        assert not fv_spec.compaction_enabled, "Batch compaction must use create_online_table"
         # Write materialized features to the online feature store
         online_store_df = online_store_df.coalesce(DEFAULT_COALESCE_FOR_OSW)
         batch_write_to_online_store(
             online_store_df, materialization_task_params, resources.get_online_store_sink(), fd.id, is_status=False
         )
         export_consumption_metrics(
             spark,
@@ -478,15 +478,15 @@
                 write_checkpoint(spark, materialization_task_params, query_feature_start_time, run_id)
 
         logger.info(f"Wrote {total_rows} total rows")
 
     if write_to_online_from_offline_store and step in (None, 2):
         assert not materialization_task_params.HasField("canary_id")
         # we don't do metrics collection here, because they already got collected in the jobs writing to the offline store
-        if fd.batch_compaction_enabled:
+        if fd.compaction_enabled:
             plan = materialization_plan.get_batch_compaction_online_materialization_plan(
                 spark=spark, feature_definition=fd, compaction_job_end_time=task_feature_end_time
             )
         else:
             # used for bootstrap bulk backfill jobs
             plan = MaterializationPlan.from_offline_store(fd, task_feature_start_time, task_feature_end_time, spark)
         if plan is not None:
```

### Comparing `tecton-0.9.0rc4/tecton_materialization/common/job_metadata.py` & `tecton-0.9.1/tecton_materialization/common/job_metadata.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/common/job_metadata_aws.py` & `tecton-0.9.1/tecton_materialization/common/job_metadata_aws.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/common/job_metadata_gcp.py` & `tecton-0.9.1/tecton_materialization/common/job_metadata_gcp.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/common/task_params.py` & `tecton-0.9.1/tecton_materialization/common/task_params.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/consumption.py` & `tecton-0.9.1/tecton_materialization/consumption.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/delta_maintenance.py` & `tecton-0.9.1/tecton_materialization/delta_maintenance.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/entity_deletion.py` & `tecton-0.9.1/tecton_materialization/entity_deletion.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/feature_export.py` & `tecton-0.9.1/tecton_materialization/feature_export.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/ingest_materialization.py` & `tecton-0.9.1/tecton_materialization/ingest_materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/job_metadata.py` & `tecton-0.9.1/tecton_materialization/job_metadata.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/materialization.py` & `tecton-0.9.1/tecton_materialization/materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/materialization_utils.py` & `tecton-0.9.1/tecton_materialization/materialization_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/ray/batch_materialization.py` & `tecton-0.9.1/tecton_materialization/ray/batch_materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/ray/delta.py` & `tecton-0.9.1/tecton_materialization/ray/delta.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/ray/feature_export.py` & `tecton-0.9.1/tecton_materialization/ray/feature_export.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/ray/ingest_materialization.py` & `tecton-0.9.1/tecton_materialization/ray/ingest_materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/ray/job_status.py` & `tecton-0.9.1/tecton_materialization/ray/job_status.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/ray/materialization.py` & `tecton-0.9.1/tecton_materialization/ray/materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/ray/materialization_utils.py` & `tecton-0.9.1/tecton_materialization/ray/materialization_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/ray/nodes.py` & `tecton-0.9.1/tecton_materialization/ray/nodes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/remote_host/pyspark_remote_host.py` & `tecton-0.9.1/tecton_materialization/remote_host/pyspark_remote_host.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/secrets.py` & `tecton-0.9.1/tecton_materialization/secrets.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_materialization/stream_materialization.py` & `tecton-0.9.1/tecton_materialization/stream_materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/amplitude/amplitude_pb2.py` & `tecton-0.9.1/tecton_proto/amplitude/amplitude_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/amplitude/client_logging_pb2.py` & `tecton-0.9.1/tecton_proto/amplitude/client_logging_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/api/featureservice/feature_service_pb2.py` & `tecton-0.9.1/tecton_proto/api/featureservice/feature_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/api/featureservice/feature_service_request_pb2.py` & `tecton-0.9.1/tecton_proto/api/featureservice/feature_service_request_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/args/basic_info_pb2.py` & `tecton-0.9.1/tecton_proto/args/basic_info_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/args/data_source_config_pb2.py` & `tecton-0.9.1/tecton_proto/args/data_source_config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/args/data_source_pb2.py` & `tecton-0.9.1/tecton_proto/args/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/args/diff_options_pb2.py` & `tecton-0.9.1/tecton_proto/args/diff_options_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/args/diff_test_pb2.py` & `tecton-0.9.1/tecton_proto/args/diff_test_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/args/entity_pb2.py` & `tecton-0.9.1/tecton_proto/args/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/args/fco_args_pb2.py` & `tecton-0.9.1/tecton_proto/args/fco_args_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/args/feature_service_pb2.py` & `tecton-0.9.1/tecton_proto/args/feature_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/args/feature_view_pb2.py` & `tecton-0.9.1/tecton_proto/args/feature_view_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from tecton_proto.common import framework_version_pb2 as tecton__proto_dot_common_dot_framework__version__pb2
 from tecton_proto.common import id_pb2 as tecton__proto_dot_common_dot_id__pb2
 from tecton_proto.common import schema_pb2 as tecton__proto_dot_common_dot_schema__pb2
 from tecton_proto.common import spark_schema_pb2 as tecton__proto_dot_common_dot_spark__schema__pb2
 from tecton_proto.common import time_window_pb2 as tecton__proto_dot_common_dot_time__window__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$tecton_proto/args/feature_view.proto\x12\x11tecton_proto.args\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\"tecton_proto/args/basic_info.proto\x1a#tecton_proto/args/data_source.proto\x1a$tecton_proto/args/diff_options.proto\x1a tecton_proto/args/pipeline.proto\x1a+tecton_proto/args/version_constraints.proto\x1a+tecton_proto/common/analytics_options.proto\x1a&tecton_proto/common/compute_mode.proto\x1a*tecton_proto/common/data_source_type.proto\x1a+tecton_proto/common/framework_version.proto\x1a\x1ctecton_proto/common/id.proto\x1a tecton_proto/common/schema.proto\x1a&tecton_proto/common/spark_schema.proto\x1a%tecton_proto/common/time_window.proto\"\xfd\r\n\x0f\x46\x65\x61tureViewArgs\x12?\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\rfeatureViewId\x12N\n\x11\x66\x65\x61ture_view_type\x18\x02 \x01(\x0e\x32\".tecton_proto.args.FeatureViewTypeR\x0f\x66\x65\x61tureViewType\x12\x37\n\x04info\x18\x03 \x01(\x0b\x32\x1c.tecton_proto.args.BasicInfoB\x05\x92M\x02\x10\x01R\x04info\x12\x46\n\x07version\x18\x1d \x01(\x0e\x32%.tecton_proto.common.FrameworkVersionB\x05\x92M\x02\x08\x05R\x07version\x12.\n\x0fprevent_destroy\x18  \x01(\x08\x42\x05\x92M\x02\x08\x01R\x0epreventDestroy\x12P\n\x07options\x18\" \x03(\x0b\x32/.tecton_proto.args.FeatureViewArgs.OptionsEntryB\x05\x92M\x02\x08\x01R\x07options\x12H\n\x0c\x63\x61\x63he_config\x18$ \x01(\x0b\x32\x1e.tecton_proto.args.CacheConfigB\x05\x92M\x02\x08\x01R\x0b\x63\x61\x63heConfig\x12G\n\x08\x65ntities\x18\x04 \x03(\x0b\x32$.tecton_proto.args.EntityKeyOverrideB\x05\x92M\x02\x08\x06R\x08\x65ntities\x12M\n\rtemporal_args\x18\x17 \x01(\x0b\x32\x1f.tecton_proto.args.TemporalArgsB\x05\x92M\x02\x10\x01H\x00R\x0ctemporalArgs\x12i\n\x17temporal_aggregate_args\x18\x18 \x01(\x0b\x32(.tecton_proto.args.TemporalAggregateArgsB\x05\x92M\x02\x10\x01H\x00R\x15temporalAggregateArgs\x12|\n\x1ematerialized_feature_view_args\x18\x1c \x01(\x0b\x32..tecton_proto.args.MaterializedFeatureViewArgsB\x05\x92M\x02\x10\x01H\x00R\x1bmaterializedFeatureViewArgs\x12N\n\x0eon_demand_args\x18\x19 \x01(\x0b\x32\x1f.tecton_proto.args.OnDemandArgsB\x05\x92M\x02\x10\x01H\x00R\x0conDemandArgs\x12Z\n\x12\x66\x65\x61ture_table_args\x18\x1a \x01(\x0b\x32#.tecton_proto.args.FeatureTableArgsB\x05\x92M\x02\x10\x01H\x00R\x10\x66\x65\x61tureTableArgs\x12\x30\n\x14online_serving_index\x18\x05 \x03(\tR\x12onlineServingIndex\x12,\n\x0eonline_enabled\x18\x0e \x01(\x08\x42\x05\x92M\x02 \x0bR\ronlineEnabled\x12.\n\x0foffline_enabled\x18\x0f \x01(\x08\x42\x05\x92M\x02 \x0bR\x0eofflineEnabled\x12Z\n\x12\x62\x61tch_compute_mode\x18# \x01(\x0e\x32%.tecton_proto.common.BatchComputeModeB\x05\x92M\x02\x08\tR\x10\x62\x61tchComputeMode\x12>\n\x08pipeline\x18\x06 \x01(\x0b\x32\x1b.tecton_proto.args.PipelineB\x05\x92M\x02\x08\x06R\x08pipeline\x12`\n\x13\x64\x61ta_quality_config\x18! \x01(\x0b\x32$.tecton_proto.args.DataQualityConfigB\n\x92M\x02\x08\x01\x92M\x02\x10\x01R\x11\x64\x61taQualityConfig\x12N\n\x12\x66orced_view_schema\x18\x1e \x01(\x0b\x32 .tecton_proto.common.SparkSchemaR\x10\x66orcedViewSchema\x12^\n\x1a\x66orced_materialized_schema\x18\x1f \x01(\x0b\x32 .tecton_proto.common.SparkSchemaR\x18\x66orcedMaterializedSchema\x1a:\n\x0cOptionsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\x0b\n\ttype_argsJ\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\rJ\x04\x08\r\x10\x0eJ\x04\x08\x10\x10\x11J\x04\x08\x11\x10\x12J\x04\x08\x12\x10\x13J\x04\x08\x13\x10\x14J\x04\x08\x14\x10\x15J\x04\x08\x15\x10\x16J\x04\x08\x16\x10\x17J\x04\x08\x1b\x10\x1c\"f\n\x11\x45ntityKeyOverride\x12\x34\n\tentity_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x08\x65ntityId\x12\x1b\n\tjoin_keys\x18\x02 \x03(\tR\x08joinKeys\"K\n\x0e\x42\x61\x63kfillConfig\x12\x39\n\x04mode\x18\x01 \x01(\x0e\x32%.tecton_proto.args.BackfillConfigModeR\x04mode\"\xce\x01\n\x0cOutputStream\x12)\n\x10include_features\x18\x01 \x01(\x08R\x0fincludeFeatures\x12\x44\n\x07kinesis\x18\x02 \x01(\x0b\x32(.tecton_proto.args.KinesisDataSourceArgsH\x00R\x07kinesis\x12>\n\x05kafka\x18\x03 \x01(\x0b\x32&.tecton_proto.args.KafkaDataSourceArgsH\x00R\x05kafkaB\r\n\x0bstream_sink\"\xb9\x08\n\x0cTemporalArgs\x12#\n\rtimestamp_key\x18\x01 \x01(\tR\x0ctimestampKey\x12\x46\n\x11schedule_interval\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\x10scheduleInterval\x12O\n\x12\x66\x65\x61ture_start_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x10\x66\x65\x61tureStartTime\x12^\n\x1emax_batch_aggregation_interval\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x1bmaxBatchAggregationInterval\x12\x41\n\x0bserving_ttl\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x06R\nservingTtl\x12S\n\x0eoffline_config\x18\x06 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigR\rofflineConfig\x12U\n\x15\x62\x61tch_materialization\x18\x07 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x14\x62\x61tchMaterialization\x12]\n\x19streaming_materialization\x18\x08 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x18streamingMaterialization\x12J\n\nmonitoring\x18\t \x01(\x0b\x32#.tecton_proto.args.MonitoringConfigB\x05\x92M\x02\x08\x01R\nmonitoring\x12M\n\x10\x64\x61ta_source_type\x18\n \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12Q\n\x0f\x62\x61\x63kfill_config\x18\x0b \x01(\x0b\x32!.tecton_proto.args.BackfillConfigB\x05\x92M\x02\x08\x03R\x0e\x62\x61\x63kfillConfig\x12T\n\x13online_store_config\x18\x0c \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigR\x11onlineStoreConfig\x12\x33\n\x15incremental_backfills\x18\r \x01(\x08R\x14incrementalBackfills\x12\x44\n\routput_stream\x18\x0e \x01(\x0b\x32\x1f.tecton_proto.args.OutputStreamR\x0coutputStream\"\xe9\x08\n\x15TemporalAggregateArgs\x12k\n!aggregation_slide_period_duration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x05R\x1e\x61ggregationSlidePeriodDuration\x12\x38\n\x18\x61ggregation_slide_period\x18\x02 \x01(\tR\x16\x61ggregationSlidePeriod\x12I\n\x0c\x61ggregations\x18\x03 \x03(\x0b\x32%.tecton_proto.args.FeatureAggregationR\x0c\x61ggregations\x12#\n\rtimestamp_key\x18\x04 \x01(\tR\x0ctimestampKey\x12\x46\n\x11schedule_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationR\x10scheduleInterval\x12O\n\x12\x66\x65\x61ture_start_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x10\x66\x65\x61tureStartTime\x12^\n\x1emax_batch_aggregation_interval\x18\x07 \x01(\x0b\x32\x19.google.protobuf.DurationR\x1bmaxBatchAggregationInterval\x12S\n\x0eoffline_config\x18\x08 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigR\rofflineConfig\x12U\n\x15\x62\x61tch_materialization\x18\t \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x14\x62\x61tchMaterialization\x12]\n\x19streaming_materialization\x18\n \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x18streamingMaterialization\x12J\n\nmonitoring\x18\x0b \x01(\x0b\x32#.tecton_proto.args.MonitoringConfigB\x05\x92M\x02\x08\x01R\nmonitoring\x12M\n\x10\x64\x61ta_source_type\x18\x0c \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12T\n\x13online_store_config\x18\r \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigR\x11onlineStoreConfig\x12\x44\n\routput_stream\x18\x0e \x01(\x0b\x32\x1f.tecton_proto.args.OutputStreamR\x0coutputStream\"\xff\x11\n\x1bMaterializedFeatureViewArgs\x12\'\n\x0ftimestamp_field\x18\x01 \x01(\tR\x0etimestampField\x12G\n\x0e\x62\x61tch_schedule\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02 \x08R\rbatchSchedule\x12O\n\x12\x66\x65\x61ture_start_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x10\x66\x65\x61tureStartTime\x12i\n manual_trigger_backfill_end_time\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x1cmanualTriggerBackfillEndTime\x12\x85\x01\n\x15max_backfill_interval\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationB6\x92M\"* \n\x1emax_batch_aggregation_interval\x92M\t*\x07\x12\x05\x30.7.0\x92M\x02\x08\x01R\x13maxBackfillInterval\x12\x41\n\x0bserving_ttl\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x06R\nservingTtl\x12\x85\x01\n\x14offline_store_legacy\x18\x06 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigB%\x92M\x02 \r\x92M\x11*\x0f\n\roffline_store\x92M\t*\x07\x12\x05\x30.8.0R\x12offlineStoreLegacy\x12Q\n\roffline_store\x18\x19 \x01(\x0b\x32%.tecton_proto.args.OfflineStoreConfigB\x05\x92M\x02 \x0cR\x0cofflineStore\x12\x45\n\rbatch_compute\x18\x07 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x0c\x62\x61tchCompute\x12G\n\x0estream_compute\x18\x08 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\rstreamCompute\x12O\n\nmonitoring\x18\t \x01(\x0b\x32#.tecton_proto.args.MonitoringConfigB\n\x92M\x02\x08\x01\x92M\x02\x10\x01R\nmonitoring\x12M\n\x10\x64\x61ta_source_type\x18\n \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12G\n\x0conline_store\x18\x0b \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigR\x0bonlineStore\x12\x33\n\x15incremental_backfills\x18\x0c \x01(\x08R\x14incrementalBackfills\x12L\n\x14\x61ggregation_interval\x18\r \x01(\x0b\x32\x19.google.protobuf.DurationR\x13\x61ggregationInterval\x12\x64\n\x16stream_processing_mode\x18\x0f \x01(\x0e\x32\'.tecton_proto.args.StreamProcessingModeB\x05\x92M\x02 \x06R\x14streamProcessingMode\x12I\n\x0c\x61ggregations\x18\x0e \x03(\x0b\x32%.tecton_proto.args.FeatureAggregationR\x0c\x61ggregations\x12\x44\n\routput_stream\x18\x10 \x01(\x0b\x32\x1f.tecton_proto.args.OutputStreamR\x0coutputStream\x12O\n\rbatch_trigger\x18\x11 \x01(\x0e\x32#.tecton_proto.args.BatchTriggerTypeB\x05\x92M\x02\x08\x01R\x0c\x62\x61tchTrigger\x12:\n\x06schema\x18\x12 \x01(\x0b\x32\x1b.tecton_proto.common.SchemaB\x05\x92M\x02\x08\x06R\x06schema\x12:\n\x19\x61ggregation_secondary_key\x18\x14 \x01(\tR\x17\x61ggregationSecondaryKey\x12s\n\x1csecondary_key_output_columns\x18\x15 \x03(\x0b\x32+.tecton_proto.args.SecondaryKeyOutputColumnB\x05\x92M\x02\x18\x05R\x19secondaryKeyOutputColumns\x12I\n\x1drun_transformation_validation\x18\x16 \x01(\x08\x42\x05\x92M\x02\x08\x01R\x1brunTransformationValidation\x12K\n\x1etecton_materialization_runtime\x18\x17 \x01(\tB\x05\x92M\x02\x08\x01R\x1ctectonMaterializationRuntime\x12J\n\x13lifetime_start_time\x18\x18 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11lifetimeStartTime\x12\x38\n\x18\x62\x61tch_compaction_enabled\x18\x1a \x01(\x08R\x16\x62\x61tchCompactionEnabled\x12:\n\x19stream_compaction_enabled\x18\x1c \x01(\x08R\x17streamCompactionEnabled\x12X\n\x1bstream_compaction_tile_size\x18\x1d \x01(\x0b\x32\x19.google.protobuf.DurationR\x18streamCompactionTileSize\x12\'\n\x0b\x65nvironment\x18\x1b \x01(\tB\x05\x92M\x02\x08\x01R\x0b\x65nvironment\"\xd3\x01\n\x0cOnDemandArgs\x12L\n\routput_schema\x18\x01 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x10\x03R\x0coutputSchema\x12?\n\x06schema\x18\x02 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x08\x05R\x06schema\x12.\n\x0c\x65nvironments\x18\x04 \x03(\tB\n\x92M\x02\x08\x01\x82}\x02\x08\x05R\x0c\x65nvironmentsJ\x04\x08\x03\x10\x04\"\x97\x08\n\x10\x46\x65\x61tureTableArgs\x12L\n\routput_schema\x18\x01 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x10\x03R\x0coutputSchema\x12?\n\x06schema\x18\x06 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x08\x05R\x06schema\x12\x41\n\x0bserving_ttl\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x06R\nservingTtl\x12Z\n\x0eoffline_config\x18\x03 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigB\x05\x82}\x02\x10\x03R\rofflineConfig\x12\x8a\x01\n\x14offline_store_legacy\x18\x07 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigB*\x82}\x02\x08\x05\x92M\x02 \r\x92M\x11*\x0f\n\roffline_store\x92M\t*\x07\x12\x05\x30.8.0R\x12offlineStoreLegacy\x12Q\n\roffline_store\x18\x0c \x01(\x0b\x32%.tecton_proto.args.OfflineStoreConfigB\x05\x92M\x02 \x0cR\x0cofflineStore\x12[\n\x13online_store_config\x18\x04 \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigB\x05\x82}\x02\x10\x03R\x11onlineStoreConfig\x12N\n\x0conline_store\x18\x08 \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigB\x05\x82}\x02\x08\x05R\x0bonlineStore\x12\\\n\x15\x62\x61tch_materialization\x18\x05 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigB\x05\x82}\x02\x10\x03R\x14\x62\x61tchMaterialization\x12L\n\rbatch_compute\x18\t \x01(\x0b\x32 .tecton_proto.args.ClusterConfigB\x05\x82}\x02\x08\x05R\x0c\x62\x61tchCompute\x12O\n\nmonitoring\x18\n \x01(\x0b\x32#.tecton_proto.args.MonitoringConfigB\n\x92M\x02\x08\x01\x92M\x02\x10\x01R\nmonitoring\x12K\n\x1etecton_materialization_runtime\x18\x0b \x01(\tB\x05\x92M\x02\x08\x01R\x1ctectonMaterializationRuntime\"\x94\x06\n\x12\x46\x65\x61tureAggregation\x12\x16\n\x06\x63olumn\x18\x01 \x01(\tR\x06\x63olumn\x12\x1a\n\x08\x66unction\x18\x02 \x01(\tR\x08\x66unction\x12\x62\n\x0f\x66unction_params\x18\x05 \x03(\x0b\x32\x39.tecton_proto.args.FeatureAggregation.FunctionParamsEntryR\x0e\x66unctionParams\x12\x43\n\x0ctime_windows\x18\x03 \x03(\x0b\x32\x19.google.protobuf.DurationB\x05\x82}\x02\x10\x03R\x0btimeWindows\x12\x34\n\x10time_window_strs\x18\x04 \x03(\tB\n\x82}\x02\x10\x03\x92M\x02\x08\x05R\x0etimeWindowStrs\x12q\n\x12time_window_legacy\x18\x06 \x01(\x0b\x32\x19.google.protobuf.DurationB(\x92M\x0f*\r\n\x0btime_window\x92M\t*\x07\x12\x05\x30.8.0\x82}\x02\x08\x05\x92M\x02 \tR\x10timeWindowLegacy\x12\x1e\n\x04name\x18\x07 \x01(\tB\n\x82}\x02\x08\x05\x92M\x02 \x01R\x04name\x12G\n\x0btime_window\x18\x08 \x01(\x0b\x32\x1d.tecton_proto.args.TimeWindowB\x05\x92M\x02 \nH\x00R\ntimeWindow\x12N\n\x0flifetime_window\x18\t \x01(\x0b\x32#.tecton_proto.common.LifetimeWindowH\x00R\x0elifetimeWindow\x12S\n\x12time_window_series\x18\n \x01(\x0b\x32#.tecton_proto.args.TimeWindowSeriesH\x00R\x10timeWindowSeries\x1a`\n\x13\x46unctionParamsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x33\n\x05value\x18\x02 \x01(\x0b\x32\x1d.tecton_proto.args.ParamValueR\x05value:\x02\x38\x01\x42\x08\n\x06window\"]\n\nParamValue\x12!\n\x0bint64_value\x18\x01 \x01(\x03H\x00R\nint64Value\x12#\n\x0c\x64ouble_value\x18\x02 \x01(\x01H\x00R\x0b\x64oubleValueB\x07\n\x05value\"\x8f\x01\n\x11\x44\x61taQualityConfig\x12\x37\n\x14\x64\x61ta_quality_enabled\x18\x01 \x01(\x08\x42\x05\x92M\x02 \x03R\x12\x64\x61taQualityEnabled\x12\x41\n\x19skip_default_expectations\x18\x02 \x01(\x08\x42\x05\x92M\x02 \x03R\x17skipDefaultExpectations\"\xac\x05\n\rClusterConfig\x12\\\n\x10\x65xisting_cluster\x18\x01 \x01(\x0b\x32(.tecton_proto.args.ExistingClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x0f\x65xistingCluster\x12S\n\x0enew_databricks\x18\x02 \x01(\x0b\x32#.tecton_proto.args.NewClusterConfigB\x05\x92M\x02\x08\x01H\x00R\rnewDatabricks\x12\x45\n\x07new_emr\x18\x03 \x01(\x0b\x32#.tecton_proto.args.NewClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x06newEmr\x12^\n\x0fimplicit_config\x18\x04 \x01(\x0b\x32\'.tecton_proto.args.DefaultClusterConfigB\n\x92M\x02\x08\x01\x92M\x02\x18\x05H\x00R\x0eimplicitConfig\x12V\n\x0fjson_databricks\x18\x05 \x01(\x0b\x32$.tecton_proto.args.JsonClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x0ejsonDatabricks\x12H\n\x08json_emr\x18\x06 \x01(\x0b\x32$.tecton_proto.args.JsonClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x07jsonEmr\x12R\n\rjson_dataproc\x18\x07 \x01(\x0b\x32$.tecton_proto.args.JsonClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x0cjsonDataproc\x12\x41\n\x04rift\x18\x08 \x01(\x0b\x32$.tecton_proto.args.RiftClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x04riftB\x08\n\x06\x63onfig\"@\n\x11JsonClusterConfig\x12+\n\x04json\x18\x01 \x01(\x0b\x32\x17.google.protobuf.StructR\x04json\"G\n\x15\x45xistingClusterConfig\x12.\n\x13\x65xisting_cluster_id\x18\x01 \x01(\tR\x11\x65xistingClusterId\"\x9f\x03\n\x10NewClusterConfig\x12#\n\rinstance_type\x18\x01 \x01(\tR\x0cinstanceType\x12\x33\n\x15instance_availability\x18\x06 \x01(\tR\x14instanceAvailability\x12*\n\x11number_of_workers\x18\x02 \x01(\x05R\x0fnumberOfWorkers\x12\x32\n\x16root_volume_size_in_gb\x18\x03 \x01(\x05R\x12rootVolumeSizeInGb\x12\x34\n\x16\x65xtra_pip_dependencies\x18\x04 \x03(\tR\x14\x65xtraPipDependencies\x12\x41\n\x0cspark_config\x18\x05 \x01(\x0b\x32\x1e.tecton_proto.args.SparkConfigR\x0bsparkConfig\x12&\n\x0f\x66irst_on_demand\x18\x07 \x01(\x05R\rfirstOnDemand\x12\x30\n\x14pinned_spark_version\x18\x08 \x01(\tR\x12pinnedSparkVersion\"8\n\x11RiftClusterConfig\x12#\n\rinstance_type\x18\x01 \x01(\tR\x0cinstanceType\"\xbd\x01\n\x14\x44\x65\x66\x61ultClusterConfig\x12\x38\n\x18\x64\x61tabricks_spark_version\x18\x01 \x01(\tR\x16\x64\x61tabricksSparkVersion\x12*\n\x11\x65mr_spark_version\x18\x02 \x01(\tR\x0f\x65mrSparkVersion\x12?\n\x1ctecton_compute_instance_type\x18\x03 \x01(\tR\x19tectonComputeInstanceType\"\x83\x03\n\x0bSparkConfig\x12.\n\x13spark_driver_memory\x18\x01 \x01(\tR\x11sparkDriverMemory\x12\x32\n\x15spark_executor_memory\x18\x02 \x01(\tR\x13sparkExecutorMemory\x12?\n\x1cspark_driver_memory_overhead\x18\x03 \x01(\tR\x19sparkDriverMemoryOverhead\x12\x43\n\x1espark_executor_memory_overhead\x18\x04 \x01(\tR\x1bsparkExecutorMemoryOverhead\x12L\n\nspark_conf\x18\x05 \x03(\x0b\x32-.tecton_proto.args.SparkConfig.SparkConfEntryR\tsparkConf\x1a<\n\x0eSparkConfEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xe6\x01\n\x11OnlineStoreConfig\x12@\n\x06\x64ynamo\x18\x01 \x01(\x0b\x32&.tecton_proto.args.DynamoDbOnlineStoreH\x00R\x06\x64ynamo\x12;\n\x05redis\x18\x02 \x01(\x0b\x32#.tecton_proto.args.RedisOnlineStoreH\x00R\x05redis\x12\x44\n\x08\x62igtable\x18\x03 \x01(\x0b\x32&.tecton_proto.args.BigtableOnlineStoreH\x00R\x08\x62igtableB\x0c\n\nstore_type\"G\n\x13\x44ynamoDbOnlineStore\x12\x18\n\x07\x65nabled\x18\x03 \x01(\x08R\x07\x65nabledJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06\"\xc8\x01\n\x10RedisOnlineStore\x12\x30\n\x10primary_endpoint\x18\x02 \x01(\tB\x05\x92M\x02\x08\x06R\x0fprimaryEndpoint\x12=\n\x14\x61uthentication_token\x18\x04 \x01(\tB\n\x92M\x02\x08\x01\x92M\x02\x18\x06R\x13\x61uthenticationToken\x12\x1f\n\x07\x65nabled\x18\x05 \x01(\x08\x42\x05\x92M\x02\x18\x05R\x07\x65nabledJ\x04\x08\x01\x10\x02J\x04\x08\x03\x10\x04J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\t\x10\n\"o\n\x13\x42igtableOnlineStore\x12\x18\n\x07\x65nabled\x18\x01 \x01(\x08R\x07\x65nabled\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x1f\n\x0binstance_id\x18\x03 \x01(\tR\ninstanceId\"\xdb\x01\n\x19OfflineFeatureStoreConfig\x12<\n\x07parquet\x18\x01 \x01(\x0b\x32 .tecton_proto.args.ParquetConfigH\x00R\x07parquet\x12\x36\n\x05\x64\x65lta\x18\x02 \x01(\x0b\x32\x1e.tecton_proto.args.DeltaConfigH\x00R\x05\x64\x65lta\x12:\n\x15subdirectory_override\x18\x03 \x01(\tB\x05\x92M\x02\x08\x01R\x14subdirectoryOverrideB\x0c\n\nstore_type\"\x0f\n\rParquetConfig\"X\n\x0b\x44\x65ltaConfig\x12I\n\x13time_partition_size\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x11timePartitionSize\"\x80\x02\n\x12OfflineStoreConfig\x12^\n\x14staging_table_format\x18\x01 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigR\x12stagingTableFormat\x12\x39\n\x15publish_full_features\x18\x02 \x01(\x08\x42\x05\x92M\x02\x08\x01R\x13publishFullFeatures\x12O\n\x12publish_start_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x10publishStartTime\"\x99\x02\n\x10MonitoringConfig\x12+\n\x11monitor_freshness\x18\x01 \x01(\x08R\x10monitorFreshness\x12^\n\x1a\x65xpected_feature_freshness\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x82}\x02\x10\x03R\x18\x65xpectedFeatureFreshness\x12O\n\x12\x65xpected_freshness\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x82}\x02\x08\x05R\x11\x65xpectedFreshness\x12\'\n\x0b\x61lert_email\x18\x03 \x01(\tB\x06\xf2\xe2\x02\x02\x08\x01R\nalertEmail\"\x9f\x02\n\x18SecondaryKeyOutputColumn\x12@\n\x0btime_window\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.args.TimeWindowH\x00R\ntimeWindow\x12N\n\x0flifetime_window\x18\x03 \x01(\x0b\x32#.tecton_proto.common.LifetimeWindowH\x00R\x0elifetimeWindow\x12S\n\x12time_window_series\x18\x04 \x01(\x0b\x32#.tecton_proto.args.TimeWindowSeriesH\x00R\x10timeWindowSeries\x12\x12\n\x04name\x18\x02 \x01(\tR\x04nameB\x08\n\x06window\"\x83\x01\n\nTimeWindow\x12\x42\n\x0fwindow_duration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x0ewindowDuration\x12\x31\n\x06offset\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\x06offset\"\x86\x02\n\x10TimeWindowSeries\x12<\n\x0cseries_start\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x0bseriesStart\x12\x38\n\nseries_end\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\tseriesEnd\x12\x36\n\tstep_size\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationR\x08stepSize\x12\x42\n\x0fwindow_duration\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x0ewindowDuration\"5\n\x0b\x43\x61\x63heConfig\x12&\n\x0fmax_age_seconds\x18\x01 \x01(\x03R\rmaxAgeSeconds*\xed\x01\n\x0f\x46\x65\x61tureViewType\x12!\n\x1d\x46\x45\x41TURE_VIEW_TYPE_UNSPECIFIED\x10\x00\x12\x1e\n\x1a\x46\x45\x41TURE_VIEW_TYPE_TEMPORAL\x10\x01\x12(\n$FEATURE_VIEW_TYPE_TEMPORAL_AGGREGATE\x10\x02\x12\x1f\n\x1b\x46\x45\x41TURE_VIEW_TYPE_ON_DEMAND\x10\x03\x12#\n\x1f\x46\x45\x41TURE_VIEW_TYPE_FEATURE_TABLE\x10\x04\x12\'\n#FEATURE_VIEW_TYPE_FWV5_FEATURE_VIEW\x10\x05*\xbf\x01\n\x12\x42\x61\x63kfillConfigMode\x12$\n BACKFILL_CONFIG_MODE_UNSPECIFIED\x10\x00\x12?\n;BACKFILL_CONFIG_MODE_SINGLE_BATCH_SCHEDULE_INTERVAL_PER_JOB\x10\x01\x12\x42\n>BACKFILL_CONFIG_MODE_MULTIPLE_BATCH_SCHEDULE_INTERVALS_PER_JOB\x10\x02*\x8f\x01\n\x14StreamProcessingMode\x12&\n\"STREAM_PROCESSING_MODE_UNSPECIFIED\x10\x00\x12(\n$STREAM_PROCESSING_MODE_TIME_INTERVAL\x10\x01\x12%\n!STREAM_PROCESSING_MODE_CONTINUOUS\x10\x02*\xa8\x01\n\x10\x42\x61tchTriggerType\x12\"\n\x1e\x42\x41TCH_TRIGGER_TYPE_UNSPECIFIED\x10\x00\x12 \n\x1c\x42\x41TCH_TRIGGER_TYPE_SCHEDULED\x10\x01\x12\x1d\n\x19\x42\x41TCH_TRIGGER_TYPE_MANUAL\x10\x02\x12/\n+BATCH_TRIGGER_TYPE_NO_BATCH_MATERIALIZATION\x10\x03\x42\x13\n\x0f\x63om.tecton.argsP\x01')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$tecton_proto/args/feature_view.proto\x12\x11tecton_proto.args\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\"tecton_proto/args/basic_info.proto\x1a#tecton_proto/args/data_source.proto\x1a$tecton_proto/args/diff_options.proto\x1a tecton_proto/args/pipeline.proto\x1a+tecton_proto/args/version_constraints.proto\x1a+tecton_proto/common/analytics_options.proto\x1a&tecton_proto/common/compute_mode.proto\x1a*tecton_proto/common/data_source_type.proto\x1a+tecton_proto/common/framework_version.proto\x1a\x1ctecton_proto/common/id.proto\x1a tecton_proto/common/schema.proto\x1a&tecton_proto/common/spark_schema.proto\x1a%tecton_proto/common/time_window.proto\"\xfd\r\n\x0f\x46\x65\x61tureViewArgs\x12?\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\rfeatureViewId\x12N\n\x11\x66\x65\x61ture_view_type\x18\x02 \x01(\x0e\x32\".tecton_proto.args.FeatureViewTypeR\x0f\x66\x65\x61tureViewType\x12\x37\n\x04info\x18\x03 \x01(\x0b\x32\x1c.tecton_proto.args.BasicInfoB\x05\x92M\x02\x10\x01R\x04info\x12\x46\n\x07version\x18\x1d \x01(\x0e\x32%.tecton_proto.common.FrameworkVersionB\x05\x92M\x02\x08\x05R\x07version\x12.\n\x0fprevent_destroy\x18  \x01(\x08\x42\x05\x92M\x02\x08\x01R\x0epreventDestroy\x12P\n\x07options\x18\" \x03(\x0b\x32/.tecton_proto.args.FeatureViewArgs.OptionsEntryB\x05\x92M\x02\x08\x01R\x07options\x12H\n\x0c\x63\x61\x63he_config\x18$ \x01(\x0b\x32\x1e.tecton_proto.args.CacheConfigB\x05\x92M\x02\x08\x01R\x0b\x63\x61\x63heConfig\x12G\n\x08\x65ntities\x18\x04 \x03(\x0b\x32$.tecton_proto.args.EntityKeyOverrideB\x05\x92M\x02\x08\x06R\x08\x65ntities\x12M\n\rtemporal_args\x18\x17 \x01(\x0b\x32\x1f.tecton_proto.args.TemporalArgsB\x05\x92M\x02\x10\x01H\x00R\x0ctemporalArgs\x12i\n\x17temporal_aggregate_args\x18\x18 \x01(\x0b\x32(.tecton_proto.args.TemporalAggregateArgsB\x05\x92M\x02\x10\x01H\x00R\x15temporalAggregateArgs\x12|\n\x1ematerialized_feature_view_args\x18\x1c \x01(\x0b\x32..tecton_proto.args.MaterializedFeatureViewArgsB\x05\x92M\x02\x10\x01H\x00R\x1bmaterializedFeatureViewArgs\x12N\n\x0eon_demand_args\x18\x19 \x01(\x0b\x32\x1f.tecton_proto.args.OnDemandArgsB\x05\x92M\x02\x10\x01H\x00R\x0conDemandArgs\x12Z\n\x12\x66\x65\x61ture_table_args\x18\x1a \x01(\x0b\x32#.tecton_proto.args.FeatureTableArgsB\x05\x92M\x02\x10\x01H\x00R\x10\x66\x65\x61tureTableArgs\x12\x30\n\x14online_serving_index\x18\x05 \x03(\tR\x12onlineServingIndex\x12,\n\x0eonline_enabled\x18\x0e \x01(\x08\x42\x05\x92M\x02 \x0bR\ronlineEnabled\x12.\n\x0foffline_enabled\x18\x0f \x01(\x08\x42\x05\x92M\x02 \x0bR\x0eofflineEnabled\x12Z\n\x12\x62\x61tch_compute_mode\x18# \x01(\x0e\x32%.tecton_proto.common.BatchComputeModeB\x05\x92M\x02\x08\tR\x10\x62\x61tchComputeMode\x12>\n\x08pipeline\x18\x06 \x01(\x0b\x32\x1b.tecton_proto.args.PipelineB\x05\x92M\x02\x08\x06R\x08pipeline\x12`\n\x13\x64\x61ta_quality_config\x18! \x01(\x0b\x32$.tecton_proto.args.DataQualityConfigB\n\x92M\x02\x08\x01\x92M\x02\x10\x01R\x11\x64\x61taQualityConfig\x12N\n\x12\x66orced_view_schema\x18\x1e \x01(\x0b\x32 .tecton_proto.common.SparkSchemaR\x10\x66orcedViewSchema\x12^\n\x1a\x66orced_materialized_schema\x18\x1f \x01(\x0b\x32 .tecton_proto.common.SparkSchemaR\x18\x66orcedMaterializedSchema\x1a:\n\x0cOptionsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\x0b\n\ttype_argsJ\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\rJ\x04\x08\r\x10\x0eJ\x04\x08\x10\x10\x11J\x04\x08\x11\x10\x12J\x04\x08\x12\x10\x13J\x04\x08\x13\x10\x14J\x04\x08\x14\x10\x15J\x04\x08\x15\x10\x16J\x04\x08\x16\x10\x17J\x04\x08\x1b\x10\x1c\"f\n\x11\x45ntityKeyOverride\x12\x34\n\tentity_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x08\x65ntityId\x12\x1b\n\tjoin_keys\x18\x02 \x03(\tR\x08joinKeys\"K\n\x0e\x42\x61\x63kfillConfig\x12\x39\n\x04mode\x18\x01 \x01(\x0e\x32%.tecton_proto.args.BackfillConfigModeR\x04mode\"\xce\x01\n\x0cOutputStream\x12)\n\x10include_features\x18\x01 \x01(\x08R\x0fincludeFeatures\x12\x44\n\x07kinesis\x18\x02 \x01(\x0b\x32(.tecton_proto.args.KinesisDataSourceArgsH\x00R\x07kinesis\x12>\n\x05kafka\x18\x03 \x01(\x0b\x32&.tecton_proto.args.KafkaDataSourceArgsH\x00R\x05kafkaB\r\n\x0bstream_sink\"\xb9\x08\n\x0cTemporalArgs\x12#\n\rtimestamp_key\x18\x01 \x01(\tR\x0ctimestampKey\x12\x46\n\x11schedule_interval\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\x10scheduleInterval\x12O\n\x12\x66\x65\x61ture_start_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x10\x66\x65\x61tureStartTime\x12^\n\x1emax_batch_aggregation_interval\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x1bmaxBatchAggregationInterval\x12\x41\n\x0bserving_ttl\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x06R\nservingTtl\x12S\n\x0eoffline_config\x18\x06 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigR\rofflineConfig\x12U\n\x15\x62\x61tch_materialization\x18\x07 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x14\x62\x61tchMaterialization\x12]\n\x19streaming_materialization\x18\x08 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x18streamingMaterialization\x12J\n\nmonitoring\x18\t \x01(\x0b\x32#.tecton_proto.args.MonitoringConfigB\x05\x92M\x02\x08\x01R\nmonitoring\x12M\n\x10\x64\x61ta_source_type\x18\n \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12Q\n\x0f\x62\x61\x63kfill_config\x18\x0b \x01(\x0b\x32!.tecton_proto.args.BackfillConfigB\x05\x92M\x02\x08\x03R\x0e\x62\x61\x63kfillConfig\x12T\n\x13online_store_config\x18\x0c \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigR\x11onlineStoreConfig\x12\x33\n\x15incremental_backfills\x18\r \x01(\x08R\x14incrementalBackfills\x12\x44\n\routput_stream\x18\x0e \x01(\x0b\x32\x1f.tecton_proto.args.OutputStreamR\x0coutputStream\"\xe9\x08\n\x15TemporalAggregateArgs\x12k\n!aggregation_slide_period_duration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x05R\x1e\x61ggregationSlidePeriodDuration\x12\x38\n\x18\x61ggregation_slide_period\x18\x02 \x01(\tR\x16\x61ggregationSlidePeriod\x12I\n\x0c\x61ggregations\x18\x03 \x03(\x0b\x32%.tecton_proto.args.FeatureAggregationR\x0c\x61ggregations\x12#\n\rtimestamp_key\x18\x04 \x01(\tR\x0ctimestampKey\x12\x46\n\x11schedule_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationR\x10scheduleInterval\x12O\n\x12\x66\x65\x61ture_start_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x10\x66\x65\x61tureStartTime\x12^\n\x1emax_batch_aggregation_interval\x18\x07 \x01(\x0b\x32\x19.google.protobuf.DurationR\x1bmaxBatchAggregationInterval\x12S\n\x0eoffline_config\x18\x08 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigR\rofflineConfig\x12U\n\x15\x62\x61tch_materialization\x18\t \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x14\x62\x61tchMaterialization\x12]\n\x19streaming_materialization\x18\n \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x18streamingMaterialization\x12J\n\nmonitoring\x18\x0b \x01(\x0b\x32#.tecton_proto.args.MonitoringConfigB\x05\x92M\x02\x08\x01R\nmonitoring\x12M\n\x10\x64\x61ta_source_type\x18\x0c \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12T\n\x13online_store_config\x18\r \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigR\x11onlineStoreConfig\x12\x44\n\routput_stream\x18\x0e \x01(\x0b\x32\x1f.tecton_proto.args.OutputStreamR\x0coutputStream\"\xd7\x11\n\x1bMaterializedFeatureViewArgs\x12\'\n\x0ftimestamp_field\x18\x01 \x01(\tR\x0etimestampField\x12G\n\x0e\x62\x61tch_schedule\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02 \x08R\rbatchSchedule\x12O\n\x12\x66\x65\x61ture_start_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x10\x66\x65\x61tureStartTime\x12i\n manual_trigger_backfill_end_time\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x1cmanualTriggerBackfillEndTime\x12\x85\x01\n\x15max_backfill_interval\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationB6\x92M\"* \n\x1emax_batch_aggregation_interval\x92M\t*\x07\x12\x05\x30.7.0\x92M\x02\x08\x01R\x13maxBackfillInterval\x12\x41\n\x0bserving_ttl\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x06R\nservingTtl\x12\x85\x01\n\x14offline_store_legacy\x18\x06 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigB%\x92M\x02 \r\x92M\x11*\x0f\n\roffline_store\x92M\t*\x07\x12\x05\x30.8.0R\x12offlineStoreLegacy\x12Q\n\roffline_store\x18\x19 \x01(\x0b\x32%.tecton_proto.args.OfflineStoreConfigB\x05\x92M\x02 \x0cR\x0cofflineStore\x12\x45\n\rbatch_compute\x18\x07 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x0c\x62\x61tchCompute\x12G\n\x0estream_compute\x18\x08 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\rstreamCompute\x12O\n\nmonitoring\x18\t \x01(\x0b\x32#.tecton_proto.args.MonitoringConfigB\n\x92M\x02\x08\x01\x92M\x02\x10\x01R\nmonitoring\x12M\n\x10\x64\x61ta_source_type\x18\n \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12G\n\x0conline_store\x18\x0b \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigR\x0bonlineStore\x12\x33\n\x15incremental_backfills\x18\x0c \x01(\x08R\x14incrementalBackfills\x12L\n\x14\x61ggregation_interval\x18\r \x01(\x0b\x32\x19.google.protobuf.DurationR\x13\x61ggregationInterval\x12\x64\n\x16stream_processing_mode\x18\x0f \x01(\x0e\x32\'.tecton_proto.args.StreamProcessingModeB\x05\x92M\x02 \x06R\x14streamProcessingMode\x12I\n\x0c\x61ggregations\x18\x0e \x03(\x0b\x32%.tecton_proto.args.FeatureAggregationR\x0c\x61ggregations\x12\x44\n\routput_stream\x18\x10 \x01(\x0b\x32\x1f.tecton_proto.args.OutputStreamR\x0coutputStream\x12O\n\rbatch_trigger\x18\x11 \x01(\x0e\x32#.tecton_proto.args.BatchTriggerTypeB\x05\x92M\x02\x08\x01R\x0c\x62\x61tchTrigger\x12:\n\x06schema\x18\x12 \x01(\x0b\x32\x1b.tecton_proto.common.SchemaB\x05\x92M\x02\x08\x06R\x06schema\x12:\n\x19\x61ggregation_secondary_key\x18\x14 \x01(\tR\x17\x61ggregationSecondaryKey\x12s\n\x1csecondary_key_output_columns\x18\x15 \x03(\x0b\x32+.tecton_proto.args.SecondaryKeyOutputColumnB\x05\x92M\x02\x18\x05R\x19secondaryKeyOutputColumns\x12I\n\x1drun_transformation_validation\x18\x16 \x01(\x08\x42\x05\x92M\x02\x08\x01R\x1brunTransformationValidation\x12K\n\x1etecton_materialization_runtime\x18\x17 \x01(\tB\x05\x92M\x02\x08\x01R\x1ctectonMaterializationRuntime\x12J\n\x13lifetime_start_time\x18\x18 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11lifetimeStartTime\x12-\n\x12\x63ompaction_enabled\x18\x1a \x01(\x08R\x11\x63ompactionEnabled\x12\x32\n\x15stream_tiling_enabled\x18\x1c \x01(\x08R\x13streamTilingEnabled\x12\x43\n\x10stream_tile_size\x18\x1d \x01(\x0b\x32\x19.google.protobuf.DurationR\x0estreamTileSize\x12\'\n\x0b\x65nvironment\x18\x1b \x01(\tB\x05\x92M\x02\x08\x01R\x0b\x65nvironment\"\xd3\x01\n\x0cOnDemandArgs\x12L\n\routput_schema\x18\x01 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x10\x03R\x0coutputSchema\x12?\n\x06schema\x18\x02 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x08\x05R\x06schema\x12.\n\x0c\x65nvironments\x18\x04 \x03(\tB\n\x92M\x02\x08\x01\x82}\x02\x08\x05R\x0c\x65nvironmentsJ\x04\x08\x03\x10\x04\"\x97\x08\n\x10\x46\x65\x61tureTableArgs\x12L\n\routput_schema\x18\x01 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x10\x03R\x0coutputSchema\x12?\n\x06schema\x18\x06 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaB\x05\x82}\x02\x08\x05R\x06schema\x12\x41\n\x0bserving_ttl\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x92M\x02\x08\x06R\nservingTtl\x12Z\n\x0eoffline_config\x18\x03 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigB\x05\x82}\x02\x10\x03R\rofflineConfig\x12\x8a\x01\n\x14offline_store_legacy\x18\x07 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigB*\x82}\x02\x08\x05\x92M\x02 \r\x92M\x11*\x0f\n\roffline_store\x92M\t*\x07\x12\x05\x30.8.0R\x12offlineStoreLegacy\x12Q\n\roffline_store\x18\x0c \x01(\x0b\x32%.tecton_proto.args.OfflineStoreConfigB\x05\x92M\x02 \x0cR\x0cofflineStore\x12[\n\x13online_store_config\x18\x04 \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigB\x05\x82}\x02\x10\x03R\x11onlineStoreConfig\x12N\n\x0conline_store\x18\x08 \x01(\x0b\x32$.tecton_proto.args.OnlineStoreConfigB\x05\x82}\x02\x08\x05R\x0bonlineStore\x12\\\n\x15\x62\x61tch_materialization\x18\x05 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigB\x05\x82}\x02\x10\x03R\x14\x62\x61tchMaterialization\x12L\n\rbatch_compute\x18\t \x01(\x0b\x32 .tecton_proto.args.ClusterConfigB\x05\x82}\x02\x08\x05R\x0c\x62\x61tchCompute\x12O\n\nmonitoring\x18\n \x01(\x0b\x32#.tecton_proto.args.MonitoringConfigB\n\x92M\x02\x08\x01\x92M\x02\x10\x01R\nmonitoring\x12K\n\x1etecton_materialization_runtime\x18\x0b \x01(\tB\x05\x92M\x02\x08\x01R\x1ctectonMaterializationRuntime\"\x94\x06\n\x12\x46\x65\x61tureAggregation\x12\x16\n\x06\x63olumn\x18\x01 \x01(\tR\x06\x63olumn\x12\x1a\n\x08\x66unction\x18\x02 \x01(\tR\x08\x66unction\x12\x62\n\x0f\x66unction_params\x18\x05 \x03(\x0b\x32\x39.tecton_proto.args.FeatureAggregation.FunctionParamsEntryR\x0e\x66unctionParams\x12\x43\n\x0ctime_windows\x18\x03 \x03(\x0b\x32\x19.google.protobuf.DurationB\x05\x82}\x02\x10\x03R\x0btimeWindows\x12\x34\n\x10time_window_strs\x18\x04 \x03(\tB\n\x82}\x02\x10\x03\x92M\x02\x08\x05R\x0etimeWindowStrs\x12q\n\x12time_window_legacy\x18\x06 \x01(\x0b\x32\x19.google.protobuf.DurationB(\x92M\x0f*\r\n\x0btime_window\x92M\t*\x07\x12\x05\x30.8.0\x82}\x02\x08\x05\x92M\x02 \tR\x10timeWindowLegacy\x12\x1e\n\x04name\x18\x07 \x01(\tB\n\x82}\x02\x08\x05\x92M\x02 \x01R\x04name\x12G\n\x0btime_window\x18\x08 \x01(\x0b\x32\x1d.tecton_proto.args.TimeWindowB\x05\x92M\x02 \nH\x00R\ntimeWindow\x12N\n\x0flifetime_window\x18\t \x01(\x0b\x32#.tecton_proto.common.LifetimeWindowH\x00R\x0elifetimeWindow\x12S\n\x12time_window_series\x18\n \x01(\x0b\x32#.tecton_proto.args.TimeWindowSeriesH\x00R\x10timeWindowSeries\x1a`\n\x13\x46unctionParamsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x33\n\x05value\x18\x02 \x01(\x0b\x32\x1d.tecton_proto.args.ParamValueR\x05value:\x02\x38\x01\x42\x08\n\x06window\"]\n\nParamValue\x12!\n\x0bint64_value\x18\x01 \x01(\x03H\x00R\nint64Value\x12#\n\x0c\x64ouble_value\x18\x02 \x01(\x01H\x00R\x0b\x64oubleValueB\x07\n\x05value\"\x8f\x01\n\x11\x44\x61taQualityConfig\x12\x37\n\x14\x64\x61ta_quality_enabled\x18\x01 \x01(\x08\x42\x05\x92M\x02 \x03R\x12\x64\x61taQualityEnabled\x12\x41\n\x19skip_default_expectations\x18\x02 \x01(\x08\x42\x05\x92M\x02 \x03R\x17skipDefaultExpectations\"\xac\x05\n\rClusterConfig\x12\\\n\x10\x65xisting_cluster\x18\x01 \x01(\x0b\x32(.tecton_proto.args.ExistingClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x0f\x65xistingCluster\x12S\n\x0enew_databricks\x18\x02 \x01(\x0b\x32#.tecton_proto.args.NewClusterConfigB\x05\x92M\x02\x08\x01H\x00R\rnewDatabricks\x12\x45\n\x07new_emr\x18\x03 \x01(\x0b\x32#.tecton_proto.args.NewClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x06newEmr\x12^\n\x0fimplicit_config\x18\x04 \x01(\x0b\x32\'.tecton_proto.args.DefaultClusterConfigB\n\x92M\x02\x08\x01\x92M\x02\x18\x05H\x00R\x0eimplicitConfig\x12V\n\x0fjson_databricks\x18\x05 \x01(\x0b\x32$.tecton_proto.args.JsonClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x0ejsonDatabricks\x12H\n\x08json_emr\x18\x06 \x01(\x0b\x32$.tecton_proto.args.JsonClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x07jsonEmr\x12R\n\rjson_dataproc\x18\x07 \x01(\x0b\x32$.tecton_proto.args.JsonClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x0cjsonDataproc\x12\x41\n\x04rift\x18\x08 \x01(\x0b\x32$.tecton_proto.args.RiftClusterConfigB\x05\x92M\x02\x08\x01H\x00R\x04riftB\x08\n\x06\x63onfig\"@\n\x11JsonClusterConfig\x12+\n\x04json\x18\x01 \x01(\x0b\x32\x17.google.protobuf.StructR\x04json\"G\n\x15\x45xistingClusterConfig\x12.\n\x13\x65xisting_cluster_id\x18\x01 \x01(\tR\x11\x65xistingClusterId\"\x9f\x03\n\x10NewClusterConfig\x12#\n\rinstance_type\x18\x01 \x01(\tR\x0cinstanceType\x12\x33\n\x15instance_availability\x18\x06 \x01(\tR\x14instanceAvailability\x12*\n\x11number_of_workers\x18\x02 \x01(\x05R\x0fnumberOfWorkers\x12\x32\n\x16root_volume_size_in_gb\x18\x03 \x01(\x05R\x12rootVolumeSizeInGb\x12\x34\n\x16\x65xtra_pip_dependencies\x18\x04 \x03(\tR\x14\x65xtraPipDependencies\x12\x41\n\x0cspark_config\x18\x05 \x01(\x0b\x32\x1e.tecton_proto.args.SparkConfigR\x0bsparkConfig\x12&\n\x0f\x66irst_on_demand\x18\x07 \x01(\x05R\rfirstOnDemand\x12\x30\n\x14pinned_spark_version\x18\x08 \x01(\tR\x12pinnedSparkVersion\"8\n\x11RiftClusterConfig\x12#\n\rinstance_type\x18\x01 \x01(\tR\x0cinstanceType\"\xbd\x01\n\x14\x44\x65\x66\x61ultClusterConfig\x12\x38\n\x18\x64\x61tabricks_spark_version\x18\x01 \x01(\tR\x16\x64\x61tabricksSparkVersion\x12*\n\x11\x65mr_spark_version\x18\x02 \x01(\tR\x0f\x65mrSparkVersion\x12?\n\x1ctecton_compute_instance_type\x18\x03 \x01(\tR\x19tectonComputeInstanceType\"\x83\x03\n\x0bSparkConfig\x12.\n\x13spark_driver_memory\x18\x01 \x01(\tR\x11sparkDriverMemory\x12\x32\n\x15spark_executor_memory\x18\x02 \x01(\tR\x13sparkExecutorMemory\x12?\n\x1cspark_driver_memory_overhead\x18\x03 \x01(\tR\x19sparkDriverMemoryOverhead\x12\x43\n\x1espark_executor_memory_overhead\x18\x04 \x01(\tR\x1bsparkExecutorMemoryOverhead\x12L\n\nspark_conf\x18\x05 \x03(\x0b\x32-.tecton_proto.args.SparkConfig.SparkConfEntryR\tsparkConf\x1a<\n\x0eSparkConfEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xe6\x01\n\x11OnlineStoreConfig\x12@\n\x06\x64ynamo\x18\x01 \x01(\x0b\x32&.tecton_proto.args.DynamoDbOnlineStoreH\x00R\x06\x64ynamo\x12;\n\x05redis\x18\x02 \x01(\x0b\x32#.tecton_proto.args.RedisOnlineStoreH\x00R\x05redis\x12\x44\n\x08\x62igtable\x18\x03 \x01(\x0b\x32&.tecton_proto.args.BigtableOnlineStoreH\x00R\x08\x62igtableB\x0c\n\nstore_type\"G\n\x13\x44ynamoDbOnlineStore\x12\x18\n\x07\x65nabled\x18\x03 \x01(\x08R\x07\x65nabledJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06\"\xc8\x01\n\x10RedisOnlineStore\x12\x30\n\x10primary_endpoint\x18\x02 \x01(\tB\x05\x92M\x02\x08\x06R\x0fprimaryEndpoint\x12=\n\x14\x61uthentication_token\x18\x04 \x01(\tB\n\x92M\x02\x08\x01\x92M\x02\x18\x06R\x13\x61uthenticationToken\x12\x1f\n\x07\x65nabled\x18\x05 \x01(\x08\x42\x05\x92M\x02\x18\x05R\x07\x65nabledJ\x04\x08\x01\x10\x02J\x04\x08\x03\x10\x04J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\t\x10\n\"o\n\x13\x42igtableOnlineStore\x12\x18\n\x07\x65nabled\x18\x01 \x01(\x08R\x07\x65nabled\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x1f\n\x0binstance_id\x18\x03 \x01(\tR\ninstanceId\"\xdb\x01\n\x19OfflineFeatureStoreConfig\x12<\n\x07parquet\x18\x01 \x01(\x0b\x32 .tecton_proto.args.ParquetConfigH\x00R\x07parquet\x12\x36\n\x05\x64\x65lta\x18\x02 \x01(\x0b\x32\x1e.tecton_proto.args.DeltaConfigH\x00R\x05\x64\x65lta\x12:\n\x15subdirectory_override\x18\x03 \x01(\tB\x05\x92M\x02\x08\x01R\x14subdirectoryOverrideB\x0c\n\nstore_type\"\x0f\n\rParquetConfig\"X\n\x0b\x44\x65ltaConfig\x12I\n\x13time_partition_size\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x11timePartitionSize\"\x80\x02\n\x12OfflineStoreConfig\x12^\n\x14staging_table_format\x18\x01 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigR\x12stagingTableFormat\x12\x39\n\x15publish_full_features\x18\x02 \x01(\x08\x42\x05\x92M\x02\x08\x01R\x13publishFullFeatures\x12O\n\x12publish_start_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x05\x92M\x02\x08\x01R\x10publishStartTime\"\x99\x02\n\x10MonitoringConfig\x12+\n\x11monitor_freshness\x18\x01 \x01(\x08R\x10monitorFreshness\x12^\n\x1a\x65xpected_feature_freshness\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x82}\x02\x10\x03R\x18\x65xpectedFeatureFreshness\x12O\n\x12\x65xpected_freshness\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationB\x05\x82}\x02\x08\x05R\x11\x65xpectedFreshness\x12\'\n\x0b\x61lert_email\x18\x03 \x01(\tB\x06\xf2\xe2\x02\x02\x08\x01R\nalertEmail\"\x9f\x02\n\x18SecondaryKeyOutputColumn\x12@\n\x0btime_window\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.args.TimeWindowH\x00R\ntimeWindow\x12N\n\x0flifetime_window\x18\x03 \x01(\x0b\x32#.tecton_proto.common.LifetimeWindowH\x00R\x0elifetimeWindow\x12S\n\x12time_window_series\x18\x04 \x01(\x0b\x32#.tecton_proto.args.TimeWindowSeriesH\x00R\x10timeWindowSeries\x12\x12\n\x04name\x18\x02 \x01(\tR\x04nameB\x08\n\x06window\"\x83\x01\n\nTimeWindow\x12\x42\n\x0fwindow_duration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x0ewindowDuration\x12\x31\n\x06offset\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\x06offset\"\x86\x02\n\x10TimeWindowSeries\x12<\n\x0cseries_start\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x0bseriesStart\x12\x38\n\nseries_end\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\tseriesEnd\x12\x36\n\tstep_size\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationR\x08stepSize\x12\x42\n\x0fwindow_duration\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x0ewindowDuration\"5\n\x0b\x43\x61\x63heConfig\x12&\n\x0fmax_age_seconds\x18\x01 \x01(\x03R\rmaxAgeSeconds*\xed\x01\n\x0f\x46\x65\x61tureViewType\x12!\n\x1d\x46\x45\x41TURE_VIEW_TYPE_UNSPECIFIED\x10\x00\x12\x1e\n\x1a\x46\x45\x41TURE_VIEW_TYPE_TEMPORAL\x10\x01\x12(\n$FEATURE_VIEW_TYPE_TEMPORAL_AGGREGATE\x10\x02\x12\x1f\n\x1b\x46\x45\x41TURE_VIEW_TYPE_ON_DEMAND\x10\x03\x12#\n\x1f\x46\x45\x41TURE_VIEW_TYPE_FEATURE_TABLE\x10\x04\x12\'\n#FEATURE_VIEW_TYPE_FWV5_FEATURE_VIEW\x10\x05*\xbf\x01\n\x12\x42\x61\x63kfillConfigMode\x12$\n BACKFILL_CONFIG_MODE_UNSPECIFIED\x10\x00\x12?\n;BACKFILL_CONFIG_MODE_SINGLE_BATCH_SCHEDULE_INTERVAL_PER_JOB\x10\x01\x12\x42\n>BACKFILL_CONFIG_MODE_MULTIPLE_BATCH_SCHEDULE_INTERVALS_PER_JOB\x10\x02*\x8f\x01\n\x14StreamProcessingMode\x12&\n\"STREAM_PROCESSING_MODE_UNSPECIFIED\x10\x00\x12(\n$STREAM_PROCESSING_MODE_TIME_INTERVAL\x10\x01\x12%\n!STREAM_PROCESSING_MODE_CONTINUOUS\x10\x02*\xa8\x01\n\x10\x42\x61tchTriggerType\x12\"\n\x1e\x42\x41TCH_TRIGGER_TYPE_UNSPECIFIED\x10\x00\x12 \n\x1c\x42\x41TCH_TRIGGER_TYPE_SCHEDULED\x10\x01\x12\x1d\n\x19\x42\x41TCH_TRIGGER_TYPE_MANUAL\x10\x02\x12/\n+BATCH_TRIGGER_TYPE_NO_BATCH_MATERIALIZATION\x10\x03\x42\x13\n\x0f\x63om.tecton.argsP\x01')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tecton_proto.args.feature_view_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\017com.tecton.argsP\001'
@@ -193,22 +193,22 @@
   _OFFLINESTORECONFIG.fields_by_name['publish_start_time']._serialized_options = b'\222M\002\010\001'
   _MONITORINGCONFIG.fields_by_name['expected_feature_freshness']._options = None
   _MONITORINGCONFIG.fields_by_name['expected_feature_freshness']._serialized_options = b'\202}\002\020\003'
   _MONITORINGCONFIG.fields_by_name['expected_freshness']._options = None
   _MONITORINGCONFIG.fields_by_name['expected_freshness']._serialized_options = b'\202}\002\010\005'
   _MONITORINGCONFIG.fields_by_name['alert_email']._options = None
   _MONITORINGCONFIG.fields_by_name['alert_email']._serialized_options = b'\362\342\002\002\010\001'
-  _FEATUREVIEWTYPE._serialized_start=13784
-  _FEATUREVIEWTYPE._serialized_end=14021
-  _BACKFILLCONFIGMODE._serialized_start=14024
-  _BACKFILLCONFIGMODE._serialized_end=14215
-  _STREAMPROCESSINGMODE._serialized_start=14218
-  _STREAMPROCESSINGMODE._serialized_end=14361
-  _BATCHTRIGGERTYPE._serialized_start=14364
-  _BATCHTRIGGERTYPE._serialized_end=14532
+  _FEATUREVIEWTYPE._serialized_start=13744
+  _FEATUREVIEWTYPE._serialized_end=13981
+  _BACKFILLCONFIGMODE._serialized_start=13984
+  _BACKFILLCONFIGMODE._serialized_end=14175
+  _STREAMPROCESSINGMODE._serialized_start=14178
+  _STREAMPROCESSINGMODE._serialized_end=14321
+  _BATCHTRIGGERTYPE._serialized_start=14324
+  _BATCHTRIGGERTYPE._serialized_end=14492
   _FEATUREVIEWARGS._serialized_start=662
   _FEATUREVIEWARGS._serialized_end=2451
   _FEATUREVIEWARGS_OPTIONSENTRY._serialized_start=2290
   _FEATUREVIEWARGS_OPTIONSENTRY._serialized_end=2348
   _ENTITYKEYOVERRIDE._serialized_start=2453
   _ENTITYKEYOVERRIDE._serialized_end=2555
   _BACKFILLCONFIG._serialized_start=2557
@@ -216,63 +216,63 @@
   _OUTPUTSTREAM._serialized_start=2635
   _OUTPUTSTREAM._serialized_end=2841
   _TEMPORALARGS._serialized_start=2844
   _TEMPORALARGS._serialized_end=3925
   _TEMPORALAGGREGATEARGS._serialized_start=3928
   _TEMPORALAGGREGATEARGS._serialized_end=5057
   _MATERIALIZEDFEATUREVIEWARGS._serialized_start=5060
-  _MATERIALIZEDFEATUREVIEWARGS._serialized_end=7363
-  _ONDEMANDARGS._serialized_start=7366
-  _ONDEMANDARGS._serialized_end=7577
-  _FEATURETABLEARGS._serialized_start=7580
-  _FEATURETABLEARGS._serialized_end=8627
-  _FEATUREAGGREGATION._serialized_start=8630
-  _FEATUREAGGREGATION._serialized_end=9418
-  _FEATUREAGGREGATION_FUNCTIONPARAMSENTRY._serialized_start=9312
-  _FEATUREAGGREGATION_FUNCTIONPARAMSENTRY._serialized_end=9408
-  _PARAMVALUE._serialized_start=9420
-  _PARAMVALUE._serialized_end=9513
-  _DATAQUALITYCONFIG._serialized_start=9516
-  _DATAQUALITYCONFIG._serialized_end=9659
-  _CLUSTERCONFIG._serialized_start=9662
-  _CLUSTERCONFIG._serialized_end=10346
-  _JSONCLUSTERCONFIG._serialized_start=10348
-  _JSONCLUSTERCONFIG._serialized_end=10412
-  _EXISTINGCLUSTERCONFIG._serialized_start=10414
-  _EXISTINGCLUSTERCONFIG._serialized_end=10485
-  _NEWCLUSTERCONFIG._serialized_start=10488
-  _NEWCLUSTERCONFIG._serialized_end=10903
-  _RIFTCLUSTERCONFIG._serialized_start=10905
-  _RIFTCLUSTERCONFIG._serialized_end=10961
-  _DEFAULTCLUSTERCONFIG._serialized_start=10964
-  _DEFAULTCLUSTERCONFIG._serialized_end=11153
-  _SPARKCONFIG._serialized_start=11156
-  _SPARKCONFIG._serialized_end=11543
-  _SPARKCONFIG_SPARKCONFENTRY._serialized_start=11483
-  _SPARKCONFIG_SPARKCONFENTRY._serialized_end=11543
-  _ONLINESTORECONFIG._serialized_start=11546
-  _ONLINESTORECONFIG._serialized_end=11776
-  _DYNAMODBONLINESTORE._serialized_start=11778
-  _DYNAMODBONLINESTORE._serialized_end=11849
-  _REDISONLINESTORE._serialized_start=11852
-  _REDISONLINESTORE._serialized_end=12052
-  _BIGTABLEONLINESTORE._serialized_start=12054
-  _BIGTABLEONLINESTORE._serialized_end=12165
-  _OFFLINEFEATURESTORECONFIG._serialized_start=12168
-  _OFFLINEFEATURESTORECONFIG._serialized_end=12387
-  _PARQUETCONFIG._serialized_start=12389
-  _PARQUETCONFIG._serialized_end=12404
-  _DELTACONFIG._serialized_start=12406
-  _DELTACONFIG._serialized_end=12494
-  _OFFLINESTORECONFIG._serialized_start=12497
-  _OFFLINESTORECONFIG._serialized_end=12753
-  _MONITORINGCONFIG._serialized_start=12756
-  _MONITORINGCONFIG._serialized_end=13037
-  _SECONDARYKEYOUTPUTCOLUMN._serialized_start=13040
-  _SECONDARYKEYOUTPUTCOLUMN._serialized_end=13327
-  _TIMEWINDOW._serialized_start=13330
-  _TIMEWINDOW._serialized_end=13461
-  _TIMEWINDOWSERIES._serialized_start=13464
-  _TIMEWINDOWSERIES._serialized_end=13726
-  _CACHECONFIG._serialized_start=13728
-  _CACHECONFIG._serialized_end=13781
+  _MATERIALIZEDFEATUREVIEWARGS._serialized_end=7323
+  _ONDEMANDARGS._serialized_start=7326
+  _ONDEMANDARGS._serialized_end=7537
+  _FEATURETABLEARGS._serialized_start=7540
+  _FEATURETABLEARGS._serialized_end=8587
+  _FEATUREAGGREGATION._serialized_start=8590
+  _FEATUREAGGREGATION._serialized_end=9378
+  _FEATUREAGGREGATION_FUNCTIONPARAMSENTRY._serialized_start=9272
+  _FEATUREAGGREGATION_FUNCTIONPARAMSENTRY._serialized_end=9368
+  _PARAMVALUE._serialized_start=9380
+  _PARAMVALUE._serialized_end=9473
+  _DATAQUALITYCONFIG._serialized_start=9476
+  _DATAQUALITYCONFIG._serialized_end=9619
+  _CLUSTERCONFIG._serialized_start=9622
+  _CLUSTERCONFIG._serialized_end=10306
+  _JSONCLUSTERCONFIG._serialized_start=10308
+  _JSONCLUSTERCONFIG._serialized_end=10372
+  _EXISTINGCLUSTERCONFIG._serialized_start=10374
+  _EXISTINGCLUSTERCONFIG._serialized_end=10445
+  _NEWCLUSTERCONFIG._serialized_start=10448
+  _NEWCLUSTERCONFIG._serialized_end=10863
+  _RIFTCLUSTERCONFIG._serialized_start=10865
+  _RIFTCLUSTERCONFIG._serialized_end=10921
+  _DEFAULTCLUSTERCONFIG._serialized_start=10924
+  _DEFAULTCLUSTERCONFIG._serialized_end=11113
+  _SPARKCONFIG._serialized_start=11116
+  _SPARKCONFIG._serialized_end=11503
+  _SPARKCONFIG_SPARKCONFENTRY._serialized_start=11443
+  _SPARKCONFIG_SPARKCONFENTRY._serialized_end=11503
+  _ONLINESTORECONFIG._serialized_start=11506
+  _ONLINESTORECONFIG._serialized_end=11736
+  _DYNAMODBONLINESTORE._serialized_start=11738
+  _DYNAMODBONLINESTORE._serialized_end=11809
+  _REDISONLINESTORE._serialized_start=11812
+  _REDISONLINESTORE._serialized_end=12012
+  _BIGTABLEONLINESTORE._serialized_start=12014
+  _BIGTABLEONLINESTORE._serialized_end=12125
+  _OFFLINEFEATURESTORECONFIG._serialized_start=12128
+  _OFFLINEFEATURESTORECONFIG._serialized_end=12347
+  _PARQUETCONFIG._serialized_start=12349
+  _PARQUETCONFIG._serialized_end=12364
+  _DELTACONFIG._serialized_start=12366
+  _DELTACONFIG._serialized_end=12454
+  _OFFLINESTORECONFIG._serialized_start=12457
+  _OFFLINESTORECONFIG._serialized_end=12713
+  _MONITORINGCONFIG._serialized_start=12716
+  _MONITORINGCONFIG._serialized_end=12997
+  _SECONDARYKEYOUTPUTCOLUMN._serialized_start=13000
+  _SECONDARYKEYOUTPUTCOLUMN._serialized_end=13287
+  _TIMEWINDOW._serialized_start=13290
+  _TIMEWINDOW._serialized_end=13421
+  _TIMEWINDOWSERIES._serialized_start=13424
+  _TIMEWINDOWSERIES._serialized_end=13686
+  _CACHECONFIG._serialized_start=13688
+  _CACHECONFIG._serialized_end=13741
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tecton-0.9.0rc4/tecton_proto/args/pipeline_pb2.py` & `tecton-0.9.1/tecton_proto/args/pipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/args/repo_metadata_pb2.py` & `tecton-0.9.1/tecton_proto/args/repo_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/args/transformation_pb2.py` & `tecton-0.9.1/tecton_proto/args/transformation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/args/user_defined_function_pb2.py` & `tecton-0.9.1/tecton_proto/args/user_defined_function_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/args/version_constraints_pb2.py` & `tecton-0.9.1/tecton_proto/args/version_constraints_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/args/virtual_data_source_pb2.py` & `tecton-0.9.1/tecton_proto/args/virtual_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/auditlog/metadata_pb2.py` & `tecton-0.9.1/tecton_proto/auditlog/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/auth/acl_pb2.py` & `tecton-0.9.1/tecton_proto/auth/acl_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/auth/authorization_service_pb2.py` & `tecton-0.9.1/tecton_proto/auth/authorization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/auth/principal_pb2.py` & `tecton-0.9.1/tecton_proto/auth/principal_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/auth/resource_pb2.py` & `tecton-0.9.1/tecton_proto/auth/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/auth/resource_role_assignments_pb2.py` & `tecton-0.9.1/tecton_proto/auth/resource_role_assignments_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/auth/service_pb2.py` & `tecton-0.9.1/tecton_proto/auth/service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/canary/type_pb2.py` & `tecton-0.9.1/tecton_proto/canary/type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/canary/update_pb2.py` & `tecton-0.9.1/tecton_proto/canary/update_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/cli/repo_diff_pb2.py` & `tecton-0.9.1/tecton_proto/cli/repo_diff_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/common/aggregation_function_pb2.py` & `tecton-0.9.1/tecton_proto/common/aggregation_function_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/common/analytics_options_pb2.py` & `tecton-0.9.1/tecton_proto/common/analytics_options_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/common/aws_credentials_pb2.py` & `tecton-0.9.1/tecton_proto/common/aws_credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/common/column_type_pb2.py` & `tecton-0.9.1/tecton_proto/common/column_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/common/compute_mode_pb2.py` & `tecton-0.9.1/tecton_proto/common/compute_mode_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/common/container_image_pb2.py` & `tecton-0.9.1/tecton_proto/common/container_image_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/common/data_source_type_pb2.py` & `tecton-0.9.1/tecton_proto/common/data_source_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/common/data_type_pb2.py` & `tecton-0.9.1/tecton_proto/common/data_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/common/fco_locator_pb2.py` & `tecton-0.9.1/tecton_proto/common/fco_locator_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/common/framework_version_pb2.py` & `tecton-0.9.1/tecton_proto/common/framework_version_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/common/id_pb2.py` & `tecton-0.9.1/tecton_proto/common/id_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/common/pair_pb2.py` & `tecton-0.9.1/tecton_proto/common/pair_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/common/schema_container_pb2.py` & `tecton-0.9.1/tecton_proto/common/schema_container_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/common/schema_pb2.py` & `tecton-0.9.1/tecton_proto/common/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/common/secret_pb2.py` & `tecton-0.9.1/tecton_proto/common/secret_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/common/spark_schema_pb2.py` & `tecton-0.9.1/tecton_proto/common/spark_schema_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/common/time_window_pb2.py` & `tecton-0.9.1/tecton_proto/common/time_window_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/consumption/consumption_pb2.py` & `tecton-0.9.1/tecton_proto/consumption/consumption_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/batch_data_source_pb2.py` & `tecton-0.9.1/tecton_proto/data/batch_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/entity_pb2.py` & `tecton-0.9.1/tecton_proto/data/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/fco_metadata_pb2.py` & `tecton-0.9.1/tecton_proto/data/fco_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/fco_pb2.py` & `tecton-0.9.1/tecton_proto/data/fco_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/feature_service_pb2.py` & `tecton-0.9.1/tecton_proto/data/feature_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/feature_store_pb2.py` & `tecton-0.9.1/tecton_proto/data/feature_store_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/feature_view_pb2.py` & `tecton-0.9.1/tecton_proto/data/feature_view_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from tecton_proto.common import time_window_pb2 as tecton__proto_dot_common_dot_time__window__pb2
 from tecton_proto.data import fco_metadata_pb2 as tecton__proto_dot_data_dot_fco__metadata__pb2
 from tecton_proto.data import fv_materialization_pb2 as tecton__proto_dot_data_dot_fv__materialization__pb2
 from tecton_proto.data import odfv_compute_pb2 as tecton__proto_dot_data_dot_odfv__compute__pb2
 from tecton_proto.validation import validator_pb2 as tecton__proto_dot_validation_dot_validator__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$tecton_proto/data/feature_view.proto\x12\x11tecton_proto.data\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a$tecton_proto/args/feature_view.proto\x1a tecton_proto/args/pipeline.proto\x1a.tecton_proto/common/aggregation_function.proto\x1a&tecton_proto/common/compute_mode.proto\x1a*tecton_proto/common/data_source_type.proto\x1a+tecton_proto/common/framework_version.proto\x1a\x1ctecton_proto/common/id.proto\x1a tecton_proto/common/schema.proto\x1a%tecton_proto/common/time_window.proto\x1a$tecton_proto/data/fco_metadata.proto\x1a*tecton_proto/data/fv_materialization.proto\x1a$tecton_proto/data/odfv_compute.proto\x1a\'tecton_proto/validation/validator.proto\"\xad\x10\n\x0b\x46\x65\x61tureView\x12?\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\rfeatureViewId\x12\x41\n\x0c\x66\x63o_metadata\x18\x02 \x01(\x0b\x32\x1e.tecton_proto.data.FcoMetadataR\x0b\x66\x63oMetadata\x12\x36\n\nentity_ids\x18\x03 \x03(\x0b\x32\x17.tecton_proto.common.IdR\tentityIds\x12\x1b\n\tjoin_keys\x18\x04 \x03(\tR\x08joinKeys\x12?\n\x07schemas\x18\x0b \x01(\x0b\x32%.tecton_proto.data.FeatureViewSchemasR\x07schemas\x12P\n\x0b\x65nrichments\x18\xe8\x07 \x01(\x0b\x32).tecton_proto.data.FeatureViewEnrichmentsB\x02\x18\x01R\x0b\x65nrichments\x12U\n\x12temporal_aggregate\x18\x07 \x01(\x0b\x32$.tecton_proto.data.TemporalAggregateH\x00R\x11temporalAggregate\x12\x39\n\x08temporal\x18\x08 \x01(\x0b\x32\x1b.tecton_proto.data.TemporalH\x00R\x08temporal\x12]\n\x16on_demand_feature_view\x18\x11 \x01(\x0b\x32&.tecton_proto.data.OnDemandFeatureViewH\x00R\x13onDemandFeatureView\x12\x46\n\rfeature_table\x18\x10 \x01(\x0b\x32\x1f.tecton_proto.data.FeatureTableH\x00R\x0c\x66\x65\x61tureTable\x12#\n\rtimestamp_key\x18\n \x01(\tR\x0ctimestampKey\x12W\n\x14online_serving_index\x18\x05 \x01(\x0b\x32%.tecton_proto.data.OnlineServingIndexR\x12onlineServingIndex\x12\x37\n\x08pipeline\x18\x06 \x01(\x0b\x32\x1b.tecton_proto.args.PipelineR\x08pipeline\x12\x62\n\x16materialization_params\x18\t \x01(\x0b\x32+.tecton_proto.data.NewMaterializationParamsR\x15materializationParams\x12\x37\n\x17materialization_enabled\x18\x0c \x01(\x08R\x16materializationEnabled\x12}\n!materialization_state_transitions\x18\r \x03(\x0b\x32\x31.tecton_proto.data.MaterializationStateTransitionR\x1fmaterializationStateTransitions\x12P\n\x11monitoring_params\x18\x0e \x01(\x0b\x32#.tecton_proto.data.MonitoringParamsR\x10monitoringParams\x12?\n\x1c\x66\x65\x61ture_store_format_version\x18\x17 \x01(\x05R\x19\x66\x65\x61tureStoreFormatVersion\x12G\n\x0esnowflake_data\x18\x18 \x01(\x0b\x32 .tecton_proto.data.SnowflakeDataR\rsnowflakeData\x12/\n\x11\x66ramework_version\x18\x13 \x01(\x05\x42\x02\x18\x01R\x10\x66rameworkVersion\x12H\n\nfw_version\x18\x1a \x01(\x0e\x32%.tecton_proto.common.FrameworkVersionB\x02\x18\x01R\tfwVersion\x12\x17\n\x07web_url\x18\x19 \x01(\tR\x06webUrl\x12H\n\rbatch_trigger\x18\x1b \x01(\x0e\x32#.tecton_proto.args.BatchTriggerTypeR\x0c\x62\x61tchTrigger\x12[\n\x0fvalidation_args\x18\x1c \x01(\x0b\x32\x32.tecton_proto.validation.FeatureViewValidationArgsR\x0evalidationArgs\x12T\n\x13\x64\x61ta_quality_config\x18\x1d \x01(\x0b\x32$.tecton_proto.data.DataQualityConfigR\x11\x64\x61taQualityConfig\x12\x45\n\x07options\x18\x1e \x03(\x0b\x32+.tecton_proto.data.FeatureView.OptionsEntryR\x07options\x12S\n\x12\x62\x61tch_compute_mode\x18\x1f \x01(\x0e\x32%.tecton_proto.common.BatchComputeModeR\x10\x62\x61tchComputeMode\x12L\n\x0c\x63\x61\x63he_config\x18  \x01(\x0b\x32).tecton_proto.data.FeatureViewCacheConfigR\x0b\x63\x61\x63heConfig\x1a:\n\x0cOptionsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\x13\n\x11\x66\x65\x61ture_view_type\"\xe8\x03\n\x11TemporalAggregate\x12@\n\x0eslide_interval\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\rslideInterval\x12\x32\n\x15slide_interval_string\x18\x05 \x01(\tR\x13slideIntervalString\x12?\n\x08\x66\x65\x61tures\x18\x02 \x03(\x0b\x32#.tecton_proto.data.AggregateFeatureR\x08\x66\x65\x61tures\x12#\n\ris_continuous\x18\x03 \x01(\x08R\x0cisContinuous\x12M\n\x10\x64\x61ta_source_type\x18\x04 \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12:\n\x19\x61ggregation_secondary_key\x18\x06 \x01(\tR\x17\x61ggregationSecondaryKey\x12l\n\x1csecondary_key_output_columns\x18\x07 \x03(\x0b\x32+.tecton_proto.data.SecondaryKeyOutputColumnR\x19secondaryKeyOutputColumns\"\x84\x03\n\x10\x41ggregateFeature\x12,\n\x12input_feature_name\x18\x01 \x01(\tR\x10inputFeatureName\x12.\n\x13output_feature_name\x18\x02 \x01(\tR\x11outputFeatureName\x12\x44\n\x08\x66unction\x18\x03 \x01(\x0e\x32(.tecton_proto.common.AggregationFunctionR\x08\x66unction\x12W\n\x0f\x66unction_params\x18\x05 \x01(\x0b\x32..tecton_proto.common.AggregationFunctionParamsR\x0e\x66unctionParams\x12\x31\n\x06window\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x06window\x12@\n\x0btime_window\x18\x06 \x01(\x0b\x32\x1f.tecton_proto.common.TimeWindowR\ntimeWindow\"\xf5\x01\n\x1dTrailingTimeWindowAggregation\x12\x19\n\x08time_key\x18\x01 \x01(\tR\x07timeKey\x12S\n\x18\x61ggregation_slide_period\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\x16\x61ggregationSlidePeriod\x12?\n\x08\x66\x65\x61tures\x18\x03 \x03(\x0b\x32#.tecton_proto.data.AggregateFeatureR\x08\x66\x65\x61tures\x12#\n\ris_continuous\x18\x04 \x01(\x08R\x0cisContinuous\"\xbb\x02\n\x08Temporal\x12:\n\x0bserving_ttl\x18\x10 \x01(\x0b\x32\x19.google.protobuf.DurationR\nservingTtl\x12M\n\x10\x64\x61ta_source_type\x18\x11 \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12J\n\x0f\x62\x61\x63kfill_config\x18\x12 \x01(\x0b\x32!.tecton_proto.args.BackfillConfigR\x0e\x62\x61\x63kfillConfig\x12\x33\n\x15incremental_backfills\x18\x13 \x01(\x08R\x14incrementalBackfills\x12#\n\ris_continuous\x18\x14 \x01(\x08R\x0cisContinuous\"\x9a\x01\n\x0c\x46\x65\x61tureTable\x12%\n\x0eonline_enabled\x18\x01 \x01(\x08R\ronlineEnabled\x12\'\n\x0foffline_enabled\x18\x02 \x01(\x08R\x0eofflineEnabled\x12:\n\x0bserving_ttl\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationR\nservingTtl\"\x8f\x01\n\x13OnDemandFeatureView\x12\x13\n\x05no_op\x18\x01 \x01(\x08R\x04noOp\x12]\n\x16supported_environments\x18\x03 \x03(\x0b\x32&.tecton_proto.data.RemoteComputeConfigR\x15supportedEnvironmentsJ\x04\x08\x02\x10\x03\"\xc5\x02\n\x12\x46\x65\x61tureViewSchemas\x12<\n\x0bview_schema\x18\x01 \x01(\x0b\x32\x1b.tecton_proto.common.SchemaR\nviewSchema\x12\x35\n\x17is_explicit_view_schema\x18\x04 \x01(\x08R\x14isExplicitViewSchema\x12R\n\x16materialization_schema\x18\x02 \x01(\x0b\x32\x1b.tecton_proto.common.SchemaR\x15materializationSchema\x12\x66\n\x19online_batch_table_format\x18\x03 \x01(\x0b\x32+.tecton_proto.common.OnlineBatchTableFormatR\x16onlineBatchTableFormat\"1\n\x12OnlineServingIndex\x12\x1b\n\tjoin_keys\x18\x01 \x03(\tR\x08joinKeys\"\xb3\x03\n\x1eMaterializationStateTransition\x12\x38\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ttimestamp\x12%\n\x0eonline_enabled\x18\x02 \x01(\x08R\ronlineEnabled\x12\'\n\x0foffline_enabled\x18\x03 \x01(\x08R\x0eofflineEnabled\x12R\n\x17\x66\x65\x61ture_start_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x15\x66\x65\x61tureStartTimestamp\x12\x44\n\x1ematerialization_serial_version\x18\x05 \x01(\x05R\x1cmaterializationSerialVersion\x12\x37\n\x18\x66orce_stream_job_restart\x18\x06 \x01(\x08R\x15\x66orceStreamJobRestart\x12\x34\n\x16tecton_runtime_version\x18\x07 \x01(\tR\x14tectonRuntimeVersion\"\xaf\x01\n\x19ParquetOfflineStoreParams\x12I\n\x13time_partition_size\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x11timePartitionSize\x12G\n\x07version\x18\x02 \x01(\x0e\x32-.tecton_proto.data.ParquetOfflineStoreVersionR\x07version\"\xab\x01\n\x17\x44\x65ltaOfflineStoreParams\x12I\n\x13time_partition_size\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x11timePartitionSize\x12\x45\n\x07version\x18\x02 \x01(\x0e\x32+.tecton_proto.data.DeltaOfflineStoreVersionR\x07version\"\xac\x01\n\x12OfflineStoreParams\x12H\n\x07parquet\x18\x01 \x01(\x0b\x32,.tecton_proto.data.ParquetOfflineStoreParamsH\x00R\x07parquet\x12\x42\n\x05\x64\x65lta\x18\x02 \x01(\x0b\x32*.tecton_proto.data.DeltaOfflineStoreParamsH\x00R\x05\x64\x65ltaB\x08\n\x06params\"\xa0\x01\n FeaturePublishOfflineStoreConfig\x12\x32\n\x15publish_full_features\x18\x01 \x01(\x08R\x13publishFullFeatures\x12H\n\x12publish_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10publishStartTime\"\x9f\x0e\n\x18NewMaterializationParams\x12\x46\n\x11schedule_interval\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x10scheduleInterval\x12\x62\n\x1fmaterialization_start_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x1dmaterializationStartTimestamp\x12R\n\x17\x66\x65\x61ture_start_timestamp\x18\r \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x15\x66\x65\x61tureStartTimestamp\x12l\n%manual_trigger_backfill_end_timestamp\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.TimestampR!manualTriggerBackfillEndTimestamp\x12M\n\x15max_backfill_interval\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationR\x13maxBackfillInterval\x12\x33\n\x16writes_to_online_store\x18\x04 \x01(\x08R\x13writesToOnlineStore\x12\x35\n\x17writes_to_offline_store\x18\x05 \x01(\x08R\x14writesToOfflineStore\x12^\n\x14offline_store_config\x18\x06 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigR\x12offlineStoreConfig\x12W\n\x14offline_store_params\x18\x0e \x01(\x0b\x32%.tecton_proto.data.OfflineStoreParamsR\x12offlineStoreParams\x12U\n\x15\x62\x61tch_materialization\x18\x07 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x14\x62\x61tchMaterialization\x12W\n\x16stream_materialization\x18\x08 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x15streamMaterialization\x12L\n\x15max_source_data_delay\x18\t \x01(\x0b\x32\x19.google.protobuf.DurationR\x12maxSourceDataDelay\x12T\n\x13online_store_params\x18\n \x01(\x0b\x32$.tecton_proto.data.OnlineStoreParamsR\x11onlineStoreParams\x12\x44\n\routput_stream\x18\x0b \x01(\x0b\x32\x1f.tecton_proto.args.OutputStreamR\x0coutputStream\x12]\n\x11time_range_policy\x18\x0c \x01(\x0e\x32\x31.tecton_proto.data.MaterializationTimeRangePolicyR\x0ftimeRangePolicy\x12\x64\n\x19online_backfill_load_type\x18\x10 \x01(\x0e\x32).tecton_proto.data.OnlineBackfillLoadTypeR\x16onlineBackfillLoadType\x12\x44\n\x1etecton_materialization_runtime\x18\x11 \x01(\tR\x1ctectonMaterializationRuntime\x12\x83\x01\n$feature_publish_offline_store_config\x18\x13 \x01(\x0b\x32\x33.tecton_proto.data.FeaturePublishOfflineStoreConfigR featurePublishOfflineStoreConfig\x12\x38\n\x18\x62\x61tch_compaction_enabled\x18\x14 \x01(\x08R\x16\x62\x61tchCompactionEnabled\x12:\n\x19stream_compaction_enabled\x18\x17 \x01(\x08R\x17streamCompactionEnabled\x12 \n\x0b\x65nvironment\x18\x15 \x01(\tR\x0b\x65nvironment\x12X\n\x1bstream_compaction_tile_size\x18\x16 \x01(\x0b\x32\x19.google.protobuf.DurationR\x18streamCompactionTileSizeJ\x04\x08\x12\x10\x13\"\x8d\x02\n\x11OnlineStoreParams\x12%\n\x0euser_specified\x18\x01 \x01(\x08R\ruserSpecified\x12@\n\x06\x64ynamo\x18\x02 \x01(\x0b\x32&.tecton_proto.data.DynamoDbOnlineStoreH\x00R\x06\x64ynamo\x12;\n\x05redis\x18\x03 \x01(\x0b\x32#.tecton_proto.data.RedisOnlineStoreH\x00R\x05redis\x12\x44\n\x08\x62igtable\x18\x04 \x01(\x0b\x32&.tecton_proto.data.BigtableOnlineStoreH\x00R\x08\x62igtableB\x0c\n\nstore_type\"\xa1\x02\n\x13\x44ynamoDbOnlineStore\x12\x33\n\x16\x63ross_account_role_arn\x18\x01 \x01(\tR\x13\x63rossAccountRoleArn\x12\x39\n\x19\x63ross_account_external_id\x18\x02 \x01(\tR\x16\x63rossAccountExternalId\x12L\n#cross_account_intermediate_role_arn\x18\x05 \x01(\tR\x1f\x63rossAccountIntermediateRoleArn\x12\x18\n\x07\x65nabled\x18\x03 \x01(\x08R\x07\x65nabled\x12\x32\n\x15\x64\x62\x66s_credentials_path\x18\x04 \x01(\tR\x13\x64\x62\x66sCredentialsPath\"\xeb\x01\n\x10RedisOnlineStore\x12)\n\x10primary_endpoint\x18\x02 \x01(\tR\x0fprimaryEndpoint\x12\x31\n\x14\x61uthentication_token\x18\x04 \x01(\tR\x13\x61uthenticationToken\x12\x1f\n\x0btls_enabled\x18\x06 \x01(\x08R\ntlsEnabled\x12\x18\n\x07\x65nabled\x18\x05 \x01(\x08R\x07\x65nabled\x12&\n\x0finject_host_sni\x18\t \x01(\x08R\rinjectHostSniJ\x04\x08\x01\x10\x02J\x04\x08\x03\x10\x04J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\t\"o\n\x13\x42igtableOnlineStore\x12\x18\n\x07\x65nabled\x18\x01 \x01(\x08R\x07\x65nabled\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x1f\n\x0binstance_id\x18\x03 \x01(\tR\ninstanceId\"\x92\x02\n\x10MonitoringParams\x12%\n\x0euser_specified\x18\x01 \x01(\x08R\ruserSpecified\x12+\n\x11monitor_freshness\x18\x02 \x01(\x08R\x10monitorFreshness\x12W\n\x1a\x65xpected_feature_freshness\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationR\x18\x65xpectedFeatureFreshness\x12\x1f\n\x0b\x61lert_email\x18\x04 \x01(\tR\nalertEmail\x12\x30\n\x14grace_period_seconds\x18\x05 \x01(\x05R\x12gracePeriodSeconds\"\x85\x01\n\x16\x46\x65\x61tureViewEnrichments\x12S\n\x12\x66p_materialization\x18\x04 \x01(\x0b\x32$.tecton_proto.data.FvMaterializationR\x11\x66pMaterializationJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x05\x10\x06\"?\n\rSnowflakeData\x12.\n\x13snowflake_view_name\x18\x01 \x01(\tR\x11snowflakeViewName\"\x81\x01\n\x11\x44\x61taQualityConfig\x12\x30\n\x14\x64\x61ta_quality_enabled\x18\x01 \x01(\x08R\x12\x64\x61taQualityEnabled\x12:\n\x19skip_default_expectations\x18\x02 \x01(\x08R\x17skipDefaultExpectations\"p\n\x18SecondaryKeyOutputColumn\x12@\n\x0btime_window\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.TimeWindowR\ntimeWindow\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\"\x92\x02\n\x16\x46\x65\x61tureViewCacheConfig\x12\x1c\n\tnamespace\x18\x01 \x01(\tR\tnamespace\x12(\n\x10\x63\x61\x63he_group_name\x18\x02 \x01(\tR\x0e\x63\x61\x63heGroupName\x12\x41\n\x0fmax_age_seconds\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationR\rmaxAgeSeconds\x12?\n\x0emax_age_jitter\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x0cmaxAgeJitter\x12,\n\x12remapped_join_keys\x18\x05 \x03(\tR\x10remappedJoinKeys*\x95\x01\n\x1aParquetOfflineStoreVersion\x12-\n)PARQUET_OFFLINE_STORE_VERSION_UNSPECIFIED\x10\x00\x12#\n\x1fPARQUET_OFFLINE_STORE_VERSION_1\x10\x01\x12#\n\x1fPARQUET_OFFLINE_STORE_VERSION_2\x10\x02*\x8d\x01\n\x18\x44\x65ltaOfflineStoreVersion\x12+\n\'DELTA_OFFLINE_STORE_VERSION_UNSPECIFIED\x10\x00\x12!\n\x1d\x44\x45LTA_OFFLINE_STORE_VERSION_1\x10\x01\x12!\n\x1d\x44\x45LTA_OFFLINE_STORE_VERSION_2\x10\x02*\xc6\x01\n\x1eMaterializationTimeRangePolicy\x12\x31\n-MATERIALIZATION_TIME_RANGE_POLICY_UNSPECIFIED\x10\x00\x12:\n6MATERIALIZATION_TIME_RANGE_POLICY_FAIL_IF_OUT_OF_RANGE\x10\x01\x12\x35\n1MATERIALIZATION_TIME_RANGE_POLICY_FILTER_TO_RANGE\x10\x02\x42\x13\n\x0f\x63om.tecton.dataP\x01')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$tecton_proto/data/feature_view.proto\x12\x11tecton_proto.data\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a$tecton_proto/args/feature_view.proto\x1a tecton_proto/args/pipeline.proto\x1a.tecton_proto/common/aggregation_function.proto\x1a&tecton_proto/common/compute_mode.proto\x1a*tecton_proto/common/data_source_type.proto\x1a+tecton_proto/common/framework_version.proto\x1a\x1ctecton_proto/common/id.proto\x1a tecton_proto/common/schema.proto\x1a%tecton_proto/common/time_window.proto\x1a$tecton_proto/data/fco_metadata.proto\x1a*tecton_proto/data/fv_materialization.proto\x1a$tecton_proto/data/odfv_compute.proto\x1a\'tecton_proto/validation/validator.proto\"\xad\x10\n\x0b\x46\x65\x61tureView\x12?\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\rfeatureViewId\x12\x41\n\x0c\x66\x63o_metadata\x18\x02 \x01(\x0b\x32\x1e.tecton_proto.data.FcoMetadataR\x0b\x66\x63oMetadata\x12\x36\n\nentity_ids\x18\x03 \x03(\x0b\x32\x17.tecton_proto.common.IdR\tentityIds\x12\x1b\n\tjoin_keys\x18\x04 \x03(\tR\x08joinKeys\x12?\n\x07schemas\x18\x0b \x01(\x0b\x32%.tecton_proto.data.FeatureViewSchemasR\x07schemas\x12P\n\x0b\x65nrichments\x18\xe8\x07 \x01(\x0b\x32).tecton_proto.data.FeatureViewEnrichmentsB\x02\x18\x01R\x0b\x65nrichments\x12U\n\x12temporal_aggregate\x18\x07 \x01(\x0b\x32$.tecton_proto.data.TemporalAggregateH\x00R\x11temporalAggregate\x12\x39\n\x08temporal\x18\x08 \x01(\x0b\x32\x1b.tecton_proto.data.TemporalH\x00R\x08temporal\x12]\n\x16on_demand_feature_view\x18\x11 \x01(\x0b\x32&.tecton_proto.data.OnDemandFeatureViewH\x00R\x13onDemandFeatureView\x12\x46\n\rfeature_table\x18\x10 \x01(\x0b\x32\x1f.tecton_proto.data.FeatureTableH\x00R\x0c\x66\x65\x61tureTable\x12#\n\rtimestamp_key\x18\n \x01(\tR\x0ctimestampKey\x12W\n\x14online_serving_index\x18\x05 \x01(\x0b\x32%.tecton_proto.data.OnlineServingIndexR\x12onlineServingIndex\x12\x37\n\x08pipeline\x18\x06 \x01(\x0b\x32\x1b.tecton_proto.args.PipelineR\x08pipeline\x12\x62\n\x16materialization_params\x18\t \x01(\x0b\x32+.tecton_proto.data.NewMaterializationParamsR\x15materializationParams\x12\x37\n\x17materialization_enabled\x18\x0c \x01(\x08R\x16materializationEnabled\x12}\n!materialization_state_transitions\x18\r \x03(\x0b\x32\x31.tecton_proto.data.MaterializationStateTransitionR\x1fmaterializationStateTransitions\x12P\n\x11monitoring_params\x18\x0e \x01(\x0b\x32#.tecton_proto.data.MonitoringParamsR\x10monitoringParams\x12?\n\x1c\x66\x65\x61ture_store_format_version\x18\x17 \x01(\x05R\x19\x66\x65\x61tureStoreFormatVersion\x12G\n\x0esnowflake_data\x18\x18 \x01(\x0b\x32 .tecton_proto.data.SnowflakeDataR\rsnowflakeData\x12/\n\x11\x66ramework_version\x18\x13 \x01(\x05\x42\x02\x18\x01R\x10\x66rameworkVersion\x12H\n\nfw_version\x18\x1a \x01(\x0e\x32%.tecton_proto.common.FrameworkVersionB\x02\x18\x01R\tfwVersion\x12\x17\n\x07web_url\x18\x19 \x01(\tR\x06webUrl\x12H\n\rbatch_trigger\x18\x1b \x01(\x0e\x32#.tecton_proto.args.BatchTriggerTypeR\x0c\x62\x61tchTrigger\x12[\n\x0fvalidation_args\x18\x1c \x01(\x0b\x32\x32.tecton_proto.validation.FeatureViewValidationArgsR\x0evalidationArgs\x12T\n\x13\x64\x61ta_quality_config\x18\x1d \x01(\x0b\x32$.tecton_proto.data.DataQualityConfigR\x11\x64\x61taQualityConfig\x12\x45\n\x07options\x18\x1e \x03(\x0b\x32+.tecton_proto.data.FeatureView.OptionsEntryR\x07options\x12S\n\x12\x62\x61tch_compute_mode\x18\x1f \x01(\x0e\x32%.tecton_proto.common.BatchComputeModeR\x10\x62\x61tchComputeMode\x12L\n\x0c\x63\x61\x63he_config\x18  \x01(\x0b\x32).tecton_proto.data.FeatureViewCacheConfigR\x0b\x63\x61\x63heConfig\x1a:\n\x0cOptionsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\x13\n\x11\x66\x65\x61ture_view_type\"\xe8\x03\n\x11TemporalAggregate\x12@\n\x0eslide_interval\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\rslideInterval\x12\x32\n\x15slide_interval_string\x18\x05 \x01(\tR\x13slideIntervalString\x12?\n\x08\x66\x65\x61tures\x18\x02 \x03(\x0b\x32#.tecton_proto.data.AggregateFeatureR\x08\x66\x65\x61tures\x12#\n\ris_continuous\x18\x03 \x01(\x08R\x0cisContinuous\x12M\n\x10\x64\x61ta_source_type\x18\x04 \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12:\n\x19\x61ggregation_secondary_key\x18\x06 \x01(\tR\x17\x61ggregationSecondaryKey\x12l\n\x1csecondary_key_output_columns\x18\x07 \x03(\x0b\x32+.tecton_proto.data.SecondaryKeyOutputColumnR\x19secondaryKeyOutputColumns\"\x84\x03\n\x10\x41ggregateFeature\x12,\n\x12input_feature_name\x18\x01 \x01(\tR\x10inputFeatureName\x12.\n\x13output_feature_name\x18\x02 \x01(\tR\x11outputFeatureName\x12\x44\n\x08\x66unction\x18\x03 \x01(\x0e\x32(.tecton_proto.common.AggregationFunctionR\x08\x66unction\x12W\n\x0f\x66unction_params\x18\x05 \x01(\x0b\x32..tecton_proto.common.AggregationFunctionParamsR\x0e\x66unctionParams\x12\x31\n\x06window\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x06window\x12@\n\x0btime_window\x18\x06 \x01(\x0b\x32\x1f.tecton_proto.common.TimeWindowR\ntimeWindow\"\xf5\x01\n\x1dTrailingTimeWindowAggregation\x12\x19\n\x08time_key\x18\x01 \x01(\tR\x07timeKey\x12S\n\x18\x61ggregation_slide_period\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\x16\x61ggregationSlidePeriod\x12?\n\x08\x66\x65\x61tures\x18\x03 \x03(\x0b\x32#.tecton_proto.data.AggregateFeatureR\x08\x66\x65\x61tures\x12#\n\ris_continuous\x18\x04 \x01(\x08R\x0cisContinuous\"\xbb\x02\n\x08Temporal\x12:\n\x0bserving_ttl\x18\x10 \x01(\x0b\x32\x19.google.protobuf.DurationR\nservingTtl\x12M\n\x10\x64\x61ta_source_type\x18\x11 \x01(\x0e\x32#.tecton_proto.common.DataSourceTypeR\x0e\x64\x61taSourceType\x12J\n\x0f\x62\x61\x63kfill_config\x18\x12 \x01(\x0b\x32!.tecton_proto.args.BackfillConfigR\x0e\x62\x61\x63kfillConfig\x12\x33\n\x15incremental_backfills\x18\x13 \x01(\x08R\x14incrementalBackfills\x12#\n\ris_continuous\x18\x14 \x01(\x08R\x0cisContinuous\"\x9a\x01\n\x0c\x46\x65\x61tureTable\x12%\n\x0eonline_enabled\x18\x01 \x01(\x08R\ronlineEnabled\x12\'\n\x0foffline_enabled\x18\x02 \x01(\x08R\x0eofflineEnabled\x12:\n\x0bserving_ttl\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationR\nservingTtl\"\x8f\x01\n\x13OnDemandFeatureView\x12\x13\n\x05no_op\x18\x01 \x01(\x08R\x04noOp\x12]\n\x16supported_environments\x18\x03 \x03(\x0b\x32&.tecton_proto.data.RemoteComputeConfigR\x15supportedEnvironmentsJ\x04\x08\x02\x10\x03\"\xc5\x02\n\x12\x46\x65\x61tureViewSchemas\x12<\n\x0bview_schema\x18\x01 \x01(\x0b\x32\x1b.tecton_proto.common.SchemaR\nviewSchema\x12\x35\n\x17is_explicit_view_schema\x18\x04 \x01(\x08R\x14isExplicitViewSchema\x12R\n\x16materialization_schema\x18\x02 \x01(\x0b\x32\x1b.tecton_proto.common.SchemaR\x15materializationSchema\x12\x66\n\x19online_batch_table_format\x18\x03 \x01(\x0b\x32+.tecton_proto.common.OnlineBatchTableFormatR\x16onlineBatchTableFormat\"1\n\x12OnlineServingIndex\x12\x1b\n\tjoin_keys\x18\x01 \x03(\tR\x08joinKeys\"\xb3\x03\n\x1eMaterializationStateTransition\x12\x38\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ttimestamp\x12%\n\x0eonline_enabled\x18\x02 \x01(\x08R\ronlineEnabled\x12\'\n\x0foffline_enabled\x18\x03 \x01(\x08R\x0eofflineEnabled\x12R\n\x17\x66\x65\x61ture_start_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x15\x66\x65\x61tureStartTimestamp\x12\x44\n\x1ematerialization_serial_version\x18\x05 \x01(\x05R\x1cmaterializationSerialVersion\x12\x37\n\x18\x66orce_stream_job_restart\x18\x06 \x01(\x08R\x15\x66orceStreamJobRestart\x12\x34\n\x16tecton_runtime_version\x18\x07 \x01(\tR\x14tectonRuntimeVersion\"\xaf\x01\n\x19ParquetOfflineStoreParams\x12I\n\x13time_partition_size\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x11timePartitionSize\x12G\n\x07version\x18\x02 \x01(\x0e\x32-.tecton_proto.data.ParquetOfflineStoreVersionR\x07version\"\xab\x01\n\x17\x44\x65ltaOfflineStoreParams\x12I\n\x13time_partition_size\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x11timePartitionSize\x12\x45\n\x07version\x18\x02 \x01(\x0e\x32+.tecton_proto.data.DeltaOfflineStoreVersionR\x07version\"\xac\x01\n\x12OfflineStoreParams\x12H\n\x07parquet\x18\x01 \x01(\x0b\x32,.tecton_proto.data.ParquetOfflineStoreParamsH\x00R\x07parquet\x12\x42\n\x05\x64\x65lta\x18\x02 \x01(\x0b\x32*.tecton_proto.data.DeltaOfflineStoreParamsH\x00R\x05\x64\x65ltaB\x08\n\x06params\"\xa0\x01\n FeaturePublishOfflineStoreConfig\x12\x32\n\x15publish_full_features\x18\x01 \x01(\x08R\x13publishFullFeatures\x12H\n\x12publish_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10publishStartTime\"\xf7\r\n\x18NewMaterializationParams\x12\x46\n\x11schedule_interval\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x10scheduleInterval\x12\x62\n\x1fmaterialization_start_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x1dmaterializationStartTimestamp\x12R\n\x17\x66\x65\x61ture_start_timestamp\x18\r \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x15\x66\x65\x61tureStartTimestamp\x12l\n%manual_trigger_backfill_end_timestamp\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.TimestampR!manualTriggerBackfillEndTimestamp\x12M\n\x15max_backfill_interval\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationR\x13maxBackfillInterval\x12\x33\n\x16writes_to_online_store\x18\x04 \x01(\x08R\x13writesToOnlineStore\x12\x35\n\x17writes_to_offline_store\x18\x05 \x01(\x08R\x14writesToOfflineStore\x12^\n\x14offline_store_config\x18\x06 \x01(\x0b\x32,.tecton_proto.args.OfflineFeatureStoreConfigR\x12offlineStoreConfig\x12W\n\x14offline_store_params\x18\x0e \x01(\x0b\x32%.tecton_proto.data.OfflineStoreParamsR\x12offlineStoreParams\x12U\n\x15\x62\x61tch_materialization\x18\x07 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x14\x62\x61tchMaterialization\x12W\n\x16stream_materialization\x18\x08 \x01(\x0b\x32 .tecton_proto.args.ClusterConfigR\x15streamMaterialization\x12L\n\x15max_source_data_delay\x18\t \x01(\x0b\x32\x19.google.protobuf.DurationR\x12maxSourceDataDelay\x12T\n\x13online_store_params\x18\n \x01(\x0b\x32$.tecton_proto.data.OnlineStoreParamsR\x11onlineStoreParams\x12\x44\n\routput_stream\x18\x0b \x01(\x0b\x32\x1f.tecton_proto.args.OutputStreamR\x0coutputStream\x12]\n\x11time_range_policy\x18\x0c \x01(\x0e\x32\x31.tecton_proto.data.MaterializationTimeRangePolicyR\x0ftimeRangePolicy\x12\x64\n\x19online_backfill_load_type\x18\x10 \x01(\x0e\x32).tecton_proto.data.OnlineBackfillLoadTypeR\x16onlineBackfillLoadType\x12\x44\n\x1etecton_materialization_runtime\x18\x11 \x01(\tR\x1ctectonMaterializationRuntime\x12\x83\x01\n$feature_publish_offline_store_config\x18\x13 \x01(\x0b\x32\x33.tecton_proto.data.FeaturePublishOfflineStoreConfigR featurePublishOfflineStoreConfig\x12-\n\x12\x63ompaction_enabled\x18\x14 \x01(\x08R\x11\x63ompactionEnabled\x12\x32\n\x15stream_tiling_enabled\x18\x17 \x01(\x08R\x13streamTilingEnabled\x12 \n\x0b\x65nvironment\x18\x15 \x01(\tR\x0b\x65nvironment\x12\x43\n\x10stream_tile_size\x18\x16 \x01(\x0b\x32\x19.google.protobuf.DurationR\x0estreamTileSizeJ\x04\x08\x12\x10\x13\"\x8d\x02\n\x11OnlineStoreParams\x12%\n\x0euser_specified\x18\x01 \x01(\x08R\ruserSpecified\x12@\n\x06\x64ynamo\x18\x02 \x01(\x0b\x32&.tecton_proto.data.DynamoDbOnlineStoreH\x00R\x06\x64ynamo\x12;\n\x05redis\x18\x03 \x01(\x0b\x32#.tecton_proto.data.RedisOnlineStoreH\x00R\x05redis\x12\x44\n\x08\x62igtable\x18\x04 \x01(\x0b\x32&.tecton_proto.data.BigtableOnlineStoreH\x00R\x08\x62igtableB\x0c\n\nstore_type\"\xa1\x02\n\x13\x44ynamoDbOnlineStore\x12\x33\n\x16\x63ross_account_role_arn\x18\x01 \x01(\tR\x13\x63rossAccountRoleArn\x12\x39\n\x19\x63ross_account_external_id\x18\x02 \x01(\tR\x16\x63rossAccountExternalId\x12L\n#cross_account_intermediate_role_arn\x18\x05 \x01(\tR\x1f\x63rossAccountIntermediateRoleArn\x12\x18\n\x07\x65nabled\x18\x03 \x01(\x08R\x07\x65nabled\x12\x32\n\x15\x64\x62\x66s_credentials_path\x18\x04 \x01(\tR\x13\x64\x62\x66sCredentialsPath\"\xeb\x01\n\x10RedisOnlineStore\x12)\n\x10primary_endpoint\x18\x02 \x01(\tR\x0fprimaryEndpoint\x12\x31\n\x14\x61uthentication_token\x18\x04 \x01(\tR\x13\x61uthenticationToken\x12\x1f\n\x0btls_enabled\x18\x06 \x01(\x08R\ntlsEnabled\x12\x18\n\x07\x65nabled\x18\x05 \x01(\x08R\x07\x65nabled\x12&\n\x0finject_host_sni\x18\t \x01(\x08R\rinjectHostSniJ\x04\x08\x01\x10\x02J\x04\x08\x03\x10\x04J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\t\"o\n\x13\x42igtableOnlineStore\x12\x18\n\x07\x65nabled\x18\x01 \x01(\x08R\x07\x65nabled\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x1f\n\x0binstance_id\x18\x03 \x01(\tR\ninstanceId\"\x92\x02\n\x10MonitoringParams\x12%\n\x0euser_specified\x18\x01 \x01(\x08R\ruserSpecified\x12+\n\x11monitor_freshness\x18\x02 \x01(\x08R\x10monitorFreshness\x12W\n\x1a\x65xpected_feature_freshness\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationR\x18\x65xpectedFeatureFreshness\x12\x1f\n\x0b\x61lert_email\x18\x04 \x01(\tR\nalertEmail\x12\x30\n\x14grace_period_seconds\x18\x05 \x01(\x05R\x12gracePeriodSeconds\"\x85\x01\n\x16\x46\x65\x61tureViewEnrichments\x12S\n\x12\x66p_materialization\x18\x04 \x01(\x0b\x32$.tecton_proto.data.FvMaterializationR\x11\x66pMaterializationJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x05\x10\x06\"?\n\rSnowflakeData\x12.\n\x13snowflake_view_name\x18\x01 \x01(\tR\x11snowflakeViewName\"\x81\x01\n\x11\x44\x61taQualityConfig\x12\x30\n\x14\x64\x61ta_quality_enabled\x18\x01 \x01(\x08R\x12\x64\x61taQualityEnabled\x12:\n\x19skip_default_expectations\x18\x02 \x01(\x08R\x17skipDefaultExpectations\"p\n\x18SecondaryKeyOutputColumn\x12@\n\x0btime_window\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.TimeWindowR\ntimeWindow\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\"\x92\x02\n\x16\x46\x65\x61tureViewCacheConfig\x12\x1c\n\tnamespace\x18\x01 \x01(\tR\tnamespace\x12(\n\x10\x63\x61\x63he_group_name\x18\x02 \x01(\tR\x0e\x63\x61\x63heGroupName\x12\x41\n\x0fmax_age_seconds\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationR\rmaxAgeSeconds\x12?\n\x0emax_age_jitter\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x0cmaxAgeJitter\x12,\n\x12remapped_join_keys\x18\x05 \x03(\tR\x10remappedJoinKeys*\x95\x01\n\x1aParquetOfflineStoreVersion\x12-\n)PARQUET_OFFLINE_STORE_VERSION_UNSPECIFIED\x10\x00\x12#\n\x1fPARQUET_OFFLINE_STORE_VERSION_1\x10\x01\x12#\n\x1fPARQUET_OFFLINE_STORE_VERSION_2\x10\x02*\x8d\x01\n\x18\x44\x65ltaOfflineStoreVersion\x12+\n\'DELTA_OFFLINE_STORE_VERSION_UNSPECIFIED\x10\x00\x12!\n\x1d\x44\x45LTA_OFFLINE_STORE_VERSION_1\x10\x01\x12!\n\x1d\x44\x45LTA_OFFLINE_STORE_VERSION_2\x10\x02*\xc6\x01\n\x1eMaterializationTimeRangePolicy\x12\x31\n-MATERIALIZATION_TIME_RANGE_POLICY_UNSPECIFIED\x10\x00\x12:\n6MATERIALIZATION_TIME_RANGE_POLICY_FAIL_IF_OUT_OF_RANGE\x10\x01\x12\x35\n1MATERIALIZATION_TIME_RANGE_POLICY_FILTER_TO_RANGE\x10\x02\x42\x13\n\x0f\x63om.tecton.dataP\x01')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tecton_proto.data.feature_view_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\017com.tecton.dataP\001'
@@ -40,20 +40,20 @@
   _FEATUREVIEW_OPTIONSENTRY._serialized_options = b'8\001'
   _FEATUREVIEW.fields_by_name['enrichments']._options = None
   _FEATUREVIEW.fields_by_name['enrichments']._serialized_options = b'\030\001'
   _FEATUREVIEW.fields_by_name['framework_version']._options = None
   _FEATUREVIEW.fields_by_name['framework_version']._serialized_options = b'\030\001'
   _FEATUREVIEW.fields_by_name['fw_version']._options = None
   _FEATUREVIEW.fields_by_name['fw_version']._serialized_options = b'\030\001'
-  _PARQUETOFFLINESTOREVERSION._serialized_start=9734
-  _PARQUETOFFLINESTOREVERSION._serialized_end=9883
-  _DELTAOFFLINESTOREVERSION._serialized_start=9886
-  _DELTAOFFLINESTOREVERSION._serialized_end=10027
-  _MATERIALIZATIONTIMERANGEPOLICY._serialized_start=10030
-  _MATERIALIZATIONTIMERANGEPOLICY._serialized_end=10228
+  _PARQUETOFFLINESTOREVERSION._serialized_start=9694
+  _PARQUETOFFLINESTOREVERSION._serialized_end=9843
+  _DELTAOFFLINESTOREVERSION._serialized_start=9846
+  _DELTAOFFLINESTOREVERSION._serialized_end=9987
+  _MATERIALIZATIONTIMERANGEPOLICY._serialized_start=9990
+  _MATERIALIZATIONTIMERANGEPOLICY._serialized_end=10188
   _FEATUREVIEW._serialized_start=638
   _FEATUREVIEW._serialized_end=2731
   _FEATUREVIEW_OPTIONSENTRY._serialized_start=2652
   _FEATUREVIEW_OPTIONSENTRY._serialized_end=2710
   _TEMPORALAGGREGATE._serialized_start=2734
   _TEMPORALAGGREGATE._serialized_end=3222
   _AGGREGATEFEATURE._serialized_start=3225
@@ -77,29 +77,29 @@
   _DELTAOFFLINESTOREPARAMS._serialized_start=5480
   _DELTAOFFLINESTOREPARAMS._serialized_end=5651
   _OFFLINESTOREPARAMS._serialized_start=5654
   _OFFLINESTOREPARAMS._serialized_end=5826
   _FEATUREPUBLISHOFFLINESTORECONFIG._serialized_start=5829
   _FEATUREPUBLISHOFFLINESTORECONFIG._serialized_end=5989
   _NEWMATERIALIZATIONPARAMS._serialized_start=5992
-  _NEWMATERIALIZATIONPARAMS._serialized_end=7815
-  _ONLINESTOREPARAMS._serialized_start=7818
-  _ONLINESTOREPARAMS._serialized_end=8087
-  _DYNAMODBONLINESTORE._serialized_start=8090
-  _DYNAMODBONLINESTORE._serialized_end=8379
-  _REDISONLINESTORE._serialized_start=8382
-  _REDISONLINESTORE._serialized_end=8617
-  _BIGTABLEONLINESTORE._serialized_start=8619
-  _BIGTABLEONLINESTORE._serialized_end=8730
-  _MONITORINGPARAMS._serialized_start=8733
-  _MONITORINGPARAMS._serialized_end=9007
-  _FEATUREVIEWENRICHMENTS._serialized_start=9010
-  _FEATUREVIEWENRICHMENTS._serialized_end=9143
-  _SNOWFLAKEDATA._serialized_start=9145
-  _SNOWFLAKEDATA._serialized_end=9208
-  _DATAQUALITYCONFIG._serialized_start=9211
-  _DATAQUALITYCONFIG._serialized_end=9340
-  _SECONDARYKEYOUTPUTCOLUMN._serialized_start=9342
-  _SECONDARYKEYOUTPUTCOLUMN._serialized_end=9454
-  _FEATUREVIEWCACHECONFIG._serialized_start=9457
-  _FEATUREVIEWCACHECONFIG._serialized_end=9731
+  _NEWMATERIALIZATIONPARAMS._serialized_end=7775
+  _ONLINESTOREPARAMS._serialized_start=7778
+  _ONLINESTOREPARAMS._serialized_end=8047
+  _DYNAMODBONLINESTORE._serialized_start=8050
+  _DYNAMODBONLINESTORE._serialized_end=8339
+  _REDISONLINESTORE._serialized_start=8342
+  _REDISONLINESTORE._serialized_end=8577
+  _BIGTABLEONLINESTORE._serialized_start=8579
+  _BIGTABLEONLINESTORE._serialized_end=8690
+  _MONITORINGPARAMS._serialized_start=8693
+  _MONITORINGPARAMS._serialized_end=8967
+  _FEATUREVIEWENRICHMENTS._serialized_start=8970
+  _FEATUREVIEWENRICHMENTS._serialized_end=9103
+  _SNOWFLAKEDATA._serialized_start=9105
+  _SNOWFLAKEDATA._serialized_end=9168
+  _DATAQUALITYCONFIG._serialized_start=9171
+  _DATAQUALITYCONFIG._serialized_end=9300
+  _SECONDARYKEYOUTPUTCOLUMN._serialized_start=9302
+  _SECONDARYKEYOUTPUTCOLUMN._serialized_end=9414
+  _FEATUREVIEWCACHECONFIG._serialized_start=9417
+  _FEATUREVIEWCACHECONFIG._serialized_end=9691
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tecton-0.9.0rc4/tecton_proto/data/freshness_status_pb2.py` & `tecton-0.9.1/tecton_proto/data/freshness_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/fv_materialization_pb2.py` & `tecton-0.9.1/tecton_proto/data/fv_materialization_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/hive_metastore_pb2.py` & `tecton-0.9.1/tecton_proto/data/hive_metastore_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/internal_spark_cluster_status_pb2.py` & `tecton-0.9.1/tecton_proto/data/internal_spark_cluster_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/materialization_roles_allowlists_pb2.py` & `tecton-0.9.1/tecton_proto/data/materialization_roles_allowlists_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/materialization_status_pb2.py` & `tecton-0.9.1/tecton_proto/data/materialization_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/odfv_compute_pb2.py` & `tecton-0.9.1/tecton_proto/data/odfv_compute_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/onboarding_pb2.py` & `tecton-0.9.1/tecton_proto/data/onboarding_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/principal_group_pb2.py` & `tecton-0.9.1/tecton_proto/data/principal_group_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/remote_compute_environment_pb2.py` & `tecton-0.9.1/tecton_proto/data/remote_compute_environment_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/remote_spark_pb2.py` & `tecton-0.9.1/tecton_proto/data/remote_spark_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/saved_feature_data_frame_pb2.py` & `tecton-0.9.1/tecton_proto/data/saved_feature_data_frame_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/serving_status_pb2.py` & `tecton-0.9.1/tecton_proto/data/serving_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/state_update_pb2.py` & `tecton-0.9.1/tecton_proto/data/state_update_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/stream_data_source_pb2.py` & `tecton-0.9.1/tecton_proto/data/stream_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/summary_pb2.py` & `tecton-0.9.1/tecton_proto/data/summary_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/tecton_api_key_pb2.py` & `tecton-0.9.1/tecton_proto/data/tecton_api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/transformation_pb2.py` & `tecton-0.9.1/tecton_proto/data/transformation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/user_deployment_settings_pb2.py` & `tecton-0.9.1/tecton_proto/data/user_deployment_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/user_pb2.py` & `tecton-0.9.1/tecton_proto/data/user_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/virtual_data_source_pb2.py` & `tecton-0.9.1/tecton_proto/data/virtual_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/data/workspace_pb2.py` & `tecton-0.9.1/tecton_proto/data/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/databricks_api/clusters_pb2.py` & `tecton-0.9.1/tecton_proto/databricks_api/clusters_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/databricks_api/dbfs_pb2.py` & `tecton-0.9.1/tecton_proto/databricks_api/dbfs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/databricks_api/error_pb2.py` & `tecton-0.9.1/tecton_proto/databricks_api/error_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/databricks_api/execution_pb2.py` & `tecton-0.9.1/tecton_proto/databricks_api/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/databricks_api/instance_profiles_pb2.py` & `tecton-0.9.1/tecton_proto/databricks_api/instance_profiles_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/databricks_api/jobs_pb2.py` & `tecton-0.9.1/tecton_proto/databricks_api/jobs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/databricks_api/libraries_pb2.py` & `tecton-0.9.1/tecton_proto/databricks_api/libraries_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/databricks_api/permissions_pb2.py` & `tecton-0.9.1/tecton_proto/databricks_api/permissions_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/databricks_api/scim_pb2.py` & `tecton-0.9.1/tecton_proto/databricks_api/scim_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/databricks_api/secrets_pb2.py` & `tecton-0.9.1/tecton_proto/databricks_api/secrets_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/databricks_api/workspace_pb2.py` & `tecton-0.9.1/tecton_proto/databricks_api/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/dataobs/config_pb2.py` & `tecton-0.9.1/tecton_proto/dataobs/config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/dataobs/expectation_pb2.py` & `tecton-0.9.1/tecton_proto/dataobs/expectation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/dataobs/metric_pb2.py` & `tecton-0.9.1/tecton_proto/dataobs/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/dataobs/validation_pb2.py` & `tecton-0.9.1/tecton_proto/dataobs/validation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/dataobs/validation_task_params_pb2.py` & `tecton-0.9.1/tecton_proto/dataobs/validation_task_params_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/dataobs/validation_task_pb2.py` & `tecton-0.9.1/tecton_proto/dataobs/validation_task_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py` & `tecton-0.9.1/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/materialization/job_metadata_pb2.py` & `tecton-0.9.1/tecton_proto/materialization/job_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/materialization/materialization_states_pb2.py` & `tecton-0.9.1/tecton_proto/materialization/materialization_states_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/materialization/materialization_task_pb2.py` & `tecton-0.9.1/tecton_proto/materialization/materialization_task_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/materialization/params_pb2.py` & `tecton-0.9.1/tecton_proto/materialization/params_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/materialization/spark_cluster_pb2.py` & `tecton-0.9.1/tecton_proto/materialization/spark_cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/materializationjobservice/materialization_job_service_pb2.py` & `tecton-0.9.1/tecton_proto/materializationjobservice/materialization_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/metadataservice/http_over_grpc_pb2.py` & `tecton-0.9.1/tecton_proto/metadataservice/http_over_grpc_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/metadataservice/metadata_service_pb2.py` & `tecton-0.9.1/tecton_proto/metadataservice/metadata_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/offlinestore/delta/metadata_pb2.py` & `tecton-0.9.1/tecton_proto/offlinestore/delta/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/offlinestore/delta/transaction_writer_pb2.py` & `tecton-0.9.1/tecton_proto/offlinestore/delta/transaction_writer_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/online_store/feature_value_pb2.py` & `tecton-0.9.1/tecton_proto/online_store/feature_value_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/online_store/status_entry_pb2.py` & `tecton-0.9.1/tecton_proto/online_store/status_entry_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/online_store_writer/config_pb2.py` & `tecton-0.9.1/tecton_proto/online_store_writer/config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/online_store_writer/copier_pb2.py` & `tecton-0.9.1/tecton_proto/online_store_writer/copier_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py` & `tecton-0.9.1/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/secrets/secrets_service_pb2.py` & `tecton-0.9.1/tecton_proto/secrets/secrets_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/snowflake/location_pb2.py` & `tecton-0.9.1/tecton_proto/snowflake/location_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/snowflake/snowflake_credentials_pb2.py` & `tecton-0.9.1/tecton_proto/snowflake/snowflake_credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/spark_api/error_pb2.py` & `tecton-0.9.1/tecton_proto/spark_api/error_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/spark_api/jobs_pb2.py` & `tecton-0.9.1/tecton_proto/spark_api/jobs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/spark_common/clusters_pb2.py` & `tecton-0.9.1/tecton_proto/spark_common/clusters_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/spark_common/libraries_pb2.py` & `tecton-0.9.1/tecton_proto/spark_common/libraries_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/testhelperservice/test_helper_service_pb2.py` & `tecton-0.9.1/tecton_proto/testhelperservice/test_helper_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_proto/validation/validator_pb2.py` & `tecton-0.9.1/tecton_proto/validation/validator_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_snowflake/pipeline_helper.py` & `tecton-0.9.1/tecton_snowflake/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_snowflake/query/aggregation_plans.py` & `tecton-0.9.1/tecton_snowflake/query/aggregation_plans.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_snowflake/query/dataframe_helper.py` & `tecton-0.9.1/tecton_snowflake/query/dataframe_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_snowflake/query/nodes.py` & `tecton-0.9.1/tecton_snowflake/query/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
             agg_from = agg_from.lateral(pypika.Field(f"FLATTEN(input=>{names[0]})"))
         # Add the condition that spine time is between partial agg time and partial agg time + window, and run the aggregation function
         agg = (
             agg_from.select(*agg_columns)
             .distinct()
             .where(pypika.AliasedQuery(left_name)._ANCHOR_TIME >= pypika.AliasedQuery(agg_name)._ANCHOR_TIME)
             .where(pypika.AliasedQuery(left_name)._ANCHOR_TIME < pypika.AliasedQuery(agg_name)._ANCHOR_TIME + window)
-            .groupby(*(pypika.AliasedQuery(left_name).field(column) for column in common_cols))
+            .groupby(*(pypika.AliasedQuery(left_name).field(column) for column in output_columns))
         )
 
         output_feature_name = query_consts.default_case(aggregate_feature.output_feature_name)
         spine_name = left_name + "_" + output_feature_name
         right_name = agg_name + "_AGG"
         feature_column = pypika.AliasedQuery(right_name).field(output_feature_name)
         # TODO(TEC-15924): This behavior is not the same as spark. We should consider consolidating this behavior.
```

### Comparing `tecton-0.9.0rc4/tecton_snowflake/query/queries.py` & `tecton-0.9.1/tecton_snowflake/query/queries.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_snowflake/query/rewrite.py` & `tecton-0.9.1/tecton_snowflake/query/rewrite.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_snowflake/query/translate.py` & `tecton-0.9.1/tecton_snowflake/query/translate.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_snowflake/schema_derivation_utils.py` & `tecton-0.9.1/tecton_snowflake/schema_derivation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_snowflake/snowflake_type_utils.py` & `tecton-0.9.1/tecton_snowflake/snowflake_type_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_snowflake/sql_helper.py` & `tecton-0.9.1/tecton_snowflake/sql_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_snowflake/templates/copier_macro.sql` & `tecton-0.9.1/tecton_snowflake/templates/copier_macro.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_snowflake/templates/delete_orphaned_schemas.sql` & `tecton-0.9.1/tecton_snowflake/templates/delete_orphaned_schemas.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_snowflake/templates/delete_staged_files.sql` & `tecton-0.9.1/tecton_snowflake/templates/delete_staged_files.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_snowflake/templates/historical_features.sql` & `tecton-0.9.1/tecton_snowflake/templates/historical_features.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_snowflake/templates/historical_features_macros.sql` & `tecton-0.9.1/tecton_snowflake/templates/historical_features_macros.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_snowflake/templates/materialization_tile.sql` & `tecton-0.9.1/tecton_snowflake/templates/materialization_tile.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_snowflake/templates/materialized_feature_view.sql` & `tecton-0.9.1/tecton_snowflake/templates/materialized_feature_view.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_snowflake/templates/offline_materialization_macros.sql` & `tecton-0.9.1/tecton_snowflake/templates/offline_materialization_macros.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_snowflake/templates/run_full_aggregation.sql` & `tecton-0.9.1/tecton_snowflake/templates/run_full_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_snowflake/templates/run_partial_aggregation.sql` & `tecton-0.9.1/tecton_snowflake/templates/run_partial_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_snowflake/templates/time_limit.sql` & `tecton-0.9.1/tecton_snowflake/templates/time_limit.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_snowflake/templates_utils.py` & `tecton-0.9.1/tecton_snowflake/templates_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/__init__.py` & `tecton-0.9.1/tecton_spark/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/aggregation_plans.py` & `tecton-0.9.1/tecton_spark/aggregation_plans.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/data_observability.py` & `tecton-0.9.1/tecton_spark/data_observability.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/data_source_credentials.py` & `tecton-0.9.1/tecton_spark/data_source_credentials.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/data_source_helper.py` & `tecton-0.9.1/tecton_spark/data_source_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/feature_view_spark_utils.py` & `tecton-0.9.1/tecton_spark/feature_view_spark_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/jars/class_loader.py` & `tecton-0.9.1/tecton_spark/jars/class_loader.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/jars/tecton-udfs-spark-3.jar` & `tecton-0.9.1/tecton_spark/jars/tecton-udfs-spark-3.jar`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/materialization_plan.py` & `tecton-0.9.1/tecton_spark/materialization_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         return self.base_data_frame
 
     @property
     def online_store_data_frame(self) -> DataFrame:
         online_df = self.base_data_frame
 
         # batch online and offline df are slightly different
-        if not self._fd.batch_compaction_enabled and self._fd.is_temporal and not online_df.isStreaming:
+        if not self._fd.compaction_enabled and self._fd.is_temporal and not online_df.isStreaming:
             version = self._fd.get_feature_store_format_version
             batch_mat_schedule = convert_timedelta_for_version(self._fd.batch_materialization_schedule, version)
             online_df = self.base_data_frame.withColumn(
                 MATERIALIZED_RAW_DATA_END_TIME, functions.col(anchor_time()) + batch_mat_schedule
             ).drop(anchor_time())
         return online_df
```

### Comparing `tecton-0.9.0rc4/tecton_spark/offline_store.py` & `tecton-0.9.1/tecton_spark/offline_store.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/partial_aggregations.py` & `tecton-0.9.1/tecton_spark/partial_aggregations.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/pipeline_helper.py` & `tecton-0.9.1/tecton_spark/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/query/data_source.py` & `tecton-0.9.1/tecton_spark/query/data_source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/query/filter.py` & `tecton-0.9.1/tecton_spark/query/filter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/query/join.py` & `tecton-0.9.1/tecton_spark/query/join.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/query/node.py` & `tecton-0.9.1/tecton_spark/query/node.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/query/pipeline.py` & `tecton-0.9.1/tecton_spark/query/pipeline.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/query/projection.py` & `tecton-0.9.1/tecton_spark/query/projection.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/query/translate.py` & `tecton-0.9.1/tecton_spark/query/translate.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/schema_derivation_utils.py` & `tecton-0.9.1/tecton_spark/schema_derivation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/schema_spark_utils.py` & `tecton-0.9.1/tecton_spark/schema_spark_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/spark_helper.py` & `tecton-0.9.1/tecton_spark/spark_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/spark_schema_wrapper.py` & `tecton-0.9.1/tecton_spark/spark_schema_wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/time_utils.py` & `tecton-0.9.1/tecton_spark/time_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.0rc4/tecton_spark/udfs.py` & `tecton-0.9.1/tecton_spark/udfs.py`

 * *Files identical despite different names*

