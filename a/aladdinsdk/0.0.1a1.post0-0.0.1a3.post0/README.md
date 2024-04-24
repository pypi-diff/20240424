# Comparing `tmp/aladdinsdk-0.0.1a1.post0.tar.gz` & `tmp/aladdinsdk-0.0.1a3.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aladdinsdk-0.0.1a1.post0.tar", last modified: Tue Apr 23 18:44:08 2024, max compression
+gzip compressed data, was "aladdinsdk-0.0.1a3.post0.tar", last modified: Wed Apr 24 18:50:23 2024, max compression
```

## Comparing `aladdinsdk-0.0.1a1.post0.tar` & `aladdinsdk-0.0.1a3.post0.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.966911 aladdinsdk-0.0.1a1.post0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    42008 2024-04-23 18:44:08.966911 aladdinsdk-0.0.1a1.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    41073 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.938911 aladdinsdk-0.0.1a1.post0/aladdinsdk/
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.938911 aladdinsdk-0.0.1a1.post0/aladdinsdk/adc/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/adc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21917 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/adc/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.942911 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26142 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.942911 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/codegen_allow_list.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.934910 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.934910 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.934910 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.934910 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.942911 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.942911 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30917 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api/default_token_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    30281 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17107 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.946911 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/any.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/rpc_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/token_api_generate_authorization_url400_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_authorization_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_check_token_exists_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    12791 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)    41125 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/swagger.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.934910 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.934910 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.934910 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.934910 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.946911 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.946911 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   123450 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api/default_train_journey_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    30448 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17260 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.954911 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/any.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_region.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_train_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/expand_expand_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/rpc_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_journey_api_cancel_longrunning_operation_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_journey_api_get_longrunning_operation400_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_station_train_station_facilities_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_station_train_station_summary_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_train_summary_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_create_train_journeys_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_create_train_journeys_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_delete_train_journeys_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_delete_train_journeys_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_update_train_journeys_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_update_train_journeys_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_control_train_journey_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_create_train_journey_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_create_train_journey_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_delete_train_journey_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_filter_train_journeys_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_filter_train_journeys_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_follow_train_journey_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_list_train_journeys_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_longrunning_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_simulate_train_journey_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_train_journey.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_train_journey_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_update_train_journey_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_update_train_journey_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    12863 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)   173990 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/swagger.json
--rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/api/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.954911 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.954911 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/authentication/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/authentication/adc.py
--rw-r--r--   0 runner    (1001) docker     (127)    23017 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/authentication/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.954911 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/authentication/basicauth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/authentication/basicauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/authentication/basicauth/basicauthutil.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.954911 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/authentication/oauth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/authentication/oauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/authentication/oauth/oauth_token_cred_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/authentication/oauth/oauth_url_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/authentication/oauth/okta_sidecar_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.954911 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/blkutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/blkutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/blkutils/blkutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.954911 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/datatransformation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/datatransformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/datatransformation/json_to_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.954911 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/error/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/error/asdkerrors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/error/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.958911 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/error/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/error/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/error/handlers/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/error/handlers/adc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/error/handlers/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/error/handlers/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.958911 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/error/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/error/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/error/notifications/email_notifications_for_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.958911 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/exports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/exports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/exports/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/exports/export_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/exports/export_excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/exports/export_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/exports/export_pickle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.958911 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/exports/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/exports/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/exports/utils/data_parse_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/exports/utils/validate_file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/exports/utils/write_file_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.958911 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/metrics/domain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.958911 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7020 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/notifications/email_notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.962911 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/retry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/retry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/retry/adc_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/retry/api_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/retry/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.962911 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/secrets/fsutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/common/secrets/keyringutil.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.962911 aladdinsdk-0.0.1a1.post0/aladdinsdk/config/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/config/asdkconf.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/config/internal_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/config/user_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.962911 aladdinsdk-0.0.1a1.post0/aladdinsdk/config/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/config/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24947 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk/config/utils/user_settings_file_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.966911 aladdinsdk-0.0.1a1.post0/aladdinsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42008 2024-04-23 18:44:08.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9706 2024-04-23 18:44:08.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:44:08.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-23 18:44:08.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-23 18:44:08.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 18:44:08.000000 aladdinsdk-0.0.1a1.post0/aladdinsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-23 18:44:08.966911 aladdinsdk-0.0.1a1.post0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:44:08.966911 aladdinsdk-0.0.1a1.post0/test/
--rw-r--r--   0 runner    (1001) docker     (127)    34511 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/test/test_adc.py
--rw-r--r--   0 runner    (1001) docker     (127)    44103 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    19299 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/test/test_common_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    16163 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/test/test_common_authentication_adc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15890 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/test/test_common_authentication_oauth_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/test/test_common_authentication_okta_sidecar_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/test/test_common_blkutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17941 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/test/test_common_datatransformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/test/test_common_datatransformation_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/test/test_common_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/test/test_common_error_notifications_email.py
--rw-r--r--   0 runner    (1001) docker     (127)    26531 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/test/test_common_exports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/test/test_common_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/test/test_common_notifications_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/test/test_common_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/test/test_common_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27929 2024-04-23 18:43:15.000000 aladdinsdk-0.0.1a1.post0/test/test_user_settings_file_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.805997 aladdinsdk-0.0.1a3.post0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    43241 2024-04-24 18:50:23.805997 aladdinsdk-0.0.1a3.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    42306 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.777996 aladdinsdk-0.0.1a3.post0/aladdinsdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.777996 aladdinsdk-0.0.1a3.post0/aladdinsdk/adc/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/adc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21917 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/adc/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.781996 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26142 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.781996 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/codegen_allow_list.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.773996 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.773996 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.773996 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.773996 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.781996 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.781996 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30917 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api/default_token_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30281 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17107 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.781996 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/any.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/rpc_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/token_api_generate_authorization_url400_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_authorization_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_check_token_exists_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12791 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41125 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/swagger.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.773996 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.773996 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.773996 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.773996 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.785996 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.785996 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   123450 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api/default_train_journey_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30448 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17260 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.793996 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/any.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_train_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/expand_expand_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/rpc_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_journey_api_cancel_longrunning_operation_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_journey_api_get_longrunning_operation400_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_station_train_station_facilities_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_station_train_station_summary_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_train_summary_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_create_train_journeys_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_create_train_journeys_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_delete_train_journeys_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_delete_train_journeys_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_update_train_journeys_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_update_train_journeys_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_control_train_journey_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_create_train_journey_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_create_train_journey_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_delete_train_journey_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_filter_train_journeys_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_filter_train_journeys_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_follow_train_journey_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_list_train_journeys_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_longrunning_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_simulate_train_journey_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_train_journey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_train_journey_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_update_train_journey_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_update_train_journey_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12863 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)   173990 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/swagger.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/api/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.793996 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.793996 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/authentication/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/authentication/adc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23017 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/authentication/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.793996 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/authentication/basicauth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/authentication/basicauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/authentication/basicauth/basicauthutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.793996 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/authentication/oauth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/authentication/oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/authentication/oauth/oauth_token_cred_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/authentication/oauth/oauth_url_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/authentication/oauth/okta_sidecar_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.793996 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/blkutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/blkutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/blkutils/blkutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.793996 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/datatransformation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/datatransformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/datatransformation/json_to_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.793996 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/error/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/error/asdkerrors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/error/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.797996 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/error/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/error/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/error/handlers/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/error/handlers/adc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/error/handlers/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/error/handlers/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.797996 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/error/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/error/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/error/notifications/email_notifications_for_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.797996 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/exports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/exports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/exports/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/exports/export_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/exports/export_excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/exports/export_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/exports/export_pickle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.797996 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/exports/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/exports/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/exports/utils/data_parse_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/exports/utils/validate_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/exports/utils/write_file_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.797996 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/metrics/domain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.797996 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7020 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/notifications/email_notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.797996 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/retry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/retry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/retry/adc_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/retry/api_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/retry/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.801997 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/secrets/fsutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/common/secrets/keyringutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.801997 aladdinsdk-0.0.1a3.post0/aladdinsdk/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/config/asdkconf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/config/internal_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/config/user_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.801997 aladdinsdk-0.0.1a3.post0/aladdinsdk/config/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/config/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24947 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk/config/utils/user_settings_file_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.805997 aladdinsdk-0.0.1a3.post0/aladdinsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43241 2024-04-24 18:50:23.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9706 2024-04-24 18:50:23.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:50:23.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 18:50:23.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-24 18:50:23.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 18:50:23.000000 aladdinsdk-0.0.1a3.post0/aladdinsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-24 18:50:23.805997 aladdinsdk-0.0.1a3.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:50:23.805997 aladdinsdk-0.0.1a3.post0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    34511 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/test/test_adc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44103 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19299 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/test/test_common_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16163 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/test/test_common_authentication_adc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15890 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/test/test_common_authentication_oauth_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/test/test_common_authentication_okta_sidecar_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/test/test_common_blkutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17941 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/test/test_common_datatransformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/test/test_common_datatransformation_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/test/test_common_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/test/test_common_error_notifications_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26531 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/test/test_common_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/test/test_common_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/test/test_common_notifications_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/test/test_common_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/test/test_common_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27929 2024-04-24 18:49:25.000000 aladdinsdk-0.0.1a3.post0/test/test_user_settings_file_util.py
```

### Comparing `aladdinsdk-0.0.1a1.post0/LICENSE` & `aladdinsdk-0.0.1a3.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/PKG-INFO` & `aladdinsdk-0.0.1a3.post0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: aladdinsdk
-Version: 0.0.1a1.post0
-Summary: AladdinSDK
-Author-email: Vedant Naik <naik.vedant@gmail.com>
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aenum~=3.1.15
-Requires-Dist: cryptography~=42.0.5
-Requires-Dist: dynaconf~=3.2.3
-Requires-Dist: jsonpath-ng~=1.6.1
-Requires-Dist: openpyxl~=3.1.2
-Requires-Dist: pandas~=2.2.1
-Requires-Dist: pick~=2.2.0
-Requires-Dist: pydantic~=1.10.12
-Requires-Dist: python_dateutil~=2.9.0
-Requires-Dist: pyopenssl~=24.0.0
-Requires-Dist: PyYAML~=6.0.1
-Requires-Dist: snowflake-connector-python[pandas]~=3.7.1
-Requires-Dist: snowflake-snowpark-python[pandas]~=1.14.0
-Requires-Dist: requests~=2.31.0
-Requires-Dist: tenacity~=8.2.3
-Requires-Dist: urllib3~=1.26.16
-
 # AladdinSDK
 
 AladdinSDK allows developers to easily integrate BlackRock's Aladdin functionality into their own applications and systems. The goal is to make it easier for everyone to efficiently access and utilize Aladdin APIs and Data Cloud.
 
 ## Table of Contents
 
 - [AladdinSDK](#aladdinsdk)
@@ -260,15 +232,34 @@
     "query": {
         "departingStationId": "TS_1441"
     }
 }
 response = api_instance_train_journey.post("/trainJourneys:filter", req_body_json)
 ```
 
-To make an OrderAPI call, install a plugin which contains this API:
+#### AladdinAPI Plugins
+
+AladdinSDK's functional capabilities can be extended as needed using API bundles or 'plugins' that can be installed separately.
+
+List of official AladdinSDK API plugins (refer documentation on PyPI for up-to-date list of APIs packaged in each plugin):
+- [asdk_plugin_accounting](https://pypi.org/project/asdk_plugin_accounting)
+- [asdk_plugin_analytics](https://pypi.org/project/asdk_plugin_analytics)
+- [asdk_plugin_clients](https://pypi.org/project/asdk_plugin_clients)
+- [asdk_plugin_compliance](https://pypi.org/project/asdk_plugin_compliance)
+- [asdk_plugin_data](https://pypi.org/project/asdk_plugin_data)
+- [asdk_plugin_investment_operations](https://pypi.org/project/asdk_plugin_investment_operations)
+- [asdk_plugin_investment_research](https://pypi.org/project/asdk_plugin_investment_research)
+- [asdk_plugin_platform](https://pypi.org/project/asdk_plugin_platform)
+- [asdk_plugin_portfolio](https://pypi.org/project/asdk_plugin_portfolio)
+- [asdk_plugin_portfolio_management](https://pypi.org/project/asdk_plugin_portfolio_management)
+- [asdk_plugin_trading](https://pypi.org/project/asdk_plugin_trading)
+
+Install plugins using pip: `pip install asdk_plugin_<bundle_name>`
+
+For example, to make an OrderAPI call, install the trading plugin which contains this API:
 ```sh
 pip install asdk_plugin_trading
 ```
 
 ```py
 from aladdinsdk.api.client import AladdinAPI
```

### Comparing `aladdinsdk-0.0.1a1.post0/README.md` & `aladdinsdk-0.0.1a3.post0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: aladdinsdk
+Version: 0.0.1a3.post0
+Summary: AladdinSDK
+Author-email: Vedant Naik <naik.vedant@gmail.com>
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aenum~=3.1.15
+Requires-Dist: cryptography~=42.0.5
+Requires-Dist: dynaconf~=3.2.3
+Requires-Dist: jsonpath-ng~=1.6.1
+Requires-Dist: openpyxl~=3.1.2
+Requires-Dist: pandas~=2.2.1
+Requires-Dist: pick~=2.2.0
+Requires-Dist: pydantic~=1.10.12
+Requires-Dist: python_dateutil~=2.9.0
+Requires-Dist: pyopenssl~=24.0.0
+Requires-Dist: PyYAML~=6.0.1
+Requires-Dist: snowflake-connector-python[pandas]~=3.7.1
+Requires-Dist: snowflake-snowpark-python[pandas]~=1.14.0
+Requires-Dist: requests~=2.31.0
+Requires-Dist: tenacity~=8.2.3
+Requires-Dist: urllib3~=1.26.16
+
 # AladdinSDK
 
 AladdinSDK allows developers to easily integrate BlackRock's Aladdin functionality into their own applications and systems. The goal is to make it easier for everyone to efficiently access and utilize Aladdin APIs and Data Cloud.
 
 ## Table of Contents
 
 - [AladdinSDK](#aladdinsdk)
@@ -232,15 +260,34 @@
     "query": {
         "departingStationId": "TS_1441"
     }
 }
 response = api_instance_train_journey.post("/trainJourneys:filter", req_body_json)
 ```
 
-To make an OrderAPI call, install a plugin which contains this API:
+#### AladdinAPI Plugins
+
+AladdinSDK's functional capabilities can be extended as needed using API bundles or 'plugins' that can be installed separately.
+
+List of official AladdinSDK API plugins (refer documentation on PyPI for up-to-date list of APIs packaged in each plugin):
+- [asdk_plugin_accounting](https://pypi.org/project/asdk_plugin_accounting)
+- [asdk_plugin_analytics](https://pypi.org/project/asdk_plugin_analytics)
+- [asdk_plugin_clients](https://pypi.org/project/asdk_plugin_clients)
+- [asdk_plugin_compliance](https://pypi.org/project/asdk_plugin_compliance)
+- [asdk_plugin_data](https://pypi.org/project/asdk_plugin_data)
+- [asdk_plugin_investment_operations](https://pypi.org/project/asdk_plugin_investment_operations)
+- [asdk_plugin_investment_research](https://pypi.org/project/asdk_plugin_investment_research)
+- [asdk_plugin_platform](https://pypi.org/project/asdk_plugin_platform)
+- [asdk_plugin_portfolio](https://pypi.org/project/asdk_plugin_portfolio)
+- [asdk_plugin_portfolio_management](https://pypi.org/project/asdk_plugin_portfolio_management)
+- [asdk_plugin_trading](https://pypi.org/project/asdk_plugin_trading)
+
+Install plugins using pip: `pip install asdk_plugin_<bundle_name>`
+
+For example, to make an OrderAPI call, install the trading plugin which contains this API:
 ```sh
 pip install asdk_plugin_trading
 ```
 
 ```py
 from aladdinsdk.api.client import AladdinAPI
```

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/__init__.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/adc/client.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/adc/client.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/client.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/client.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/codegen_allow_list.yaml` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/codegen_allow_list.yaml`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/__init__.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/__init__.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api/default_token_api.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api/default_token_api.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api_client.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api_client.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api_response.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/api_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/configuration.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/configuration.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/exceptions.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/exceptions.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/__init__.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/any.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/any.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/rpc_status.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/rpc_status.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/token_api_generate_authorization_url400_response.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/token_api_generate_authorization_url400_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_authorization_url.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_authorization_url.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_check_token_exists_response.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_check_token_exists_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_token.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/models/v1_token.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/rest.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/rest.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/swagger.json` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/platform/infrastructure/token/v1/TokenAPI/swagger.json`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/__init__.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/__init__.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api/default_train_journey_api.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api/default_train_journey_api.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api_client.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api_client.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api_response.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/api_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/configuration.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/configuration.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/exceptions.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/exceptions.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/__init__.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/any.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/any.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_operator.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_operator.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_region.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_region.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_size.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_size.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_train_type.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/enums_train_type.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/expand_expand_mask.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/expand_expand_mask.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/rpc_status.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/rpc_status.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_journey_api_cancel_longrunning_operation_request.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_journey_api_cancel_longrunning_operation_request.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_journey_api_get_longrunning_operation400_response.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_journey_api_get_longrunning_operation400_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_station_train_station_facilities_slice.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_station_train_station_facilities_slice.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_station_train_station_summary_slice.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_station_train_station_summary_slice.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_train_summary_slice.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/train_train_summary_slice.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_create_train_journeys_request.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_create_train_journeys_request.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_create_train_journeys_response.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_create_train_journeys_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_delete_train_journeys_request.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_delete_train_journeys_request.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_delete_train_journeys_response.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_delete_train_journeys_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_update_train_journeys_request.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_update_train_journeys_request.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_update_train_journeys_response.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_batch_update_train_journeys_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_control_train_journey_response.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_control_train_journey_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_create_train_journey_request.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_create_train_journey_request.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_create_train_journey_result.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_create_train_journey_result.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_delete_train_journey_result.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_delete_train_journey_result.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_filter_train_journeys_request.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_filter_train_journeys_request.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_filter_train_journeys_response.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_filter_train_journeys_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_follow_train_journey_response.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_follow_train_journey_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_list_train_journeys_response.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_list_train_journeys_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_longrunning_operation.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_longrunning_operation.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_simulate_train_journey_response.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_simulate_train_journey_response.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_train_journey.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_train_journey.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_train_journey_query.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_train_journey_query.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_update_train_journey_request.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_update_train_journey_request.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_update_train_journey_result.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/models/v1_update_train_journey_result.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/rest.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/rest.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/swagger.json` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/codegen/reference_architecture/demo/train_journey/v1/TrainJourneyAPI/swagger.json`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/api/registry.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/api/registry.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/authentication/adc.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/authentication/adc.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/authentication/api.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/authentication/api.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/authentication/basicauth/basicauthutil.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/authentication/basicauth/basicauthutil.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/authentication/oauth/oauth_token_cred_client.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/authentication/oauth/oauth_token_cred_client.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/authentication/oauth/oauth_url_client.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/authentication/oauth/oauth_url_client.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/authentication/oauth/okta_sidecar_client.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/authentication/oauth/okta_sidecar_client.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/blkutils/blkutils.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/blkutils/blkutils.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/datatransformation/json_to_pandas.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/datatransformation/json_to_pandas.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/error/asdkerrors.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/error/asdkerrors.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/error/handler.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/error/handler.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/error/handlers/abstract.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/error/handlers/abstract.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/error/handlers/adc.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/error/handlers/adc.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/error/handlers/api.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/error/handlers/api.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/error/handlers/internal.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/error/handlers/internal.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/error/notifications/email_notifications_for_errors.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/error/notifications/email_notifications_for_errors.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/exports/export.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/exports/export.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/exports/export_csv.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/exports/export_csv.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/exports/export_excel.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/exports/export_excel.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/exports/export_json.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/exports/export_json.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/exports/export_pickle.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/exports/export_pickle.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/exports/utils/data_parse_util.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/exports/utils/data_parse_util.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/exports/utils/validate_file_util.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/exports/utils/validate_file_util.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/exports/utils/write_file_util.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/exports/utils/write_file_util.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/metrics/domain.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/metrics/domain.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/notifications/email_notifications.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/notifications/email_notifications.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/retry/adc_retry.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/retry/adc_retry.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/retry/api_retry.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/retry/api_retry.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/retry/utils.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/retry/utils.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/secrets/fsutil.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/secrets/fsutil.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/common/secrets/keyringutil.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/common/secrets/keyringutil.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/config/asdkconf.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/config/asdkconf.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/config/internal_settings.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/config/internal_settings.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/config/user_settings.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/config/user_settings.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk/config/utils/user_settings_file_util.py` & `aladdinsdk-0.0.1a3.post0/aladdinsdk/config/utils/user_settings_file_util.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk.egg-info/PKG-INFO` & `aladdinsdk-0.0.1a3.post0/aladdinsdk.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aladdinsdk
-Version: 0.0.1a1.post0
+Version: 0.0.1a3.post0
 Summary: AladdinSDK
 Author-email: Vedant Naik <naik.vedant@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -260,15 +260,34 @@
     "query": {
         "departingStationId": "TS_1441"
     }
 }
 response = api_instance_train_journey.post("/trainJourneys:filter", req_body_json)
 ```
 
-To make an OrderAPI call, install a plugin which contains this API:
+#### AladdinAPI Plugins
+
+AladdinSDK's functional capabilities can be extended as needed using API bundles or 'plugins' that can be installed separately.
+
+List of official AladdinSDK API plugins (refer documentation on PyPI for up-to-date list of APIs packaged in each plugin):
+- [asdk_plugin_accounting](https://pypi.org/project/asdk_plugin_accounting)
+- [asdk_plugin_analytics](https://pypi.org/project/asdk_plugin_analytics)
+- [asdk_plugin_clients](https://pypi.org/project/asdk_plugin_clients)
+- [asdk_plugin_compliance](https://pypi.org/project/asdk_plugin_compliance)
+- [asdk_plugin_data](https://pypi.org/project/asdk_plugin_data)
+- [asdk_plugin_investment_operations](https://pypi.org/project/asdk_plugin_investment_operations)
+- [asdk_plugin_investment_research](https://pypi.org/project/asdk_plugin_investment_research)
+- [asdk_plugin_platform](https://pypi.org/project/asdk_plugin_platform)
+- [asdk_plugin_portfolio](https://pypi.org/project/asdk_plugin_portfolio)
+- [asdk_plugin_portfolio_management](https://pypi.org/project/asdk_plugin_portfolio_management)
+- [asdk_plugin_trading](https://pypi.org/project/asdk_plugin_trading)
+
+Install plugins using pip: `pip install asdk_plugin_<bundle_name>`
+
+For example, to make an OrderAPI call, install the trading plugin which contains this API:
 ```sh
 pip install asdk_plugin_trading
 ```
 
 ```py
 from aladdinsdk.api.client import AladdinAPI
```

### Comparing `aladdinsdk-0.0.1a1.post0/aladdinsdk.egg-info/SOURCES.txt` & `aladdinsdk-0.0.1a3.post0/aladdinsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/pyproject.toml` & `aladdinsdk-0.0.1a3.post0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/test/test_adc.py` & `aladdinsdk-0.0.1a3.post0/test/test_adc.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/test/test_api.py` & `aladdinsdk-0.0.1a3.post0/test/test_api.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/test/test_common_authentication.py` & `aladdinsdk-0.0.1a3.post0/test/test_common_authentication.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/test/test_common_authentication_adc.py` & `aladdinsdk-0.0.1a3.post0/test/test_common_authentication_adc.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/test/test_common_authentication_oauth_client.py` & `aladdinsdk-0.0.1a3.post0/test/test_common_authentication_oauth_client.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/test/test_common_authentication_okta_sidecar_client.py` & `aladdinsdk-0.0.1a3.post0/test/test_common_authentication_okta_sidecar_client.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/test/test_common_blkutils.py` & `aladdinsdk-0.0.1a3.post0/test/test_common_blkutils.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/test/test_common_datatransformation.py` & `aladdinsdk-0.0.1a3.post0/test/test_common_datatransformation.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/test/test_common_datatransformation_options.py` & `aladdinsdk-0.0.1a3.post0/test/test_common_datatransformation_options.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/test/test_common_error_handling.py` & `aladdinsdk-0.0.1a3.post0/test/test_common_error_handling.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/test/test_common_error_notifications_email.py` & `aladdinsdk-0.0.1a3.post0/test/test_common_error_notifications_email.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/test/test_common_exports.py` & `aladdinsdk-0.0.1a3.post0/test/test_common_exports.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/test/test_common_metrics.py` & `aladdinsdk-0.0.1a3.post0/test/test_common_metrics.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/test/test_common_notifications_email.py` & `aladdinsdk-0.0.1a3.post0/test/test_common_notifications_email.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/test/test_common_retry.py` & `aladdinsdk-0.0.1a3.post0/test/test_common_retry.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/test/test_common_secrets.py` & `aladdinsdk-0.0.1a3.post0/test/test_common_secrets.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/test/test_config.py` & `aladdinsdk-0.0.1a3.post0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `aladdinsdk-0.0.1a1.post0/test/test_user_settings_file_util.py` & `aladdinsdk-0.0.1a3.post0/test/test_user_settings_file_util.py`

 * *Files identical despite different names*

